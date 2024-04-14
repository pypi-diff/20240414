# Comparing `tmp/fsai_proto_specs-0.0.8.tar.gz` & `tmp/fsai_proto_specs-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsai_proto_specs-0.0.8.tar", max compression
+gzip compressed data, was "fsai_proto_specs-0.0.9.tar", max compression
```

## Comparing `fsai_proto_specs-0.0.8.tar` & `fsai_proto_specs-0.0.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0       70 2023-10-25 20:49:04.422646 fsai_proto_specs-0.0.8/README.md
--rw-r--r--   0        0        0        0 2023-10-25 20:49:04.422646 fsai_proto_specs-0.0.8/data_grpc_service/__init__.py
--rw-r--r--   0        0        0        0 2023-10-25 20:49:04.422646 fsai_proto_specs-0.0.8/data_grpc_service/protos/__init__.py
--rw-r--r--   0        0        0     2739 2023-10-25 20:49:04.422646 fsai_proto_specs-0.0.8/data_grpc_service/protos/detection_instance_data_api_pb2.py
--rw-r--r--   0        0        0     5421 2023-10-25 20:49:04.422646 fsai_proto_specs-0.0.8/data_grpc_service/protos/detection_instance_data_api_pb2_grpc.py
--rw-r--r--   0        0        0     1446 2023-10-25 20:49:04.422646 fsai_proto_specs-0.0.8/data_grpc_service/protos/image_data_api_pb2.py
--rw-r--r--   0        0        0     2855 2023-10-25 20:49:04.422646 fsai_proto_specs-0.0.8/data_grpc_service/protos/image_data_api_pb2_grpc.py
--rw-r--r--   0        0        0    13194 2023-10-25 20:49:04.422646 fsai_proto_specs-0.0.8/data_grpc_service/protos/protoc_gen_validate/validate_pb2.py
--rw-r--r--   0        0        0      159 2023-10-25 20:49:04.422646 fsai_proto_specs-0.0.8/data_grpc_service/protos/protoc_gen_validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-10-25 20:49:04.422646 fsai_proto_specs-0.0.8/geospatial_toolkit_grpc_service/__init__.py
--rw-r--r--   0        0        0        0 2023-10-25 20:49:04.422646 fsai_proto_specs-0.0.8/geospatial_toolkit_grpc_service/protos/__init__.py
--rw-r--r--   0        0        0     2148 2023-10-25 20:49:04.422646 fsai_proto_specs-0.0.8/geospatial_toolkit_grpc_service/protos/function_api_pb2.py
--rw-r--r--   0        0        0     5069 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/geospatial_toolkit_grpc_service/protos/function_api_pb2_grpc.py
--rw-r--r--   0        0        0    13236 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/geospatial_toolkit_grpc_service/protos/protoc_gen_validate/validate_pb2.py
--rw-r--r--   0        0        0      159 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/geospatial_toolkit_grpc_service/protos/protoc_gen_validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/__init__.py
--rw-r--r--   0        0        0        0 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/__init__.py
--rw-r--r--   0        0        0     5587 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/area_of_interest_api_pb2.py
--rw-r--r--   0        0        0    13226 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/area_of_interest_api_pb2_grpc.py
--rw-r--r--   0        0        0     2867 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/category_api_pb2.py
--rw-r--r--   0        0        0     4639 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/category_api_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/detection_api_pb2.py
--rw-r--r--   0        0        0     2877 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/detection_api_pb2_grpc.py
--rw-r--r--   0        0        0    11778 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/detection_instance_api_pb2.py
--rw-r--r--   0        0        0    27218 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/detection_instance_api_pb2_grpc.py
--rw-r--r--   0        0        0     2858 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/feature_api_pb2.py
--rw-r--r--   0        0        0     4663 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/feature_api_pb2_grpc.py
--rw-r--r--   0        0        0     2740 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/image_api_pb2.py
--rw-r--r--   0        0        0     4624 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/image_api_pb2_grpc.py
--rw-r--r--   0        0        0     3532 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/metric_api_pb2.py
--rw-r--r--   0        0        0     7001 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/metric_api_pb2_grpc.py
--rw-r--r--   0        0        0     4896 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/mission_api_pb2.py
--rw-r--r--   0        0        0    12116 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/mission_api_pb2_grpc.py
--rw-r--r--   0        0        0     2485 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/permission_api_pb2.py
--rw-r--r--   0        0        0     4843 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/permission_api_pb2_grpc.py
--rw-r--r--   0        0        0    13209 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/protoc_gen_validate/validate_pb2.py
--rw-r--r--   0        0        0      159 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/protoc_gen_validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0     4467 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/query_api_pb2.py
--rw-r--r--   0        0        0     6782 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/query_api_pb2_grpc.py
--rw-r--r--   0        0        0     1529 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/review_api_pb2.py
--rw-r--r--   0        0        0     3008 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/review_api_pb2_grpc.py
--rw-r--r--   0        0        0     2287 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/role_api_pb2.py
--rw-r--r--   0        0        0     4549 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/role_api_pb2_grpc.py
--rw-r--r--   0        0        0     1994 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/signed_url_api_pb2.py
--rw-r--r--   0        0        0     4847 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/signed_url_api_pb2_grpc.py
--rw-r--r--   0        0        0     2038 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/source_api_pb2.py
--rw-r--r--   0        0        0     2793 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/source_api_pb2_grpc.py
--rw-r--r--   0        0        0     2594 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/team_api_pb2.py
--rw-r--r--   0        0        0     4571 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/team_api_pb2_grpc.py
--rw-r--r--   0        0        0     2305 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/team_member_api_pb2.py
--rw-r--r--   0        0        0     2992 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/team_member_api_pb2_grpc.py
--rw-r--r--   0        0        0     3169 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/user_api_pb2.py
--rw-r--r--   0        0        0     6380 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/user_api_pb2_grpc.py
--rw-r--r--   0        0        0     1589 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/utils_pb2.py
--rw-r--r--   0        0        0      159 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/utils_pb2_grpc.py
--rw-r--r--   0        0        0     2975 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/workflow_analyzer_api_pb2.py
--rw-r--r--   0        0        0     7132 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/workflow_analyzer_api_pb2_grpc.py
--rw-r--r--   0        0        0     7211 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/workflow_api_pb2.py
--rw-r--r--   0        0        0    20243 2023-10-25 20:49:04.426646 fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/workflow_api_pb2_grpc.py
--rw-r--r--   0        0        0     1222 2023-10-25 20:49:05.186652 fsai_proto_specs-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-25 20:49:04.430647 fsai_proto_specs-0.0.8/search_grpc_service/__init__.py
--rw-r--r--   0        0        0        0 2023-10-25 20:49:04.430647 fsai_proto_specs-0.0.8/search_grpc_service/protos/__init__.py
--rw-r--r--   0        0        0     1978 2023-10-25 20:49:04.430647 fsai_proto_specs-0.0.8/search_grpc_service/protos/index_api_pb2.py
--rw-r--r--   0        0        0     6787 2023-10-25 20:49:04.430647 fsai_proto_specs-0.0.8/search_grpc_service/protos/index_api_pb2_grpc.py
--rw-r--r--   0        0        0    13200 2023-10-25 20:49:04.430647 fsai_proto_specs-0.0.8/search_grpc_service/protos/protoc_gen_validate/validate_pb2.py
--rw-r--r--   0        0        0      159 2023-10-25 20:49:04.430647 fsai_proto_specs-0.0.8/search_grpc_service/protos/protoc_gen_validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0      929 1970-01-01 00:00:00.000000 fsai_proto_specs-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       70 2023-10-26 01:22:05.482304 fsai_proto_specs-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-10-26 01:22:05.482304 fsai_proto_specs-0.0.9/data_grpc_service/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-26 01:22:05.482304 fsai_proto_specs-0.0.9/data_grpc_service/protos/__init__.py
+-rw-r--r--   0        0        0     2739 2023-10-26 01:22:05.482304 fsai_proto_specs-0.0.9/data_grpc_service/protos/detection_instance_data_api_pb2.py
+-rw-r--r--   0        0        0     5421 2023-10-26 01:22:05.482304 fsai_proto_specs-0.0.9/data_grpc_service/protos/detection_instance_data_api_pb2_grpc.py
+-rw-r--r--   0        0        0     1446 2023-10-26 01:22:05.482304 fsai_proto_specs-0.0.9/data_grpc_service/protos/image_data_api_pb2.py
+-rw-r--r--   0        0        0     2855 2023-10-26 01:22:05.482304 fsai_proto_specs-0.0.9/data_grpc_service/protos/image_data_api_pb2_grpc.py
+-rw-r--r--   0        0        0    13194 2023-10-26 01:22:05.482304 fsai_proto_specs-0.0.9/data_grpc_service/protos/protoc_gen_validate/validate_pb2.py
+-rw-r--r--   0        0        0      159 2023-10-26 01:22:05.482304 fsai_proto_specs-0.0.9/data_grpc_service/protos/protoc_gen_validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-10-26 01:22:05.482304 fsai_proto_specs-0.0.9/geospatial_toolkit_grpc_service/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-26 01:22:05.482304 fsai_proto_specs-0.0.9/geospatial_toolkit_grpc_service/protos/__init__.py
+-rw-r--r--   0        0        0     2148 2023-10-26 01:22:05.482304 fsai_proto_specs-0.0.9/geospatial_toolkit_grpc_service/protos/function_api_pb2.py
+-rw-r--r--   0        0        0     5069 2023-10-26 01:22:05.482304 fsai_proto_specs-0.0.9/geospatial_toolkit_grpc_service/protos/function_api_pb2_grpc.py
+-rw-r--r--   0        0        0    13236 2023-10-26 01:22:05.482304 fsai_proto_specs-0.0.9/geospatial_toolkit_grpc_service/protos/protoc_gen_validate/validate_pb2.py
+-rw-r--r--   0        0        0      159 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/geospatial_toolkit_grpc_service/protos/protoc_gen_validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/__init__.py
+-rw-r--r--   0        0        0     5587 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/area_of_interest_api_pb2.py
+-rw-r--r--   0        0        0    13226 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/area_of_interest_api_pb2_grpc.py
+-rw-r--r--   0        0        0     2867 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/category_api_pb2.py
+-rw-r--r--   0        0        0     4639 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/category_api_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/detection_api_pb2.py
+-rw-r--r--   0        0        0     2877 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/detection_api_pb2_grpc.py
+-rw-r--r--   0        0        0    11778 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/detection_instance_api_pb2.py
+-rw-r--r--   0        0        0    27218 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/detection_instance_api_pb2_grpc.py
+-rw-r--r--   0        0        0     2858 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/feature_api_pb2.py
+-rw-r--r--   0        0        0     4663 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/feature_api_pb2_grpc.py
+-rw-r--r--   0        0        0     2740 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/image_api_pb2.py
+-rw-r--r--   0        0        0     4624 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/image_api_pb2_grpc.py
+-rw-r--r--   0        0        0     3532 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/metric_api_pb2.py
+-rw-r--r--   0        0        0     7001 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/metric_api_pb2_grpc.py
+-rw-r--r--   0        0        0     4896 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/mission_api_pb2.py
+-rw-r--r--   0        0        0    12116 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/mission_api_pb2_grpc.py
+-rw-r--r--   0        0        0     2485 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/permission_api_pb2.py
+-rw-r--r--   0        0        0     4843 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/permission_api_pb2_grpc.py
+-rw-r--r--   0        0        0    13209 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/protoc_gen_validate/validate_pb2.py
+-rw-r--r--   0        0        0      159 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/protoc_gen_validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0     4467 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/query_api_pb2.py
+-rw-r--r--   0        0        0     6782 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/query_api_pb2_grpc.py
+-rw-r--r--   0        0        0     1529 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/review_api_pb2.py
+-rw-r--r--   0        0        0     3008 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/review_api_pb2_grpc.py
+-rw-r--r--   0        0        0     2287 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/role_api_pb2.py
+-rw-r--r--   0        0        0     4549 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/role_api_pb2_grpc.py
+-rw-r--r--   0        0        0     1994 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/signed_url_api_pb2.py
+-rw-r--r--   0        0        0     4847 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/signed_url_api_pb2_grpc.py
+-rw-r--r--   0        0        0     2038 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/source_api_pb2.py
+-rw-r--r--   0        0        0     2793 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/source_api_pb2_grpc.py
+-rw-r--r--   0        0        0     2594 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/team_api_pb2.py
+-rw-r--r--   0        0        0     4571 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/team_api_pb2_grpc.py
+-rw-r--r--   0        0        0     2305 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/team_member_api_pb2.py
+-rw-r--r--   0        0        0     2992 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/team_member_api_pb2_grpc.py
+-rw-r--r--   0        0        0     3169 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/user_api_pb2.py
+-rw-r--r--   0        0        0     6380 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/user_api_pb2_grpc.py
+-rw-r--r--   0        0        0     1651 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/utils_pb2.py
+-rw-r--r--   0        0        0      159 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/utils_pb2_grpc.py
+-rw-r--r--   0        0        0     2975 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/workflow_analyzer_api_pb2.py
+-rw-r--r--   0        0        0     7132 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/workflow_analyzer_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7211 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/workflow_api_pb2.py
+-rw-r--r--   0        0        0    20243 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/workflow_api_pb2_grpc.py
+-rw-r--r--   0        0        0     1222 2023-10-26 01:22:06.054315 fsai_proto_specs-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/search_grpc_service/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/search_grpc_service/protos/__init__.py
+-rw-r--r--   0        0        0     1952 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/search_grpc_service/protos/index_api_pb2.py
+-rw-r--r--   0        0        0     6579 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/search_grpc_service/protos/index_api_pb2_grpc.py
+-rw-r--r--   0        0        0    13200 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/search_grpc_service/protos/protoc_gen_validate/validate_pb2.py
+-rw-r--r--   0        0        0      159 2023-10-26 01:22:05.486304 fsai_proto_specs-0.0.9/search_grpc_service/protos/protoc_gen_validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0      929 1970-01-01 00:00:00.000000 fsai_proto_specs-0.0.9/PKG-INFO
```

### Comparing `fsai_proto_specs-0.0.8/data_grpc_service/protos/detection_instance_data_api_pb2.py` & `fsai_proto_specs-0.0.9/data_grpc_service/protos/detection_instance_data_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/data_grpc_service/protos/detection_instance_data_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/data_grpc_service/protos/detection_instance_data_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/data_grpc_service/protos/image_data_api_pb2.py` & `fsai_proto_specs-0.0.9/data_grpc_service/protos/image_data_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/data_grpc_service/protos/image_data_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/data_grpc_service/protos/image_data_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/data_grpc_service/protos/protoc_gen_validate/validate_pb2.py` & `fsai_proto_specs-0.0.9/data_grpc_service/protos/protoc_gen_validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/geospatial_toolkit_grpc_service/protos/function_api_pb2.py` & `fsai_proto_specs-0.0.9/geospatial_toolkit_grpc_service/protos/function_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/geospatial_toolkit_grpc_service/protos/function_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/geospatial_toolkit_grpc_service/protos/function_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/geospatial_toolkit_grpc_service/protos/protoc_gen_validate/validate_pb2.py` & `fsai_proto_specs-0.0.9/geospatial_toolkit_grpc_service/protos/protoc_gen_validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/area_of_interest_api_pb2.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/area_of_interest_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/area_of_interest_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/area_of_interest_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/category_api_pb2.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/category_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/category_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/category_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/detection_api_pb2.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/detection_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/detection_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/detection_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/detection_instance_api_pb2.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/detection_instance_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/detection_instance_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/detection_instance_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/feature_api_pb2.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/feature_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/feature_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/feature_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/image_api_pb2.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/image_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/image_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/image_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/metric_api_pb2.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/metric_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/metric_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/metric_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/mission_api_pb2.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/mission_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/mission_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/mission_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/permission_api_pb2.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/permission_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/permission_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/permission_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/protoc_gen_validate/validate_pb2.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/protoc_gen_validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/query_api_pb2.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/query_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/query_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/query_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/review_api_pb2.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/review_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/review_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/review_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/role_api_pb2.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/role_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/role_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/role_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/signed_url_api_pb2.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/signed_url_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/signed_url_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/signed_url_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/source_api_pb2.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/source_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/source_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/source_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/team_api_pb2.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/team_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/team_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/team_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/team_member_api_pb2.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/team_member_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/team_member_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/team_member_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/user_api_pb2.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/user_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/user_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/user_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/utils_pb2.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/utils_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)global_vo_grpc_service/protos/utils.proto\"M\n\x07GeoBbox\x12\x0f\n\x07min_lat\x18\x01 \x01(\x02\x12\x0f\n\x07max_lat\x18\x02 \x01(\x02\x12\x0f\n\x07min_lon\x18\x03 \x01(\x02\x12\x0f\n\x07max_lon\x18\x04 \x01(\x02\"$\n\x08GeoPoint\x12\x0b\n\x03lat\x18\x01 \x01(\x02\x12\x0b\n\x03lon\x18\x02 \x01(\x02*q\n\nChangeType\x12\x17\n\x13UNKNOWN_CHANGE_TYPE\x10\x00\x12\x0b\n\x07\x43REATED\x10\x01\x12\x08\n\x04READ\x10\x02\x12\x0b\n\x07UPDATED\x10\x03\x12\x0b\n\x07\x44\x45LETED\x10\x04\x12\n\n\x06\x45XISTS\x10\x05\x12\r\n\tNOT_FOUND\x10\x06\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)global_vo_grpc_service/protos/utils.proto\"M\n\x07GeoBbox\x12\x0f\n\x07min_lat\x18\x01 \x01(\x02\x12\x0f\n\x07max_lat\x18\x02 \x01(\x02\x12\x0f\n\x07min_lon\x18\x03 \x01(\x02\x12\x0f\n\x07max_lon\x18\x04 \x01(\x02\"$\n\x08GeoPoint\x12\x0b\n\x03lat\x18\x01 \x01(\x02\x12\x0b\n\x03lon\x18\x02 \x01(\x02*\x8a\x01\n\nChangeType\x12\x17\n\x13UNKNOWN_CHANGE_TYPE\x10\x00\x12\x0b\n\x07\x43REATED\x10\x01\x12\x08\n\x04READ\x10\x02\x12\x0b\n\x07UPDATED\x10\x03\x12\x0b\n\x07\x44\x45LETED\x10\x04\x12\n\n\x06\x45XISTS\x10\x05\x12\r\n\tNOT_FOUND\x10\x06\x12\n\n\x06QUEUED\x10\x07\x12\x0b\n\x07INDEXED\x10\x08\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'global_vo_grpc_service.protos.utils_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _CHANGETYPE._serialized_start=162
-  _CHANGETYPE._serialized_end=275
+  _CHANGETYPE._serialized_start=163
+  _CHANGETYPE._serialized_end=301
   _GEOBBOX._serialized_start=45
   _GEOBBOX._serialized_end=122
   _GEOPOINT._serialized_start=124
   _GEOPOINT._serialized_end=160
 # @@protoc_insertion_point(module_scope)
```

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/workflow_analyzer_api_pb2.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/workflow_analyzer_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/workflow_analyzer_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/workflow_analyzer_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/workflow_api_pb2.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/workflow_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/global_vo_grpc_service/protos/workflow_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/global_vo_grpc_service/protos/workflow_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/pyproject.toml` & `fsai_proto_specs-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fsai-proto-specs"
-version = "v0.0.8"
+version = "v0.0.9"
 description = "Auto-generated library for use with GRPC API."
 authors = ["Michael Mohamed <michael@foundationstack.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/fsai-dev/fsai-proto-specs"
 repository = "https://github.com/fsai-dev/fsai-proto-specs"
```

### Comparing `fsai_proto_specs-0.0.8/search_grpc_service/protos/index_api_pb2.py` & `fsai_proto_specs-0.0.9/search_grpc_service/protos/index_api_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from global_vo_grpc_service.protos import utils_pb2 as global__vo__grpc__service_dot_protos_dot_utils__pb2
-from global_vo_grpc_service.protos import query_api_pb2 as global__vo__grpc__service_dot_protos_dot_query__api__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*search_grpc_service/protos/index_api.proto\x1a)global_vo_grpc_service/protos/utils.proto\x1a-global_vo_grpc_service/protos/query_api.proto\"0\n\"DeleteDetectionInstanceByIdRequest\x12\n\n\x02id\x18\x01 \x01(\x05\"4\n\x10IndexApiResponse\x12 \n\x0b\x63hange_type\x18\x01 \x01(\x0e\x32\x0b.ChangeType2\x8e\x02\n\x08IndexApi\x12U\n\x1b\x44\x65leteDetectionInstanceById\x12#.DeleteDetectionInstanceByIdRequest\x1a\x11.IndexApiResponse\x12U\n\x1bUpdateDetectionInstanceById\x12#.DetectionInstancesForSearchPayload\x1a\x11.IndexApiResponse\x12T\n\x1aQueueAllDetectionInstances\x12#.DetectionInstancesForSearchPayload\x1a\x11.IndexApiResponseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*search_grpc_service/protos/index_api.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a)global_vo_grpc_service/protos/utils.proto\"/\n!IndexDetectionInstanceByIdRequest\x12\n\n\x02id\x18\x01 \x01(\x05\"@\n\x10IndexApiResponse\x12 \n\x0b\x63hange_type\x18\x01 \x01(\x0e\x32\x0b.ChangeType\x12\n\n\x02id\x18\x02 \x01(\x05\x32\x81\x02\n\x08IndexApi\x12T\n\x1b\x44\x65leteDetectionInstanceById\x12\".IndexDetectionInstanceByIdRequest\x1a\x11.IndexApiResponse\x12T\n\x1bUpdateDetectionInstanceById\x12\".IndexDetectionInstanceByIdRequest\x1a\x11.IndexApiResponse\x12I\n\x1aQueueAllDetectionInstances\x12\x16.google.protobuf.Empty\x1a\x11.IndexApiResponse0\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'search_grpc_service.protos.index_api_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _DELETEDETECTIONINSTANCEBYIDREQUEST._serialized_start=136
-  _DELETEDETECTIONINSTANCEBYIDREQUEST._serialized_end=184
-  _INDEXAPIRESPONSE._serialized_start=186
-  _INDEXAPIRESPONSE._serialized_end=238
-  _INDEXAPI._serialized_start=241
-  _INDEXAPI._serialized_end=511
+  _INDEXDETECTIONINSTANCEBYIDREQUEST._serialized_start=118
+  _INDEXDETECTIONINSTANCEBYIDREQUEST._serialized_end=165
+  _INDEXAPIRESPONSE._serialized_start=167
+  _INDEXAPIRESPONSE._serialized_end=231
+  _INDEXAPI._serialized_start=234
+  _INDEXAPI._serialized_end=491
 # @@protoc_insertion_point(module_scope)
```

### Comparing `fsai_proto_specs-0.0.8/search_grpc_service/protos/index_api_pb2_grpc.py` & `fsai_proto_specs-0.0.9/search_grpc_service/protos/index_api_pb2_grpc.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from global_vo_grpc_service.protos import query_api_pb2 as global__vo__grpc__service_dot_protos_dot_query__api__pb2
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from search_grpc_service.protos import index_api_pb2 as search__grpc__service_dot_protos_dot_index__api__pb2
 
 
 class IndexApiStub(object):
     """Service that interacts with the index api.
     """
 
@@ -14,25 +14,25 @@
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.DeleteDetectionInstanceById = channel.unary_unary(
                 '/IndexApi/DeleteDetectionInstanceById',
-                request_serializer=search__grpc__service_dot_protos_dot_index__api__pb2.DeleteDetectionInstanceByIdRequest.SerializeToString,
+                request_serializer=search__grpc__service_dot_protos_dot_index__api__pb2.IndexDetectionInstanceByIdRequest.SerializeToString,
                 response_deserializer=search__grpc__service_dot_protos_dot_index__api__pb2.IndexApiResponse.FromString,
                 )
         self.UpdateDetectionInstanceById = channel.unary_unary(
                 '/IndexApi/UpdateDetectionInstanceById',
-                request_serializer=global__vo__grpc__service_dot_protos_dot_query__api__pb2.DetectionInstancesForSearchPayload.SerializeToString,
+                request_serializer=search__grpc__service_dot_protos_dot_index__api__pb2.IndexDetectionInstanceByIdRequest.SerializeToString,
                 response_deserializer=search__grpc__service_dot_protos_dot_index__api__pb2.IndexApiResponse.FromString,
                 )
-        self.QueueAllDetectionInstances = channel.unary_unary(
+        self.QueueAllDetectionInstances = channel.unary_stream(
                 '/IndexApi/QueueAllDetectionInstances',
-                request_serializer=global__vo__grpc__service_dot_protos_dot_query__api__pb2.DetectionInstancesForSearchPayload.SerializeToString,
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
                 response_deserializer=search__grpc__service_dot_protos_dot_index__api__pb2.IndexApiResponse.FromString,
                 )
 
 
 class IndexApiServicer(object):
     """Service that interacts with the index api.
     """
@@ -56,25 +56,25 @@
         raise NotImplementedError('Method not implemented!')
 
 
 def add_IndexApiServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'DeleteDetectionInstanceById': grpc.unary_unary_rpc_method_handler(
                     servicer.DeleteDetectionInstanceById,
-                    request_deserializer=search__grpc__service_dot_protos_dot_index__api__pb2.DeleteDetectionInstanceByIdRequest.FromString,
+                    request_deserializer=search__grpc__service_dot_protos_dot_index__api__pb2.IndexDetectionInstanceByIdRequest.FromString,
                     response_serializer=search__grpc__service_dot_protos_dot_index__api__pb2.IndexApiResponse.SerializeToString,
             ),
             'UpdateDetectionInstanceById': grpc.unary_unary_rpc_method_handler(
                     servicer.UpdateDetectionInstanceById,
-                    request_deserializer=global__vo__grpc__service_dot_protos_dot_query__api__pb2.DetectionInstancesForSearchPayload.FromString,
+                    request_deserializer=search__grpc__service_dot_protos_dot_index__api__pb2.IndexDetectionInstanceByIdRequest.FromString,
                     response_serializer=search__grpc__service_dot_protos_dot_index__api__pb2.IndexApiResponse.SerializeToString,
             ),
-            'QueueAllDetectionInstances': grpc.unary_unary_rpc_method_handler(
+            'QueueAllDetectionInstances': grpc.unary_stream_rpc_method_handler(
                     servicer.QueueAllDetectionInstances,
-                    request_deserializer=global__vo__grpc__service_dot_protos_dot_query__api__pb2.DetectionInstancesForSearchPayload.FromString,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                     response_serializer=search__grpc__service_dot_protos_dot_index__api__pb2.IndexApiResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'IndexApi', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
@@ -92,15 +92,15 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/IndexApi/DeleteDetectionInstanceById',
-            search__grpc__service_dot_protos_dot_index__api__pb2.DeleteDetectionInstanceByIdRequest.SerializeToString,
+            search__grpc__service_dot_protos_dot_index__api__pb2.IndexDetectionInstanceByIdRequest.SerializeToString,
             search__grpc__service_dot_protos_dot_index__api__pb2.IndexApiResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def UpdateDetectionInstanceById(request,
             target,
@@ -109,15 +109,15 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/IndexApi/UpdateDetectionInstanceById',
-            global__vo__grpc__service_dot_protos_dot_query__api__pb2.DetectionInstancesForSearchPayload.SerializeToString,
+            search__grpc__service_dot_protos_dot_index__api__pb2.IndexDetectionInstanceByIdRequest.SerializeToString,
             search__grpc__service_dot_protos_dot_index__api__pb2.IndexApiResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def QueueAllDetectionInstances(request,
             target,
@@ -125,12 +125,12 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/IndexApi/QueueAllDetectionInstances',
-            global__vo__grpc__service_dot_protos_dot_query__api__pb2.DetectionInstancesForSearchPayload.SerializeToString,
+        return grpc.experimental.unary_stream(request, target, '/IndexApi/QueueAllDetectionInstances',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             search__grpc__service_dot_protos_dot_index__api__pb2.IndexApiResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `fsai_proto_specs-0.0.8/search_grpc_service/protos/protoc_gen_validate/validate_pb2.py` & `fsai_proto_specs-0.0.9/search_grpc_service/protos/protoc_gen_validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_proto_specs-0.0.8/PKG-INFO` & `fsai_proto_specs-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsai-proto-specs
-Version: 0.0.8
+Version: 0.0.9
 Summary: Auto-generated library for use with GRPC API.
 Home-page: https://github.com/fsai-dev/fsai-proto-specs
 License: MIT
 Author: Michael Mohamed
 Author-email: michael@foundationstack.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


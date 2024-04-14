# Comparing `tmp/superwise_api-1.2.0.tar.gz` & `tmp/superwise_api-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superwise_api-1.2.0.tar", max compression
+gzip compressed data, was "superwise_api-1.3.0.tar", max compression
```

## Comparing `superwise_api-1.2.0.tar` & `superwise_api-1.3.0.tar`

### file list

```diff
@@ -1,203 +1,207 @@
--rw-r--r--   0        0        0      487 2024-03-14 16:53:40.125704 superwise_api-1.2.0/README.md
--rw-r--r--   0        0        0      828 2024-03-14 16:53:56.459288 superwise_api-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      276 2024-03-14 16:53:40.158707 superwise_api-1.2.0/superwise_api/__init__.py
--rw-r--r--   0        0        0    10657 2024-03-14 16:53:40.158707 superwise_api-1.2.0/superwise_api/client/__init__.py
--rw-r--r--   0        0        0      768 2024-03-14 16:53:40.158707 superwise_api-1.2.0/superwise_api/client/api/__init__.py
--rw-r--r--   0        0        0    88468 2024-03-14 16:53:40.159707 superwise_api-1.2.0/superwise_api/client/api/applications_api.py
--rw-r--r--   0        0        0    26731 2024-03-14 16:53:40.159707 superwise_api-1.2.0/superwise_api/client/api/dashboard_items_api.py
--rw-r--r--   0        0        0    31775 2024-03-14 16:53:40.160707 superwise_api-1.2.0/superwise_api/client/api/dashboards_api.py
--rw-r--r--   0        0        0    43860 2024-03-14 16:53:40.160707 superwise_api-1.2.0/superwise_api/client/api/dataset_api.py
--rw-r--r--   0        0        0    38374 2024-03-14 16:53:40.160707 superwise_api-1.2.0/superwise_api/client/api/dataset_sources_api.py
--rw-r--r--   0        0        0    36742 2024-03-14 16:53:40.161707 superwise_api-1.2.0/superwise_api/client/api/destinations_api.py
--rw-r--r--   0        0        0    21619 2024-03-14 16:53:40.161707 superwise_api-1.2.0/superwise_api/client/api/integrations_api.py
--rw-r--r--   0        0        0    21525 2024-03-14 16:53:40.161707 superwise_api-1.2.0/superwise_api/client/api/models_api.py
--rw-r--r--   0        0        0    44731 2024-03-14 16:53:40.162707 superwise_api-1.2.0/superwise_api/client/api/policies_api.py
--rw-r--r--   0        0        0    38625 2024-03-14 16:53:40.162707 superwise_api-1.2.0/superwise_api/client/api/sources_api.py
--rw-r--r--   0        0        0    36699 2024-03-14 16:53:40.162707 superwise_api-1.2.0/superwise_api/client/api/tools_api.py
--rw-r--r--   0        0        0    28011 2024-03-14 16:53:40.163708 superwise_api-1.2.0/superwise_api/client/api_client.py
--rw-r--r--   0        0        0      862 2024-03-14 16:53:40.163708 superwise_api-1.2.0/superwise_api/client/api_response.py
--rw-r--r--   0        0        0    14478 2024-03-14 16:53:40.163708 superwise_api-1.2.0/superwise_api/client/configuration.py
--rw-r--r--   0        0        0     5283 2024-03-14 16:53:40.163708 superwise_api-1.2.0/superwise_api/client/exceptions.py
--rw-r--r--   0        0        0     9336 2024-03-14 16:53:40.163708 superwise_api-1.2.0/superwise_api/client/models/__init__.py
--rw-r--r--   0        0        0      796 2024-03-14 16:53:40.164708 superwise_api-1.2.0/superwise_api/client/models/alert_on_status_direction.py
--rw-r--r--   0        0        0     2634 2024-03-14 16:53:40.164708 superwise_api-1.2.0/superwise_api/client/models/application_create.py
--rw-r--r--   0        0        0     3046 2024-03-14 16:53:40.164708 superwise_api-1.2.0/superwise_api/client/models/application_response.py
--rw-r--r--   0        0        0     4816 2024-03-14 16:53:40.164708 superwise_api-1.2.0/superwise_api/client/models/application_type.py
--rw-r--r--   0        0        0     2816 2024-03-14 16:53:40.164708 superwise_api-1.2.0/superwise_api/client/models/application_update.py
--rw-r--r--   0        0        0     2160 2024-03-14 16:53:40.165708 superwise_api-1.2.0/superwise_api/client/models/ask_config.py
--rw-r--r--   0        0        0     3106 2024-03-14 16:53:40.165708 superwise_api-1.2.0/superwise_api/client/models/ask_request_payload.py
--rw-r--r--   0        0        0     1837 2024-03-14 16:53:40.165708 superwise_api-1.2.0/superwise_api/client/models/ask_response_payload.py
--rw-r--r--   0        0        0     2588 2024-03-14 16:53:40.165708 superwise_api-1.2.0/superwise_api/client/models/aws_credentials_request.py
--rw-r--r--   0        0        0     2577 2024-03-14 16:53:40.165708 superwise_api-1.2.0/superwise_api/client/models/aws_credentials_response.py
--rw-r--r--   0        0        0     2650 2024-03-14 16:53:40.165708 superwise_api-1.2.0/superwise_api/client/models/azure_credentials_request.py
--rw-r--r--   0        0        0     2643 2024-03-14 16:53:40.166708 superwise_api-1.2.0/superwise_api/client/models/azure_credentials_response.py
--rw-r--r--   0        0        0     1966 2024-03-14 16:53:40.166708 superwise_api-1.2.0/superwise_api/client/models/chat_history_entry.py
--rw-r--r--   0        0        0     8587 2024-03-14 16:53:40.166708 superwise_api-1.2.0/superwise_api/client/models/config.py
--rw-r--r--   0        0        0     9021 2024-03-14 16:53:40.166708 superwise_api-1.2.0/superwise_api/client/models/config1.py
--rw-r--r--   0        0        0     4756 2024-03-14 16:53:40.166708 superwise_api-1.2.0/superwise_api/client/models/created_by.py
--rw-r--r--   0        0        0     2304 2024-03-14 16:53:40.166708 superwise_api-1.2.0/superwise_api/client/models/dashboard.py
--rw-r--r--   0        0        0     1780 2024-03-14 16:53:40.167708 superwise_api-1.2.0/superwise_api/client/models/dashboard_create.py
--rw-r--r--   0        0        0     3285 2024-03-14 16:53:40.167708 superwise_api-1.2.0/superwise_api/client/models/dashboard_item.py
--rw-r--r--   0        0        0     3049 2024-03-14 16:53:40.167708 superwise_api-1.2.0/superwise_api/client/models/dashboard_item_create.py
--rw-r--r--   0        0        0     3994 2024-03-14 16:53:40.167708 superwise_api-1.2.0/superwise_api/client/models/dashboard_item_query.py
--rw-r--r--   0        0        0     4956 2024-03-14 16:53:40.167708 superwise_api-1.2.0/superwise_api/client/models/dashboard_item_query_order.py
--rw-r--r--   0        0        0     1910 2024-03-14 16:53:40.167708 superwise_api-1.2.0/superwise_api/client/models/dashboard_update.py
--rw-r--r--   0        0        0     3397 2024-03-14 16:53:40.167708 superwise_api-1.2.0/superwise_api/client/models/dataset_create.py
--rw-r--r--   0        0        0     3971 2024-03-14 16:53:40.167708 superwise_api-1.2.0/superwise_api/client/models/dataset_response.py
--rw-r--r--   0        0        0     2593 2024-03-14 16:53:40.168708 superwise_api-1.2.0/superwise_api/client/models/dataset_source_create.py
--rw-r--r--   0        0        0     2904 2024-03-14 16:53:40.168708 superwise_api-1.2.0/superwise_api/client/models/dataset_source_response.py
--rw-r--r--   0        0        0     3355 2024-03-14 16:53:40.168708 superwise_api-1.2.0/superwise_api/client/models/dataset_source_response_with_source.py
--rw-r--r--   0        0        0     2514 2024-03-14 16:53:40.168708 superwise_api-1.2.0/superwise_api/client/models/dataset_source_update.py
--rw-r--r--   0        0        0     1769 2024-03-14 16:53:40.168708 superwise_api-1.2.0/superwise_api/client/models/dataset_tag.py
--rw-r--r--   0        0        0     2632 2024-03-14 16:53:40.168708 superwise_api-1.2.0/superwise_api/client/models/dataset_update.py
--rw-r--r--   0        0        0      678 2024-03-14 16:53:40.168708 superwise_api-1.2.0/superwise_api/client/models/datasource.py
--rw-r--r--   0        0        0     6335 2024-03-14 16:53:40.169708 superwise_api-1.2.0/superwise_api/client/models/default_value.py
--rw-r--r--   0        0        0     6127 2024-03-14 16:53:40.169708 superwise_api-1.2.0/superwise_api/client/models/default_value1.py
--rw-r--r--   0        0        0     4776 2024-03-14 16:53:40.169708 superwise_api-1.2.0/superwise_api/client/models/description.py
--rw-r--r--   0        0        0     2113 2024-03-14 16:53:40.169708 superwise_api-1.2.0/superwise_api/client/models/destination_create_base.py
--rw-r--r--   0        0        0     2614 2024-03-14 16:53:40.169708 superwise_api-1.2.0/superwise_api/client/models/destination_response.py
--rw-r--r--   0        0        0     1963 2024-03-14 16:53:40.169708 superwise_api-1.2.0/superwise_api/client/models/destination_update_base.py
--rw-r--r--   0        0        0     5042 2024-03-14 16:53:40.170708 superwise_api-1.2.0/superwise_api/client/models/embedding_model.py
--rw-r--r--   0        0        0     2226 2024-03-14 16:53:40.170708 superwise_api-1.2.0/superwise_api/client/models/filter.py
--rw-r--r--   0        0        0     2384 2024-03-14 16:53:40.170708 superwise_api-1.2.0/superwise_api/client/models/gcp_credentials_request.py
--rw-r--r--   0        0        0     2369 2024-03-14 16:53:40.170708 superwise_api-1.2.0/superwise_api/client/models/gcp_credentials_response.py
--rw-r--r--   0        0        0      771 2024-03-14 16:53:40.170708 superwise_api-1.2.0/superwise_api/client/models/google_model_version.py
--rw-r--r--   0        0        0      770 2024-03-14 16:53:40.170708 superwise_api-1.2.0/superwise_api/client/models/granularity.py
--rw-r--r--   0        0        0     2375 2024-03-14 16:53:40.170708 superwise_api-1.2.0/superwise_api/client/models/http_validation_error.py
--rw-r--r--   0        0        0      674 2024-03-14 16:53:40.171708 superwise_api-1.2.0/superwise_api/client/models/ingest_type.py
--rw-r--r--   0        0        0     2478 2024-03-14 16:53:40.171708 superwise_api-1.2.0/superwise_api/client/models/integration_response.py
--rw-r--r--   0        0        0      670 2024-03-14 16:53:40.171708 superwise_api-1.2.0/superwise_api/client/models/integration_type.py
--rw-r--r--   0        0        0     2418 2024-03-14 16:53:40.171708 superwise_api-1.2.0/superwise_api/client/models/model_create.py
--rw-r--r--   0        0        0     4736 2024-03-14 16:53:40.171708 superwise_api-1.2.0/superwise_api/client/models/model_id.py
--rw-r--r--   0        0        0      736 2024-03-14 16:53:40.171708 superwise_api-1.2.0/superwise_api/client/models/model_provider.py
--rw-r--r--   0        0        0     2788 2024-03-14 16:53:40.172709 superwise_api-1.2.0/superwise_api/client/models/model_response.py
--rw-r--r--   0        0        0     1802 2024-03-14 16:53:40.172709 superwise_api-1.2.0/superwise_api/client/models/model_schema.py
--rw-r--r--   0        0        0     4786 2024-03-14 16:53:40.172709 superwise_api-1.2.0/superwise_api/client/models/model_version.py
--rw-r--r--   0        0        0     5717 2024-03-14 16:53:40.172709 superwise_api-1.2.0/superwise_api/client/models/model_version_response.py
--rw-r--r--   0        0        0     4706 2024-03-14 16:53:40.172709 superwise_api-1.2.0/superwise_api/client/models/name.py
--rw-r--r--   0        0        0     1009 2024-03-14 16:53:40.172709 superwise_api-1.2.0/superwise_api/client/models/open_ai_model_version.py
--rw-r--r--   0        0        0     4697 2024-03-14 16:53:40.173709 superwise_api-1.2.0/superwise_api/client/models/order.py
--rw-r--r--   0        0        0     4786 2024-03-14 16:53:40.173709 superwise_api-1.2.0/superwise_api/client/models/order1.py
--rw-r--r--   0        0        0     4750 2024-03-14 16:53:40.173709 superwise_api-1.2.0/superwise_api/client/models/page.py
--rw-r--r--   0        0        0     3816 2024-03-14 16:53:40.173709 superwise_api-1.2.0/superwise_api/client/models/page_application_response.py
--rw-r--r--   0        0        0     3093 2024-03-14 16:53:40.173709 superwise_api-1.2.0/superwise_api/client/models/page_dashboard.py
--rw-r--r--   0        0        0     3142 2024-03-14 16:53:40.174709 superwise_api-1.2.0/superwise_api/client/models/page_dashboard_item.py
--rw-r--r--   0        0        0     3166 2024-03-14 16:53:40.174709 superwise_api-1.2.0/superwise_api/client/models/page_dataset_response.py
--rw-r--r--   0        0        0     3361 2024-03-14 16:53:40.174709 superwise_api-1.2.0/superwise_api/client/models/page_dataset_source_response_with_source.py
--rw-r--r--   0        0        0     3214 2024-03-14 16:53:40.174709 superwise_api-1.2.0/superwise_api/client/models/page_destination_response.py
--rw-r--r--   0        0        0     3214 2024-03-14 16:53:40.174709 superwise_api-1.2.0/superwise_api/client/models/page_integration_response.py
--rw-r--r--   0        0        0     3744 2024-03-14 16:53:40.175709 superwise_api-1.2.0/superwise_api/client/models/page_model_response.py
--rw-r--r--   0        0        0     3154 2024-03-14 16:53:40.175709 superwise_api-1.2.0/superwise_api/client/models/page_policy_response.py
--rw-r--r--   0        0        0     3154 2024-03-14 16:53:40.175709 superwise_api-1.2.0/superwise_api/client/models/page_source_response.py
--rw-r--r--   0        0        0     3732 2024-03-14 16:53:40.175709 superwise_api-1.2.0/superwise_api/client/models/page_tool_response.py
--rw-r--r--   0        0        0     4760 2024-03-14 16:53:40.175709 superwise_api-1.2.0/superwise_api/client/models/pages.py
--rw-r--r--   0        0        0     8597 2024-03-14 16:53:40.175709 superwise_api-1.2.0/superwise_api/client/models/payload.py
--rw-r--r--   0        0        0     4615 2024-03-14 16:53:40.175709 superwise_api-1.2.0/superwise_api/client/models/policy_create.py
--rw-r--r--   0        0        0     3192 2024-03-14 16:53:40.175709 superwise_api-1.2.0/superwise_api/client/models/policy_query.py
--rw-r--r--   0        0        0     2314 2024-03-14 16:53:40.176709 superwise_api-1.2.0/superwise_api/client/models/policy_query_filter.py
--rw-r--r--   0        0        0     1842 2024-03-14 16:53:40.176709 superwise_api-1.2.0/superwise_api/client/models/policy_query_order.py
--rw-r--r--   0        0        0     5592 2024-03-14 16:53:40.176709 superwise_api-1.2.0/superwise_api/client/models/policy_response.py
--rw-r--r--   0        0        0      740 2024-03-14 16:53:40.176709 superwise_api-1.2.0/superwise_api/client/models/policy_status.py
--rw-r--r--   0        0        0     4020 2024-03-14 16:53:40.176709 superwise_api-1.2.0/superwise_api/client/models/policy_update.py
--rw-r--r--   0        0        0     4726 2024-03-14 16:53:40.177709 superwise_api-1.2.0/superwise_api/client/models/prompt.py
--rw-r--r--   0        0        0     4746 2024-03-14 16:53:40.177709 superwise_api-1.2.0/superwise_api/client/models/provider.py
--rw-r--r--   0        0        0     3815 2024-03-14 16:53:40.177709 superwise_api-1.2.0/superwise_api/client/models/query.py
--rw-r--r--   0        0        0      748 2024-03-14 16:53:40.177709 superwise_api-1.2.0/superwise_api/client/models/query_type.py
--rw-r--r--   0        0        0      629 2024-03-14 16:53:40.177709 superwise_api-1.2.0/superwise_api/client/models/role.py
--rw-r--r--   0        0        0     2100 2024-03-14 16:53:40.177709 superwise_api-1.2.0/superwise_api/client/models/schema_item.py
--rw-r--r--   0        0        0     1810 2024-03-14 16:53:40.177709 superwise_api-1.2.0/superwise_api/client/models/schema_update.py
--rw-r--r--   0        0        0     2248 2024-03-14 16:53:40.177709 superwise_api-1.2.0/superwise_api/client/models/schema_update_item.py
--rw-r--r--   0        0        0     4750 2024-03-14 16:53:40.178709 superwise_api-1.2.0/superwise_api/client/models/size.py
--rw-r--r--   0        0        0     6051 2024-03-14 16:53:40.178709 superwise_api-1.2.0/superwise_api/client/models/source.py
--rw-r--r--   0        0        0     3409 2024-03-14 16:53:40.178709 superwise_api-1.2.0/superwise_api/client/models/source_azure_params.py
--rw-r--r--   0        0        0     5617 2024-03-14 16:53:40.178709 superwise_api-1.2.0/superwise_api/client/models/source_create.py
--rw-r--r--   0        0        0     3250 2024-03-14 16:53:40.178709 superwise_api-1.2.0/superwise_api/client/models/source_create_azure.py
--rw-r--r--   0        0        0     3162 2024-03-14 16:53:40.179709 superwise_api-1.2.0/superwise_api/client/models/source_create_gcs.py
--rw-r--r--   0        0        0     5687 2024-03-14 16:53:40.179709 superwise_api-1.2.0/superwise_api/client/models/source_create_payload.py
--rw-r--r--   0        0        0     3142 2024-03-14 16:53:40.179709 superwise_api-1.2.0/superwise_api/client/models/source_create_s3.py
--rw-r--r--   0        0        0     2781 2024-03-14 16:53:40.179709 superwise_api-1.2.0/superwise_api/client/models/source_gcs_params.py
--rw-r--r--   0        0        0     3533 2024-03-14 16:53:40.179709 superwise_api-1.2.0/superwise_api/client/models/source_get_azure.py
--rw-r--r--   0        0        0     3471 2024-03-14 16:53:40.179709 superwise_api-1.2.0/superwise_api/client/models/source_get_gcs.py
--rw-r--r--   0        0        0     3453 2024-03-14 16:53:40.180709 superwise_api-1.2.0/superwise_api/client/models/source_get_s3.py
--rw-r--r--   0        0        0     6147 2024-03-14 16:53:40.180709 superwise_api-1.2.0/superwise_api/client/models/source_response.py
--rw-r--r--   0        0        0     2815 2024-03-14 16:53:40.180709 superwise_api-1.2.0/superwise_api/client/models/source_s3_params.py
--rw-r--r--   0        0        0      706 2024-03-14 16:53:40.180709 superwise_api-1.2.0/superwise_api/client/models/source_type.py
--rw-r--r--   0        0        0     5595 2024-03-14 16:53:40.180709 superwise_api-1.2.0/superwise_api/client/models/source_update.py
--rw-r--r--   0        0        0     3143 2024-03-14 16:53:40.181709 superwise_api-1.2.0/superwise_api/client/models/source_update_gcs.py
--rw-r--r--   0        0        0     3127 2024-03-14 16:53:40.181709 superwise_api-1.2.0/superwise_api/client/models/source_update_s3.py
--rw-r--r--   0        0        0     1908 2024-03-14 16:53:40.181709 superwise_api-1.2.0/superwise_api/client/models/time_dimension.py
--rw-r--r--   0        0        0      736 2024-03-14 16:53:40.181709 superwise_api-1.2.0/superwise_api/client/models/time_range_unit.py
--rw-r--r--   0        0        0     9354 2024-03-14 16:53:40.181709 superwise_api-1.2.0/superwise_api/client/models/tool_config.py
--rw-r--r--   0        0        0     2339 2024-03-14 16:53:40.181709 superwise_api-1.2.0/superwise_api/client/models/tool_config_big_query.py
--rw-r--r--   0        0        0     2820 2024-03-14 16:53:40.182710 superwise_api-1.2.0/superwise_api/client/models/tool_config_pg_vector.py
--rw-r--r--   0        0        0     2563 2024-03-14 16:53:40.182710 superwise_api-1.2.0/superwise_api/client/models/tool_config_sql_database_mssql.py
--rw-r--r--   0        0        0     2563 2024-03-14 16:53:40.182710 superwise_api-1.2.0/superwise_api/client/models/tool_config_sql_database_my_sql.py
--rw-r--r--   0        0        0     2573 2024-03-14 16:53:40.182710 superwise_api-1.2.0/superwise_api/client/models/tool_config_sql_database_oracle.py
--rw-r--r--   0        0        0     2597 2024-03-14 16:53:40.182710 superwise_api-1.2.0/superwise_api/client/models/tool_config_sql_database_postgres.py
--rw-r--r--   0        0        0     2648 2024-03-14 16:53:40.182710 superwise_api-1.2.0/superwise_api/client/models/tool_create.py
--rw-r--r--   0        0        0     4813 2024-03-14 16:53:40.182710 superwise_api-1.2.0/superwise_api/client/models/tool_name.py
--rw-r--r--   0        0        0     4873 2024-03-14 16:53:40.183709 superwise_api-1.2.0/superwise_api/client/models/tool_name_update.py
--rw-r--r--   0        0        0     2911 2024-03-14 16:53:40.183709 superwise_api-1.2.0/superwise_api/client/models/tool_response.py
--rw-r--r--   0        0        0     4674 2024-03-14 16:53:40.183709 superwise_api-1.2.0/superwise_api/client/models/tool_type.py
--rw-r--r--   0        0        0     2863 2024-03-14 16:53:40.183709 superwise_api-1.2.0/superwise_api/client/models/tool_update.py
--rw-r--r--   0        0        0     4760 2024-03-14 16:53:40.183709 superwise_api-1.2.0/superwise_api/client/models/total.py
--rw-r--r--   0        0        0      720 2024-03-14 16:53:40.183709 superwise_api-1.2.0/superwise_api/client/models/type.py
--rw-r--r--   0        0        0     2537 2024-03-14 16:53:40.183709 superwise_api-1.2.0/superwise_api/client/models/validation_error.py
--rw-r--r--   0        0        0     2013 2024-03-14 16:53:40.183709 superwise_api-1.2.0/superwise_api/client/models/validation_error_detail.py
--rw-r--r--   0        0        0     4912 2024-03-14 16:53:40.183709 superwise_api-1.2.0/superwise_api/client/models/validation_error_loc_inner.py
--rw-r--r--   0        0        0     2512 2024-03-14 16:53:40.184710 superwise_api-1.2.0/superwise_api/client/models/validation_result.py
--rw-r--r--   0        0        0     4726 2024-03-14 16:53:40.184710 superwise_api-1.2.0/superwise_api/client/models/values.py
--rw-r--r--   0        0        0     4736 2024-03-14 16:53:40.184710 superwise_api-1.2.0/superwise_api/client/models/version.py
--rw-r--r--   0        0        0     5597 2024-03-14 16:53:40.184710 superwise_api-1.2.0/superwise_api/client/models/version1.py
--rw-r--r--   0        0        0     2593 2024-03-14 16:53:40.184710 superwise_api-1.2.0/superwise_api/client/models/vertex_ai_model_garden_embedding_model.py
--rw-r--r--   0        0        0      794 2024-03-14 16:53:40.184710 superwise_api-1.2.0/superwise_api/client/models/visualization_type.py
--rw-r--r--   0        0        0     2007 2024-03-14 16:53:40.184710 superwise_api-1.2.0/superwise_api/client/models/widget_meta.py
--rw-r--r--   0        0        0    13894 2024-03-14 16:53:40.185710 superwise_api-1.2.0/superwise_api/client/rest.py
--rw-r--r--   0        0        0     1184 2024-03-14 16:53:40.185710 superwise_api-1.2.0/superwise_api/config.py
--rw-r--r--   0        0        0        0 2024-03-14 16:53:40.295720 superwise_api-1.2.0/superwise_api/entities/__init__.py
--rw-r--r--   0        0        0     3584 2024-03-14 16:53:40.185710 superwise_api-1.2.0/superwise_api/entities/application.py
--rw-r--r--   0        0        0     2991 2024-03-14 16:53:40.185710 superwise_api-1.2.0/superwise_api/entities/dashboard.py
--rw-r--r--   0        0        0     3222 2024-03-14 16:53:40.185710 superwise_api-1.2.0/superwise_api/entities/dashboard_item.py
--rw-r--r--   0        0        0     4004 2024-03-14 16:53:40.185710 superwise_api-1.2.0/superwise_api/entities/dataset.py
--rw-r--r--   0        0        0     3638 2024-03-14 16:53:40.185710 superwise_api-1.2.0/superwise_api/entities/dataset_source.py
--rw-r--r--   0        0        0     3035 2024-03-14 16:53:40.185710 superwise_api-1.2.0/superwise_api/entities/destination.py
--rw-r--r--   0        0        0     1549 2024-03-14 16:53:40.186710 superwise_api-1.2.0/superwise_api/entities/integration.py
--rw-r--r--   0        0        0     1017 2024-03-14 16:53:40.186710 superwise_api-1.2.0/superwise_api/entities/model.py
--rw-r--r--   0        0        0     4797 2024-03-14 16:53:40.186710 superwise_api-1.2.0/superwise_api/entities/policy.py
--rw-r--r--   0        0        0     5410 2024-03-14 16:53:40.186710 superwise_api-1.2.0/superwise_api/entities/source.py
--rw-r--r--   0        0        0     3470 2024-03-14 16:53:40.186710 superwise_api-1.2.0/superwise_api/entities/tool.py
--rw-r--r--   0        0        0     1489 2024-03-14 16:53:40.186710 superwise_api-1.2.0/superwise_api/errors.py
--rw-r--r--   0        0        0     9202 2024-03-14 16:53:40.186710 superwise_api-1.2.0/superwise_api/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 16:53:40.297721 superwise_api-1.2.0/superwise_api/models/application/__init__.py
--rw-r--r--   0        0        0      524 2024-03-14 16:53:40.187710 superwise_api-1.2.0/superwise_api/models/application/application.py
--rw-r--r--   0        0        0      614 2024-03-14 16:53:40.187710 superwise_api-1.2.0/superwise_api/models/application/application_update.py
--rw-r--r--   0        0        0        0 2024-03-14 16:53:40.298721 superwise_api-1.2.0/superwise_api/models/dashboard/__init__.py
--rw-r--r--   0        0        0      838 2024-03-14 16:53:40.187710 superwise_api-1.2.0/superwise_api/models/dashboard/dashboard_response.py
--rw-r--r--   0        0        0     1261 2024-03-14 16:53:40.187710 superwise_api-1.2.0/superwise_api/models/dashboard/page_dashboard.py
--rw-r--r--   0        0        0        0 2024-03-14 16:53:40.298721 superwise_api-1.2.0/superwise_api/models/dashboard_item/__init__.py
--rw-r--r--   0        0        0     1333 2024-03-14 16:53:40.187710 superwise_api-1.2.0/superwise_api/models/dashboard_item/dashboard_item.py
--rw-r--r--   0        0        0     1499 2024-03-14 16:53:40.187710 superwise_api-1.2.0/superwise_api/models/dashboard_item/dashboard_item_create.py
--rw-r--r--   0        0        0     1280 2024-03-14 16:53:40.188710 superwise_api-1.2.0/superwise_api/models/dashboard_item/dashboard_item_response.py
--rw-r--r--   0        0        0     1328 2024-03-14 16:53:40.188710 superwise_api-1.2.0/superwise_api/models/dashboard_item/page_dashboard_item.py
--rw-r--r--   0        0        0     1308 2024-03-14 16:53:40.188710 superwise_api-1.2.0/superwise_api/models/dashboard_item/query.py
--rw-r--r--   0        0        0      799 2024-03-14 16:53:40.188710 superwise_api-1.2.0/superwise_api/models/dashboard_item/query_filter.py
--rw-r--r--   0        0        0     1131 2024-03-14 16:53:40.188710 superwise_api-1.2.0/superwise_api/models/dataset/__init__.py
--rw-r--r--   0        0        0     1439 2024-03-14 16:53:40.188710 superwise_api-1.2.0/superwise_api/models/dataset/dataset_response.py
--rw-r--r--   0        0        0      620 2024-03-14 16:53:40.188710 superwise_api-1.2.0/superwise_api/models/dataset/dataset_schema.py
--rw-r--r--   0        0        0      400 2024-03-14 16:53:40.188710 superwise_api-1.2.0/superwise_api/models/dataset/dataset_update.py
--rw-r--r--   0        0        0     1207 2024-03-14 16:53:40.188710 superwise_api-1.2.0/superwise_api/models/dataset/page_dataset_response.py
--rw-r--r--   0        0        0        0 2024-03-14 16:53:40.299721 superwise_api-1.2.0/superwise_api/models/model/__init__.py
--rw-r--r--   0        0        0      331 2024-03-14 16:53:40.189710 superwise_api-1.2.0/superwise_api/models/model/model_create.py
--rw-r--r--   0        0        0      688 2024-03-14 16:53:40.189710 superwise_api-1.2.0/superwise_api/models/policy/__init__.py
--rw-r--r--   0        0        0     1300 2024-03-14 16:53:40.189710 superwise_api-1.2.0/superwise_api/models/policy/page_policy_response.py
--rw-r--r--   0        0        0     1933 2024-03-14 16:53:40.189710 superwise_api-1.2.0/superwise_api/models/policy/policy_response.py
--rw-r--r--   0        0        0     3179 2024-03-14 16:53:40.189710 superwise_api-1.2.0/superwise_api/models/policy/query.py
--rw-r--r--   0        0        0      799 2024-03-14 16:53:40.189710 superwise_api-1.2.0/superwise_api/models/policy/query_filter.py
--rw-r--r--   0        0        0        0 2024-03-14 16:53:40.300721 superwise_api-1.2.0/superwise_api/models/tool/__init__.py
--rw-r--r--   0        0        0      165 2024-03-14 16:53:40.190710 superwise_api-1.2.0/superwise_api/models/tool/embeding_model.py
--rw-r--r--   0        0        0     1265 2024-03-14 16:53:40.190710 superwise_api-1.2.0/superwise_api/models/tool/page_tool_response.py
--rw-r--r--   0        0        0      288 2024-03-14 16:53:40.190710 superwise_api-1.2.0/superwise_api/models/tool/tool_config_pg_vector.py
--rw-r--r--   0        0        0     1281 2024-03-14 16:53:40.190710 superwise_api-1.2.0/superwise_api/models/tool/tool_create.py
--rw-r--r--   0        0        0     1196 2024-03-14 16:53:40.190710 superwise_api-1.2.0/superwise_api/models/tool/tool_response.py
--rw-r--r--   0        0        0    11338 2024-03-14 16:53:40.190710 superwise_api-1.2.0/superwise_api/superwise_client.py
--rw-r--r--   0        0        0     1241 1970-01-01 00:00:00.000000 superwise_api-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      487 2024-04-14 09:12:10.632515 superwise_api-1.3.0/README.md
+-rw-r--r--   0        0        0      828 2024-04-14 09:12:30.199422 superwise_api-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      276 2024-04-14 09:12:10.671519 superwise_api-1.3.0/superwise_api/__init__.py
+-rw-r--r--   0        0        0     9994 2024-04-14 09:12:10.671519 superwise_api-1.3.0/superwise_api/client/__init__.py
+-rw-r--r--   0        0        0      654 2024-04-14 09:12:10.672519 superwise_api-1.3.0/superwise_api/client/api/__init__.py
+-rw-r--r--   0        0        0    54734 2024-04-14 09:12:10.672519 superwise_api-1.3.0/superwise_api/client/api/applications_api.py
+-rw-r--r--   0        0        0    33591 2024-04-14 09:12:10.673519 superwise_api-1.3.0/superwise_api/client/api/dashboard_items_api.py
+-rw-r--r--   0        0        0    31775 2024-04-14 09:12:10.673519 superwise_api-1.3.0/superwise_api/client/api/dashboards_api.py
+-rw-r--r--   0        0        0    43860 2024-04-14 09:12:10.674519 superwise_api-1.3.0/superwise_api/client/api/dataset_api.py
+-rw-r--r--   0        0        0    38374 2024-04-14 09:12:10.674519 superwise_api-1.3.0/superwise_api/client/api/dataset_sources_api.py
+-rw-r--r--   0        0        0    36742 2024-04-14 09:12:10.675519 superwise_api-1.3.0/superwise_api/client/api/destinations_api.py
+-rw-r--r--   0        0        0    21619 2024-04-14 09:12:10.675519 superwise_api-1.3.0/superwise_api/client/api/integrations_api.py
+-rw-r--r--   0        0        0    44731 2024-04-14 09:12:10.676519 superwise_api-1.3.0/superwise_api/client/api/policies_api.py
+-rw-r--r--   0        0        0    38625 2024-04-14 09:12:10.676519 superwise_api-1.3.0/superwise_api/client/api/sources_api.py
+-rw-r--r--   0        0        0    28011 2024-04-14 09:12:10.677519 superwise_api-1.3.0/superwise_api/client/api_client.py
+-rw-r--r--   0        0        0      862 2024-04-14 09:12:10.677519 superwise_api-1.3.0/superwise_api/client/api_response.py
+-rw-r--r--   0        0        0    14478 2024-04-14 09:12:10.677519 superwise_api-1.3.0/superwise_api/client/configuration.py
+-rw-r--r--   0        0        0     5283 2024-04-14 09:12:10.677519 superwise_api-1.3.0/superwise_api/client/exceptions.py
+-rw-r--r--   0        0        0     8787 2024-04-14 09:12:10.678519 superwise_api-1.3.0/superwise_api/client/models/__init__.py
+-rw-r--r--   0        0        0      796 2024-04-14 09:12:10.678519 superwise_api-1.3.0/superwise_api/client/models/alert_on_status_direction.py
+-rw-r--r--   0        0        0     4546 2024-04-14 09:12:10.678519 superwise_api-1.3.0/superwise_api/client/models/application.py
+-rw-r--r--   0        0        0     3116 2024-04-14 09:12:10.678519 superwise_api-1.3.0/superwise_api/client/models/application_config.py
+-rw-r--r--   0        0        0     3299 2024-04-14 09:12:10.678519 superwise_api-1.3.0/superwise_api/client/models/application_config_payload.py
+-rw-r--r--   0        0        0     2634 2024-04-14 09:12:10.679519 superwise_api-1.3.0/superwise_api/client/models/application_create.py
+-rw-r--r--   0        0        0     4781 2024-04-14 09:12:10.679519 superwise_api-1.3.0/superwise_api/client/models/application_model.py
+-rw-r--r--   0        0        0     3046 2024-04-14 09:12:10.679519 superwise_api-1.3.0/superwise_api/client/models/application_response.py
+-rw-r--r--   0        0        0     4816 2024-04-14 09:12:10.679519 superwise_api-1.3.0/superwise_api/client/models/application_type.py
+-rw-r--r--   0        0        0     2816 2024-04-14 09:12:10.679519 superwise_api-1.3.0/superwise_api/client/models/application_update.py
+-rw-r--r--   0        0        0     2160 2024-04-14 09:12:10.680519 superwise_api-1.3.0/superwise_api/client/models/ask_config.py
+-rw-r--r--   0        0        0     3138 2024-04-14 09:12:10.680519 superwise_api-1.3.0/superwise_api/client/models/ask_request_payload.py
+-rw-r--r--   0        0        0     1837 2024-04-14 09:12:10.680519 superwise_api-1.3.0/superwise_api/client/models/ask_response_payload.py
+-rw-r--r--   0        0        0     2588 2024-04-14 09:12:10.680519 superwise_api-1.3.0/superwise_api/client/models/aws_credentials_request.py
+-rw-r--r--   0        0        0     2577 2024-04-14 09:12:10.680519 superwise_api-1.3.0/superwise_api/client/models/aws_credentials_response.py
+-rw-r--r--   0        0        0     2650 2024-04-14 09:12:10.681520 superwise_api-1.3.0/superwise_api/client/models/azure_credentials_request.py
+-rw-r--r--   0        0        0     2643 2024-04-14 09:12:10.681520 superwise_api-1.3.0/superwise_api/client/models/azure_credentials_response.py
+-rw-r--r--   0        0        0     1966 2024-04-14 09:12:10.681520 superwise_api-1.3.0/superwise_api/client/models/chat_history_entry.py
+-rw-r--r--   0        0        0     8587 2024-04-14 09:12:10.681520 superwise_api-1.3.0/superwise_api/client/models/config.py
+-rw-r--r--   0        0        0     5642 2024-04-14 09:12:10.681520 superwise_api-1.3.0/superwise_api/client/models/config1.py
+-rw-r--r--   0        0        0     4820 2024-04-14 09:12:10.682520 superwise_api-1.3.0/superwise_api/client/models/created_at.py
+-rw-r--r--   0        0        0     4756 2024-04-14 09:12:10.682520 superwise_api-1.3.0/superwise_api/client/models/created_by.py
+-rw-r--r--   0        0        0     2304 2024-04-14 09:12:10.682520 superwise_api-1.3.0/superwise_api/client/models/dashboard.py
+-rw-r--r--   0        0        0     1780 2024-04-14 09:12:10.682520 superwise_api-1.3.0/superwise_api/client/models/dashboard_create.py
+-rw-r--r--   0        0        0     3285 2024-04-14 09:12:10.682520 superwise_api-1.3.0/superwise_api/client/models/dashboard_item.py
+-rw-r--r--   0        0        0     3049 2024-04-14 09:12:10.682520 superwise_api-1.3.0/superwise_api/client/models/dashboard_item_create.py
+-rw-r--r--   0        0        0     3994 2024-04-14 09:12:10.682520 superwise_api-1.3.0/superwise_api/client/models/dashboard_item_query.py
+-rw-r--r--   0        0        0     4956 2024-04-14 09:12:10.682520 superwise_api-1.3.0/superwise_api/client/models/dashboard_item_query_order.py
+-rw-r--r--   0        0        0     2929 2024-04-14 09:12:10.683520 superwise_api-1.3.0/superwise_api/client/models/dashboard_item_update.py
+-rw-r--r--   0        0        0     1910 2024-04-14 09:12:10.683520 superwise_api-1.3.0/superwise_api/client/models/dashboard_update.py
+-rw-r--r--   0        0        0     4297 2024-04-14 09:12:10.683520 superwise_api-1.3.0/superwise_api/client/models/dataset_create.py
+-rw-r--r--   0        0        0     4756 2024-04-14 09:12:10.683520 superwise_api-1.3.0/superwise_api/client/models/dataset_id.py
+-rw-r--r--   0        0        0     3971 2024-04-14 09:12:10.683520 superwise_api-1.3.0/superwise_api/client/models/dataset_response.py
+-rw-r--r--   0        0        0     4317 2024-04-14 09:12:10.683520 superwise_api-1.3.0/superwise_api/client/models/dataset_source_create.py
+-rw-r--r--   0        0        0     2904 2024-04-14 09:12:10.684520 superwise_api-1.3.0/superwise_api/client/models/dataset_source_response.py
+-rw-r--r--   0        0        0     3355 2024-04-14 09:12:10.684520 superwise_api-1.3.0/superwise_api/client/models/dataset_source_response_with_source.py
+-rw-r--r--   0        0        0     2514 2024-04-14 09:12:10.684520 superwise_api-1.3.0/superwise_api/client/models/dataset_source_update.py
+-rw-r--r--   0        0        0     1769 2024-04-14 09:12:10.684520 superwise_api-1.3.0/superwise_api/client/models/dataset_tag.py
+-rw-r--r--   0        0        0     2632 2024-04-14 09:12:10.684520 superwise_api-1.3.0/superwise_api/client/models/dataset_update.py
+-rw-r--r--   0        0        0      678 2024-04-14 09:12:10.684520 superwise_api-1.3.0/superwise_api/client/models/datasource.py
+-rw-r--r--   0        0        0     6335 2024-04-14 09:12:10.684520 superwise_api-1.3.0/superwise_api/client/models/default_value.py
+-rw-r--r--   0        0        0     6127 2024-04-14 09:12:10.684520 superwise_api-1.3.0/superwise_api/client/models/default_value1.py
+-rw-r--r--   0        0        0     4776 2024-04-14 09:12:10.685520 superwise_api-1.3.0/superwise_api/client/models/description.py
+-rw-r--r--   0        0        0     2113 2024-04-14 09:12:10.685520 superwise_api-1.3.0/superwise_api/client/models/destination_create_base.py
+-rw-r--r--   0        0        0     2614 2024-04-14 09:12:10.685520 superwise_api-1.3.0/superwise_api/client/models/destination_response.py
+-rw-r--r--   0        0        0     1963 2024-04-14 09:12:10.685520 superwise_api-1.3.0/superwise_api/client/models/destination_update_base.py
+-rw-r--r--   0        0        0     5042 2024-04-14 09:12:10.685520 superwise_api-1.3.0/superwise_api/client/models/embedding_model.py
+-rw-r--r--   0        0        0     2226 2024-04-14 09:12:10.685520 superwise_api-1.3.0/superwise_api/client/models/filter.py
+-rw-r--r--   0        0        0     2384 2024-04-14 09:12:10.685520 superwise_api-1.3.0/superwise_api/client/models/gcp_credentials_request.py
+-rw-r--r--   0        0        0     2369 2024-04-14 09:12:10.685520 superwise_api-1.3.0/superwise_api/client/models/gcp_credentials_response.py
+-rw-r--r--   0        0        0      771 2024-04-14 09:12:10.686520 superwise_api-1.3.0/superwise_api/client/models/google_model_version.py
+-rw-r--r--   0        0        0      770 2024-04-14 09:12:10.686520 superwise_api-1.3.0/superwise_api/client/models/granularity.py
+-rw-r--r--   0        0        0     2375 2024-04-14 09:12:10.686520 superwise_api-1.3.0/superwise_api/client/models/http_validation_error.py
+-rw-r--r--   0        0        0      674 2024-04-14 09:12:10.686520 superwise_api-1.3.0/superwise_api/client/models/ingest_type.py
+-rw-r--r--   0        0        0     2478 2024-04-14 09:12:10.686520 superwise_api-1.3.0/superwise_api/client/models/integration_response.py
+-rw-r--r--   0        0        0      670 2024-04-14 09:12:10.686520 superwise_api-1.3.0/superwise_api/client/models/integration_type.py
+-rw-r--r--   0        0        0     2418 2024-04-14 09:12:10.686520 superwise_api-1.3.0/superwise_api/client/models/model_create.py
+-rw-r--r--   0        0        0     4736 2024-04-14 09:12:10.686520 superwise_api-1.3.0/superwise_api/client/models/model_id.py
+-rw-r--r--   0        0        0     2156 2024-04-14 09:12:10.687520 superwise_api-1.3.0/superwise_api/client/models/model_llm.py
+-rw-r--r--   0        0        0      736 2024-04-14 09:12:10.687520 superwise_api-1.3.0/superwise_api/client/models/model_provider.py
+-rw-r--r--   0        0        0     2788 2024-04-14 09:12:10.687520 superwise_api-1.3.0/superwise_api/client/models/model_response.py
+-rw-r--r--   0        0        0     1802 2024-04-14 09:12:10.687520 superwise_api-1.3.0/superwise_api/client/models/model_schema.py
+-rw-r--r--   0        0        0     5637 2024-04-14 09:12:10.687520 superwise_api-1.3.0/superwise_api/client/models/model_version.py
+-rw-r--r--   0        0        0     5717 2024-04-14 09:12:10.687520 superwise_api-1.3.0/superwise_api/client/models/model_version_response.py
+-rw-r--r--   0        0        0     4706 2024-04-14 09:12:10.688520 superwise_api-1.3.0/superwise_api/client/models/name.py
+-rw-r--r--   0        0        0     1009 2024-04-14 09:12:10.688520 superwise_api-1.3.0/superwise_api/client/models/open_ai_model_version.py
+-rw-r--r--   0        0        0     4697 2024-04-14 09:12:10.688520 superwise_api-1.3.0/superwise_api/client/models/order.py
+-rw-r--r--   0        0        0     4786 2024-04-14 09:12:10.688520 superwise_api-1.3.0/superwise_api/client/models/order1.py
+-rw-r--r--   0        0        0     4750 2024-04-14 09:12:10.688520 superwise_api-1.3.0/superwise_api/client/models/page.py
+-rw-r--r--   0        0        0     3719 2024-04-14 09:12:10.689520 superwise_api-1.3.0/superwise_api/client/models/page_application.py
+-rw-r--r--   0        0        0     3816 2024-04-14 09:12:10.689520 superwise_api-1.3.0/superwise_api/client/models/page_application_response.py
+-rw-r--r--   0        0        0     3093 2024-04-14 09:12:10.689520 superwise_api-1.3.0/superwise_api/client/models/page_dashboard.py
+-rw-r--r--   0        0        0     3142 2024-04-14 09:12:10.689520 superwise_api-1.3.0/superwise_api/client/models/page_dashboard_item.py
+-rw-r--r--   0        0        0     3166 2024-04-14 09:12:10.689520 superwise_api-1.3.0/superwise_api/client/models/page_dataset_response.py
+-rw-r--r--   0        0        0     3361 2024-04-14 09:12:10.689520 superwise_api-1.3.0/superwise_api/client/models/page_dataset_source_response_with_source.py
+-rw-r--r--   0        0        0     3214 2024-04-14 09:12:10.689520 superwise_api-1.3.0/superwise_api/client/models/page_destination_response.py
+-rw-r--r--   0        0        0     3214 2024-04-14 09:12:10.690520 superwise_api-1.3.0/superwise_api/client/models/page_integration_response.py
+-rw-r--r--   0        0        0     3744 2024-04-14 09:12:10.690520 superwise_api-1.3.0/superwise_api/client/models/page_model_response.py
+-rw-r--r--   0        0        0     3154 2024-04-14 09:12:10.690520 superwise_api-1.3.0/superwise_api/client/models/page_policy_response.py
+-rw-r--r--   0        0        0     3154 2024-04-14 09:12:10.690520 superwise_api-1.3.0/superwise_api/client/models/page_source_response.py
+-rw-r--r--   0        0        0     3732 2024-04-14 09:12:10.690520 superwise_api-1.3.0/superwise_api/client/models/page_tool_response.py
+-rw-r--r--   0        0        0     4760 2024-04-14 09:12:10.690520 superwise_api-1.3.0/superwise_api/client/models/pages.py
+-rw-r--r--   0        0        0     8597 2024-04-14 09:12:10.690520 superwise_api-1.3.0/superwise_api/client/models/payload.py
+-rw-r--r--   0        0        0     4615 2024-04-14 09:12:10.691521 superwise_api-1.3.0/superwise_api/client/models/policy_create.py
+-rw-r--r--   0        0        0     3876 2024-04-14 09:12:10.691521 superwise_api-1.3.0/superwise_api/client/models/policy_query.py
+-rw-r--r--   0        0        0     2314 2024-04-14 09:12:10.691521 superwise_api-1.3.0/superwise_api/client/models/policy_query_filter.py
+-rw-r--r--   0        0        0     1842 2024-04-14 09:12:10.691521 superwise_api-1.3.0/superwise_api/client/models/policy_query_order.py
+-rw-r--r--   0        0        0     5592 2024-04-14 09:12:10.691521 superwise_api-1.3.0/superwise_api/client/models/policy_response.py
+-rw-r--r--   0        0        0      740 2024-04-14 09:12:10.692521 superwise_api-1.3.0/superwise_api/client/models/policy_status.py
+-rw-r--r--   0        0        0     4020 2024-04-14 09:12:10.692521 superwise_api-1.3.0/superwise_api/client/models/policy_update.py
+-rw-r--r--   0        0        0     4726 2024-04-14 09:12:10.692521 superwise_api-1.3.0/superwise_api/client/models/prompt.py
+-rw-r--r--   0        0        0     4746 2024-04-14 09:12:10.692521 superwise_api-1.3.0/superwise_api/client/models/provider.py
+-rw-r--r--   0        0        0     3815 2024-04-14 09:12:10.692521 superwise_api-1.3.0/superwise_api/client/models/query.py
+-rw-r--r--   0        0        0      748 2024-04-14 09:12:10.692521 superwise_api-1.3.0/superwise_api/client/models/query_type.py
+-rw-r--r--   0        0        0      629 2024-04-14 09:12:10.693521 superwise_api-1.3.0/superwise_api/client/models/role.py
+-rw-r--r--   0        0        0     2100 2024-04-14 09:12:10.693521 superwise_api-1.3.0/superwise_api/client/models/schema_item.py
+-rw-r--r--   0        0        0     1810 2024-04-14 09:12:10.693521 superwise_api-1.3.0/superwise_api/client/models/schema_update.py
+-rw-r--r--   0        0        0     2908 2024-04-14 09:12:10.693521 superwise_api-1.3.0/superwise_api/client/models/schema_update_item.py
+-rw-r--r--   0        0        0     4750 2024-04-14 09:12:10.693521 superwise_api-1.3.0/superwise_api/client/models/size.py
+-rw-r--r--   0        0        0     6051 2024-04-14 09:12:10.693521 superwise_api-1.3.0/superwise_api/client/models/source.py
+-rw-r--r--   0        0        0     3409 2024-04-14 09:12:10.694521 superwise_api-1.3.0/superwise_api/client/models/source_azure_params.py
+-rw-r--r--   0        0        0     5617 2024-04-14 09:12:10.694521 superwise_api-1.3.0/superwise_api/client/models/source_create.py
+-rw-r--r--   0        0        0     4059 2024-04-14 09:12:10.694521 superwise_api-1.3.0/superwise_api/client/models/source_create_azure.py
+-rw-r--r--   0        0        0     4001 2024-04-14 09:12:10.694521 superwise_api-1.3.0/superwise_api/client/models/source_create_gcs.py
+-rw-r--r--   0        0        0     5687 2024-04-14 09:12:10.694521 superwise_api-1.3.0/superwise_api/client/models/source_create_payload.py
+-rw-r--r--   0        0        0     3983 2024-04-14 09:12:10.695521 superwise_api-1.3.0/superwise_api/client/models/source_create_s3.py
+-rw-r--r--   0        0        0     2781 2024-04-14 09:12:10.695521 superwise_api-1.3.0/superwise_api/client/models/source_gcs_params.py
+-rw-r--r--   0        0        0     3533 2024-04-14 09:12:10.695521 superwise_api-1.3.0/superwise_api/client/models/source_get_azure.py
+-rw-r--r--   0        0        0     3471 2024-04-14 09:12:10.695521 superwise_api-1.3.0/superwise_api/client/models/source_get_gcs.py
+-rw-r--r--   0        0        0     3453 2024-04-14 09:12:10.695521 superwise_api-1.3.0/superwise_api/client/models/source_get_s3.py
+-rw-r--r--   0        0        0     6147 2024-04-14 09:12:10.695521 superwise_api-1.3.0/superwise_api/client/models/source_response.py
+-rw-r--r--   0        0        0     2815 2024-04-14 09:12:10.696521 superwise_api-1.3.0/superwise_api/client/models/source_s3_params.py
+-rw-r--r--   0        0        0      706 2024-04-14 09:12:10.696521 superwise_api-1.3.0/superwise_api/client/models/source_type.py
+-rw-r--r--   0        0        0     5595 2024-04-14 09:12:10.696521 superwise_api-1.3.0/superwise_api/client/models/source_update.py
+-rw-r--r--   0        0        0     3143 2024-04-14 09:12:10.696521 superwise_api-1.3.0/superwise_api/client/models/source_update_gcs.py
+-rw-r--r--   0        0        0     3127 2024-04-14 09:12:10.696521 superwise_api-1.3.0/superwise_api/client/models/source_update_s3.py
+-rw-r--r--   0        0        0     1908 2024-04-14 09:12:10.696521 superwise_api-1.3.0/superwise_api/client/models/time_dimension.py
+-rw-r--r--   0        0        0      736 2024-04-14 09:12:10.697521 superwise_api-1.3.0/superwise_api/client/models/time_range_unit.py
+-rw-r--r--   0        0        0     9354 2024-04-14 09:12:10.697521 superwise_api-1.3.0/superwise_api/client/models/tool_config.py
+-rw-r--r--   0        0        0     2339 2024-04-14 09:12:10.697521 superwise_api-1.3.0/superwise_api/client/models/tool_config_big_query.py
+-rw-r--r--   0        0        0     2820 2024-04-14 09:12:10.697521 superwise_api-1.3.0/superwise_api/client/models/tool_config_pg_vector.py
+-rw-r--r--   0        0        0     2181 2024-04-14 09:12:10.697521 superwise_api-1.3.0/superwise_api/client/models/tool_config_sql_database.py
+-rw-r--r--   0        0        0     2563 2024-04-14 09:12:10.697521 superwise_api-1.3.0/superwise_api/client/models/tool_config_sql_database_mssql.py
+-rw-r--r--   0        0        0     2563 2024-04-14 09:12:10.698521 superwise_api-1.3.0/superwise_api/client/models/tool_config_sql_database_my_sql.py
+-rw-r--r--   0        0        0     2573 2024-04-14 09:12:10.698521 superwise_api-1.3.0/superwise_api/client/models/tool_config_sql_database_oracle.py
+-rw-r--r--   0        0        0     2597 2024-04-14 09:12:10.698521 superwise_api-1.3.0/superwise_api/client/models/tool_config_sql_database_postgres.py
+-rw-r--r--   0        0        0     2648 2024-04-14 09:12:10.698521 superwise_api-1.3.0/superwise_api/client/models/tool_create.py
+-rw-r--r--   0        0        0     2439 2024-04-14 09:12:10.698521 superwise_api-1.3.0/superwise_api/client/models/tool_def_input.py
+-rw-r--r--   0        0        0     2636 2024-04-14 09:12:10.698521 superwise_api-1.3.0/superwise_api/client/models/tool_def_output.py
+-rw-r--r--   0        0        0     4813 2024-04-14 09:12:10.698521 superwise_api-1.3.0/superwise_api/client/models/tool_name.py
+-rw-r--r--   0        0        0     4873 2024-04-14 09:12:10.698521 superwise_api-1.3.0/superwise_api/client/models/tool_name_update.py
+-rw-r--r--   0        0        0     2911 2024-04-14 09:12:10.698521 superwise_api-1.3.0/superwise_api/client/models/tool_response.py
+-rw-r--r--   0        0        0     4674 2024-04-14 09:12:10.699521 superwise_api-1.3.0/superwise_api/client/models/tool_type.py
+-rw-r--r--   0        0        0     2863 2024-04-14 09:12:10.699521 superwise_api-1.3.0/superwise_api/client/models/tool_update.py
+-rw-r--r--   0        0        0     4760 2024-04-14 09:12:10.699521 superwise_api-1.3.0/superwise_api/client/models/total.py
+-rw-r--r--   0        0        0      720 2024-04-14 09:12:10.699521 superwise_api-1.3.0/superwise_api/client/models/type.py
+-rw-r--r--   0        0        0     4820 2024-04-14 09:12:10.699521 superwise_api-1.3.0/superwise_api/client/models/updated_at.py
+-rw-r--r--   0        0        0     2537 2024-04-14 09:12:10.699521 superwise_api-1.3.0/superwise_api/client/models/validation_error.py
+-rw-r--r--   0        0        0     2013 2024-04-14 09:12:10.699521 superwise_api-1.3.0/superwise_api/client/models/validation_error_detail.py
+-rw-r--r--   0        0        0     4912 2024-04-14 09:12:10.699521 superwise_api-1.3.0/superwise_api/client/models/validation_error_loc_inner.py
+-rw-r--r--   0        0        0     2512 2024-04-14 09:12:10.700521 superwise_api-1.3.0/superwise_api/client/models/validation_result.py
+-rw-r--r--   0        0        0     4726 2024-04-14 09:12:10.700521 superwise_api-1.3.0/superwise_api/client/models/values.py
+-rw-r--r--   0        0        0     4736 2024-04-14 09:12:10.700521 superwise_api-1.3.0/superwise_api/client/models/version.py
+-rw-r--r--   0        0        0     5597 2024-04-14 09:12:10.700521 superwise_api-1.3.0/superwise_api/client/models/version1.py
+-rw-r--r--   0        0        0     2593 2024-04-14 09:12:10.700521 superwise_api-1.3.0/superwise_api/client/models/vertex_ai_model_garden_embedding_model.py
+-rw-r--r--   0        0        0      794 2024-04-14 09:12:10.700521 superwise_api-1.3.0/superwise_api/client/models/visualization_type.py
+-rw-r--r--   0        0        0     2355 2024-04-14 09:12:10.700521 superwise_api-1.3.0/superwise_api/client/models/widget_meta.py
+-rw-r--r--   0        0        0    13894 2024-04-14 09:12:10.701521 superwise_api-1.3.0/superwise_api/client/rest.py
+-rw-r--r--   0        0        0     1184 2024-04-14 09:12:10.701521 superwise_api-1.3.0/superwise_api/config.py
+-rw-r--r--   0        0        0        0 2024-04-14 09:12:10.870538 superwise_api-1.3.0/superwise_api/entities/__init__.py
+-rw-r--r--   0        0        0     3035 2024-04-14 09:12:10.701521 superwise_api-1.3.0/superwise_api/entities/application.py
+-rw-r--r--   0        0        0     2991 2024-04-14 09:12:10.702522 superwise_api-1.3.0/superwise_api/entities/dashboard.py
+-rw-r--r--   0        0        0     3222 2024-04-14 09:12:10.702522 superwise_api-1.3.0/superwise_api/entities/dashboard_item.py
+-rw-r--r--   0        0        0     4004 2024-04-14 09:12:10.702522 superwise_api-1.3.0/superwise_api/entities/dataset.py
+-rw-r--r--   0        0        0     3638 2024-04-14 09:12:10.702522 superwise_api-1.3.0/superwise_api/entities/dataset_source.py
+-rw-r--r--   0        0        0     3035 2024-04-14 09:12:10.703522 superwise_api-1.3.0/superwise_api/entities/destination.py
+-rw-r--r--   0        0        0     1549 2024-04-14 09:12:10.703522 superwise_api-1.3.0/superwise_api/entities/integration.py
+-rw-r--r--   0        0        0     4797 2024-04-14 09:12:10.703522 superwise_api-1.3.0/superwise_api/entities/policy.py
+-rw-r--r--   0        0        0     5410 2024-04-14 09:12:10.703522 superwise_api-1.3.0/superwise_api/entities/source.py
+-rw-r--r--   0        0        0     1489 2024-04-14 09:12:10.703522 superwise_api-1.3.0/superwise_api/errors.py
+-rw-r--r--   0        0        0     7125 2024-04-14 09:12:10.703522 superwise_api-1.3.0/superwise_api/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 09:12:10.871538 superwise_api-1.3.0/superwise_api/models/application/__init__.py
+-rw-r--r--   0        0        0      686 2024-04-14 09:12:10.704522 superwise_api-1.3.0/superwise_api/models/application/enums.py
+-rw-r--r--   0        0        0     3776 2024-04-14 09:12:10.704522 superwise_api-1.3.0/superwise_api/models/application/schemas.py
+-rw-r--r--   0        0        0        0 2024-04-14 09:12:10.872538 superwise_api-1.3.0/superwise_api/models/dashboard/__init__.py
+-rw-r--r--   0        0        0      838 2024-04-14 09:12:10.704522 superwise_api-1.3.0/superwise_api/models/dashboard/dashboard_response.py
+-rw-r--r--   0        0        0     1261 2024-04-14 09:12:10.704522 superwise_api-1.3.0/superwise_api/models/dashboard/page_dashboard.py
+-rw-r--r--   0        0        0        0 2024-04-14 09:12:10.873538 superwise_api-1.3.0/superwise_api/models/dashboard_item/__init__.py
+-rw-r--r--   0        0        0     1333 2024-04-14 09:12:10.705522 superwise_api-1.3.0/superwise_api/models/dashboard_item/dashboard_item.py
+-rw-r--r--   0        0        0     1499 2024-04-14 09:12:10.705522 superwise_api-1.3.0/superwise_api/models/dashboard_item/dashboard_item_create.py
+-rw-r--r--   0        0        0     1280 2024-04-14 09:12:10.705522 superwise_api-1.3.0/superwise_api/models/dashboard_item/dashboard_item_response.py
+-rw-r--r--   0        0        0     1328 2024-04-14 09:12:10.705522 superwise_api-1.3.0/superwise_api/models/dashboard_item/page_dashboard_item.py
+-rw-r--r--   0        0        0     1308 2024-04-14 09:12:10.705522 superwise_api-1.3.0/superwise_api/models/dashboard_item/query.py
+-rw-r--r--   0        0        0      799 2024-04-14 09:12:10.705522 superwise_api-1.3.0/superwise_api/models/dashboard_item/query_filter.py
+-rw-r--r--   0        0        0     1131 2024-04-14 09:12:10.705522 superwise_api-1.3.0/superwise_api/models/dataset/__init__.py
+-rw-r--r--   0        0        0     1439 2024-04-14 09:12:10.706522 superwise_api-1.3.0/superwise_api/models/dataset/dataset_response.py
+-rw-r--r--   0        0        0      620 2024-04-14 09:12:10.706522 superwise_api-1.3.0/superwise_api/models/dataset/dataset_schema.py
+-rw-r--r--   0        0        0      400 2024-04-14 09:12:10.706522 superwise_api-1.3.0/superwise_api/models/dataset/dataset_update.py
+-rw-r--r--   0        0        0     1207 2024-04-14 09:12:10.706522 superwise_api-1.3.0/superwise_api/models/dataset/page_dataset_response.py
+-rw-r--r--   0        0        0      688 2024-04-14 09:12:10.706522 superwise_api-1.3.0/superwise_api/models/policy/__init__.py
+-rw-r--r--   0        0        0     1300 2024-04-14 09:12:10.706522 superwise_api-1.3.0/superwise_api/models/policy/page_policy_response.py
+-rw-r--r--   0        0        0     1933 2024-04-14 09:12:10.706522 superwise_api-1.3.0/superwise_api/models/policy/policy_response.py
+-rw-r--r--   0        0        0     3179 2024-04-14 09:12:10.707522 superwise_api-1.3.0/superwise_api/models/policy/query.py
+-rw-r--r--   0        0        0      799 2024-04-14 09:12:10.707522 superwise_api-1.3.0/superwise_api/models/policy/query_filter.py
+-rw-r--r--   0        0        0        0 2024-04-14 09:12:10.874538 superwise_api-1.3.0/superwise_api/models/tool/__init__.py
+-rw-r--r--   0        0        0      749 2024-04-14 09:12:10.707522 superwise_api-1.3.0/superwise_api/models/tool/enums.py
+-rw-r--r--   0        0        0     3208 2024-04-14 09:12:10.707522 superwise_api-1.3.0/superwise_api/models/tool/schemas.py
+-rw-r--r--   0        0        0    10222 2024-04-14 09:12:10.707522 superwise_api-1.3.0/superwise_api/superwise_client.py
+-rw-r--r--   0        0        0     1241 1970-01-01 00:00:00.000000 superwise_api-1.3.0/PKG-INFO
```

### Comparing `superwise_api-1.2.0/pyproject.toml` & `superwise_api-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "superwise-api"
 packages = [{include = "superwise_api", from = "."}]
-version = "1.2.0"
+version = "1.3.0"
 description = "Superwise SDK for Python"
 authors = ["Superwise"]
 license = "MIT"
 readme = "README.md"
 keywords = ["OpenAPI", "SuperwiseSDK"]
 include = ["superwise_api/client/py.typed"]
```

### Comparing `superwise_api-1.2.0/superwise_api/client/__init__.py` & `superwise_api-1.3.0/superwise_api/client/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 # flake8: noqa
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 __version__ = "1.0.0"
@@ -18,18 +18,16 @@
 from superwise_api.client.api.applications_api import ApplicationsApi
 from superwise_api.client.api.dashboard_items_api import DashboardItemsApi
 from superwise_api.client.api.dashboards_api import DashboardsApi
 from superwise_api.client.api.dataset_api import DatasetApi
 from superwise_api.client.api.dataset_sources_api import DatasetSourcesApi
 from superwise_api.client.api.destinations_api import DestinationsApi
 from superwise_api.client.api.integrations_api import IntegrationsApi
-from superwise_api.client.api.models_api import ModelsApi
 from superwise_api.client.api.policies_api import PoliciesApi
 from superwise_api.client.api.sources_api import SourcesApi
-from superwise_api.client.api.tools_api import ToolsApi
 
 # import ApiClient
 from superwise_api.client.api_response import ApiResponse
 from superwise_api.client.api_client import ApiClient
 from superwise_api.client.configuration import Configuration
 from superwise_api.client.exceptions import OpenApiException
 from superwise_api.client.exceptions import ApiTypeError
@@ -38,34 +36,35 @@
 from superwise_api.client.exceptions import ApiAttributeError
 from superwise_api.client.exceptions import ApiException
 
 # import models into sdk package
 from superwise_api.client.models.aws_credentials_request import AWSCredentialsRequest
 from superwise_api.client.models.aws_credentials_response import AWSCredentialsResponse
 from superwise_api.client.models.alert_on_status_direction import AlertOnStatusDirection
-from superwise_api.client.models.application_create import ApplicationCreate
-from superwise_api.client.models.application_response import ApplicationResponse
-from superwise_api.client.models.application_update import ApplicationUpdate
-from superwise_api.client.models.ask_config import AskConfig
+from superwise_api.client.models.application import Application
+from superwise_api.client.models.application_config import ApplicationConfig
+from superwise_api.client.models.application_config_payload import ApplicationConfigPayload
+from superwise_api.client.models.application_model import ApplicationModel
 from superwise_api.client.models.ask_request_payload import AskRequestPayload
-from superwise_api.client.models.ask_response_payload import AskResponsePayload
 from superwise_api.client.models.azure_credentials_request import AzureCredentialsRequest
 from superwise_api.client.models.azure_credentials_response import AzureCredentialsResponse
 from superwise_api.client.models.chat_history_entry import ChatHistoryEntry
 from superwise_api.client.models.config import Config
-from superwise_api.client.models.config1 import Config1
+from superwise_api.client.models.created_at import CreatedAt
 from superwise_api.client.models.created_by import CreatedBy
 from superwise_api.client.models.dashboard import Dashboard
 from superwise_api.client.models.dashboard_create import DashboardCreate
 from superwise_api.client.models.dashboard_item import DashboardItem
 from superwise_api.client.models.dashboard_item_create import DashboardItemCreate
 from superwise_api.client.models.dashboard_item_query import DashboardItemQuery
 from superwise_api.client.models.dashboard_item_query_order import DashboardItemQueryOrder
+from superwise_api.client.models.dashboard_item_update import DashboardItemUpdate
 from superwise_api.client.models.dashboard_update import DashboardUpdate
 from superwise_api.client.models.dataset_create import DatasetCreate
+from superwise_api.client.models.dataset_id import DatasetId
 from superwise_api.client.models.dataset_response import DatasetResponse
 from superwise_api.client.models.dataset_source_create import DatasetSourceCreate
 from superwise_api.client.models.dataset_source_response import DatasetSourceResponse
 from superwise_api.client.models.dataset_source_response_with_source import DatasetSourceResponseWithSource
 from superwise_api.client.models.dataset_source_update import DatasetSourceUpdate
 from superwise_api.client.models.dataset_tag import DatasetTag
 from superwise_api.client.models.dataset_update import DatasetUpdate
@@ -80,46 +79,40 @@
 from superwise_api.client.models.gcp_credentials_response import GCPCredentialsResponse
 from superwise_api.client.models.google_model_version import GoogleModelVersion
 from superwise_api.client.models.granularity import Granularity
 from superwise_api.client.models.http_validation_error import HTTPValidationError
 from superwise_api.client.models.ingest_type import IngestType
 from superwise_api.client.models.integration_response import IntegrationResponse
 from superwise_api.client.models.integration_type import IntegrationType
-from superwise_api.client.models.model_create import ModelCreate
-from superwise_api.client.models.model_id import ModelId
+from superwise_api.client.models.model_llm import ModelLLM
 from superwise_api.client.models.model_provider import ModelProvider
-from superwise_api.client.models.model_response import ModelResponse
 from superwise_api.client.models.model_schema import ModelSchema
 from superwise_api.client.models.model_version import ModelVersion
-from superwise_api.client.models.model_version_response import ModelVersionResponse
 from superwise_api.client.models.name import Name
 from superwise_api.client.models.open_ai_model_version import OpenAIModelVersion
 from superwise_api.client.models.page import Page
-from superwise_api.client.models.page_application_response import PageApplicationResponse
+from superwise_api.client.models.page_application import PageApplication
 from superwise_api.client.models.page_dashboard import PageDashboard
 from superwise_api.client.models.page_dashboard_item import PageDashboardItem
 from superwise_api.client.models.page_dataset_response import PageDatasetResponse
 from superwise_api.client.models.page_dataset_source_response_with_source import PageDatasetSourceResponseWithSource
 from superwise_api.client.models.page_destination_response import PageDestinationResponse
 from superwise_api.client.models.page_integration_response import PageIntegrationResponse
-from superwise_api.client.models.page_model_response import PageModelResponse
 from superwise_api.client.models.page_policy_response import PagePolicyResponse
 from superwise_api.client.models.page_source_response import PageSourceResponse
-from superwise_api.client.models.page_tool_response import PageToolResponse
 from superwise_api.client.models.pages import Pages
 from superwise_api.client.models.payload import Payload
 from superwise_api.client.models.policy_create import PolicyCreate
 from superwise_api.client.models.policy_query import PolicyQuery
 from superwise_api.client.models.policy_query_filter import PolicyQueryFilter
 from superwise_api.client.models.policy_query_order import PolicyQueryOrder
 from superwise_api.client.models.policy_response import PolicyResponse
 from superwise_api.client.models.policy_status import PolicyStatus
 from superwise_api.client.models.policy_update import PolicyUpdate
 from superwise_api.client.models.prompt import Prompt
-from superwise_api.client.models.provider import Provider
 from superwise_api.client.models.query_type import QueryType
 from superwise_api.client.models.role import Role
 from superwise_api.client.models.schema_item import SchemaItem
 from superwise_api.client.models.schema_update import SchemaUpdate
 from superwise_api.client.models.schema_update_item import SchemaUpdateItem
 from superwise_api.client.models.size import Size
 from superwise_api.client.models.source import Source
@@ -142,22 +135,19 @@
 from superwise_api.client.models.time_range_unit import TimeRangeUnit
 from superwise_api.client.models.tool_config_big_query import ToolConfigBigQuery
 from superwise_api.client.models.tool_config_pg_vector import ToolConfigPGVector
 from superwise_api.client.models.tool_config_sql_database_mssql import ToolConfigSQLDatabaseMSSQL
 from superwise_api.client.models.tool_config_sql_database_my_sql import ToolConfigSQLDatabaseMySQL
 from superwise_api.client.models.tool_config_sql_database_oracle import ToolConfigSQLDatabaseOracle
 from superwise_api.client.models.tool_config_sql_database_postgres import ToolConfigSQLDatabasePostgres
-from superwise_api.client.models.tool_create import ToolCreate
-from superwise_api.client.models.tool_name import ToolName
-from superwise_api.client.models.tool_name_update import ToolNameUpdate
-from superwise_api.client.models.tool_response import ToolResponse
-from superwise_api.client.models.tool_type import ToolType
-from superwise_api.client.models.tool_update import ToolUpdate
+from superwise_api.client.models.tool_def_input import ToolDefInput
+from superwise_api.client.models.tool_def_output import ToolDefOutput
 from superwise_api.client.models.total import Total
 from superwise_api.client.models.type import Type
+from superwise_api.client.models.updated_at import UpdatedAt
 from superwise_api.client.models.validation_error import ValidationError
 from superwise_api.client.models.validation_error_detail import ValidationErrorDetail
 from superwise_api.client.models.validation_error_loc_inner import ValidationErrorLocInner
 from superwise_api.client.models.validation_result import ValidationResult
 from superwise_api.client.models.values import Values
 from superwise_api.client.models.vertex_ai_model_garden_embedding_model import VertexAIModelGardenEmbeddingModel
 from superwise_api.client.models.visualization_type import VisualizationType
```

### Comparing `superwise_api-1.2.0/superwise_api/client/api/__init__.py` & `superwise_api-1.3.0/superwise_api/client/api/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,11 +3,9 @@
 from superwise_api.client.api.applications_api import ApplicationsApi
 from superwise_api.client.api.dashboard_items_api import DashboardItemsApi
 from superwise_api.client.api.dashboards_api import DashboardsApi
 from superwise_api.client.api.dataset_api import DatasetApi
 from superwise_api.client.api.dataset_sources_api import DatasetSourcesApi
 from superwise_api.client.api.destinations_api import DestinationsApi
 from superwise_api.client.api.integrations_api import IntegrationsApi
-from superwise_api.client.api.models_api import ModelsApi
 from superwise_api.client.api.policies_api import PoliciesApi
 from superwise_api.client.api.sources_api import SourcesApi
-from superwise_api.client.api.tools_api import ToolsApi
```

### Comparing `superwise_api-1.2.0/superwise_api/client/api/applications_api.py` & `superwise_api-1.3.0/superwise_api/client/api/applications_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import io
 import re  # noqa: F401
 import warnings
@@ -21,26 +21,20 @@
 from pydantic import validate_arguments
 from pydantic import ValidationError
 from typing_extensions import Annotated
 
 from superwise_api.client.api_client import ApiClient
 from superwise_api.client.api_response import ApiResponse
 from superwise_api.client.exceptions import ApiTypeError
-from superwise_api.client.exceptions import ApiValueError
-from superwise_api.client.models.application_create import ApplicationCreate
-from superwise_api.client.models.application_response import ApplicationResponse
-from superwise_api.client.models.application_update import ApplicationUpdate
-from superwise_api.client.models.ask_request_payload import AskRequestPayload
-from superwise_api.client.models.ask_response_payload import AskResponsePayload
-from superwise_api.client.models.page_application_response import PageApplicationResponse
-from superwise_api.client.models.page_tool_response import PageToolResponse
+from superwise_api.client.models import Application
+from superwise_api.client.models import ApplicationConfigPayload
+from superwise_api.client.models import AskRequestPayload
+from superwise_api.client.models import ModelLLM
+from superwise_api.client.models.page_application import PageApplication
 from superwise_api.client.models.payload import Payload
-from superwise_api.client.models.tool_create import ToolCreate
-from superwise_api.client.models.tool_response import ToolResponse
-from superwise_api.client.models.tool_update import ToolUpdate
 
 
 class ApplicationsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -48,62 +42,54 @@
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def ask(
-        self, application_id: StrictStr, ask_request_payload: AskRequestPayload, **kwargs
-    ) -> AskResponsePayload:  # noqa: E501
-        """Ask  # noqa: E501
+    def ask_application(self, ask_request_payload: Any, **kwargs) -> object:  # noqa: E501
+        """Ask Application  # noqa: E501
 
-        Ask the application a question.  Parameters:  - **payload**: Instance of AskRequestPayload model.     - **input**: Input to the application.     - **config**: Configuration for the application is an ApplicationCreate model.         - **name**: Name of the application.         - **model_id**: UUID of the model.         - **prompt**: Prompt for the application.     - **chat_history**: Chat history for the application is a List[ChatHistoryEntry].         - **role**: Role of the chat history entry. (HUMAN or AI)         - **message**: Message of the chat history entry.  # noqa: E501
+        Ask an application.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.ask(application_id, ask_request_payload, async_req=True)
+        >>> thread = api.ask_application(ask_request_payload, async_req=True)
         >>> result = thread.get()
 
-        :param application_id: (required)
-        :type application_id: str
         :param ask_request_payload: (required)
         :type ask_request_payload: AskRequestPayload
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: AskResponsePayload
+        :rtype: object
         """
         kwargs["_return_http_data_only"] = True
         if "_preload_content" in kwargs:
-            message = "Error! Please call the ask_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            message = "Error! Please call the ask_application_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
-        return self.ask_with_http_info(application_id, ask_request_payload, **kwargs)  # noqa: E501
+        return self.ask_application_with_http_info(ask_request_payload, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def ask_with_http_info(
-        self, application_id: StrictStr, ask_request_payload: AskRequestPayload, **kwargs
-    ) -> ApiResponse:  # noqa: E501
-        """Ask  # noqa: E501
+    def ask_application_with_http_info(self, ask_request_payload: Any, **kwargs) -> ApiResponse:  # noqa: E501
+        """Ask Application  # noqa: E501
 
-        Ask the application a question.  Parameters:  - **payload**: Instance of AskRequestPayload model.     - **input**: Input to the application.     - **config**: Configuration for the application is an ApplicationCreate model.         - **name**: Name of the application.         - **model_id**: UUID of the model.         - **prompt**: Prompt for the application.     - **chat_history**: Chat history for the application is a List[ChatHistoryEntry].         - **role**: Role of the chat history entry. (HUMAN or AI)         - **message**: Message of the chat history entry.  # noqa: E501
+        Ask an application.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.ask_with_http_info(application_id, ask_request_payload, async_req=True)
+        >>> thread = api.ask_application_with_http_info(ask_request_payload, async_req=True)
         >>> result = thread.get()
 
-        :param application_id: (required)
-        :type application_id: str
         :param ask_request_payload: (required)
         :type ask_request_payload: AskRequestPayload
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
@@ -120,20 +106,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(AskResponsePayload, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
-        _all_params = ["application_id", "ask_request_payload"]
+        _all_params = ["ask_request_payload"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -141,24 +127,22 @@
                 "_headers",
             ]
         )
 
         # validate the arguments
         for _key, _val in _params["kwargs"].items():
             if _key not in _all_params:
-                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method ask" % _key)
+                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method ask_application" % _key)
             _params[_key] = _val
         del _params["kwargs"]
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params["application_id"] is not None:
-            _path_params["application_id"] = _params["application_id"]
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
         # process the form parameters
         _form_params = []
@@ -178,22 +162,21 @@
         if _content_types_list:
             _header_params["Content-Type"] = _content_types_list
 
         # authentication setting
         _auth_settings = ["implicit"]  # noqa: E501
 
         _response_types_map = {
-            "200": "AskResponsePayload",
-            "404": None,
-            "422": "HTTPValidationError",
+            "200": "object",
+            "422": None,
             "500": None,
         }
 
         return self.api_client.call_api(
-            "/v1/applications/{application_id}/ask",
+            "/v1/applications/ask",
             "POST",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -204,58 +187,56 @@
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
-    def create_application(self, application_create: ApplicationCreate, **kwargs) -> ApplicationResponse:  # noqa: E501
+    def create_application(self, application_config_payload: Any, **kwargs) -> Application:  # noqa: E501
         """Create Application  # noqa: E501
 
-        Create a new application.  Parameters:  - **payload**: Instance of ApplicationCreate model.     - **name**: Name of the application.     - **model_id**: UUID of the model.     - **prompt**: Prompt for the application.  # noqa: E501
+        Create a new application.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_application(application_create, async_req=True)
+        >>> thread = api.create_application(application_config_payload, async_req=True)
         >>> result = thread.get()
 
-        :param application_create: (required)
-        :type application_create: ApplicationCreate
+        :param application_config_payload: (required)
+        :type application_config_payload: Any
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: ApplicationResponse
+        :rtype: Application
         """
         kwargs["_return_http_data_only"] = True
         if "_preload_content" in kwargs:
             message = "Error! Please call the create_application_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
-        return self.create_application_with_http_info(application_create, **kwargs)  # noqa: E501
+        return self.create_application_with_http_info(application_config_payload, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_application_with_http_info(
-        self, application_create: ApplicationCreate, **kwargs
-    ) -> ApiResponse:  # noqa: E501
+    def create_application_with_http_info(self, application_config_payload: Any, **kwargs) -> ApiResponse:  # noqa: E501
         """Create Application  # noqa: E501
 
-        Create a new application.  Parameters:  - **payload**: Instance of ApplicationCreate model.     - **name**: Name of the application.     - **model_id**: UUID of the model.     - **prompt**: Prompt for the application.  # noqa: E501
+        Create a new application.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_application_with_http_info(application_create, async_req=True)
+        >>> thread = api.create_application_with_http_info(application_config_payload, async_req=True)
         >>> result = thread.get()
 
-        :param application_create: (required)
-        :type application_create: ApplicationCreate
+        :param application_config_payload: (required)
+        :type application_config_payload: Any
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
@@ -270,20 +251,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(ApplicationResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(Application, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
-        _all_params = ["application_create"]
+        _all_params = ["application_config_payload"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -309,16 +290,16 @@
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params["application_create"] is not None:
-            _body_params = _params["application_create"]
+        if _params["application_config_payload"] is not None:
+            _body_params = _params["application_config_payload"]
 
         # set the HTTP header `Accept`
         _header_params["Accept"] = self.api_client.select_header_accept(["application/json"])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get(
             "_content_type", self.api_client.select_header_content_type(["application/json"])
@@ -326,16 +307,16 @@
         if _content_types_list:
             _header_params["Content-Type"] = _content_types_list
 
         # authentication setting
         _auth_settings = ["implicit"]  # noqa: E501
 
         _response_types_map = {
-            "201": "ApplicationResponse",
-            "422": "HTTPValidationError",
+            "201": "Application",
+            "422": None,
             "500": None,
         }
 
         return self.api_client.call_api(
             "/v1/applications",
             "POST",
             _path_params,
@@ -351,171 +332,18 @@
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
-    def create_tool(self, application_id: StrictStr, tool_create: ToolCreate, **kwargs) -> ToolResponse:  # noqa: E501
-        """Create Tool  # noqa: E501
-
-        Create a tool for the application.  Parameters:  - **application_id**: UUID of the application. - **payload**: Information about the tool to be created which should match one of the following configurations based on the tool type:     - **SQL Database Tool**         - **name**: A human-readable name for the tool.         - **description**: A brief summary describing the tool's purpose or use. This description will be a part of the prompt that the LLM uses for the database.         - **type**: An identifier for the tool type, specifically for SQL databases in this case.         - **secrets**: Connection information required to access the SQL database, such as a connection string.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.create_tool(application_id, tool_create, async_req=True)
-        >>> result = thread.get()
-
-        :param application_id: (required)
-        :type application_id: str
-        :param tool_create: (required)
-        :type tool_create: ToolCreate
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _request_timeout: timeout setting for this request.
-               If one number provided, it will be total request
-               timeout. It can also be a pair (tuple) of
-               (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: ToolResponse
-        """
-        kwargs["_return_http_data_only"] = True
-        if "_preload_content" in kwargs:
-            message = "Error! Please call the create_tool_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
-            raise ValueError(message)
-        return self.create_tool_with_http_info(application_id, tool_create, **kwargs)  # noqa: E501
-
-    @validate_arguments
-    def create_tool_with_http_info(
-        self, application_id: StrictStr, tool_create: ToolCreate, **kwargs
-    ) -> ApiResponse:  # noqa: E501
-        """Create Tool  # noqa: E501
-
-        Create a tool for the application.  Parameters:  - **application_id**: UUID of the application. - **payload**: Information about the tool to be created which should match one of the following configurations based on the tool type:     - **SQL Database Tool**         - **name**: A human-readable name for the tool.         - **description**: A brief summary describing the tool's purpose or use. This description will be a part of the prompt that the LLM uses for the database.         - **type**: An identifier for the tool type, specifically for SQL databases in this case.         - **secrets**: Connection information required to access the SQL database, such as a connection string.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.create_tool_with_http_info(application_id, tool_create, async_req=True)
-        >>> result = thread.get()
-
-        :param application_id: (required)
-        :type application_id: str
-        :param tool_create: (required)
-        :type tool_create: ToolCreate
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the ApiResponse.data will
-                                 be set to none and raw_data will store the
-                                 HTTP response body without reading/decoding.
-                                 Default is True.
-        :type _preload_content: bool, optional
-        :param _return_http_data_only: response data instead of ApiResponse
-                                       object with status code, headers, etc
-        :type _return_http_data_only: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(ToolResponse, status_code(int), headers(HTTPHeaderDict))
-        """
-
-        _params = locals()
-
-        _all_params = ["application_id", "tool_create"]
-        _all_params.extend(
-            [
-                "async_req",
-                "_return_http_data_only",
-                "_preload_content",
-                "_request_timeout",
-                "_request_auth",
-                "_content_type",
-                "_headers",
-            ]
-        )
-
-        # validate the arguments
-        for _key, _val in _params["kwargs"].items():
-            if _key not in _all_params:
-                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method create_tool" % _key)
-            _params[_key] = _val
-        del _params["kwargs"]
-
-        _collection_formats = {}
-
-        # process the path parameters
-        _path_params = {}
-        if _params["application_id"] is not None:
-            _path_params["application_id"] = _params["application_id"]
-
-        # process the query parameters
-        _query_params = []
-        # process the header parameters
-        _header_params = dict(_params.get("_headers", {}))
-        # process the form parameters
-        _form_params = []
-        _files = {}
-        # process the body parameter
-        _body_params = None
-        if _params["tool_create"] is not None:
-            _body_params = _params["tool_create"]
-
-        # set the HTTP header `Accept`
-        _header_params["Accept"] = self.api_client.select_header_accept(["application/json"])  # noqa: E501
-
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get(
-            "_content_type", self.api_client.select_header_content_type(["application/json"])
-        )
-        if _content_types_list:
-            _header_params["Content-Type"] = _content_types_list
-
-        # authentication setting
-        _auth_settings = ["implicit"]  # noqa: E501
-
-        _response_types_map = {
-            "201": "ToolResponse",
-            "422": "HTTPValidationError",
-            "500": None,
-        }
-
-        return self.api_client.call_api(
-            "/v1/applications/{application_id}/tools",
-            "POST",
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get("async_req"),
-            _return_http_data_only=_params.get("_return_http_data_only"),  # noqa: E501
-            _preload_content=_params.get("_preload_content", True),
-            _request_timeout=_params.get("_request_timeout"),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get("_request_auth"),
-        )
-
-    @validate_arguments
     def delete_application(self, application_id: StrictStr, **kwargs) -> None:  # noqa: E501
         """Delete Application  # noqa: E501
 
-        Delete an application.  Parameters:  - **application_id**: UUID of the application.  # noqa: E501
+        Delete an application.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_application(application_id, async_req=True)
         >>> result = thread.get()
 
         :param application_id: (required)
@@ -537,15 +365,15 @@
             raise ValueError(message)
         return self.delete_application_with_http_info(application_id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def delete_application_with_http_info(self, application_id: StrictStr, **kwargs) -> ApiResponse:  # noqa: E501
         """Delete Application  # noqa: E501
 
-        Delete an application.  Parameters:  - **application_id**: UUID of the application.  # noqa: E501
+        Delete an application.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_application_with_http_info(application_id, async_req=True)
         >>> result = thread.get()
 
         :param application_id: (required)
@@ -609,17 +437,14 @@
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        # set the HTTP header `Accept`
-        _header_params["Accept"] = self.api_client.select_header_accept(["application/json"])  # noqa: E501
-
         # authentication setting
         _auth_settings = ["implicit"]  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             "/v1/applications/{application_id}",
@@ -637,160 +462,18 @@
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
-    def delete_tool(self, application_id: StrictStr, tool_id: StrictStr, **kwargs) -> None:  # noqa: E501
-        """Delete Tool  # noqa: E501
-
-        Delete a tool based on the given tool_id.  - **application_id**: UUID of the application. - **tool_id**: UUID of the tool.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.delete_tool(application_id, tool_id, async_req=True)
-        >>> result = thread.get()
-
-        :param application_id: (required)
-        :type application_id: str
-        :param tool_id: (required)
-        :type tool_id: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _request_timeout: timeout setting for this request.
-               If one number provided, it will be total request
-               timeout. It can also be a pair (tuple) of
-               (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: None
-        """
-        kwargs["_return_http_data_only"] = True
-        if "_preload_content" in kwargs:
-            message = "Error! Please call the delete_tool_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
-            raise ValueError(message)
-        return self.delete_tool_with_http_info(application_id, tool_id, **kwargs)  # noqa: E501
-
-    @validate_arguments
-    def delete_tool_with_http_info(
-        self, application_id: StrictStr, tool_id: StrictStr, **kwargs
-    ) -> ApiResponse:  # noqa: E501
-        """Delete Tool  # noqa: E501
-
-        Delete a tool based on the given tool_id.  - **application_id**: UUID of the application. - **tool_id**: UUID of the tool.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.delete_tool_with_http_info(application_id, tool_id, async_req=True)
-        >>> result = thread.get()
-
-        :param application_id: (required)
-        :type application_id: str
-        :param tool_id: (required)
-        :type tool_id: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the ApiResponse.data will
-                                 be set to none and raw_data will store the
-                                 HTTP response body without reading/decoding.
-                                 Default is True.
-        :type _preload_content: bool, optional
-        :param _return_http_data_only: response data instead of ApiResponse
-                                       object with status code, headers, etc
-        :type _return_http_data_only: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: None
-        """
-
-        _params = locals()
-
-        _all_params = ["application_id", "tool_id"]
-        _all_params.extend(
-            [
-                "async_req",
-                "_return_http_data_only",
-                "_preload_content",
-                "_request_timeout",
-                "_request_auth",
-                "_content_type",
-                "_headers",
-            ]
-        )
-
-        # validate the arguments
-        for _key, _val in _params["kwargs"].items():
-            if _key not in _all_params:
-                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method delete_tool" % _key)
-            _params[_key] = _val
-        del _params["kwargs"]
-
-        _collection_formats = {}
-
-        # process the path parameters
-        _path_params = {}
-        if _params["application_id"] is not None:
-            _path_params["application_id"] = _params["application_id"]
-
-        if _params["tool_id"] is not None:
-            _path_params["tool_id"] = _params["tool_id"]
-
-        # process the query parameters
-        _query_params = []
-        # process the header parameters
-        _header_params = dict(_params.get("_headers", {}))
-        # process the form parameters
-        _form_params = []
-        _files = {}
-        # process the body parameter
-        _body_params = None
-        # set the HTTP header `Accept`
-        _header_params["Accept"] = self.api_client.select_header_accept(["application/json"])  # noqa: E501
-
-        # authentication setting
-        _auth_settings = ["implicit"]  # noqa: E501
-
-        _response_types_map = {}
-
-        return self.api_client.call_api(
-            "/v1/applications/{application_id}/tools/{tool_id}",
-            "DELETE",
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get("async_req"),
-            _return_http_data_only=_params.get("_return_http_data_only"),  # noqa: E501
-            _preload_content=_params.get("_preload_content", True),
-            _request_timeout=_params.get("_request_timeout"),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get("_request_auth"),
-        )
-
-    @validate_arguments
-    def get_application_by_id(self, application_id: StrictStr, **kwargs) -> ApplicationResponse:  # noqa: E501
+    def get_application_by_id(self, application_id: StrictStr, **kwargs) -> Application:  # noqa: E501
         """Get Application By Id  # noqa: E501
 
-        Get an application by its id.  Parameters:  - **application_id**: UUID of the application.  # noqa: E501
+        Get an application by id.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_application_by_id(application_id, async_req=True)
         >>> result = thread.get()
 
         :param application_id: (required)
@@ -800,27 +483,27 @@
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: ApplicationResponse
+        :rtype: Application
         """
         kwargs["_return_http_data_only"] = True
         if "_preload_content" in kwargs:
             message = "Error! Please call the get_application_by_id_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
         return self.get_application_by_id_with_http_info(application_id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def get_application_by_id_with_http_info(self, application_id: StrictStr, **kwargs) -> ApiResponse:  # noqa: E501
         """Get Application By Id  # noqa: E501
 
-        Get an application by its id.  Parameters:  - **application_id**: UUID of the application.  # noqa: E501
+        Get an application by id.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_application_by_id_with_http_info(application_id, async_req=True)
         >>> result = thread.get()
 
         :param application_id: (required)
@@ -843,15 +526,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(ApplicationResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(Application, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = ["application_id"]
         _all_params.extend(
             [
@@ -891,17 +574,17 @@
         # set the HTTP header `Accept`
         _header_params["Accept"] = self.api_client.select_header_accept(["application/json"])  # noqa: E501
 
         # authentication setting
         _auth_settings = ["implicit"]  # noqa: E501
 
         _response_types_map = {
-            "200": "ApplicationResponse",
+            "200": "Application",
             "404": None,
-            "422": "HTTPValidationError",
+            "422": None,
             "500": None,
         }
 
         return self.api_client.call_api(
             "/v1/applications/{application_id}",
             "GET",
             _path_params,
@@ -921,88 +604,88 @@
         )
 
     @validate_arguments
     def get_applications(
         self,
         name: Optional[Any] = None,
         created_by: Optional[Any] = None,
-        model_id: Optional[Any] = None,
         prompt: Optional[Any] = None,
+        dataset_id: Optional[Any] = None,
         page: Annotated[Optional[conint(strict=True, ge=1)], Field(description="Page number")] = None,
         size: Annotated[Optional[conint(strict=True, le=100, ge=1)], Field(description="Page size")] = None,
         **kwargs
-    ) -> PageApplicationResponse:  # noqa: E501
+    ) -> PageApplication:  # noqa: E501
         """Get Applications  # noqa: E501
 
-        Get all applications. Filter if provided with name, created_by, model_id, or prompt.  Parameters: - **name**: Name of the application. (optional) - **created_by**: User ID of the user who created the application. (optional) - **model_id**: UUID of the model. (optional) - **prompt**: Prompt for the application. (optional)  # noqa: E501
+        Get applications.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_applications(name, created_by, model_id, prompt, page, size, async_req=True)
+        >>> thread = api.get_applications(name, created_by, prompt, dataset_id, page, size, async_req=True)
         >>> result = thread.get()
 
         :param name:
         :type name: Name
         :param created_by:
         :type created_by: CreatedBy
-        :param model_id:
-        :type model_id: ModelId
         :param prompt:
         :type prompt: Prompt
+        :param dataset_id:
+        :type dataset_id: DatasetId
         :param page: Page number
         :type page: int
         :param size: Page size
         :type size: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: PageApplicationResponse
+        :rtype: PageApplication
         """
         kwargs["_return_http_data_only"] = True
         if "_preload_content" in kwargs:
             message = "Error! Please call the get_applications_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
         return self.get_applications_with_http_info(
-            name, created_by, model_id, prompt, page, size, **kwargs
+            name, created_by, prompt, dataset_id, page, size, **kwargs
         )  # noqa: E501
 
     @validate_arguments
     def get_applications_with_http_info(
         self,
         name: Optional[Any] = None,
         created_by: Optional[Any] = None,
-        model_id: Optional[Any] = None,
         prompt: Optional[Any] = None,
+        dataset_id: Optional[Any] = None,
         page: Annotated[Optional[conint(strict=True, ge=1)], Field(description="Page number")] = None,
         size: Annotated[Optional[conint(strict=True, le=100, ge=1)], Field(description="Page size")] = None,
         **kwargs
     ) -> ApiResponse:  # noqa: E501
         """Get Applications  # noqa: E501
 
-        Get all applications. Filter if provided with name, created_by, model_id, or prompt.  Parameters: - **name**: Name of the application. (optional) - **created_by**: User ID of the user who created the application. (optional) - **model_id**: UUID of the model. (optional) - **prompt**: Prompt for the application. (optional)  # noqa: E501
+        Get applications.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_applications_with_http_info(name, created_by, model_id, prompt, page, size, async_req=True)
+        >>> thread = api.get_applications_with_http_info(name, created_by, prompt, dataset_id, page, size, async_req=True)
         >>> result = thread.get()
 
         :param name:
         :type name: Name
         :param created_by:
         :type created_by: CreatedBy
-        :param model_id:
-        :type model_id: ModelId
         :param prompt:
         :type prompt: Prompt
+        :param dataset_id:
+        :type dataset_id: DatasetId
         :param page: Page number
         :type page: int
         :param size: Page size
         :type size: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
@@ -1021,20 +704,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(PageApplicationResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(PageApplication, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
-        _all_params = ["name", "created_by", "model_id", "prompt", "page", "size"]
+        _all_params = ["name", "created_by", "prompt", "dataset_id", "page", "size"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -1059,20 +742,20 @@
         _query_params = []
         if _params.get("name") is not None:  # noqa: E501
             _query_params.append(("name", _params["name"]))
 
         if _params.get("created_by") is not None:  # noqa: E501
             _query_params.append(("created_by", _params["created_by"]))
 
-        if _params.get("model_id") is not None:  # noqa: E501
-            _query_params.append(("model_id", _params["model_id"]))
-
         if _params.get("prompt") is not None:  # noqa: E501
             _query_params.append(("prompt", _params["prompt"]))
 
+        if _params.get("dataset_id") is not None:  # noqa: E501
+            _query_params.append(("dataset_id", _params["dataset_id"]))
+
         if _params.get("page") is not None:  # noqa: E501
             _query_params.append(("page", _params["page"]))
 
         if _params.get("size") is not None:  # noqa: E501
             _query_params.append(("size", _params["size"]))
 
         # process the header parameters
@@ -1085,16 +768,16 @@
         # set the HTTP header `Accept`
         _header_params["Accept"] = self.api_client.select_header_accept(["application/json"])  # noqa: E501
 
         # authentication setting
         _auth_settings = ["implicit"]  # noqa: E501
 
         _response_types_map = {
-            "200": "PageApplicationResponse",
-            "422": "HTTPValidationError",
+            "200": "PageApplication",
+            "422": None,
             "500": None,
         }
 
         return self.api_client.call_api(
             "/v1/applications",
             "GET",
             _path_params,
@@ -1110,62 +793,64 @@
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
-    def get_tool(self, application_id: StrictStr, tool_id: StrictStr, **kwargs) -> ToolResponse:  # noqa: E501
-        """Get Tool  # noqa: E501
+    def put_application(
+        self, application_id: StrictStr, application_config_payload: Any, **kwargs
+    ) -> Application:  # noqa: E501
+        """Put Application  # noqa: E501
 
-        Retrieve a Tool based on the given tool_id.  - **application_id**: UUID of the application. - **tool_id**: UUID of the tool.  # noqa: E501
+        Update an application.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_tool(application_id, tool_id, async_req=True)
+        >>> thread = api.put_application(application_id, application_config_payload, async_req=True)
         >>> result = thread.get()
 
         :param application_id: (required)
         :type application_id: str
-        :param tool_id: (required)
-        :type tool_id: str
+        :param application_config_payload: (required)
+        :type application_config_payload: Any
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: ToolResponse
+        :rtype: Application
         """
         kwargs["_return_http_data_only"] = True
         if "_preload_content" in kwargs:
-            message = "Error! Please call the get_tool_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            message = "Error! Please call the put_application_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
-        return self.get_tool_with_http_info(application_id, tool_id, **kwargs)  # noqa: E501
+        return self.put_application_with_http_info(application_id, application_config_payload, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_tool_with_http_info(
-        self, application_id: StrictStr, tool_id: StrictStr, **kwargs
+    def put_application_with_http_info(
+        self, application_id: StrictStr, application_config_payload: Any, **kwargs
     ) -> ApiResponse:  # noqa: E501
-        """Get Tool  # noqa: E501
+        """Put Application  # noqa: E501
 
-        Retrieve a Tool based on the given tool_id.  - **application_id**: UUID of the application. - **tool_id**: UUID of the tool.  # noqa: E501
+        Update an application.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_tool_with_http_info(application_id, tool_id, async_req=True)
+        >>> thread = api.put_application_with_http_info(application_id, application_config_payload, async_req=True)
         >>> result = thread.get()
 
         :param application_id: (required)
         :type application_id: str
-        :param tool_id: (required)
-        :type tool_id: str
+        :param application_config_payload: (required)
+        :type application_config_payload: Any
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
@@ -1180,20 +865,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(ToolResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(Application, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
-        _all_params = ["application_id", "tool_id"]
+        _all_params = ["application_id", "application_config_payload"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -1201,53 +886,60 @@
                 "_headers",
             ]
         )
 
         # validate the arguments
         for _key, _val in _params["kwargs"].items():
             if _key not in _all_params:
-                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method get_tool" % _key)
+                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method put_application" % _key)
             _params[_key] = _val
         del _params["kwargs"]
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params["application_id"] is not None:
             _path_params["application_id"] = _params["application_id"]
 
-        if _params["tool_id"] is not None:
-            _path_params["tool_id"] = _params["tool_id"]
-
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
+        if _params["application_config_payload"] is not None:
+            _body_params = _params["application_config_payload"]
+
         # set the HTTP header `Accept`
         _header_params["Accept"] = self.api_client.select_header_accept(["application/json"])  # noqa: E501
 
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get(
+            "_content_type", self.api_client.select_header_content_type(["application/json"])
+        )
+        if _content_types_list:
+            _header_params["Content-Type"] = _content_types_list
+
         # authentication setting
         _auth_settings = ["implicit"]  # noqa: E501
 
         _response_types_map = {
-            "200": "ToolResponse",
+            "200": "Application",
             "404": None,
-            "422": "HTTPValidationError",
+            "422": None,
             "500": None,
         }
 
         return self.api_client.call_api(
-            "/v1/applications/{application_id}/tools/{tool_id}",
-            "GET",
+            "/v1/applications/{application_id}",
+            "PUT",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1257,88 +949,54 @@
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
         )
 
     @validate_arguments
-    def get_tools(
-        self,
-        application_id: StrictStr,
-        name: Optional[Any] = None,
-        type: Optional[Any] = None,
-        page: Annotated[Optional[conint(strict=True, ge=1)], Field(description="Page number")] = None,
-        size: Annotated[Optional[conint(strict=True, le=100, ge=1)], Field(description="Page size")] = None,
-        **kwargs
-    ) -> PageToolResponse:  # noqa: E501
-        """Get Tools  # noqa: E501
+    def test_model_connection(self, model_llm: ModelLLM, **kwargs) -> None:  # noqa: E501
+        """Test Model Connection  # noqa: E501
 
-        Retrieve Tools under a given application ID based on the provided filters.  - **application_id**: UUID of the application. - **name**: Name of the tool. - **type**: Type of the tool.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_tools(application_id, name, type, page, size, async_req=True)
+        >>> thread = api.test_model_connection(model_llm, async_req=True)
         >>> result = thread.get()
 
-        :param application_id: (required)
-        :type application_id: str
-        :param name:
-        :type name: Name
-        :param type:
-        :type type: ToolType
-        :param page: Page number
-        :type page: int
-        :param size: Page size
-        :type size: int
+        :param model_llm: (required)
+        :type model_llm: ModelLLM
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: PageToolResponse
+        :rtype: None
         """
         kwargs["_return_http_data_only"] = True
         if "_preload_content" in kwargs:
-            message = "Error! Please call the get_tools_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            message = "Error! Please call the test_model_connection_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
-        return self.get_tools_with_http_info(application_id, name, type, page, size, **kwargs)  # noqa: E501
+        return self.test_model_connection_with_http_info(model_llm, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_tools_with_http_info(
-        self,
-        application_id: StrictStr,
-        name: Optional[Any] = None,
-        type: Optional[Any] = None,
-        page: Annotated[Optional[conint(strict=True, ge=1)], Field(description="Page number")] = None,
-        size: Annotated[Optional[conint(strict=True, le=100, ge=1)], Field(description="Page size")] = None,
-        **kwargs
-    ) -> ApiResponse:  # noqa: E501
-        """Get Tools  # noqa: E501
+    def test_model_connection_with_http_info(self, model_llm: ModelLLM, **kwargs) -> ApiResponse:  # noqa: E501
+        """Test Model Connection  # noqa: E501
 
-        Retrieve Tools under a given application ID based on the provided filters.  - **application_id**: UUID of the application. - **name**: Name of the tool. - **type**: Type of the tool.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_tools_with_http_info(application_id, name, type, page, size, async_req=True)
+        >>> thread = api.test_model_connection_with_http_info(model_llm, async_req=True)
         >>> result = thread.get()
 
-        :param application_id: (required)
-        :type application_id: str
-        :param name:
-        :type name: Name
-        :param type:
-        :type type: ToolType
-        :param page: Page number
-        :type page: int
-        :param size: Page size
-        :type size: int
+        :param model_llm: (required)
+        :type model_llm: ModelLLM
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
@@ -1353,20 +1011,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(PageToolResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: None
         """
 
         _params = locals()
 
-        _all_params = ["application_id", "name", "type", "page", "size"]
+        _all_params = ["model_llm"]
         _all_params.extend(
             [
                 "async_req",
                 "_return_http_data_only",
                 "_preload_content",
                 "_request_timeout",
                 "_request_auth",
@@ -1374,61 +1032,50 @@
                 "_headers",
             ]
         )
 
         # validate the arguments
         for _key, _val in _params["kwargs"].items():
             if _key not in _all_params:
-                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method get_tools" % _key)
+                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method test_model_connection" % _key)
             _params[_key] = _val
         del _params["kwargs"]
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params["application_id"] is not None:
-            _path_params["application_id"] = _params["application_id"]
 
         # process the query parameters
         _query_params = []
-        if _params.get("name") is not None:  # noqa: E501
-            _query_params.append(("name", _params["name"]))
-
-        if _params.get("type") is not None:  # noqa: E501
-            _query_params.append(("type", _params["type"]))
-
-        if _params.get("page") is not None:  # noqa: E501
-            _query_params.append(("page", _params["page"]))
-
-        if _params.get("size") is not None:  # noqa: E501
-            _query_params.append(("size", _params["size"]))
-
         # process the header parameters
         _header_params = dict(_params.get("_headers", {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        # set the HTTP header `Accept`
-        _header_params["Accept"] = self.api_client.select_header_accept(["application/json"])  # noqa: E501
+        if _params["model_llm"] is not None:
+            _body_params = _params["model_llm"]
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get(
+            "_content_type", self.api_client.select_header_content_type(["application/json"])
+        )
+        if _content_types_list:
+            _header_params["Content-Type"] = _content_types_list
 
         # authentication setting
         _auth_settings = ["implicit"]  # noqa: E501
 
-        _response_types_map = {
-            "200": "PageToolResponse",
-            "422": "HTTPValidationError",
-            "500": None,
-        }
+        _response_types_map = {}
 
         return self.api_client.call_api(
-            "/v1/applications/{application_id}/tools",
-            "GET",
+            "/v1/applications/test-model-connection",
+            "POST",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1566,334 +1213,14 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get("async_req"),
-            _return_http_data_only=_params.get("_return_http_data_only"),  # noqa: E501
-            _preload_content=_params.get("_preload_content", True),
-            _request_timeout=_params.get("_request_timeout"),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get("_request_auth"),
-        )
-
-    @validate_arguments
-    def update_application(
-        self, application_id: StrictStr, application_update: ApplicationUpdate, **kwargs
-    ) -> ApplicationResponse:  # noqa: E501
-        """Update Application  # noqa: E501
-
-        Update an application.  Parameters:  - **application_id**: UUID of the application. - **payload**: Instance of ApplicationUpdate model.     - **name**: Name of the application. (optional)     - **model_id**: UUID of the model. (optional)     - **prompt**: Prompt for the application. (optional)  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.update_application(application_id, application_update, async_req=True)
-        >>> result = thread.get()
-
-        :param application_id: (required)
-        :type application_id: str
-        :param application_update: (required)
-        :type application_update: ApplicationUpdate
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _request_timeout: timeout setting for this request.
-               If one number provided, it will be total request
-               timeout. It can also be a pair (tuple) of
-               (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: ApplicationResponse
-        """
-        kwargs["_return_http_data_only"] = True
-        if "_preload_content" in kwargs:
-            message = "Error! Please call the update_application_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
-            raise ValueError(message)
-        return self.update_application_with_http_info(application_id, application_update, **kwargs)  # noqa: E501
-
-    @validate_arguments
-    def update_application_with_http_info(
-        self, application_id: StrictStr, application_update: ApplicationUpdate, **kwargs
-    ) -> ApiResponse:  # noqa: E501
-        """Update Application  # noqa: E501
-
-        Update an application.  Parameters:  - **application_id**: UUID of the application. - **payload**: Instance of ApplicationUpdate model.     - **name**: Name of the application. (optional)     - **model_id**: UUID of the model. (optional)     - **prompt**: Prompt for the application. (optional)  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.update_application_with_http_info(application_id, application_update, async_req=True)
-        >>> result = thread.get()
-
-        :param application_id: (required)
-        :type application_id: str
-        :param application_update: (required)
-        :type application_update: ApplicationUpdate
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the ApiResponse.data will
-                                 be set to none and raw_data will store the
-                                 HTTP response body without reading/decoding.
-                                 Default is True.
-        :type _preload_content: bool, optional
-        :param _return_http_data_only: response data instead of ApiResponse
-                                       object with status code, headers, etc
-        :type _return_http_data_only: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(ApplicationResponse, status_code(int), headers(HTTPHeaderDict))
-        """
-
-        _params = locals()
-
-        _all_params = ["application_id", "application_update"]
-        _all_params.extend(
-            [
-                "async_req",
-                "_return_http_data_only",
-                "_preload_content",
-                "_request_timeout",
-                "_request_auth",
-                "_content_type",
-                "_headers",
-            ]
-        )
-
-        # validate the arguments
-        for _key, _val in _params["kwargs"].items():
-            if _key not in _all_params:
-                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method update_application" % _key)
-            _params[_key] = _val
-        del _params["kwargs"]
-
-        _collection_formats = {}
-
-        # process the path parameters
-        _path_params = {}
-        if _params["application_id"] is not None:
-            _path_params["application_id"] = _params["application_id"]
-
-        # process the query parameters
-        _query_params = []
-        # process the header parameters
-        _header_params = dict(_params.get("_headers", {}))
-        # process the form parameters
-        _form_params = []
-        _files = {}
-        # process the body parameter
-        _body_params = None
-        if _params["application_update"] is not None:
-            _body_params = _params["application_update"]
-
-        # set the HTTP header `Accept`
-        _header_params["Accept"] = self.api_client.select_header_accept(["application/json"])  # noqa: E501
-
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get(
-            "_content_type", self.api_client.select_header_content_type(["application/json"])
-        )
-        if _content_types_list:
-            _header_params["Content-Type"] = _content_types_list
-
-        # authentication setting
-        _auth_settings = ["implicit"]  # noqa: E501
-
-        _response_types_map = {
-            "200": "ApplicationResponse",
-            "404": None,
-            "409": None,
-            "422": "HTTPValidationError",
-            "500": None,
-        }
-
-        return self.api_client.call_api(
-            "/v1/applications/{application_id}",
-            "PATCH",
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get("async_req"),
-            _return_http_data_only=_params.get("_return_http_data_only"),  # noqa: E501
-            _preload_content=_params.get("_preload_content", True),
-            _request_timeout=_params.get("_request_timeout"),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get("_request_auth"),
-        )
-
-    @validate_arguments
-    def update_tool(
-        self, application_id: StrictStr, tool_id: StrictStr, tool_update: ToolUpdate, **kwargs
-    ) -> ToolResponse:  # noqa: E501
-        """Update Tool  # noqa: E501
-
-        Update a tool based on the given tool_id.  - **application_id**: UUID of the application. - **tool_id**: UUID of the tool.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.update_tool(application_id, tool_id, tool_update, async_req=True)
-        >>> result = thread.get()
-
-        :param application_id: (required)
-        :type application_id: str
-        :param tool_id: (required)
-        :type tool_id: str
-        :param tool_update: (required)
-        :type tool_update: ToolUpdate
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _request_timeout: timeout setting for this request.
-               If one number provided, it will be total request
-               timeout. It can also be a pair (tuple) of
-               (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: ToolResponse
-        """
-        kwargs["_return_http_data_only"] = True
-        if "_preload_content" in kwargs:
-            message = "Error! Please call the update_tool_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
-            raise ValueError(message)
-        return self.update_tool_with_http_info(application_id, tool_id, tool_update, **kwargs)  # noqa: E501
-
-    @validate_arguments
-    def update_tool_with_http_info(
-        self, application_id: StrictStr, tool_id: StrictStr, tool_update: ToolUpdate, **kwargs
-    ) -> ApiResponse:  # noqa: E501
-        """Update Tool  # noqa: E501
-
-        Update a tool based on the given tool_id.  - **application_id**: UUID of the application. - **tool_id**: UUID of the tool.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.update_tool_with_http_info(application_id, tool_id, tool_update, async_req=True)
-        >>> result = thread.get()
-
-        :param application_id: (required)
-        :type application_id: str
-        :param tool_id: (required)
-        :type tool_id: str
-        :param tool_update: (required)
-        :type tool_update: ToolUpdate
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the ApiResponse.data will
-                                 be set to none and raw_data will store the
-                                 HTTP response body without reading/decoding.
-                                 Default is True.
-        :type _preload_content: bool, optional
-        :param _return_http_data_only: response data instead of ApiResponse
-                                       object with status code, headers, etc
-        :type _return_http_data_only: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(ToolResponse, status_code(int), headers(HTTPHeaderDict))
-        """
-
-        _params = locals()
-
-        _all_params = ["application_id", "tool_id", "tool_update"]
-        _all_params.extend(
-            [
-                "async_req",
-                "_return_http_data_only",
-                "_preload_content",
-                "_request_timeout",
-                "_request_auth",
-                "_content_type",
-                "_headers",
-            ]
-        )
-
-        # validate the arguments
-        for _key, _val in _params["kwargs"].items():
-            if _key not in _all_params:
-                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method update_tool" % _key)
-            _params[_key] = _val
-        del _params["kwargs"]
-
-        _collection_formats = {}
-
-        # process the path parameters
-        _path_params = {}
-        if _params["application_id"] is not None:
-            _path_params["application_id"] = _params["application_id"]
-
-        if _params["tool_id"] is not None:
-            _path_params["tool_id"] = _params["tool_id"]
-
-        # process the query parameters
-        _query_params = []
-        # process the header parameters
-        _header_params = dict(_params.get("_headers", {}))
-        # process the form parameters
-        _form_params = []
-        _files = {}
-        # process the body parameter
-        _body_params = None
-        if _params["tool_update"] is not None:
-            _body_params = _params["tool_update"]
-
-        # set the HTTP header `Accept`
-        _header_params["Accept"] = self.api_client.select_header_accept(["application/json"])  # noqa: E501
-
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get(
-            "_content_type", self.api_client.select_header_content_type(["application/json"])
-        )
-        if _content_types_list:
-            _header_params["Content-Type"] = _content_types_list
-
-        # authentication setting
-        _auth_settings = ["implicit"]  # noqa: E501
-
-        _response_types_map = {
-            "200": "ToolResponse",
-            "404": None,
-            "422": "HTTPValidationError",
-            "500": None,
-        }
-
-        return self.api_client.call_api(
-            "/v1/applications/{application_id}/tools/{tool_id}",
-            "PATCH",
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get("async_req"),
             _return_http_data_only=_params.get("_return_http_data_only"),  # noqa: E501
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
```

### Comparing `superwise_api-1.2.0/superwise_api/client/api/dashboard_items_api.py` & `superwise_api-1.3.0/superwise_api/client/api/dashboard_items_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import io
 import re  # noqa: F401
 import warnings
@@ -21,14 +21,15 @@
 
 from superwise_api.client.api_client import ApiClient
 from superwise_api.client.api_response import ApiResponse
 from superwise_api.client.exceptions import ApiTypeError
 from superwise_api.client.exceptions import ApiValueError
 from superwise_api.client.models.dashboard_item import DashboardItem
 from superwise_api.client.models.dashboard_item_create import DashboardItemCreate
+from superwise_api.client.models.dashboard_item_update import DashboardItemUpdate
 from superwise_api.client.models.page_dashboard_item import PageDashboardItem
 
 
 class DashboardItemsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
@@ -618,14 +619,170 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get("async_req"),
+            _return_http_data_only=_params.get("_return_http_data_only"),  # noqa: E501
+            _preload_content=_params.get("_preload_content", True),
+            _request_timeout=_params.get("_request_timeout"),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get("_request_auth"),
+        )
+
+    @validate_arguments
+    def update_dashboard_item(
+        self, dashboard_item_id: StrictStr, dashboard_item_update: DashboardItemUpdate, **kwargs
+    ) -> DashboardItem:  # noqa: E501
+        """Update dashboard item by ID  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.update_dashboard_item(dashboard_item_id, dashboard_item_update, async_req=True)
+        >>> result = thread.get()
+
+        :param dashboard_item_id: (required)
+        :type dashboard_item_id: str
+        :param dashboard_item_update: (required)
+        :type dashboard_item_update: DashboardItemUpdate
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: DashboardItem
+        """
+        kwargs["_return_http_data_only"] = True
+        if "_preload_content" in kwargs:
+            message = "Error! Please call the update_dashboard_item_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+        return self.update_dashboard_item_with_http_info(
+            dashboard_item_id, dashboard_item_update, **kwargs
+        )  # noqa: E501
+
+    @validate_arguments
+    def update_dashboard_item_with_http_info(
+        self, dashboard_item_id: StrictStr, dashboard_item_update: DashboardItemUpdate, **kwargs
+    ) -> ApiResponse:  # noqa: E501
+        """Update dashboard item by ID  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.update_dashboard_item_with_http_info(dashboard_item_id, dashboard_item_update, async_req=True)
+        >>> result = thread.get()
+
+        :param dashboard_item_id: (required)
+        :type dashboard_item_id: str
+        :param dashboard_item_update: (required)
+        :type dashboard_item_update: DashboardItemUpdate
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(DashboardItem, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = ["dashboard_item_id", "dashboard_item_update"]
+        _all_params.extend(
+            [
+                "async_req",
+                "_return_http_data_only",
+                "_preload_content",
+                "_request_timeout",
+                "_request_auth",
+                "_content_type",
+                "_headers",
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params["kwargs"].items():
+            if _key not in _all_params:
+                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method update_dashboard_item" % _key)
+            _params[_key] = _val
+        del _params["kwargs"]
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params["dashboard_item_id"] is not None:
+            _path_params["dashboard_item_id"] = _params["dashboard_item_id"]
+
+        # process the query parameters
+        _query_params = []
+        # process the header parameters
+        _header_params = dict(_params.get("_headers", {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        if _params["dashboard_item_update"] is not None:
+            _body_params = _params["dashboard_item_update"]
+
+        # set the HTTP header `Accept`
+        _header_params["Accept"] = self.api_client.select_header_accept(["application/json"])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get(
+            "_content_type", self.api_client.select_header_content_type(["application/json"])
+        )
+        if _content_types_list:
+            _header_params["Content-Type"] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ["implicit"]  # noqa: E501
+
+        _response_types_map = {
+            "200": "DashboardItem",
+            "404": None,
+            "422": None,
+            "500": None,
+        }
+
+        return self.api_client.call_api(
+            "/v1/dashboard-items/{dashboard_item_id}",
+            "PATCH",
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get("async_req"),
             _return_http_data_only=_params.get("_return_http_data_only"),  # noqa: E501
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
```

### Comparing `superwise_api-1.2.0/superwise_api/client/api/dashboards_api.py` & `superwise_api-1.3.0/superwise_api/client/api/dashboards_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import io
 import re  # noqa: F401
 import warnings
```

### Comparing `superwise_api-1.2.0/superwise_api/client/api/dataset_api.py` & `superwise_api-1.3.0/superwise_api/client/api/dataset_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import io
 import re  # noqa: F401
 import warnings
```

### Comparing `superwise_api-1.2.0/superwise_api/client/api/dataset_sources_api.py` & `superwise_api-1.3.0/superwise_api/client/api/dataset_sources_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import io
 import re  # noqa: F401
 import warnings
```

### Comparing `superwise_api-1.2.0/superwise_api/client/api/destinations_api.py` & `superwise_api-1.3.0/superwise_api/client/api/destinations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import io
 import re  # noqa: F401
 import warnings
```

### Comparing `superwise_api-1.2.0/superwise_api/client/api/integrations_api.py` & `superwise_api-1.3.0/superwise_api/client/api/integrations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import io
 import re  # noqa: F401
 import warnings
```

### Comparing `superwise_api-1.2.0/superwise_api/client/api/policies_api.py` & `superwise_api-1.3.0/superwise_api/client/api/policies_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import io
 import re  # noqa: F401
 import warnings
```

### Comparing `superwise_api-1.2.0/superwise_api/client/api/sources_api.py` & `superwise_api-1.3.0/superwise_api/client/api/sources_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import io
 import re  # noqa: F401
 import warnings
```

### Comparing `superwise_api-1.2.0/superwise_api/client/api_client.py` & `superwise_api-1.3.0/superwise_api/client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import atexit
 import datetime
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/api_response.py` & `superwise_api-1.3.0/superwise_api/client/api_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/client/configuration.py` & `superwise_api-1.3.0/superwise_api/client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import copy
 import http.client as httplib
 import logging
@@ -380,15 +380,15 @@
 
         :return: The report for debugging.
         """
         return (
             "Python SDK Debug Report:\n"
             "OS: {env}\n"
             "Python Version: {pyversion}\n"
-            "Version of the API: 1.5.0\n"
+            "Version of the API: 1.6.2\n"
             "SDK Package Version: 1.0.0".format(env=sys.platform, pyversion=sys.version)
         )
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `superwise_api-1.2.0/superwise_api/client/exceptions.py` & `superwise_api-1.3.0/superwise_api/client/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/__init__.py` & `superwise_api-1.3.0/superwise_api/client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # coding: utf-8
 # flake8: noqa
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 # import models into model package
 from superwise_api.client.models.alert_on_status_direction import AlertOnStatusDirection
-from superwise_api.client.models.application_create import ApplicationCreate
-from superwise_api.client.models.application_response import ApplicationResponse
-from superwise_api.client.models.application_update import ApplicationUpdate
-from superwise_api.client.models.ask_config import AskConfig
+from superwise_api.client.models.application import Application
+from superwise_api.client.models.application_config import ApplicationConfig
+from superwise_api.client.models.application_config_payload import ApplicationConfigPayload
+from superwise_api.client.models.application_model import ApplicationModel
 from superwise_api.client.models.ask_request_payload import AskRequestPayload
-from superwise_api.client.models.ask_response_payload import AskResponsePayload
 from superwise_api.client.models.aws_credentials_request import AWSCredentialsRequest
 from superwise_api.client.models.aws_credentials_response import AWSCredentialsResponse
 from superwise_api.client.models.azure_credentials_request import AzureCredentialsRequest
 from superwise_api.client.models.azure_credentials_response import AzureCredentialsResponse
 from superwise_api.client.models.chat_history_entry import ChatHistoryEntry
 from superwise_api.client.models.config import Config
-from superwise_api.client.models.config1 import Config1
+from superwise_api.client.models.created_at import CreatedAt
 from superwise_api.client.models.created_by import CreatedBy
 from superwise_api.client.models.dashboard import Dashboard
 from superwise_api.client.models.dashboard_create import DashboardCreate
 from superwise_api.client.models.dashboard_item import DashboardItem
 from superwise_api.client.models.dashboard_item_create import DashboardItemCreate
 from superwise_api.client.models.dashboard_item_query import DashboardItemQuery
 from superwise_api.client.models.dashboard_item_query_order import DashboardItemQueryOrder
+from superwise_api.client.models.dashboard_item_update import DashboardItemUpdate
 from superwise_api.client.models.dashboard_update import DashboardUpdate
 from superwise_api.client.models.dataset_create import DatasetCreate
+from superwise_api.client.models.dataset_id import DatasetId
 from superwise_api.client.models.dataset_response import DatasetResponse
 from superwise_api.client.models.dataset_source_create import DatasetSourceCreate
 from superwise_api.client.models.dataset_source_response import DatasetSourceResponse
 from superwise_api.client.models.dataset_source_response_with_source import DatasetSourceResponseWithSource
 from superwise_api.client.models.dataset_source_update import DatasetSourceUpdate
 from superwise_api.client.models.dataset_tag import DatasetTag
 from superwise_api.client.models.dataset_update import DatasetUpdate
@@ -52,46 +53,40 @@
 from superwise_api.client.models.gcp_credentials_response import GCPCredentialsResponse
 from superwise_api.client.models.google_model_version import GoogleModelVersion
 from superwise_api.client.models.granularity import Granularity
 from superwise_api.client.models.http_validation_error import HTTPValidationError
 from superwise_api.client.models.ingest_type import IngestType
 from superwise_api.client.models.integration_response import IntegrationResponse
 from superwise_api.client.models.integration_type import IntegrationType
-from superwise_api.client.models.model_create import ModelCreate
-from superwise_api.client.models.model_id import ModelId
+from superwise_api.client.models.model_llm import ModelLLM
 from superwise_api.client.models.model_provider import ModelProvider
-from superwise_api.client.models.model_response import ModelResponse
 from superwise_api.client.models.model_schema import ModelSchema
 from superwise_api.client.models.model_version import ModelVersion
-from superwise_api.client.models.model_version_response import ModelVersionResponse
 from superwise_api.client.models.name import Name
 from superwise_api.client.models.open_ai_model_version import OpenAIModelVersion
 from superwise_api.client.models.page import Page
-from superwise_api.client.models.page_application_response import PageApplicationResponse
+from superwise_api.client.models.page_application import PageApplication
 from superwise_api.client.models.page_dashboard import PageDashboard
 from superwise_api.client.models.page_dashboard_item import PageDashboardItem
 from superwise_api.client.models.page_dataset_response import PageDatasetResponse
 from superwise_api.client.models.page_dataset_source_response_with_source import PageDatasetSourceResponseWithSource
 from superwise_api.client.models.page_destination_response import PageDestinationResponse
 from superwise_api.client.models.page_integration_response import PageIntegrationResponse
-from superwise_api.client.models.page_model_response import PageModelResponse
 from superwise_api.client.models.page_policy_response import PagePolicyResponse
 from superwise_api.client.models.page_source_response import PageSourceResponse
-from superwise_api.client.models.page_tool_response import PageToolResponse
 from superwise_api.client.models.pages import Pages
 from superwise_api.client.models.payload import Payload
 from superwise_api.client.models.policy_create import PolicyCreate
 from superwise_api.client.models.policy_query import PolicyQuery
 from superwise_api.client.models.policy_query_filter import PolicyQueryFilter
 from superwise_api.client.models.policy_query_order import PolicyQueryOrder
 from superwise_api.client.models.policy_response import PolicyResponse
 from superwise_api.client.models.policy_status import PolicyStatus
 from superwise_api.client.models.policy_update import PolicyUpdate
 from superwise_api.client.models.prompt import Prompt
-from superwise_api.client.models.provider import Provider
 from superwise_api.client.models.query_type import QueryType
 from superwise_api.client.models.role import Role
 from superwise_api.client.models.schema_item import SchemaItem
 from superwise_api.client.models.schema_update import SchemaUpdate
 from superwise_api.client.models.schema_update_item import SchemaUpdateItem
 from superwise_api.client.models.size import Size
 from superwise_api.client.models.source import Source
@@ -114,22 +109,19 @@
 from superwise_api.client.models.time_range_unit import TimeRangeUnit
 from superwise_api.client.models.tool_config_big_query import ToolConfigBigQuery
 from superwise_api.client.models.tool_config_pg_vector import ToolConfigPGVector
 from superwise_api.client.models.tool_config_sql_database_mssql import ToolConfigSQLDatabaseMSSQL
 from superwise_api.client.models.tool_config_sql_database_my_sql import ToolConfigSQLDatabaseMySQL
 from superwise_api.client.models.tool_config_sql_database_oracle import ToolConfigSQLDatabaseOracle
 from superwise_api.client.models.tool_config_sql_database_postgres import ToolConfigSQLDatabasePostgres
-from superwise_api.client.models.tool_create import ToolCreate
-from superwise_api.client.models.tool_name import ToolName
-from superwise_api.client.models.tool_name_update import ToolNameUpdate
-from superwise_api.client.models.tool_response import ToolResponse
-from superwise_api.client.models.tool_type import ToolType
-from superwise_api.client.models.tool_update import ToolUpdate
+from superwise_api.client.models.tool_def_input import ToolDefInput
+from superwise_api.client.models.tool_def_output import ToolDefOutput
 from superwise_api.client.models.total import Total
 from superwise_api.client.models.type import Type
+from superwise_api.client.models.updated_at import UpdatedAt
 from superwise_api.client.models.validation_error import ValidationError
 from superwise_api.client.models.validation_error_detail import ValidationErrorDetail
 from superwise_api.client.models.validation_error_loc_inner import ValidationErrorLocInner
 from superwise_api.client.models.validation_result import ValidationResult
 from superwise_api.client.models.values import Values
 from superwise_api.client.models.vertex_ai_model_garden_embedding_model import VertexAIModelGardenEmbeddingModel
 from superwise_api.client.models.visualization_type import VisualizationType
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/alert_on_status_direction.py` & `superwise_api-1.3.0/superwise_api/client/models/alert_on_status_direction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import json
 import pprint
 import re  # noqa: F401
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/application_create.py` & `superwise_api-1.3.0/superwise_api/client/models/application_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.4.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/application_response.py` & `superwise_api-1.3.0/superwise_api/client/models/application_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.4.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/application_type.py` & `superwise_api-1.3.0/superwise_api/client/models/application_type.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/client/models/application_update.py` & `superwise_api-1.3.0/superwise_api/client/models/application_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.4.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/ask_config.py` & `superwise_api-1.3.0/superwise_api/client/models/ask_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.4.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/ask_request_payload.py` & `superwise_api-1.3.0/superwise_api/client/models/ask_request_payload.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
@@ -17,24 +17,24 @@
 from typing import List
 
 from pydantic import BaseModel
 from pydantic import conlist
 from pydantic import Field
 from pydantic import StrictStr
 
-from superwise_api.client.models.ask_config import AskConfig
+from superwise_api.client.models.application_config import ApplicationConfig
 from superwise_api.client.models.chat_history_entry import ChatHistoryEntry
 
 
 class AskRequestPayload(BaseModel):
     """
     AskRequestPayload
     """
 
-    config: AskConfig = Field(..., description="The application configuration.")
+    config: ApplicationConfig = Field(..., description="The application configuration.")
     input: StrictStr = Field(..., description="The user's current message or question to the AI agent.")
     chat_history: conlist(ChatHistoryEntry) = Field(
         ..., description="The existing conversation history with the AI agent."
     )
     __properties = ["config", "input", "chat_history"]
 
     class Config:
@@ -78,15 +78,15 @@
             return None
 
         if not isinstance(obj, dict):
             return AskRequestPayload.parse_obj(obj)
 
         _obj = AskRequestPayload.parse_obj(
             {
-                "config": AskConfig.from_dict(obj.get("config")) if obj.get("config") is not None else None,
+                "config": ApplicationConfig.from_dict(obj.get("config")) if obj.get("config") is not None else None,
                 "input": obj.get("input"),
                 "chat_history": [ChatHistoryEntry.from_dict(_item) for _item in obj.get("chat_history")]
                 if obj.get("chat_history") is not None
                 else None,
             }
         )
         return _obj
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/ask_response_payload.py` & `superwise_api-1.3.0/superwise_api/client/models/ask_response_payload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.4.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/aws_credentials_request.py` & `superwise_api-1.3.0/superwise_api/client/models/aws_credentials_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/aws_credentials_response.py` & `superwise_api-1.3.0/superwise_api/client/models/aws_credentials_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/azure_credentials_request.py` & `superwise_api-1.3.0/superwise_api/client/models/azure_credentials_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/azure_credentials_response.py` & `superwise_api-1.3.0/superwise_api/client/models/azure_credentials_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/chat_history_entry.py` & `superwise_api-1.3.0/superwise_api/client/models/chat_history_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/config.py` & `superwise_api-1.3.0/superwise_api/client/models/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/config1.py` & `superwise_api-1.3.0/superwise_api/client/models/tool_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,81 +1,103 @@
 # coding: utf-8
-
 """
     Superwise Main Entities
 
     API reference
 
     The version of the OpenAPI document: 1.5.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
-
-
 from __future__ import annotations
-from inspect import getfullargspec
+
 import json
 import pprint
 import re  # noqa: F401
+from inspect import getfullargspec
+from typing import Any
+from typing import List
+from typing import Optional
+from typing import TYPE_CHECKING
+from typing import Union
+
+from pydantic import BaseModel
+from pydantic import Field
+from pydantic import StrictStr
+from pydantic import ValidationError
+from pydantic import validator
 
-from typing import Any, Optional
-from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
 from superwise_api.client.models.tool_config_big_query import ToolConfigBigQuery
 from superwise_api.client.models.tool_config_pg_vector import ToolConfigPGVector
 from superwise_api.client.models.tool_config_sql_database_mssql import ToolConfigSQLDatabaseMSSQL
 from superwise_api.client.models.tool_config_sql_database_my_sql import ToolConfigSQLDatabaseMySQL
 from superwise_api.client.models.tool_config_sql_database_oracle import ToolConfigSQLDatabaseOracle
 from superwise_api.client.models.tool_config_sql_database_postgres import ToolConfigSQLDatabasePostgres
-from typing import Union, Any, List, TYPE_CHECKING
-from pydantic import StrictStr, Field
 
-CONFIG1_ANY_OF_SCHEMAS = ["ToolConfigBigQuery", "ToolConfigPGVector", "ToolConfigSQLDatabaseMSSQL", "ToolConfigSQLDatabaseMySQL", "ToolConfigSQLDatabaseOracle", "ToolConfigSQLDatabasePostgres", "object"]
+TOOL_CONFIG_ANY_OF_SCHEMAS = [
+    "ToolConfigBigQuery",
+    "ToolConfigPGVector",
+    "ToolConfigSQLDatabaseMSSQL",
+    "ToolConfigSQLDatabaseMySQL",
+    "ToolConfigSQLDatabaseOracle",
+    "ToolConfigSQLDatabasePostgres",
+    "object",
+]
 
-class Config1(BaseModel):
+
+class ToolConfig(BaseModel):
     """
-    Config1
+    ToolConfig
     """
 
     # data type: ToolConfigSQLDatabasePostgres
     anyof_schema_1_validator: Optional[ToolConfigSQLDatabasePostgres] = None
     # data type: ToolConfigSQLDatabaseMySQL
     anyof_schema_2_validator: Optional[ToolConfigSQLDatabaseMySQL] = None
     # data type: ToolConfigSQLDatabaseMSSQL
-    anyof_schema_3_validator: Optional[ToolConfigSQLDatabaseMSSQL] = None
+    anyof_schema_4_validator: Optional[ToolConfigSQLDatabaseMSSQL] = None
     # data type: ToolConfigSQLDatabaseOracle
-    anyof_schema_4_validator: Optional[ToolConfigSQLDatabaseOracle] = None
+    anyof_schema_5_validator: Optional[ToolConfigSQLDatabaseOracle] = None
     # data type: ToolConfigBigQuery
-    anyof_schema_5_validator: Optional[ToolConfigBigQuery] = None
+    anyof_schema_6_validator: Optional[ToolConfigBigQuery] = None
     # data type: ToolConfigPGVector
-    anyof_schema_6_validator: Optional[ToolConfigPGVector] = None
+    anyof_schema_7_validator: Optional[ToolConfigPGVector] = None
     # data type: object
-    anyof_schema_7_validator: Optional[Any] = None
+    anyof_schema_8_validator: Optional[Any] = None
     if TYPE_CHECKING:
-        actual_instance: Union[ToolConfigBigQuery, ToolConfigPGVector, ToolConfigSQLDatabaseMSSQL, ToolConfigSQLDatabaseMySQL, ToolConfigSQLDatabaseOracle, ToolConfigSQLDatabasePostgres, object]
+        actual_instance: Union[
+            ToolConfigBigQuery,
+            ToolConfigPGVector,
+            ToolConfigSQLDatabaseMSSQL,
+            ToolConfigSQLDatabaseMySQL,
+            ToolConfigSQLDatabaseOracle,
+            ToolConfigSQLDatabasePostgres,
+            object,
+        ]
     else:
         actual_instance: Any
-    any_of_schemas: List[str] = Field(CONFIG1_ANY_OF_SCHEMAS, const=True)
+    any_of_schemas: List[str] = Field(TOOL_CONFIG_ANY_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
     def __init__(self, *args, **kwargs) -> None:
         if args:
             if len(args) > 1:
                 raise ValueError("If a position argument is used, only 1 is allowed to set `actual_instance`")
             if kwargs:
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
-    @validator('actual_instance')
+    @validator("actual_instance")
     def actual_instance_must_validate_anyof(cls, v):
-        instance = Config1.construct()
+        instance = ToolConfig.construct()
         error_messages = []
         # validate data type: ToolConfigSQLDatabasePostgres
         if not isinstance(v, ToolConfigSQLDatabasePostgres):
             error_messages.append(f"Error! Input type `{type(v)}` is not `ToolConfigSQLDatabasePostgres`")
         else:
             return v
 
@@ -107,82 +129,88 @@
         if not isinstance(v, ToolConfigPGVector):
             error_messages.append(f"Error! Input type `{type(v)}` is not `ToolConfigPGVector`")
         else:
             return v
 
         # validate data type: object
         try:
-            instance.anyof_schema_7_validator = v
+            instance.anyof_schema_8_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in Config1 with anyOf schemas: ToolConfigBigQuery, ToolConfigPGVector, ToolConfigSQLDatabaseMSSQL, ToolConfigSQLDatabaseMySQL, ToolConfigSQLDatabaseOracle, ToolConfigSQLDatabasePostgres, object. Details: " + ", ".join(error_messages))
+            raise ValueError(
+                "No match found when setting the actual_instance in ToolConfig with anyOf schemas: ToolConfigBigQuery, ToolConfigPGVector, ToolConfigSQLDatabaseMSSQL, ToolConfigSQLDatabaseMySQL, ToolConfigSQLDatabaseOracle, ToolConfigSQLDatabasePostgres, object. Details: "
+                + ", ".join(error_messages)
+            )
         else:
             return v
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Config1:
+    def from_dict(cls, obj: dict) -> ToolConfig:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
-    def from_json(cls, json_str: str) -> Config1:
+    def from_json(cls, json_str: str) -> ToolConfig:
         """Returns the object represented by the json string"""
-        instance = Config1.construct()
+        instance = ToolConfig.construct()
         error_messages = []
         # anyof_schema_1_validator: Optional[ToolConfigSQLDatabasePostgres] = None
         try:
             instance.actual_instance = ToolConfigSQLDatabasePostgres.from_json(json_str)
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
+            error_messages.append(str(e))
         # anyof_schema_2_validator: Optional[ToolConfigSQLDatabaseMySQL] = None
         try:
             instance.actual_instance = ToolConfigSQLDatabaseMySQL.from_json(json_str)
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
-        # anyof_schema_3_validator: Optional[ToolConfigSQLDatabaseMSSQL] = None
+            error_messages.append(str(e))
+        # anyof_schema_4_validator: Optional[ToolConfigSQLDatabaseMSSQL] = None
         try:
             instance.actual_instance = ToolConfigSQLDatabaseMSSQL.from_json(json_str)
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
-        # anyof_schema_4_validator: Optional[ToolConfigSQLDatabaseOracle] = None
+            error_messages.append(str(e))
+        # anyof_schema_5_validator: Optional[ToolConfigSQLDatabaseOracle] = None
         try:
             instance.actual_instance = ToolConfigSQLDatabaseOracle.from_json(json_str)
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
-        # anyof_schema_5_validator: Optional[ToolConfigBigQuery] = None
+            error_messages.append(str(e))
+        # anyof_schema_6_validator: Optional[ToolConfigBigQuery] = None
         try:
             instance.actual_instance = ToolConfigBigQuery.from_json(json_str)
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
-        # anyof_schema_6_validator: Optional[ToolConfigPGVector] = None
+            error_messages.append(str(e))
+        # anyof_schema_7_validator: Optional[ToolConfigPGVector] = None
         try:
             instance.actual_instance = ToolConfigPGVector.from_json(json_str)
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
+            error_messages.append(str(e))
         # deserialize data into object
         try:
             # validation
-            instance.anyof_schema_7_validator = json.loads(json_str)
+            instance.anyof_schema_8_validator = json.loads(json_str)
             # assign value to actual_instance
-            instance.actual_instance = instance.anyof_schema_7_validator
+            instance.actual_instance = instance.anyof_schema_8_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into Config1 with anyOf schemas: ToolConfigBigQuery, ToolConfigPGVector, ToolConfigSQLDatabaseMSSQL, ToolConfigSQLDatabaseMySQL, ToolConfigSQLDatabaseOracle, ToolConfigSQLDatabasePostgres, object. Details: " + ", ".join(error_messages))
+            raise ValueError(
+                "No match found when deserializing the JSON string into ToolConfig with anyOf schemas: ToolConfigBigQuery, ToolConfigPGVector, ToolConfigSQLDatabaseMSSQL, ToolConfigSQLDatabaseMySQL, ToolConfigSQLDatabaseOracle, ToolConfigSQLDatabasePostgres, object. Details: "
+                + ", ".join(error_messages)
+            )
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
@@ -203,9 +231,7 @@
             return self.actual_instance.to_dict()
         else:
             return json.dumps(self.actual_instance)
 
     def to_str(self) -> str:
         """Returns the string representation of the actual instance"""
         return pprint.pformat(self.dict())
-
-
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/created_by.py` & `superwise_api-1.3.0/superwise_api/client/models/created_by.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/dashboard.py` & `superwise_api-1.3.0/superwise_api/client/models/dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/dashboard_create.py` & `superwise_api-1.3.0/superwise_api/client/models/dashboard_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/dashboard_item.py` & `superwise_api-1.3.0/superwise_api/client/models/dashboard_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/dashboard_item_create.py` & `superwise_api-1.3.0/superwise_api/client/models/dashboard_item_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/dashboard_item_query.py` & `superwise_api-1.3.0/superwise_api/client/models/dashboard_item_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/dashboard_item_query_order.py` & `superwise_api-1.3.0/superwise_api/client/models/dashboard_item_query_order.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/dashboard_update.py` & `superwise_api-1.3.0/superwise_api/client/models/dashboard_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/dataset_create.py` & `superwise_api-1.3.0/superwise_api/client/models/page_application_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.4.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
 import pprint
 import re  # noqa: F401
 from typing import List
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import conlist
-from pydantic import constr
 from pydantic import Field
-from pydantic import StrictStr
 
-from superwise_api.client.models.dataset_tag import DatasetTag
-from superwise_api.client.models.model_schema import ModelSchema
+from superwise_api.client.models.application_response import ApplicationResponse
+from superwise_api.client.models.page import Page
+from superwise_api.client.models.pages import Pages
+from superwise_api.client.models.size import Size
+from superwise_api.client.models.total import Total
 
 
-class DatasetCreate(BaseModel):
+class PageApplicationResponse(BaseModel):
     """
-    DatasetCreate
+    PageApplicationResponse
     """
 
-    name: constr(strict=True, max_length=100, min_length=1) = Field(
-        ..., description="A descriptive name for this dataset"
-    )
-    description: Optional[StrictStr] = Field(None, description="Relevant information about the context of this dataset")
-    id: Optional[StrictStr] = None
-    model_version_id: Optional[StrictStr] = None
-    tags: Optional[conlist(DatasetTag)] = None
-    var_schema: Optional[ModelSchema] = Field(None, alias="schema")
-    __properties = ["name", "description", "id", "model_version_id", "tags", "schema"]
+    items: conlist(ApplicationResponse) = Field(...)
+    total: Total = Field(...)
+    page: Page = Field(...)
+    size: Size = Field(...)
+    pages: Optional[Pages] = None
+    __properties = ["items", "total", "page", "size", "pages"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -53,48 +51,56 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> DatasetCreate:
-        """Create an instance of DatasetCreate from a JSON string"""
+    def from_json(cls, json_str: str) -> PageApplicationResponse:
+        """Create an instance of PageApplicationResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in tags (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in items (list)
         _items = []
-        if self.tags:
-            for _item in self.tags:
+        if self.items:
+            for _item in self.items:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict["tags"] = _items
-        # override the default output from pydantic by calling `to_dict()` of var_schema
-        if self.var_schema:
-            _dict["schema"] = self.var_schema.to_dict()
+            _dict["items"] = _items
+        # override the default output from pydantic by calling `to_dict()` of total
+        if self.total:
+            _dict["total"] = self.total.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of page
+        if self.page:
+            _dict["page"] = self.page.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of size
+        if self.size:
+            _dict["size"] = self.size.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of pages
+        if self.pages:
+            _dict["pages"] = self.pages.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> DatasetCreate:
-        """Create an instance of DatasetCreate from a dict"""
+    def from_dict(cls, obj: dict) -> PageApplicationResponse:
+        """Create an instance of PageApplicationResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return DatasetCreate.parse_obj(obj)
+            return PageApplicationResponse.parse_obj(obj)
 
-        _obj = DatasetCreate.parse_obj(
+        _obj = PageApplicationResponse.parse_obj(
             {
-                "name": obj.get("name"),
-                "description": obj.get("description"),
-                "id": obj.get("id"),
-                "model_version_id": obj.get("model_version_id"),
-                "tags": [DatasetTag.from_dict(_item) for _item in obj.get("tags")]
-                if obj.get("tags") is not None
+                "items": [ApplicationResponse.from_dict(_item) for _item in obj.get("items")]
+                if obj.get("items") is not None
                 else None,
-                "var_schema": ModelSchema.from_dict(obj.get("schema")) if obj.get("schema") is not None else None,
+                "total": Total.from_dict(obj.get("total")) if obj.get("total") is not None else None,
+                "page": Page.from_dict(obj.get("page")) if obj.get("page") is not None else None,
+                "size": Size.from_dict(obj.get("size")) if obj.get("size") is not None else None,
+                "pages": Pages.from_dict(obj.get("pages")) if obj.get("pages") is not None else None,
             }
         )
         return _obj
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/dataset_response.py` & `superwise_api-1.3.0/superwise_api/client/models/dataset_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/dataset_source_create.py` & `superwise_api-1.3.0/superwise_api/client/models/dataset_source_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
 import pprint
 import re  # noqa: F401
-from datetime import datetime
 from typing import Optional
 
 from pydantic import BaseModel
-from pydantic import Field
 from pydantic import StrictStr
 
 from superwise_api.client.models.ingest_type import IngestType
 
 
-class DatasetSourceCreate(BaseModel):
+class DatasetSourceUpdate(BaseModel):
     """
-    DatasetSourceCreate
+    DatasetSourceUpdate
     """
 
-    dataset_id: StrictStr = Field(...)
-    source_id: StrictStr = Field(...)
+    id: Optional[StrictStr] = None
+    dataset_id: Optional[StrictStr] = None
+    source_id: Optional[StrictStr] = None
     folder: Optional[StrictStr] = None
     query: Optional[StrictStr] = None
-    created_at: Optional[datetime] = None
-    updated_at: Optional[datetime] = None
     ingest_type: Optional[IngestType] = None
-    __properties = ["dataset_id", "source_id", "folder", "query", "created_at", "updated_at", "ingest_type"]
+    created_by: Optional[StrictStr] = None
+    __properties = ["id", "dataset_id", "source_id", "folder", "query", "ingest_type", "created_by"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -49,37 +47,37 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> DatasetSourceCreate:
-        """Create an instance of DatasetSourceCreate from a JSON string"""
+    def from_json(cls, json_str: str) -> DatasetSourceUpdate:
+        """Create an instance of DatasetSourceUpdate from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> DatasetSourceCreate:
-        """Create an instance of DatasetSourceCreate from a dict"""
+    def from_dict(cls, obj: dict) -> DatasetSourceUpdate:
+        """Create an instance of DatasetSourceUpdate from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return DatasetSourceCreate.parse_obj(obj)
+            return DatasetSourceUpdate.parse_obj(obj)
 
-        _obj = DatasetSourceCreate.parse_obj(
+        _obj = DatasetSourceUpdate.parse_obj(
             {
+                "id": obj.get("id"),
                 "dataset_id": obj.get("dataset_id"),
                 "source_id": obj.get("source_id"),
                 "folder": obj.get("folder"),
                 "query": obj.get("query"),
-                "created_at": obj.get("created_at"),
-                "updated_at": obj.get("updated_at"),
                 "ingest_type": obj.get("ingest_type"),
+                "created_by": obj.get("created_by"),
             }
         )
         return _obj
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/dataset_source_response.py` & `superwise_api-1.3.0/superwise_api/client/models/dataset_source_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/dataset_source_response_with_source.py` & `superwise_api-1.3.0/superwise_api/client/models/dataset_source_response_with_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/dataset_source_update.py` & `superwise_api-1.3.0/superwise_api/client/models/source_update_s3.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,53 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
 import pprint
 import re  # noqa: F401
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import StrictStr
+from pydantic import validator
 
-from superwise_api.client.models.ingest_type import IngestType
+from superwise_api.client.models.aws_credentials_request import AWSCredentialsRequest
+from superwise_api.client.models.source_s3_params import SourceS3Params
 
 
-class DatasetSourceUpdate(BaseModel):
+class SourceUpdateS3(BaseModel):
     """
-    DatasetSourceUpdate
+    SourceUpdateS3
     """
 
-    id: Optional[StrictStr] = None
-    dataset_id: Optional[StrictStr] = None
-    source_id: Optional[StrictStr] = None
-    folder: Optional[StrictStr] = None
-    query: Optional[StrictStr] = None
-    ingest_type: Optional[IngestType] = None
-    created_by: Optional[StrictStr] = None
-    __properties = ["id", "dataset_id", "source_id", "folder", "query", "ingest_type", "created_by"]
+    name: Optional[StrictStr] = None
+    credentials: Optional[AWSCredentialsRequest] = None
+    params: Optional[SourceS3Params] = None
+    type: Optional[StrictStr] = "S3"
+    __properties = ["name", "credentials", "params", "type"]
+
+    @validator("type")
+    def type_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ("S3"):
+            raise ValueError("must be one of enum values ('S3')")
+        return value
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -47,37 +56,42 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> DatasetSourceUpdate:
-        """Create an instance of DatasetSourceUpdate from a JSON string"""
+    def from_json(cls, json_str: str) -> SourceUpdateS3:
+        """Create an instance of SourceUpdateS3 from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of credentials
+        if self.credentials:
+            _dict["credentials"] = self.credentials.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of params
+        if self.params:
+            _dict["params"] = self.params.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> DatasetSourceUpdate:
-        """Create an instance of DatasetSourceUpdate from a dict"""
+    def from_dict(cls, obj: dict) -> SourceUpdateS3:
+        """Create an instance of SourceUpdateS3 from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return DatasetSourceUpdate.parse_obj(obj)
+            return SourceUpdateS3.parse_obj(obj)
 
-        _obj = DatasetSourceUpdate.parse_obj(
+        _obj = SourceUpdateS3.parse_obj(
             {
-                "id": obj.get("id"),
-                "dataset_id": obj.get("dataset_id"),
-                "source_id": obj.get("source_id"),
-                "folder": obj.get("folder"),
-                "query": obj.get("query"),
-                "ingest_type": obj.get("ingest_type"),
-                "created_by": obj.get("created_by"),
+                "name": obj.get("name"),
+                "credentials": AWSCredentialsRequest.from_dict(obj.get("credentials"))
+                if obj.get("credentials") is not None
+                else None,
+                "params": SourceS3Params.from_dict(obj.get("params")) if obj.get("params") is not None else None,
+                "type": obj.get("type") if obj.get("type") is not None else "S3",
             }
         )
         return _obj
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/dataset_tag.py` & `superwise_api-1.3.0/superwise_api/client/models/dataset_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/dataset_update.py` & `superwise_api-1.3.0/superwise_api/client/models/dataset_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/datasource.py` & `superwise_api-1.3.0/superwise_api/client/models/role.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import json
 import pprint
 import re  # noqa: F401
 
 from aenum import Enum
 from aenum import no_arg
 
 
-class Datasource(str, Enum):
+class Role(str, Enum):
     """
-    An enumeration.
+    Role
     """
 
     """
     allowed enum values
     """
-    DATASETS = "datasets"
-    EVENTS = "events"
+    HUMAN = "human"
+    AI = "ai"
 
     @classmethod
-    def from_json(cls, json_str: str) -> Datasource:
-        """Create an instance of Datasource from a JSON string"""
-        return Datasource(json.loads(json_str))
+    def from_json(cls, json_str: str) -> Role:
+        """Create an instance of Role from a JSON string"""
+        return Role(json.loads(json_str))
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/default_value.py` & `superwise_api-1.3.0/superwise_api/client/models/default_value.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/client/models/default_value1.py` & `superwise_api-1.3.0/superwise_api/client/models/default_value1.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/client/models/description.py` & `superwise_api-1.3.0/superwise_api/client/models/description.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/destination_create_base.py` & `superwise_api-1.3.0/superwise_api/client/models/destination_create_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/destination_response.py` & `superwise_api-1.3.0/superwise_api/client/models/destination_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/destination_update_base.py` & `superwise_api-1.3.0/superwise_api/client/models/destination_update_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/embedding_model.py` & `superwise_api-1.3.0/superwise_api/client/models/embedding_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/filter.py` & `superwise_api-1.3.0/superwise_api/client/models/filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/gcp_credentials_request.py` & `superwise_api-1.3.0/superwise_api/client/models/gcp_credentials_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/gcp_credentials_response.py` & `superwise_api-1.3.0/superwise_api/client/models/gcp_credentials_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/google_model_version.py` & `superwise_api-1.3.0/superwise_api/client/models/google_model_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import json
 import pprint
 import re  # noqa: F401
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/granularity.py` & `superwise_api-1.3.0/superwise_api/client/models/granularity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import json
 import pprint
 import re  # noqa: F401
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/http_validation_error.py` & `superwise_api-1.3.0/superwise_api/client/models/http_validation_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/ingest_type.py` & `superwise_api-1.3.0/superwise_api/client/models/ingest_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import json
 import pprint
 import re  # noqa: F401
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/integration_response.py` & `superwise_api-1.3.0/superwise_api/client/models/integration_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/integration_type.py` & `superwise_api-1.3.0/superwise_api/client/models/integration_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import json
 import pprint
 import re  # noqa: F401
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/model_create.py` & `superwise_api-1.3.0/superwise_api/client/models/model_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.4.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/model_id.py` & `superwise_api-1.3.0/superwise_api/client/models/model_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.4.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/model_provider.py` & `superwise_api-1.3.0/superwise_api/client/models/model_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import json
 import pprint
 import re  # noqa: F401
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/model_response.py` & `superwise_api-1.3.0/superwise_api/client/models/model_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.4.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/model_schema.py` & `superwise_api-1.3.0/superwise_api/client/models/model_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/model_version.py` & `superwise_api-1.3.0/superwise_api/client/models/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 0.1.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
@@ -23,31 +23,31 @@
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import StrictStr
 from pydantic import ValidationError
 from pydantic import validator
 
-MODELVERSION_ANY_OF_SCHEMAS = ["object", "str"]
+VERSION_ANY_OF_SCHEMAS = ["object", "str"]
 
 
-class ModelVersion(BaseModel):
+class Version(BaseModel):
     """
-    ModelVersion
+    Version
     """
 
     # data type: str
     anyof_schema_1_validator: Optional[StrictStr] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
         actual_instance: Union[object, str]
     else:
         actual_instance: Any
-    any_of_schemas: List[str] = Field(MODELVERSION_ANY_OF_SCHEMAS, const=True)
+    any_of_schemas: List[str] = Field(VERSION_ANY_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
     def __init__(self, *args, **kwargs) -> None:
         if args:
             if len(args) > 1:
@@ -56,15 +56,15 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @validator("actual_instance")
     def actual_instance_must_validate_anyof(cls, v):
-        instance = ModelVersion.construct()
+        instance = Version.construct()
         error_messages = []
         # validate data type: str
         try:
             instance.anyof_schema_1_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
@@ -73,28 +73,28 @@
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
             raise ValueError(
-                "No match found when setting the actual_instance in ModelVersion with anyOf schemas: object, str. Details: "
+                "No match found when setting the actual_instance in Version with anyOf schemas: object, str. Details: "
                 + ", ".join(error_messages)
             )
         else:
             return v
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ModelVersion:
+    def from_dict(cls, obj: dict) -> Version:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
-    def from_json(cls, json_str: str) -> ModelVersion:
+    def from_json(cls, json_str: str) -> Version:
         """Returns the object represented by the json string"""
-        instance = ModelVersion.construct()
+        instance = Version.construct()
         error_messages = []
         # deserialize data into str
         try:
             # validation
             instance.anyof_schema_1_validator = json.loads(json_str)
             # assign value to actual_instance
             instance.actual_instance = instance.anyof_schema_1_validator
@@ -110,15 +110,15 @@
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
             raise ValueError(
-                "No match found when deserializing the JSON string into ModelVersion with anyOf schemas: object, str. Details: "
+                "No match found when deserializing the JSON string into Version with anyOf schemas: object, str. Details: "
                 + ", ".join(error_messages)
             )
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/model_version_response.py` & `superwise_api-1.3.0/superwise_api/client/models/model_version_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.4.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/name.py` & `superwise_api-1.3.0/superwise_api/client/models/name.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/open_ai_model_version.py` & `superwise_api-1.3.0/superwise_api/client/models/open_ai_model_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import json
 import pprint
 import re  # noqa: F401
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/order.py` & `superwise_api-1.3.0/superwise_api/client/models/order.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/client/models/order1.py` & `superwise_api-1.3.0/superwise_api/client/models/order1.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/client/models/page.py` & `superwise_api-1.3.0/superwise_api/client/models/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/page_application_response.py` & `superwise_api-1.3.0/superwise_api/client/models/page_application.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
@@ -17,27 +17,27 @@
 from typing import List
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import conlist
 from pydantic import Field
 
-from superwise_api.client.models.application_response import ApplicationResponse
+from superwise_api.client.models.application import Application
 from superwise_api.client.models.page import Page
 from superwise_api.client.models.pages import Pages
 from superwise_api.client.models.size import Size
 from superwise_api.client.models.total import Total
 
 
-class PageApplicationResponse(BaseModel):
+class PageApplication(BaseModel):
     """
-    PageApplicationResponse
+    PageApplication
     """
 
-    items: conlist(ApplicationResponse) = Field(...)
+    items: conlist(Application) = Field(...)
     total: Total = Field(...)
     page: Page = Field(...)
     size: Size = Field(...)
     pages: Optional[Pages] = None
     __properties = ["items", "total", "page", "size", "pages"]
 
     class Config:
@@ -51,16 +51,16 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> PageApplicationResponse:
-        """Create an instance of PageApplicationResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> PageApplication:
+        """Create an instance of PageApplication from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of each item in items (list)
         _items = []
@@ -80,25 +80,25 @@
             _dict["size"] = self.size.to_dict()
         # override the default output from pydantic by calling `to_dict()` of pages
         if self.pages:
             _dict["pages"] = self.pages.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PageApplicationResponse:
-        """Create an instance of PageApplicationResponse from a dict"""
+    def from_dict(cls, obj: dict) -> PageApplication:
+        """Create an instance of PageApplication from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return PageApplicationResponse.parse_obj(obj)
+            return PageApplication.parse_obj(obj)
 
-        _obj = PageApplicationResponse.parse_obj(
+        _obj = PageApplication.parse_obj(
             {
-                "items": [ApplicationResponse.from_dict(_item) for _item in obj.get("items")]
+                "items": [Application.from_dict(_item) for _item in obj.get("items")]
                 if obj.get("items") is not None
                 else None,
                 "total": Total.from_dict(obj.get("total")) if obj.get("total") is not None else None,
                 "page": Page.from_dict(obj.get("page")) if obj.get("page") is not None else None,
                 "size": Size.from_dict(obj.get("size")) if obj.get("size") is not None else None,
                 "pages": Pages.from_dict(obj.get("pages")) if obj.get("pages") is not None else None,
             }
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/page_dashboard.py` & `superwise_api-1.3.0/superwise_api/client/models/page_dashboard.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/page_dashboard_item.py` & `superwise_api-1.3.0/superwise_api/client/models/page_dashboard_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/page_dataset_response.py` & `superwise_api-1.3.0/superwise_api/client/models/page_dataset_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/page_dataset_source_response_with_source.py` & `superwise_api-1.3.0/superwise_api/client/models/page_dataset_source_response_with_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/page_destination_response.py` & `superwise_api-1.3.0/superwise_api/client/models/page_destination_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/page_integration_response.py` & `superwise_api-1.3.0/superwise_api/client/models/page_integration_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/page_model_response.py` & `superwise_api-1.3.0/superwise_api/client/models/page_model_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.4.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/page_policy_response.py` & `superwise_api-1.3.0/superwise_api/client/models/page_policy_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/page_source_response.py` & `superwise_api-1.3.0/superwise_api/client/models/page_source_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/page_tool_response.py` & `superwise_api-1.3.0/superwise_api/client/models/page_tool_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.4.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/pages.py` & `superwise_api-1.3.0/superwise_api/client/models/pages.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/payload.py` & `superwise_api-1.3.0/superwise_api/client/models/payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/policy_create.py` & `superwise_api-1.3.0/superwise_api/client/models/policy_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/policy_query.py` & `superwise_api-1.3.0/superwise_api/client/models/query.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 0.1.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
@@ -16,31 +16,35 @@
 import re  # noqa: F401
 from typing import List
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import conlist
 from pydantic import Field
+from pydantic import StrictInt
 from pydantic import StrictStr
 
-from superwise_api.client.models.dashboard_item_query_order import DashboardItemQueryOrder
-from superwise_api.client.models.policy_query_filter import PolicyQueryFilter
+from superwise_api.client.models.filter import Filter
+from superwise_api.client.models.order import Order
+from superwise_api.client.models.time_dimension import TimeDimension
 
 
-class PolicyQuery(BaseModel):
+class Query(BaseModel):
     """
-    PolicyQuery
+    Query
     """
 
     measures: conlist(StrictStr) = Field(...)
-    order: Optional[DashboardItemQueryOrder] = None
+    order: Optional[Order] = None
     dimensions: Optional[conlist(StrictStr)] = None
     timezone: Optional[StrictStr] = "UTC"
-    filters: Optional[conlist(PolicyQueryFilter)] = None
-    __properties = ["measures", "order", "dimensions", "timezone", "filters"]
+    filters: Optional[conlist(Filter)] = None
+    limit: StrictInt = Field(...)
+    time_dimensions: conlist(TimeDimension) = Field(...)
+    __properties = ["measures", "order", "dimensions", "timezone", "filters", "limit", "time_dimensions"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -49,16 +53,16 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> PolicyQuery:
-        """Create an instance of PolicyQuery from a JSON string"""
+    def from_json(cls, json_str: str) -> Query:
+        """Create an instance of Query from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of order
         if self.order:
@@ -66,30 +70,41 @@
         # override the default output from pydantic by calling `to_dict()` of each item in filters (list)
         _items = []
         if self.filters:
             for _item in self.filters:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["filters"] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in time_dimensions (list)
+        _items = []
+        if self.time_dimensions:
+            for _item in self.time_dimensions:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict["time_dimensions"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PolicyQuery:
-        """Create an instance of PolicyQuery from a dict"""
+    def from_dict(cls, obj: dict) -> Query:
+        """Create an instance of Query from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return PolicyQuery.parse_obj(obj)
+            return Query.parse_obj(obj)
 
-        _obj = PolicyQuery.parse_obj(
+        _obj = Query.parse_obj(
             {
                 "measures": obj.get("measures"),
-                "order": DashboardItemQueryOrder.from_dict(obj.get("order")) if obj.get("order") is not None else None,
+                "order": Order.from_dict(obj.get("order")) if obj.get("order") is not None else None,
                 "dimensions": obj.get("dimensions"),
                 "timezone": obj.get("timezone") if obj.get("timezone") is not None else "UTC",
-                "filters": [PolicyQueryFilter.from_dict(_item) for _item in obj.get("filters")]
+                "filters": [Filter.from_dict(_item) for _item in obj.get("filters")]
                 if obj.get("filters") is not None
                 else None,
+                "limit": obj.get("limit"),
+                "time_dimensions": [TimeDimension.from_dict(_item) for _item in obj.get("time_dimensions")]
+                if obj.get("time_dimensions") is not None
+                else None,
             }
         )
         return _obj
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/policy_query_filter.py` & `superwise_api-1.3.0/superwise_api/client/models/policy_query_filter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/policy_query_order.py` & `superwise_api-1.3.0/superwise_api/client/models/policy_query_order.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/policy_response.py` & `superwise_api-1.3.0/superwise_api/client/models/policy_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/policy_status.py` & `superwise_api-1.3.0/superwise_api/client/models/policy_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import json
 import pprint
 import re  # noqa: F401
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/policy_update.py` & `superwise_api-1.3.0/superwise_api/client/models/policy_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/prompt.py` & `superwise_api-1.3.0/superwise_api/client/models/prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/provider.py` & `superwise_api-1.3.0/superwise_api/client/models/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.4.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/query.py` & `superwise_api-1.3.0/superwise_api/client/models/application_config_payload.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
@@ -16,35 +16,31 @@
 import re  # noqa: F401
 from typing import List
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import conlist
 from pydantic import Field
-from pydantic import StrictInt
 from pydantic import StrictStr
 
-from superwise_api.client.models.filter import Filter
-from superwise_api.client.models.order import Order
-from superwise_api.client.models.time_dimension import TimeDimension
+from superwise_api.client.models.application_model import ApplicationModel
+from superwise_api.client.models.prompt import Prompt
+from superwise_api.client.models.tool_def_input import ToolDefInput
 
 
-class Query(BaseModel):
+class ApplicationConfigPayload(BaseModel):
     """
-    Query
+    ApplicationConfigPayload
     """
 
-    measures: conlist(StrictStr) = Field(...)
-    order: Optional[Order] = None
-    dimensions: Optional[conlist(StrictStr)] = None
-    timezone: Optional[StrictStr] = "UTC"
-    filters: Optional[conlist(Filter)] = None
-    limit: StrictInt = Field(...)
-    time_dimensions: conlist(TimeDimension) = Field(...)
-    __properties = ["measures", "order", "dimensions", "timezone", "filters", "limit", "time_dimensions"]
+    model: Optional[ApplicationModel] = None
+    prompt: Optional[Prompt] = None
+    tools: conlist(ToolDefInput) = Field(...)
+    name: StrictStr = Field(...)
+    __properties = ["model", "prompt", "tools", "name"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -53,58 +49,49 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Query:
-        """Create an instance of Query from a JSON string"""
+    def from_json(cls, json_str: str) -> ApplicationConfigPayload:
+        """Create an instance of ApplicationConfigPayload from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of order
-        if self.order:
-            _dict["order"] = self.order.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in filters (list)
+        _dict = self.dict(by_alias=True, exclude={}, exclude_none=False)
+        # override the default output from pydantic by calling `to_dict()` of model
+        if self.model:
+            _dict["model"] = self.model.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of prompt
+        if self.prompt:
+            _dict["prompt"] = self.prompt.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in tools (list)
         _items = []
-        if self.filters:
-            for _item in self.filters:
+        if self.tools:
+            for _item in self.tools:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict["filters"] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in time_dimensions (list)
-        _items = []
-        if self.time_dimensions:
-            for _item in self.time_dimensions:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict["time_dimensions"] = _items
+            _dict["tools"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Query:
-        """Create an instance of Query from a dict"""
+    def from_dict(cls, obj: dict) -> ApplicationConfigPayload:
+        """Create an instance of ApplicationConfigPayload from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return Query.parse_obj(obj)
+            return ApplicationConfigPayload.parse_obj(obj)
 
-        _obj = Query.parse_obj(
+        _obj = ApplicationConfigPayload.parse_obj(
             {
-                "measures": obj.get("measures"),
-                "order": Order.from_dict(obj.get("order")) if obj.get("order") is not None else None,
-                "dimensions": obj.get("dimensions"),
-                "timezone": obj.get("timezone") if obj.get("timezone") is not None else "UTC",
-                "filters": [Filter.from_dict(_item) for _item in obj.get("filters")]
-                if obj.get("filters") is not None
-                else None,
-                "limit": obj.get("limit"),
-                "time_dimensions": [TimeDimension.from_dict(_item) for _item in obj.get("time_dimensions")]
-                if obj.get("time_dimensions") is not None
+                "model": ApplicationModel.from_dict(obj.get("model")) if obj.get("model") is not None else None,
+                "prompt": Prompt.from_dict(obj.get("prompt")) if obj.get("prompt") is not None else None,
+                "tools": [ToolDefInput.from_dict(_item) for _item in obj.get("tools")]
+                if obj.get("tools") is not None
                 else None,
+                "name": obj.get("name"),
             }
         )
         return _obj
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/query_type.py` & `superwise_api-1.3.0/superwise_api/client/models/query_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import json
 import pprint
 import re  # noqa: F401
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/role.py` & `superwise_api-1.3.0/superwise_api/client/models/type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import json
 import pprint
 import re  # noqa: F401
 
 from aenum import Enum
 from aenum import no_arg
 
 
-class Role(str, Enum):
+class Type(str, Enum):
     """
-    Role
+    An enumeration.
     """
 
     """
     allowed enum values
     """
-    HUMAN = "human"
-    AI = "ai"
+    NUMERIC = "numeric"
+    STRING = "string"
+    BOOLEAN = "boolean"
+    DATETIME = "datetime"
+    DATE = "date"
 
     @classmethod
-    def from_json(cls, json_str: str) -> Role:
-        """Create an instance of Role from a JSON string"""
-        return Role(json.loads(json_str))
+    def from_json(cls, json_str: str) -> Type:
+        """Create an instance of Type from a JSON string"""
+        return Type(json.loads(json_str))
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/schema_item.py` & `superwise_api-1.3.0/superwise_api/client/models/schema_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/schema_update.py` & `superwise_api-1.3.0/superwise_api/client/models/schema_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/schema_update_item.py` & `superwise_api-1.3.0/superwise_api/client/models/tool_config_big_query.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
 import pprint
 import re  # noqa: F401
 from typing import Any
 from typing import Optional
 
 from pydantic import BaseModel
+from pydantic import Field
 from pydantic import StrictStr
 
-from superwise_api.client.models.type import Type
 
-
-class SchemaUpdateItem(BaseModel):
+class ToolConfigBigQuery(BaseModel):
     """
-    SchemaUpdateItem
+    ToolConfigBigQuery
     """
 
-    name: Optional[StrictStr] = None
-    type: Optional[Type] = None
-    default_value: Optional[Any] = None
-    __properties = ["name", "type", "default_value"]
+    type: Optional[Any] = Field(...)
+    project_id: StrictStr = Field(...)
+    dataset_id: StrictStr = Field(...)
+    service_account: Any = Field(...)
+    __properties = ["type", "project_id", "dataset_id", "service_account"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -44,34 +44,38 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SchemaUpdateItem:
-        """Create an instance of SchemaUpdateItem from a JSON string"""
+    def from_json(cls, json_str: str) -> ToolConfigBigQuery:
+        """Create an instance of ToolConfigBigQuery from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
-        # set to None if default_value (nullable) is None
+        # set to None if type (nullable) is None
         # and __fields_set__ contains the field
-        if self.default_value is None and "default_value" in self.__fields_set__:
-            _dict["default_value"] = None
+        if self.type is None and "type" in self.__fields_set__:
+            _dict["type"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SchemaUpdateItem:
-        """Create an instance of SchemaUpdateItem from a dict"""
+    def from_dict(cls, obj: dict) -> ToolConfigBigQuery:
+        """Create an instance of ToolConfigBigQuery from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return SchemaUpdateItem.parse_obj(obj)
+            return ToolConfigBigQuery.parse_obj(obj)
 
-        _obj = SchemaUpdateItem.parse_obj(
-            {"name": obj.get("name"), "type": obj.get("type"), "default_value": obj.get("default_value")}
+        _obj = ToolConfigBigQuery.parse_obj(
+            {
+                "type": obj.get("type"),
+                "project_id": obj.get("project_id"),
+                "dataset_id": obj.get("dataset_id"),
+            }
         )
         return _obj
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/size.py` & `superwise_api-1.3.0/superwise_api/client/models/total.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
@@ -24,31 +24,31 @@
 from pydantic import BaseModel
 from pydantic import conint
 from pydantic import Field
 from pydantic import StrictStr
 from pydantic import ValidationError
 from pydantic import validator
 
-SIZE_ANY_OF_SCHEMAS = ["int", "object"]
+TOTAL_ANY_OF_SCHEMAS = ["int", "object"]
 
 
-class Size(BaseModel):
+class Total(BaseModel):
     """
-    Size
+    Total
     """
 
     # data type: int
-    anyof_schema_1_validator: Optional[conint(strict=True, ge=1)] = None
+    anyof_schema_1_validator: Optional[conint(strict=True, ge=0)] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
         actual_instance: Union[int, object]
     else:
         actual_instance: Any
-    any_of_schemas: List[str] = Field(SIZE_ANY_OF_SCHEMAS, const=True)
+    any_of_schemas: List[str] = Field(TOTAL_ANY_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
     def __init__(self, *args, **kwargs) -> None:
         if args:
             if len(args) > 1:
@@ -57,15 +57,15 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @validator("actual_instance")
     def actual_instance_must_validate_anyof(cls, v):
-        instance = Size.construct()
+        instance = Total.construct()
         error_messages = []
         # validate data type: int
         try:
             instance.anyof_schema_1_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
@@ -74,28 +74,28 @@
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
             raise ValueError(
-                "No match found when setting the actual_instance in Size with anyOf schemas: int, object. Details: "
+                "No match found when setting the actual_instance in Total with anyOf schemas: int, object. Details: "
                 + ", ".join(error_messages)
             )
         else:
             return v
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Size:
+    def from_dict(cls, obj: dict) -> Total:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
-    def from_json(cls, json_str: str) -> Size:
+    def from_json(cls, json_str: str) -> Total:
         """Returns the object represented by the json string"""
-        instance = Size.construct()
+        instance = Total.construct()
         error_messages = []
         # deserialize data into int
         try:
             # validation
             instance.anyof_schema_1_validator = json.loads(json_str)
             # assign value to actual_instance
             instance.actual_instance = instance.anyof_schema_1_validator
@@ -111,15 +111,15 @@
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
             raise ValueError(
-                "No match found when deserializing the JSON string into Size with anyOf schemas: int, object. Details: "
+                "No match found when deserializing the JSON string into Total with anyOf schemas: int, object. Details: "
                 + ", ".join(error_messages)
             )
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/source.py` & `superwise_api-1.3.0/superwise_api/client/models/source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/source_azure_params.py` & `superwise_api-1.3.0/superwise_api/client/models/source_azure_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/source_create.py` & `superwise_api-1.3.0/superwise_api/client/models/source_create.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/client/models/source_create_azure.py` & `superwise_api-1.3.0/superwise_api/client/models/source_update_gcs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
 import pprint
 import re  # noqa: F401
 from typing import Optional
 
 from pydantic import BaseModel
-from pydantic import Field
 from pydantic import StrictStr
 from pydantic import validator
 
-from superwise_api.client.models.azure_credentials_request import AzureCredentialsRequest
-from superwise_api.client.models.source_azure_params import SourceAzureParams
+from superwise_api.client.models.gcp_credentials_request import GCPCredentialsRequest
+from superwise_api.client.models.source_gcs_params import SourceGCSParams
 
 
-class SourceCreateAzure(BaseModel):
+class SourceUpdateGCS(BaseModel):
     """
-    SourceCreateAzure
+    SourceUpdateGCS
     """
 
-    name: StrictStr = Field(...)
-    type: Optional[StrictStr] = "AZURE_BLOB_STORAGE"
-    credentials: AzureCredentialsRequest = Field(...)
-    params: SourceAzureParams = Field(...)
-    __properties = ["name", "type", "credentials", "params"]
+    name: Optional[StrictStr] = None
+    credentials: Optional[GCPCredentialsRequest] = None
+    params: Optional[SourceGCSParams] = None
+    type: Optional[StrictStr] = "GCS"
+    __properties = ["name", "credentials", "params", "type"]
 
     @validator("type")
     def type_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("AZURE_BLOB_STORAGE"):
-            raise ValueError("must be one of enum values ('AZURE_BLOB_STORAGE')")
+        if value not in ("GCS"):
+            raise ValueError("must be one of enum values ('GCS')")
         return value
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
@@ -57,42 +56,42 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SourceCreateAzure:
-        """Create an instance of SourceCreateAzure from a JSON string"""
+    def from_json(cls, json_str: str) -> SourceUpdateGCS:
+        """Create an instance of SourceUpdateGCS from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of credentials
         if self.credentials:
             _dict["credentials"] = self.credentials.to_dict()
         # override the default output from pydantic by calling `to_dict()` of params
         if self.params:
             _dict["params"] = self.params.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SourceCreateAzure:
-        """Create an instance of SourceCreateAzure from a dict"""
+    def from_dict(cls, obj: dict) -> SourceUpdateGCS:
+        """Create an instance of SourceUpdateGCS from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return SourceCreateAzure.parse_obj(obj)
+            return SourceUpdateGCS.parse_obj(obj)
 
-        _obj = SourceCreateAzure.parse_obj(
+        _obj = SourceUpdateGCS.parse_obj(
             {
                 "name": obj.get("name"),
-                "type": obj.get("type") if obj.get("type") is not None else "AZURE_BLOB_STORAGE",
-                "credentials": AzureCredentialsRequest.from_dict(obj.get("credentials"))
+                "credentials": GCPCredentialsRequest.from_dict(obj.get("credentials"))
                 if obj.get("credentials") is not None
                 else None,
-                "params": SourceAzureParams.from_dict(obj.get("params")) if obj.get("params") is not None else None,
+                "params": SourceGCSParams.from_dict(obj.get("params")) if obj.get("params") is not None else None,
+                "type": obj.get("type") if obj.get("type") is not None else "GCS",
             }
         )
         return _obj
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/source_create_gcs.py` & `superwise_api-1.3.0/superwise_api/client/models/source_get_s3.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
 import pprint
 import re  # noqa: F401
+from datetime import datetime
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import StrictStr
 from pydantic import validator
 
-from superwise_api.client.models.gcp_credentials_request import GCPCredentialsRequest
-from superwise_api.client.models.source_gcs_params import SourceGCSParams
+from superwise_api.client.models.aws_credentials_response import AWSCredentialsResponse
+from superwise_api.client.models.source_s3_params import SourceS3Params
 
 
-class SourceCreateGCS(BaseModel):
+class SourceGetS3(BaseModel):
     """
-    SourceCreateGCS
+    SourceGetS3
     """
 
+    id: StrictStr = Field(...)
     name: StrictStr = Field(...)
-    type: Optional[StrictStr] = "GCS"
-    credentials: Optional[GCPCredentialsRequest] = None
-    params: SourceGCSParams = Field(...)
-    __properties = ["name", "type", "credentials", "params"]
+    created_at: Optional[datetime] = None
+    updated_at: Optional[datetime] = None
+    created_by: StrictStr = Field(...)
+    type: StrictStr = Field(...)
+    params: SourceS3Params = Field(...)
+    credentials: AWSCredentialsResponse = Field(...)
+    __properties = ["id", "name", "created_at", "updated_at", "created_by", "type", "params", "credentials"]
 
     @validator("type")
     def type_validate_enum(cls, value):
         """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in ("GCS"):
-            raise ValueError("must be one of enum values ('GCS')")
+        if value not in ("S3"):
+            raise ValueError("must be one of enum values ('S3')")
         return value
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
@@ -57,42 +59,46 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SourceCreateGCS:
-        """Create an instance of SourceCreateGCS from a JSON string"""
+    def from_json(cls, json_str: str) -> SourceGetS3:
+        """Create an instance of SourceGetS3 from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of credentials
-        if self.credentials:
-            _dict["credentials"] = self.credentials.to_dict()
         # override the default output from pydantic by calling `to_dict()` of params
         if self.params:
             _dict["params"] = self.params.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of credentials
+        if self.credentials:
+            _dict["credentials"] = self.credentials.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SourceCreateGCS:
-        """Create an instance of SourceCreateGCS from a dict"""
+    def from_dict(cls, obj: dict) -> SourceGetS3:
+        """Create an instance of SourceGetS3 from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return SourceCreateGCS.parse_obj(obj)
+            return SourceGetS3.parse_obj(obj)
 
-        _obj = SourceCreateGCS.parse_obj(
+        _obj = SourceGetS3.parse_obj(
             {
+                "id": obj.get("id"),
                 "name": obj.get("name"),
-                "type": obj.get("type") if obj.get("type") is not None else "GCS",
-                "credentials": GCPCredentialsRequest.from_dict(obj.get("credentials"))
+                "created_at": obj.get("created_at"),
+                "updated_at": obj.get("updated_at"),
+                "created_by": obj.get("created_by"),
+                "type": obj.get("type"),
+                "params": SourceS3Params.from_dict(obj.get("params")) if obj.get("params") is not None else None,
+                "credentials": AWSCredentialsResponse.from_dict(obj.get("credentials"))
                 if obj.get("credentials") is not None
                 else None,
-                "params": SourceGCSParams.from_dict(obj.get("params")) if obj.get("params") is not None else None,
             }
         )
         return _obj
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/source_create_payload.py` & `superwise_api-1.3.0/superwise_api/client/models/source_create_payload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/source_create_s3.py` & `superwise_api-1.3.0/superwise_api/client/models/tool_config_sql_database.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,39 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.4.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
 import pprint
 import re  # noqa: F401
+from typing import Any
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import StrictStr
-from pydantic import validator
 
-from superwise_api.client.models.aws_credentials_request import AWSCredentialsRequest
-from superwise_api.client.models.source_s3_params import SourceS3Params
 
-
-class SourceCreateS3(BaseModel):
+class ToolConfigSQLDatabase(BaseModel):
     """
-    SourceCreateS3
+    ToolConfigSQLDatabase
     """
 
-    name: StrictStr = Field(...)
-    type: Optional[StrictStr] = "S3"
-    credentials: AWSCredentialsRequest = Field(...)
-    params: SourceS3Params = Field(...)
-    __properties = ["name", "type", "credentials", "params"]
-
-    @validator("type")
-    def type_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in ("S3"):
-            raise ValueError("must be one of enum values ('S3')")
-        return value
+    type: Optional[Any] = Field(...)
+    connection_string: StrictStr = Field(...)
+    __properties = ["type", "connection_string"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -57,42 +42,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SourceCreateS3:
-        """Create an instance of SourceCreateS3 from a JSON string"""
+    def from_json(cls, json_str: str) -> ToolConfigSQLDatabase:
+        """Create an instance of ToolConfigSQLDatabase from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of credentials
-        if self.credentials:
-            _dict["credentials"] = self.credentials.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of params
-        if self.params:
-            _dict["params"] = self.params.to_dict()
+        # set to None if type (nullable) is None
+        # and __fields_set__ contains the field
+        if self.type is None and "type" in self.__fields_set__:
+            _dict["type"] = None
+
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SourceCreateS3:
-        """Create an instance of SourceCreateS3 from a dict"""
+    def from_dict(cls, obj: dict) -> ToolConfigSQLDatabase:
+        """Create an instance of ToolConfigSQLDatabase from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return SourceCreateS3.parse_obj(obj)
+            return ToolConfigSQLDatabase.parse_obj(obj)
 
-        _obj = SourceCreateS3.parse_obj(
-            {
-                "name": obj.get("name"),
-                "type": obj.get("type") if obj.get("type") is not None else "S3",
-                "credentials": AWSCredentialsRequest.from_dict(obj.get("credentials"))
-                if obj.get("credentials") is not None
-                else None,
-                "params": SourceS3Params.from_dict(obj.get("params")) if obj.get("params") is not None else None,
-            }
+        _obj = ToolConfigSQLDatabase.parse_obj(
+            {"type": obj.get("type"), "connection_string": obj.get("connection_string")}
         )
         return _obj
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/source_gcs_params.py` & `superwise_api-1.3.0/superwise_api/client/models/source_gcs_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/source_get_azure.py` & `superwise_api-1.3.0/superwise_api/client/models/source_get_azure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/source_get_gcs.py` & `superwise_api-1.3.0/superwise_api/client/models/source_get_gcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/source_get_s3.py` & `superwise_api-1.3.0/superwise_api/client/models/tool_config_sql_database_mssql.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,46 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
 import pprint
 import re  # noqa: F401
-from datetime import datetime
+from typing import Any
 from typing import Optional
 
 from pydantic import BaseModel
+from pydantic import constr
 from pydantic import Field
-from pydantic import StrictStr
 from pydantic import validator
 
-from superwise_api.client.models.aws_credentials_response import AWSCredentialsResponse
-from superwise_api.client.models.source_s3_params import SourceS3Params
 
-
-class SourceGetS3(BaseModel):
+class ToolConfigSQLDatabaseMSSQL(BaseModel):
     """
-    SourceGetS3
+    ToolConfigSQLDatabaseMSSQL
     """
 
-    id: StrictStr = Field(...)
-    name: StrictStr = Field(...)
-    created_at: Optional[datetime] = None
-    updated_at: Optional[datetime] = None
-    created_by: StrictStr = Field(...)
-    type: StrictStr = Field(...)
-    params: SourceS3Params = Field(...)
-    credentials: AWSCredentialsResponse = Field(...)
-    __properties = ["id", "name", "created_at", "updated_at", "created_by", "type", "params", "credentials"]
-
-    @validator("type")
-    def type_validate_enum(cls, value):
-        """Validates the enum"""
-        if value not in ("S3"):
-            raise ValueError("must be one of enum values ('S3')")
+    type: Optional[Any] = Field(...)
+    connection_string: constr(strict=True) = Field(...)
+    __properties = ["type", "connection_string"]
+
+    @validator("connection_string")
+    def connection_string_validate_regular_expression(cls, value):
+        """Validates the regular expression"""
+        if not re.match(r"^mssql:\/\/", value):
+            raise ValueError(r"must validate the regular expression /^mssql:\/\//")
         return value
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
@@ -59,46 +50,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SourceGetS3:
-        """Create an instance of SourceGetS3 from a JSON string"""
+    def from_json(cls, json_str: str) -> ToolConfigSQLDatabaseMSSQL:
+        """Create an instance of ToolConfigSQLDatabaseMSSQL from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of params
-        if self.params:
-            _dict["params"] = self.params.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of credentials
-        if self.credentials:
-            _dict["credentials"] = self.credentials.to_dict()
+        # set to None if type (nullable) is None
+        # and __fields_set__ contains the field
+        if self.type is None and "type" in self.__fields_set__:
+            _dict["type"] = None
+
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SourceGetS3:
-        """Create an instance of SourceGetS3 from a dict"""
+    def from_dict(cls, obj: dict) -> ToolConfigSQLDatabaseMSSQL:
+        """Create an instance of ToolConfigSQLDatabaseMSSQL from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return SourceGetS3.parse_obj(obj)
+            return ToolConfigSQLDatabaseMSSQL.parse_obj(obj)
 
-        _obj = SourceGetS3.parse_obj(
-            {
-                "id": obj.get("id"),
-                "name": obj.get("name"),
-                "created_at": obj.get("created_at"),
-                "updated_at": obj.get("updated_at"),
-                "created_by": obj.get("created_by"),
-                "type": obj.get("type"),
-                "params": SourceS3Params.from_dict(obj.get("params")) if obj.get("params") is not None else None,
-                "credentials": AWSCredentialsResponse.from_dict(obj.get("credentials"))
-                if obj.get("credentials") is not None
-                else None,
-            }
+        _obj = ToolConfigSQLDatabaseMSSQL.parse_obj(
+            {"type": obj.get("type"), "connection_string": obj.get("connection_string")}
         )
         return _obj
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/source_response.py` & `superwise_api-1.3.0/superwise_api/client/models/source_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/source_s3_params.py` & `superwise_api-1.3.0/superwise_api/client/models/source_s3_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/source_type.py` & `superwise_api-1.3.0/superwise_api/client/models/datasource.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import json
 import pprint
 import re  # noqa: F401
 
 from aenum import Enum
 from aenum import no_arg
 
 
-class SourceType(str, Enum):
+class Datasource(str, Enum):
     """
     An enumeration.
     """
 
     """
     allowed enum values
     """
-    GCS = "GCS"
-    S3 = "S3"
-    AZURE_BLOB_STORAGE = "AZURE_BLOB_STORAGE"
+    DATASETS = "datasets"
+    EVENTS = "events"
 
     @classmethod
-    def from_json(cls, json_str: str) -> SourceType:
-        """Create an instance of SourceType from a JSON string"""
-        return SourceType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> Datasource:
+        """Create an instance of Datasource from a JSON string"""
+        return Datasource(json.loads(json_str))
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/source_update.py` & `superwise_api-1.3.0/superwise_api/client/models/source_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/source_update_gcs.py` & `superwise_api-1.3.0/superwise_api/client/models/validation_result.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,41 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
 import pprint
 import re  # noqa: F401
+from typing import List
 from typing import Optional
 
 from pydantic import BaseModel
-from pydantic import StrictStr
-from pydantic import validator
+from pydantic import conlist
+from pydantic import StrictBool
 
-from superwise_api.client.models.gcp_credentials_request import GCPCredentialsRequest
-from superwise_api.client.models.source_gcs_params import SourceGCSParams
+from superwise_api.client.models.validation_error_detail import ValidationErrorDetail
 
 
-class SourceUpdateGCS(BaseModel):
+class ValidationResult(BaseModel):
     """
-    SourceUpdateGCS
+    ValidationResult
     """
 
-    name: Optional[StrictStr] = None
-    credentials: Optional[GCPCredentialsRequest] = None
-    params: Optional[SourceGCSParams] = None
-    type: Optional[StrictStr] = "GCS"
-    __properties = ["name", "credentials", "params", "type"]
-
-    @validator("type")
-    def type_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in ("GCS"):
-            raise ValueError("must be one of enum values ('GCS')")
-        return value
+    is_valid: Optional[StrictBool] = None
+    errors: Optional[conlist(ValidationErrorDetail)] = None
+    __properties = ["is_valid", "errors"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -56,42 +44,41 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SourceUpdateGCS:
-        """Create an instance of SourceUpdateGCS from a JSON string"""
+    def from_json(cls, json_str: str) -> ValidationResult:
+        """Create an instance of ValidationResult from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of credentials
-        if self.credentials:
-            _dict["credentials"] = self.credentials.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of params
-        if self.params:
-            _dict["params"] = self.params.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in errors (list)
+        _items = []
+        if self.errors:
+            for _item in self.errors:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict["errors"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SourceUpdateGCS:
-        """Create an instance of SourceUpdateGCS from a dict"""
+    def from_dict(cls, obj: dict) -> ValidationResult:
+        """Create an instance of ValidationResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return SourceUpdateGCS.parse_obj(obj)
+            return ValidationResult.parse_obj(obj)
 
-        _obj = SourceUpdateGCS.parse_obj(
+        _obj = ValidationResult.parse_obj(
             {
-                "name": obj.get("name"),
-                "credentials": GCPCredentialsRequest.from_dict(obj.get("credentials"))
-                if obj.get("credentials") is not None
+                "is_valid": obj.get("is_valid"),
+                "errors": [ValidationErrorDetail.from_dict(_item) for _item in obj.get("errors")]
+                if obj.get("errors") is not None
                 else None,
-                "params": SourceGCSParams.from_dict(obj.get("params")) if obj.get("params") is not None else None,
-                "type": obj.get("type") if obj.get("type") is not None else "GCS",
             }
         )
         return _obj
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/source_update_s3.py` & `superwise_api-1.3.0/superwise_api/client/models/dashboard_item_update.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,47 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
 import pprint
 import re  # noqa: F401
+from typing import Any
 from typing import Optional
 
 from pydantic import BaseModel
-from pydantic import StrictStr
-from pydantic import validator
+from pydantic import constr
 
-from superwise_api.client.models.aws_credentials_request import AWSCredentialsRequest
-from superwise_api.client.models.source_s3_params import SourceS3Params
+from superwise_api.client.models.dashboard_item_query import DashboardItemQuery
+from superwise_api.client.models.datasource import Datasource
+from superwise_api.client.models.query_type import QueryType
+from superwise_api.client.models.visualization_type import VisualizationType
 
 
-class SourceUpdateS3(BaseModel):
+class DashboardItemUpdate(BaseModel):
     """
-    SourceUpdateS3
+    DashboardItemUpdate
     """
 
-    name: Optional[StrictStr] = None
-    credentials: Optional[AWSCredentialsRequest] = None
-    params: Optional[SourceS3Params] = None
-    type: Optional[StrictStr] = "S3"
-    __properties = ["name", "credentials", "params", "type"]
-
-    @validator("type")
-    def type_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in ("S3"):
-            raise ValueError("must be one of enum values ('S3')")
-        return value
+    name: Optional[constr(strict=True, max_length=50, min_length=1)] = None
+    query_type: Optional[QueryType] = None
+    datasource: Optional[Datasource] = None
+    query: Optional[DashboardItemQuery] = None
+    item_metadata: Optional[Any] = None
+    visualization_type: Optional[VisualizationType] = None
+    __properties = ["name", "query_type", "datasource", "query", "item_metadata", "visualization_type"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -56,42 +50,38 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SourceUpdateS3:
-        """Create an instance of SourceUpdateS3 from a JSON string"""
+    def from_json(cls, json_str: str) -> DashboardItemUpdate:
+        """Create an instance of DashboardItemUpdate from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of credentials
-        if self.credentials:
-            _dict["credentials"] = self.credentials.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of params
-        if self.params:
-            _dict["params"] = self.params.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of query
+        if self.query:
+            _dict["query"] = self.query.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SourceUpdateS3:
-        """Create an instance of SourceUpdateS3 from a dict"""
+    def from_dict(cls, obj: dict) -> DashboardItemUpdate:
+        """Create an instance of DashboardItemUpdate from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return SourceUpdateS3.parse_obj(obj)
+            return DashboardItemUpdate.parse_obj(obj)
 
-        _obj = SourceUpdateS3.parse_obj(
+        _obj = DashboardItemUpdate.parse_obj(
             {
                 "name": obj.get("name"),
-                "credentials": AWSCredentialsRequest.from_dict(obj.get("credentials"))
-                if obj.get("credentials") is not None
-                else None,
-                "params": SourceS3Params.from_dict(obj.get("params")) if obj.get("params") is not None else None,
-                "type": obj.get("type") if obj.get("type") is not None else "S3",
+                "query_type": obj.get("query_type"),
+                "datasource": obj.get("datasource"),
+                "query": DashboardItemQuery.from_dict(obj.get("query")) if obj.get("query") is not None else None,
+                "visualization_type": obj.get("visualization_type"),
             }
         )
         return _obj
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/time_dimension.py` & `superwise_api-1.3.0/superwise_api/client/models/time_dimension.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/time_range_unit.py` & `superwise_api-1.3.0/superwise_api/client/models/time_range_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import json
 import pprint
 import re  # noqa: F401
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/tool_config_big_query.py` & `superwise_api-1.3.0/superwise_api/client/models/tool_def_input.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
 import pprint
 import re  # noqa: F401
-from typing import Any
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import StrictStr
 
+from superwise_api.client.models.config import Config
+from superwise_api.client.models.description import Description
 
-class ToolConfigBigQuery(BaseModel):
+
+class ToolDefInput(BaseModel):
     """
-    ToolConfigBigQuery
+    ToolDefInput
     """
 
-    type: Optional[Any] = Field(...)
-    project_id: StrictStr = Field(...)
-    dataset_id: StrictStr = Field(...)
-    service_account: Any = Field(...)
-    __properties = ["type", "project_id", "dataset_id", "service_account"]
+    name: StrictStr = Field(...)
+    description: Optional[str] = None
+    config: Config = Field(...)
+    __properties = ["name", "description", "config"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -44,38 +45,38 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ToolConfigBigQuery:
-        """Create an instance of ToolConfigBigQuery from a JSON string"""
+    def from_json(cls, json_str: str) -> ToolDefInput:
+        """Create an instance of ToolDefInput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
-        # set to None if type (nullable) is None
-        # and __fields_set__ contains the field
-        if self.type is None and "type" in self.__fields_set__:
-            _dict["type"] = None
-
+        # override the default output from pydantic by calling `to_dict()` of config
+        if self.config:
+            _dict["config"] = self.config.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ToolConfigBigQuery:
-        """Create an instance of ToolConfigBigQuery from a dict"""
+    def from_dict(cls, obj: dict) -> ToolDefInput:
+        """Create an instance of ToolDefInput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ToolConfigBigQuery.parse_obj(obj)
+            return ToolDefInput.parse_obj(obj)
 
-        _obj = ToolConfigBigQuery.parse_obj(
+        _obj = ToolDefInput.parse_obj(
             {
-                "type": obj.get("type"),
-                "project_id": obj.get("project_id"),
-                "dataset_id": obj.get("dataset_id"),
+                "name": obj.get("name"),
+                "description": Description.from_dict(obj.get("description"))
+                if obj.get("description") is not None
+                else None,
+                "config": Config.from_dict(obj.get("config")) if obj.get("config") is not None else None,
             }
         )
         return _obj
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/tool_config_pg_vector.py` & `superwise_api-1.3.0/superwise_api/client/models/tool_config_pg_vector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/tool_config_sql_database_mssql.py` & `superwise_api-1.3.0/superwise_api/client/models/tool_config_sql_database_my_sql.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
@@ -19,28 +19,28 @@
 
 from pydantic import BaseModel
 from pydantic import constr
 from pydantic import Field
 from pydantic import validator
 
 
-class ToolConfigSQLDatabaseMSSQL(BaseModel):
+class ToolConfigSQLDatabaseMySQL(BaseModel):
     """
-    ToolConfigSQLDatabaseMSSQL
+    ToolConfigSQLDatabaseMySQL
     """
 
     type: Optional[Any] = Field(...)
     connection_string: constr(strict=True) = Field(...)
     __properties = ["type", "connection_string"]
 
     @validator("connection_string")
     def connection_string_validate_regular_expression(cls, value):
         """Validates the regular expression"""
-        if not re.match(r"^mssql:\/\/", value):
-            raise ValueError(r"must validate the regular expression /^mssql:\/\//")
+        if not re.match(r"^mysql:\/\/", value):
+            raise ValueError(r"must validate the regular expression /^mysql:\/\//")
         return value
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
@@ -50,34 +50,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ToolConfigSQLDatabaseMSSQL:
-        """Create an instance of ToolConfigSQLDatabaseMSSQL from a JSON string"""
+    def from_json(cls, json_str: str) -> ToolConfigSQLDatabaseMySQL:
+        """Create an instance of ToolConfigSQLDatabaseMySQL from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         # set to None if type (nullable) is None
         # and __fields_set__ contains the field
         if self.type is None and "type" in self.__fields_set__:
             _dict["type"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ToolConfigSQLDatabaseMSSQL:
-        """Create an instance of ToolConfigSQLDatabaseMSSQL from a dict"""
+    def from_dict(cls, obj: dict) -> ToolConfigSQLDatabaseMySQL:
+        """Create an instance of ToolConfigSQLDatabaseMySQL from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ToolConfigSQLDatabaseMSSQL.parse_obj(obj)
+            return ToolConfigSQLDatabaseMySQL.parse_obj(obj)
 
-        _obj = ToolConfigSQLDatabaseMSSQL.parse_obj(
+        _obj = ToolConfigSQLDatabaseMySQL.parse_obj(
             {"type": obj.get("type"), "connection_string": obj.get("connection_string")}
         )
         return _obj
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/tool_config_sql_database_my_sql.py` & `superwise_api-1.3.0/superwise_api/client/models/tool_config_sql_database_oracle.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
@@ -19,28 +19,28 @@
 
 from pydantic import BaseModel
 from pydantic import constr
 from pydantic import Field
 from pydantic import validator
 
 
-class ToolConfigSQLDatabaseMySQL(BaseModel):
+class ToolConfigSQLDatabaseOracle(BaseModel):
     """
-    ToolConfigSQLDatabaseMySQL
+    ToolConfigSQLDatabaseOracle
     """
 
     type: Optional[Any] = Field(...)
     connection_string: constr(strict=True) = Field(...)
     __properties = ["type", "connection_string"]
 
     @validator("connection_string")
     def connection_string_validate_regular_expression(cls, value):
         """Validates the regular expression"""
-        if not re.match(r"^mysql:\/\/", value):
-            raise ValueError(r"must validate the regular expression /^mysql:\/\//")
+        if not re.match(r"^oracle:\/\/", value):
+            raise ValueError(r"must validate the regular expression /^oracle:\/\//")
         return value
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
@@ -50,34 +50,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ToolConfigSQLDatabaseMySQL:
-        """Create an instance of ToolConfigSQLDatabaseMySQL from a JSON string"""
+    def from_json(cls, json_str: str) -> ToolConfigSQLDatabaseOracle:
+        """Create an instance of ToolConfigSQLDatabaseOracle from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         # set to None if type (nullable) is None
         # and __fields_set__ contains the field
         if self.type is None and "type" in self.__fields_set__:
             _dict["type"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ToolConfigSQLDatabaseMySQL:
-        """Create an instance of ToolConfigSQLDatabaseMySQL from a dict"""
+    def from_dict(cls, obj: dict) -> ToolConfigSQLDatabaseOracle:
+        """Create an instance of ToolConfigSQLDatabaseOracle from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ToolConfigSQLDatabaseMySQL.parse_obj(obj)
+            return ToolConfigSQLDatabaseOracle.parse_obj(obj)
 
-        _obj = ToolConfigSQLDatabaseMySQL.parse_obj(
+        _obj = ToolConfigSQLDatabaseOracle.parse_obj(
             {"type": obj.get("type"), "connection_string": obj.get("connection_string")}
         )
         return _obj
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/tool_config_sql_database_oracle.py` & `superwise_api-1.3.0/superwise_api/client/models/tool_config_sql_database_postgres.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
@@ -19,28 +19,28 @@
 
 from pydantic import BaseModel
 from pydantic import constr
 from pydantic import Field
 from pydantic import validator
 
 
-class ToolConfigSQLDatabaseOracle(BaseModel):
+class ToolConfigSQLDatabasePostgres(BaseModel):
     """
-    ToolConfigSQLDatabaseOracle
+    ToolConfigSQLDatabasePostgres
     """
 
     type: Optional[Any] = Field(...)
     connection_string: constr(strict=True) = Field(...)
     __properties = ["type", "connection_string"]
 
     @validator("connection_string")
     def connection_string_validate_regular_expression(cls, value):
         """Validates the regular expression"""
-        if not re.match(r"^oracle:\/\/", value):
-            raise ValueError(r"must validate the regular expression /^oracle:\/\//")
+        if not re.match(r"^postgresql:\/\/", value):
+            raise ValueError(r"must validate the regular expression /^postgresql:\/\//")
         return value
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
@@ -50,34 +50,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ToolConfigSQLDatabaseOracle:
-        """Create an instance of ToolConfigSQLDatabaseOracle from a JSON string"""
+    def from_json(cls, json_str: str) -> ToolConfigSQLDatabasePostgres:
+        """Create an instance of ToolConfigSQLDatabasePostgres from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         # set to None if type (nullable) is None
         # and __fields_set__ contains the field
         if self.type is None and "type" in self.__fields_set__:
             _dict["type"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ToolConfigSQLDatabaseOracle:
-        """Create an instance of ToolConfigSQLDatabaseOracle from a dict"""
+    def from_dict(cls, obj: dict) -> ToolConfigSQLDatabasePostgres:
+        """Create an instance of ToolConfigSQLDatabasePostgres from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ToolConfigSQLDatabaseOracle.parse_obj(obj)
+            return ToolConfigSQLDatabasePostgres.parse_obj(obj)
 
-        _obj = ToolConfigSQLDatabaseOracle.parse_obj(
+        _obj = ToolConfigSQLDatabasePostgres.parse_obj(
             {"type": obj.get("type"), "connection_string": obj.get("connection_string")}
         )
         return _obj
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/tool_config_sql_database_postgres.py` & `superwise_api-1.3.0/superwise_api/client/models/validation_error_detail.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,39 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
 import pprint
 import re  # noqa: F401
-from typing import Any
 from typing import Optional
 
 from pydantic import BaseModel
-from pydantic import constr
 from pydantic import Field
-from pydantic import validator
+from pydantic import StrictStr
 
 
-class ToolConfigSQLDatabasePostgres(BaseModel):
+class ValidationErrorDetail(BaseModel):
     """
-    ToolConfigSQLDatabasePostgres
+    ValidationErrorDetail
     """
 
-    type: Optional[Any] = Field(...)
-    connection_string: constr(strict=True) = Field(...)
-    __properties = ["type", "connection_string"]
-
-    @validator("connection_string")
-    def connection_string_validate_regular_expression(cls, value):
-        """Validates the regular expression"""
-        if not re.match(r"^postgresql:\/\/", value):
-            raise ValueError(r"must validate the regular expression /^postgresql:\/\//")
-        return value
+    type: StrictStr = Field(...)
+    detail: StrictStr = Field(...)
+    invalid_key: Optional[StrictStr] = None
+    __properties = ["type", "detail", "invalid_key"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -50,34 +42,29 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ToolConfigSQLDatabasePostgres:
-        """Create an instance of ToolConfigSQLDatabasePostgres from a JSON string"""
+    def from_json(cls, json_str: str) -> ValidationErrorDetail:
+        """Create an instance of ValidationErrorDetail from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
-        # set to None if type (nullable) is None
-        # and __fields_set__ contains the field
-        if self.type is None and "type" in self.__fields_set__:
-            _dict["type"] = None
-
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ToolConfigSQLDatabasePostgres:
-        """Create an instance of ToolConfigSQLDatabasePostgres from a dict"""
+    def from_dict(cls, obj: dict) -> ValidationErrorDetail:
+        """Create an instance of ValidationErrorDetail from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ToolConfigSQLDatabasePostgres.parse_obj(obj)
+            return ValidationErrorDetail.parse_obj(obj)
 
-        _obj = ToolConfigSQLDatabasePostgres.parse_obj(
-            {"type": obj.get("type"), "connection_string": obj.get("connection_string")}
+        _obj = ValidationErrorDetail.parse_obj(
+            {"type": obj.get("type"), "detail": obj.get("detail"), "invalid_key": obj.get("invalid_key")}
         )
         return _obj
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/tool_create.py` & `superwise_api-1.3.0/superwise_api/client/models/tool_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.4.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/tool_name.py` & `superwise_api-1.3.0/superwise_api/client/models/tool_name.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.4.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/tool_name_update.py` & `superwise_api-1.3.0/superwise_api/client/models/tool_name_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.4.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/tool_response.py` & `superwise_api-1.3.0/superwise_api/client/models/tool_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.4.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/tool_type.py` & `superwise_api-1.3.0/superwise_api/client/models/tool_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.4.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/tool_update.py` & `superwise_api-1.3.0/superwise_api/client/models/tool_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.4.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/total.py` & `superwise_api-1.3.0/superwise_api/client/models/created_at.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
 import pprint
 import re  # noqa: F401
+from datetime import datetime
 from inspect import getfullargspec
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import TYPE_CHECKING
 from typing import Union
 
 from pydantic import BaseModel
-from pydantic import conint
 from pydantic import Field
 from pydantic import StrictStr
 from pydantic import ValidationError
 from pydantic import validator
 
-TOTAL_ANY_OF_SCHEMAS = ["int", "object"]
+CREATEDAT_ANY_OF_SCHEMAS = ["datetime", "object"]
 
 
-class Total(BaseModel):
+class CreatedAt(BaseModel):
     """
-    Total
+    CreatedAt
     """
 
-    # data type: int
-    anyof_schema_1_validator: Optional[conint(strict=True, ge=0)] = None
+    # data type: datetime
+    anyof_schema_1_validator: Optional[datetime] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
-        actual_instance: Union[int, object]
+        actual_instance: Union[datetime, object]
     else:
         actual_instance: Any
-    any_of_schemas: List[str] = Field(TOTAL_ANY_OF_SCHEMAS, const=True)
+    any_of_schemas: List[str] = Field(CREATEDAT_ANY_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
     def __init__(self, *args, **kwargs) -> None:
         if args:
             if len(args) > 1:
@@ -57,47 +57,47 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @validator("actual_instance")
     def actual_instance_must_validate_anyof(cls, v):
-        instance = Total.construct()
+        instance = CreatedAt.construct()
         error_messages = []
-        # validate data type: int
+        # validate data type: datetime
         try:
             instance.anyof_schema_1_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         # validate data type: object
         try:
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
             raise ValueError(
-                "No match found when setting the actual_instance in Total with anyOf schemas: int, object. Details: "
+                "No match found when setting the actual_instance in CreatedAt with anyOf schemas: datetime, object. Details: "
                 + ", ".join(error_messages)
             )
         else:
             return v
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Total:
+    def from_dict(cls, obj: dict) -> CreatedAt:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
-    def from_json(cls, json_str: str) -> Total:
+    def from_json(cls, json_str: str) -> CreatedAt:
         """Returns the object represented by the json string"""
-        instance = Total.construct()
+        instance = CreatedAt.construct()
         error_messages = []
-        # deserialize data into int
+        # deserialize data into datetime
         try:
             # validation
             instance.anyof_schema_1_validator = json.loads(json_str)
             # assign value to actual_instance
             instance.actual_instance = instance.anyof_schema_1_validator
             return instance
         except (ValidationError, ValueError) as e:
@@ -111,15 +111,15 @@
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
             raise ValueError(
-                "No match found when deserializing the JSON string into Total with anyOf schemas: int, object. Details: "
+                "No match found when deserializing the JSON string into CreatedAt with anyOf schemas: datetime, object. Details: "
                 + ", ".join(error_messages)
             )
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/validation_error.py` & `superwise_api-1.3.0/superwise_api/client/models/validation_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/validation_error_detail.py` & `superwise_api-1.3.0/superwise_api/client/models/widget_meta.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
 import pprint
 import re  # noqa: F401
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Field
-from pydantic import StrictStr
+from pydantic import StrictInt
 
+from superwise_api.client.models.visualization_type import VisualizationType
 
-class ValidationErrorDetail(BaseModel):
+
+class WidgetMeta(BaseModel):
     """
-    ValidationErrorDetail
+    WidgetMeta
     """
 
-    type: StrictStr = Field(...)
-    detail: StrictStr = Field(...)
-    invalid_key: Optional[StrictStr] = None
-    __properties = ["type", "detail", "invalid_key"]
+    visualization_type: VisualizationType = Field(...)
+    x_pos: StrictInt = Field(...)
+    y_pos: StrictInt = Field(...)
+    height: Optional[StrictInt] = 0
+    width: Optional[StrictInt] = 0
+    __properties = ["visualization_type", "x_pos", "y_pos", "height", "width"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -42,29 +46,35 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ValidationErrorDetail:
-        """Create an instance of ValidationErrorDetail from a JSON string"""
+    def from_json(cls, json_str: str) -> WidgetMeta:
+        """Create an instance of WidgetMeta from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ValidationErrorDetail:
-        """Create an instance of ValidationErrorDetail from a dict"""
+    def from_dict(cls, obj: dict) -> WidgetMeta:
+        """Create an instance of WidgetMeta from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ValidationErrorDetail.parse_obj(obj)
+            return WidgetMeta.parse_obj(obj)
 
-        _obj = ValidationErrorDetail.parse_obj(
-            {"type": obj.get("type"), "detail": obj.get("detail"), "invalid_key": obj.get("invalid_key")}
+        _obj = WidgetMeta.parse_obj(
+            {
+                "visualization_type": obj.get("visualization_type"),
+                "x_pos": obj.get("x_pos"),
+                "y_pos": obj.get("y_pos"),
+                "height": obj.get("height") if obj.get("height") is not None else 0,
+                "width": obj.get("width") if obj.get("width") is not None else 0,
+            }
         )
         return _obj
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/validation_error_loc_inner.py` & `superwise_api-1.3.0/superwise_api/client/models/validation_error_loc_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/validation_result.py` & `superwise_api-1.3.0/superwise_api/client/models/model_llm.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
 import pprint
 import re  # noqa: F401
-from typing import List
-from typing import Optional
 
 from pydantic import BaseModel
-from pydantic import conlist
-from pydantic import StrictBool
+from pydantic import Field
+from pydantic import StrictStr
 
-from superwise_api.client.models.validation_error_detail import ValidationErrorDetail
+from superwise_api.client.models.model_provider import ModelProvider
+from superwise_api.client.models.model_version import ModelVersion
 
 
-class ValidationResult(BaseModel):
+class ModelLLM(BaseModel):
     """
-    ValidationResult
+    ModelLLM
     """
 
-    is_valid: Optional[StrictBool] = None
-    errors: Optional[conlist(ValidationErrorDetail)] = None
-    __properties = ["is_valid", "errors"]
+    provider: ModelProvider = Field(...)
+    version: str = Field(...)
+    api_token: StrictStr = Field(...)
+    __properties = ["provider", "version", "api_token"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -44,41 +44,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ValidationResult:
-        """Create an instance of ValidationResult from a JSON string"""
+    def from_json(cls, json_str: str) -> ModelLLM:
+        """Create an instance of ModelLLM from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in errors (list)
-        _items = []
-        if self.errors:
-            for _item in self.errors:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict["errors"] = _items
+
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ValidationResult:
-        """Create an instance of ValidationResult from a dict"""
+    def from_dict(cls, obj: dict) -> ModelLLM:
+        """Create an instance of ModelLLM from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ValidationResult.parse_obj(obj)
+            return ModelLLM.parse_obj(obj)
 
-        _obj = ValidationResult.parse_obj(
+        _obj = ModelLLM.parse_obj(
             {
-                "is_valid": obj.get("is_valid"),
-                "errors": [ValidationErrorDetail.from_dict(_item) for _item in obj.get("errors")]
-                if obj.get("errors") is not None
-                else None,
+                "provider": obj.get("provider"),
+                "version": ModelVersion.from_dict(obj.get("version")) if obj.get("version") is not None else None,
+                "api_token": obj.get("api_token"),
             }
         )
         return _obj
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/values.py` & `superwise_api-1.3.0/superwise_api/client/models/values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/version.py` & `superwise_api-1.3.0/superwise_api/client/models/dataset_id.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
@@ -23,31 +23,31 @@
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import StrictStr
 from pydantic import ValidationError
 from pydantic import validator
 
-VERSION_ANY_OF_SCHEMAS = ["object", "str"]
+DATASETID_ANY_OF_SCHEMAS = ["object", "str"]
 
 
-class Version(BaseModel):
+class DatasetId(BaseModel):
     """
-    Version
+    DatasetId
     """
 
     # data type: str
     anyof_schema_1_validator: Optional[StrictStr] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
         actual_instance: Union[object, str]
     else:
         actual_instance: Any
-    any_of_schemas: List[str] = Field(VERSION_ANY_OF_SCHEMAS, const=True)
+    any_of_schemas: List[str] = Field(DATASETID_ANY_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
     def __init__(self, *args, **kwargs) -> None:
         if args:
             if len(args) > 1:
@@ -56,15 +56,15 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @validator("actual_instance")
     def actual_instance_must_validate_anyof(cls, v):
-        instance = Version.construct()
+        instance = DatasetId.construct()
         error_messages = []
         # validate data type: str
         try:
             instance.anyof_schema_1_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
@@ -73,28 +73,28 @@
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
             raise ValueError(
-                "No match found when setting the actual_instance in Version with anyOf schemas: object, str. Details: "
+                "No match found when setting the actual_instance in DatasetId with anyOf schemas: object, str. Details: "
                 + ", ".join(error_messages)
             )
         else:
             return v
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Version:
+    def from_dict(cls, obj: dict) -> DatasetId:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
-    def from_json(cls, json_str: str) -> Version:
+    def from_json(cls, json_str: str) -> DatasetId:
         """Returns the object represented by the json string"""
-        instance = Version.construct()
+        instance = DatasetId.construct()
         error_messages = []
         # deserialize data into str
         try:
             # validation
             instance.anyof_schema_1_validator = json.loads(json_str)
             # assign value to actual_instance
             instance.actual_instance = instance.anyof_schema_1_validator
@@ -110,15 +110,15 @@
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
             raise ValueError(
-                "No match found when deserializing the JSON string into Version with anyOf schemas: object, str. Details: "
+                "No match found when deserializing the JSON string into DatasetId with anyOf schemas: object, str. Details: "
                 + ", ".join(error_messages)
             )
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/version1.py` & `superwise_api-1.3.0/superwise_api/client/models/version1.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/client/models/vertex_ai_model_garden_embedding_model.py` & `superwise_api-1.3.0/superwise_api/client/models/vertex_ai_model_garden_embedding_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/visualization_type.py` & `superwise_api-1.3.0/superwise_api/client/models/visualization_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import json
 import pprint
 import re  # noqa: F401
```

### Comparing `superwise_api-1.2.0/superwise_api/client/models/widget_meta.py` & `superwise_api-1.3.0/superwise_api/client/models/application_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
 import pprint
 import re  # noqa: F401
+from typing import List
+from typing import Optional
 
 from pydantic import BaseModel
+from pydantic import conlist
 from pydantic import Field
-from pydantic import StrictInt
 
-from superwise_api.client.models.visualization_type import VisualizationType
+from superwise_api.client.models.application_model import ApplicationModel
+from superwise_api.client.models.prompt import Prompt
+from superwise_api.client.models.tool_def_input import ToolDefInput
 
 
-class WidgetMeta(BaseModel):
+class ApplicationConfig(BaseModel):
     """
-    WidgetMeta
+    ApplicationConfig
     """
 
-    visualization_type: VisualizationType = Field(...)
-    x_pos: StrictInt = Field(...)
-    y_pos: StrictInt = Field(...)
-    __properties = ["visualization_type", "x_pos", "y_pos"]
+    model: Optional[ApplicationModel] = None
+    prompt: Optional[str] = None
+    tools: conlist(ToolDefInput) = Field(...)
+    __properties = ["model", "prompt", "tools"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -43,29 +47,48 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> WidgetMeta:
-        """Create an instance of WidgetMeta from a JSON string"""
+    def from_json(cls, json_str: str) -> ApplicationConfig:
+        """Create an instance of ApplicationConfig from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of model
+        if self.model:
+            _dict["model"] = self.model.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of prompt
+        if self.prompt:
+            _dict["prompt"] = self.prompt
+        # override the default output from pydantic by calling `to_dict()` of each item in tools (list)
+        _items = []
+        if self.tools:
+            for _item in self.tools:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict["tools"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> WidgetMeta:
-        """Create an instance of WidgetMeta from a dict"""
+    def from_dict(cls, obj: dict) -> ApplicationConfig:
+        """Create an instance of ApplicationConfig from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return WidgetMeta.parse_obj(obj)
+            return ApplicationConfig.parse_obj(obj)
 
-        _obj = WidgetMeta.parse_obj(
-            {"visualization_type": obj.get("visualization_type"), "x_pos": obj.get("x_pos"), "y_pos": obj.get("y_pos")}
+        _obj = ApplicationConfig.parse_obj(
+            {
+                "model": ApplicationModel.from_dict(obj.get("model")) if obj.get("model") is not None else None,
+                "prompt": Prompt.from_dict(obj.get("prompt")) if obj.get("prompt") is not None else None,
+                "tools": [ToolDefInput.from_dict(_item) for _item in obj.get("tools")]
+                if obj.get("tools") is not None
+                else None,
+            }
         )
         return _obj
```

### Comparing `superwise_api-1.2.0/superwise_api/client/rest.py` & `superwise_api-1.3.0/superwise_api/client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Superwise Main Entities
 
     API reference
 
-    The version of the OpenAPI document: 1.5.0
+    The version of the OpenAPI document: 1.6.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 import io
 import json
 import logging
```

### Comparing `superwise_api-1.2.0/superwise_api/config.py` & `superwise_api-1.3.0/superwise_api/config.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/entities/application.py` & `superwise_api-1.3.0/superwise_api/entities/application.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 from superwise_api.client import ApplicationsApi
-from superwise_api.client import AskRequestPayload
 from superwise_api.errors import raise_exception
-from superwise_api.models import ApplicationCreate
-from superwise_api.models import ApplicationUpdate
+from superwise_api.models.application.schemas import ApplicationConfigPayload
+from superwise_api.models.application.schemas import AskRequestPayload
+from superwise_api.models.application.schemas import ModelLLM
 
 
 class Application:
     """
     Method | HTTP request | Description
     ------------- | ------------- | -------------
     **ask** | **POST** /v1/applications/ask | Ask
     **create_application** | **POST** /v1/applications | Create Application
     """
 
     def __init__(self, client):
         self.api = ApplicationsApi(client)
 
     @raise_exception
-    def create(self, application_create: ApplicationCreate, **kwargs):
+    def create(self, application_config_payload: ApplicationConfigPayload, **kwargs):
         """
         Create a new application.
 
-        Parameters:
-
-        - **payload**: Instance of ApplicationCreate model.
-            - **name**: Name of the application.
-            - **model_id**: UUID of the model.
-            - **prompt**: Prompt for the application.
         """
-        return self.api.create_application(application_create, **kwargs)
+        return self.api.create_application(application_config_payload, **kwargs)
 
     @raise_exception
-    def ask(self, application_id: str, ask_request_payload: AskRequestPayload, **kwargs):
+    def ask(self, ask_request_payload: AskRequestPayload, **kwargs):
         """
         Ask the application a question.
 
         Parameters:
 
         - **payload**: Instance of AskRequestPayload model.
             - **input**: Input to the application.
@@ -43,26 +37,21 @@
                 - **name**: Name of the application.
                 - **model_id**: UUID of the model.
                 - **prompt**: Prompt for the application.
             - **chat_history**: Chat history for the application is a List[ChatHistoryEntry].
                 - **role**: Role of the chat history entry. (HUMAN or AI)
                 - **message**: Message of the chat history entry.
         """
-        return self.api.ask(application_id, ask_request_payload, **kwargs)
+        return self.api.ask_application(ask_request_payload, **kwargs)
 
     @raise_exception
     def get_applications(self, **query_params):
         """
-        Get all applications. Filter if provided with name, created_by, model_id, or prompt.
+        Get all applications. Filter if provided with name, created_by, or prompt.
 
-        Parameters:
-        - **name**: Name of the application. (optional)
-        - **created_by**: User ID of the user who created the application. (optional)
-        - **model_id**: UUID of the model. (optional)
-        - **prompt**: Prompt for the application. (optional)
         """
         return self.api.get_applications(**query_params)
 
     @raise_exception
     def get_application_by_id(self, application_id: str, **kwargs):
         """
         Get an application by its id.
@@ -70,31 +59,31 @@
         Parameters:
 
         - **application_id**: UUID of the application.
         """
         return self.api.get_application_by_id(application_id, **kwargs)
 
     @raise_exception
-    def update(self, application_id: str, application_update: ApplicationUpdate, **kwargs):
+    def put(self, application_id: str, application_config_payload: ApplicationConfigPayload, **kwargs):
         """
         Update an application.
 
-        Parameters:
-
-        - **application_id**: UUID of the application.
-        - **payload**: Instance of ApplicationUpdate model.
-            - **name**: Name of the application. (optional)
-            - **model_id**: UUID of the model. (optional)
-            - **prompt**: Prompt for the application. (optional)
         """
-        return self.api.update_application(application_id, application_update, **kwargs)
+        return self.api.put_application(application_id, application_config_payload, **kwargs)
 
     @raise_exception
     def delete(self, application_id: str, **kwargs):
         """
         Delete an application.
 
         Parameters:
 
         - **application_id**: UUID of the application.
         """
         return self.api.delete_application(application_id, **kwargs)
+
+    @raise_exception
+    def test_model_connection(self, model: ModelLLM, **kwargs):
+        """
+        Test the connection to the model.
+        """
+        return self.api.test_model_connection(model, **kwargs)
```

### Comparing `superwise_api-1.2.0/superwise_api/entities/dashboard.py` & `superwise_api-1.3.0/superwise_api/entities/dashboard.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/entities/dashboard_item.py` & `superwise_api-1.3.0/superwise_api/entities/dashboard_item.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/entities/dataset.py` & `superwise_api-1.3.0/superwise_api/entities/dataset.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/entities/dataset_source.py` & `superwise_api-1.3.0/superwise_api/entities/dataset_source.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/entities/destination.py` & `superwise_api-1.3.0/superwise_api/entities/destination.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/entities/integration.py` & `superwise_api-1.3.0/superwise_api/entities/integration.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/entities/policy.py` & `superwise_api-1.3.0/superwise_api/entities/policy.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/entities/source.py` & `superwise_api-1.3.0/superwise_api/entities/source.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/errors.py` & `superwise_api-1.3.0/superwise_api/errors.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/models/__init__.py` & `superwise_api-1.3.0/superwise_api/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-from superwise_api.client import ToolConfigBigQuery
-from superwise_api.client import ToolConfigSQLDatabaseMSSQL
-from superwise_api.client import ToolConfigSQLDatabaseMySQL
-from superwise_api.client import ToolConfigSQLDatabaseOracle
-from superwise_api.client import ToolConfigSQLDatabasePostgres
 from superwise_api.client.models import AlertOnStatusDirection
 from superwise_api.client.models import AWSCredentialsRequest
 from superwise_api.client.models import AWSCredentialsResponse
 from superwise_api.client.models import AzureCredentialsRequest
 from superwise_api.client.models import AzureCredentialsResponse
 from superwise_api.client.models import DashboardCreate
 from superwise_api.client.models import DashboardUpdate
@@ -53,59 +48,39 @@
 from superwise_api.client.models import SourceType
 from superwise_api.client.models import SourceUpdateGCS
 from superwise_api.client.models import SourceUpdateS3
 from superwise_api.client.models import TimeRangeUnit
 from superwise_api.client.models import ValidationError
 from superwise_api.client.models import ValidationErrorLocInner
 from superwise_api.client.models import VisualizationType
-from superwise_api.client.models.application_response import ApplicationResponse
-from superwise_api.client.models.application_type import ApplicationType
-from superwise_api.client.models.ask_config import AskConfig
-from superwise_api.client.models.ask_request_payload import AskRequestPayload
-from superwise_api.client.models.ask_response_payload import AskResponsePayload
 from superwise_api.client.models.description import Description
-from superwise_api.client.models.model_provider import ModelProvider
-from superwise_api.client.models.model_response import ModelResponse
-from superwise_api.client.models.model_version import ModelVersion
-from superwise_api.client.models.model_version_response import ModelVersionResponse
-from superwise_api.client.models.open_ai_model_version import OpenAIModelVersion
 from superwise_api.client.models.order import Order
-from superwise_api.client.models.page_application_response import PageApplicationResponse
-from superwise_api.client.models.page_model_response import PageModelResponse
 from superwise_api.client.models.prompt import Prompt
-from superwise_api.client.models.provider import Provider
 from superwise_api.client.models.source_update import SourceUpdate
-from superwise_api.client.models.tool_name import ToolName
-from superwise_api.client.models.tool_name_update import ToolNameUpdate
-from superwise_api.client.models.tool_type import ToolType
 from superwise_api.client.models.type import Type as FieldType
-from superwise_api.models.application.application import ApplicationCreate
-from superwise_api.models.application.application_update import ApplicationUpdate
+from superwise_api.models.application.enums import *
+from superwise_api.models.application.schemas import *
 from superwise_api.models.dashboard.dashboard_response import Dashboard
 from superwise_api.models.dashboard.page_dashboard import PageDashboard
 from superwise_api.models.dashboard_item.dashboard_item import DashboardItem
 from superwise_api.models.dashboard_item.dashboard_item_create import DashboardItemCreate
 from superwise_api.models.dashboard_item.dashboard_item_response import DashboardItemResponse
 from superwise_api.models.dashboard_item.page_dashboard_item import PageDashboardItem
 from superwise_api.models.dashboard_item.query import Query as DashboardItemQuery
 from superwise_api.models.dashboard_item.query_filter import QueryFilter as DashboardItemQueryFilter
 from superwise_api.models.dataset.dataset_response import DatasetResponse
 from superwise_api.models.dataset.dataset_schema import DatasetSchema
 from superwise_api.models.dataset.dataset_update import DatasetUpdate
 from superwise_api.models.dataset.page_dataset_response import PageDatasetResponse
-from superwise_api.models.model.model_create import ModelCreate
 from superwise_api.models.policy.page_policy_response import PagePolicyResponse
 from superwise_api.models.policy.policy_response import PolicyResponse
 from superwise_api.models.policy.query import Query as PolicyQuery
 from superwise_api.models.policy.query_filter import QueryFilter
-from superwise_api.models.tool.embeding_model import EmbeddingModel
-from superwise_api.models.tool.page_tool_response import PageToolResponse
-from superwise_api.models.tool.tool_config_pg_vector import ToolConfigPGVector
-from superwise_api.models.tool.tool_create import ToolCreate
-from superwise_api.models.tool.tool_response import ToolResponse
+from superwise_api.models.tool.enums import *
+from superwise_api.models.tool.schemas import *
 
 __all__ = [
     "DatasetCreate",
     "ValidationError",
     "DatasetSchema",
     "AlertOnStatusDirection",
     "DatasetResponse",
@@ -173,39 +148,28 @@
     "PageDashboard",
     "DashboardUpdate",
     "DashboardItemCreate",
     "QueryType",
     "VisualizationType",
     "Datasource",
     "DashboardItem",
-    "ModelCreate",
-    "ApplicationCreate",
-    "ApplicationResponse",
-    "ModelResponse",
     "Prompt",
-    "ApplicationType",
-    "ApplicationUpdate",
-    "AskConfig",
     "AskRequestPayload",
     "AskResponsePayload",
     "ModelProvider",
-    "ModelVersion",
-    "ModelVersionResponse",
     "OpenAIModelVersion",
-    "PageApplicationResponse",
-    "PageModelResponse",
-    "PageToolResponse",
-    "Provider",
-    "ToolCreate",
-    "ToolName",
-    "ToolNameUpdate",
-    "ToolResponse",
-    "ToolType",
+    "GoogleModelVersion",
+    "VertexAIModelGardenVersion",
+    "Role",
     "EmbeddingModel",
-    "ToolConfigPGVector",
-    "ToolConfigBigQuery",
-    "ToolConfigSQLDatabasePostgres",
-    "ToolConfigSQLDatabaseMSSQL",
-    "ToolConfigSQLDatabaseOracle",
-    "ToolConfigSQLDatabaseMySQL",
     "Description",
+    "ToolType",
+    "EmbeddingModelProvider",
+    "OpenAIEmbeddingModelVersion",
+    "GoogleAIEmbeddingModelVersion",
+    "ChatHistoryEntry",
+    "ApplicationConfigPayload",
+    "ApplicationConfig",
+    "Application",
+    "PageApplication",
+    "ModelLLM",
 ]
```

### Comparing `superwise_api-1.2.0/superwise_api/models/dashboard/dashboard_response.py` & `superwise_api-1.3.0/superwise_api/models/dashboard/dashboard_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/models/dashboard/page_dashboard.py` & `superwise_api-1.3.0/superwise_api/models/dashboard/page_dashboard.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/models/dashboard_item/dashboard_item.py` & `superwise_api-1.3.0/superwise_api/models/dashboard_item/dashboard_item.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/models/dashboard_item/dashboard_item_create.py` & `superwise_api-1.3.0/superwise_api/models/dashboard_item/dashboard_item_create.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/models/dashboard_item/dashboard_item_response.py` & `superwise_api-1.3.0/superwise_api/models/dashboard_item/dashboard_item_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/models/dashboard_item/page_dashboard_item.py` & `superwise_api-1.3.0/superwise_api/models/dashboard_item/page_dashboard_item.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/models/dashboard_item/query.py` & `superwise_api-1.3.0/superwise_api/models/dashboard_item/query.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/models/dashboard_item/query_filter.py` & `superwise_api-1.3.0/superwise_api/models/dashboard_item/query_filter.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/models/dataset/__init__.py` & `superwise_api-1.3.0/superwise_api/models/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/models/dataset/dataset_response.py` & `superwise_api-1.3.0/superwise_api/models/dataset/dataset_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/models/dataset/dataset_schema.py` & `superwise_api-1.3.0/superwise_api/models/dataset/dataset_schema.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/models/dataset/page_dataset_response.py` & `superwise_api-1.3.0/superwise_api/models/dataset/page_dataset_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/models/policy/__init__.py` & `superwise_api-1.3.0/superwise_api/models/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/models/policy/page_policy_response.py` & `superwise_api-1.3.0/superwise_api/models/policy/page_policy_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/models/policy/policy_response.py` & `superwise_api-1.3.0/superwise_api/models/policy/policy_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/models/policy/query.py` & `superwise_api-1.3.0/superwise_api/models/policy/query.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/models/policy/query_filter.py` & `superwise_api-1.3.0/superwise_api/models/policy/query_filter.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.2.0/superwise_api/superwise_client.py` & `superwise_api-1.3.0/superwise_api/superwise_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,18 +9,16 @@
 from superwise_api.entities.application import Application
 from superwise_api.entities.dashboard import Dashboard
 from superwise_api.entities.dashboard_item import DashboardItem
 from superwise_api.entities.dataset import Dataset
 from superwise_api.entities.dataset_source import DatasetSource
 from superwise_api.entities.destination import Destination
 from superwise_api.entities.integration import Integration
-from superwise_api.entities.model import Model
 from superwise_api.entities.policy import Policy
 from superwise_api.entities.source import Source
-from superwise_api.entities.tool import Tool
 
 
 class SuperwiseClient(ApiClient):
     def __init__(
         self,
         client_id: Optional[str] = None,
         client_secret: Optional[str] = None,
@@ -39,29 +37,14 @@
         self.configuration.access_token = self._fetch_token(
             auth_url=self.settings.auth_url,
             client_id=self.settings.client_id,
             client_secret=self.settings.client_secret,
         )
 
     @property
-    def tool(self):
-        """
-        *ToolsApi* | [**create_tool**](client/docs/ToolsApi.md#create_tool) | **POST** /v1/applications/{application_id}/tools | Create Tool
-
-        *ToolsApi* | [**delete_tool**](client/docs/ToolsApi.md#delete_tool) | **DELETE** /v1/applications/{application_id}/tools/{tool_id} | Delete Tool
-
-        *ToolsApi* | [**get_tool**](client/docs/ToolsApi.md#get_tool) | **GET** /v1/applications/{application_id}/tools/{tool_id} | Get Tool
-
-        *ToolsApi* | [**get_tools**](client/docs/ToolsApi.md#get_tools) | **GET** /v1/applications/{application_id}/tools | Get Tools
-
-        *ToolsApi* | [**update_tool**](client/docs/ToolsApi.md#update_tool) | **PATCH** /v1/applications/{application_id}/tools/{tool_id} | Update Tool
-        """
-        return Tool(self)
-
-    @property
     def dataset(self):
         """
         **Dataset** | [**create**](../docs/dataset/schemas/DatasetApi.md#create_dataset) | **POST** /v1/datasets | Create Dataset
 
         **Dataset** | [**delete**](../docs/dataset/schemas/DatasetApi.md#delete_dataset) | **DELETE** /v1/datasets/{dataset_id} | Delete Dataset
 
         **Dataset** | [**get_by_id**](../docs/dataset/schemas/DatasetApi.md#get_dataset) | **GET** /v1/datasets/{dataset_id} | Get Dataset
@@ -178,21 +161,14 @@
         """
         *ApplicationsApi* | [**ask**](../docs/application/schemas/ApplicationsApi.md#ask) | **POST** /v1/applications/ask | Ask
 
         *ApplicationsApi* | [**create_application**](../docs/application/schemas/ApplicationsApi.md#create_application) | **POST** /v1/applications | Create Application
         """
         return Application(self)
 
-    @property
-    def model(self):
-        """
-        *ModelsApi* | [**create_model**](../docs/model/schemas/ModelsApi.md#create_model) | **POST** /v1/models | Create Model
-        """
-        return Model(self)
-
     @staticmethod
     def _fetch_token(auth_url: str, client_id: str, client_secret: str) -> str:
         response = requests.post(
             auth_url,
             json={
                 "clientId": client_id,
                 "secret": client_secret,
```

### Comparing `superwise_api-1.2.0/PKG-INFO` & `superwise_api-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superwise-api
-Version: 1.2.0
+Version: 1.3.0
 Summary: Superwise SDK for Python
 License: MIT
 Keywords: OpenAPI,SuperwiseSDK
 Author: Superwise
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


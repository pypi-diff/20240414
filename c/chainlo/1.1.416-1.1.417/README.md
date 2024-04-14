# Comparing `tmp/chainlo-1.1.416.tar.gz` & `tmp/chainlo-1.1.417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlo-1.1.416.tar", max compression
+gzip compressed data, was "chainlo-1.1.417.tar", max compression
```

## Comparing `chainlo-1.1.416.tar` & `chainlo-1.1.417.tar`

### file list

```diff
@@ -1,187 +1,187 @@
--rw-r--r--   0        0        0        0 2024-03-28 12:59:00.277858 chainlo-1.1.416/README.md
--rw-r--r--   0        0        0     9640 2024-04-02 18:01:22.602103 chainlo-1.1.416/chainlo/__init__.py
--rw-r--r--   0        0        0       85 2024-04-02 18:00:53.775192 chainlo-1.1.416/chainlo/__main__.py
--rw-r--r--   0        0        0     1408 2024-04-02 20:00:55.227821 chainlo-1.1.416/chainlo/action.py
--rw-r--r--   0        0        0    26017 2024-03-29 15:38:21.217731 chainlo-1.1.416/chainlo/agenta_cli/README.md
--rw-r--r--   0        0        0      493 2024-03-29 15:38:21.221195 chainlo-1.1.416/chainlo/agenta_cli/agenta/__init__.py
--rw-r--r--   0        0        0      493 2024-04-02 20:00:55.228018 chainlo-1.1.416/chainlo/agenta_cli/agenta/cli/evaluation_commands.py
--rw-r--r--   0        0        0     6237 2024-04-02 20:00:55.228164 chainlo-1.1.416/chainlo/agenta_cli/agenta/cli/helper.py
--rw-r--r--   0        0        0     9530 2024-04-02 20:00:54.885868 chainlo-1.1.416/chainlo/agenta_cli/agenta/cli/main.py
--rw-r--r--   0        0        0     1336 2024-04-02 20:00:55.228042 chainlo-1.1.416/chainlo/agenta_cli/agenta/cli/telemetry.py
--rw-r--r--   0        0        0    16972 2024-04-02 20:00:55.228192 chainlo-1.1.416/chainlo/agenta_cli/agenta/cli/variant_commands.py
--rw-r--r--   0        0        0     1312 2024-04-02 20:00:55.228061 chainlo-1.1.416/chainlo/agenta_cli/agenta/cli/variant_configs.py
--rw-r--r--   0        0        0     2756 2024-03-29 15:38:21.228131 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/Readme.md
--rw-r--r--   0        0        0        0 2024-03-29 15:38:21.228597 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/__init__.py
--rw-r--r--   0        0        0     2505 2024-04-02 20:00:54.885886 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/api.py
--rw-r--r--   0        0        0      623 2024-03-29 15:38:21.229938 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/api_models.py
--rw-r--r--   0        0        0     2666 2024-03-29 15:38:21.231650 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/__init__.py
--rw-r--r--   0        0        0   259068 2024-03-29 15:38:21.233513 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/client.py
--rw-r--r--   0        0        0      519 2024-03-29 15:38:21.234601 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/core/__init__.py
--rw-r--r--   0        0        0      440 2024-03-29 15:38:21.235211 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/core/api_error.py
--rw-r--r--   0        0        0      972 2024-03-29 15:38:21.235881 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/core/client_wrapper.py
--rw-r--r--   0        0        0     1069 2024-03-29 15:38:21.236559 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/core/datetime_utils.py
--rw-r--r--   0        0        0     3825 2024-03-29 15:38:21.237211 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-03-29 15:38:21.237761 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      170 2024-03-29 15:38:21.239005 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-03-29 15:38:21.239732 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0     4008 2024-03-29 15:38:21.241610 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/__init__.py
--rw-r--r--   0        0        0      211 2024-03-29 15:38:21.242318 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/add_variant_from_base_and_config_response.py
--rw-r--r--   0        0        0     1083 2024-03-29 15:38:21.243231 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/aggregated_result.py
--rw-r--r--   0        0        0      974 2024-03-29 15:38:21.243870 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/app.py
--rw-r--r--   0        0        0     1268 2024-03-29 15:38:21.244420 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output.py
--rw-r--r--   0        0        0     1394 2024-03-29 15:38:21.245000 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output_extended.py
--rw-r--r--   0        0        0     1075 2024-03-29 15:38:21.245538 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/app_variant_revision.py
--rw-r--r--   0        0        0      983 2024-03-29 15:38:21.246051 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/base_output.py
--rw-r--r--   0        0        0     1061 2024-03-29 15:38:21.246493 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/body_import_testset.py
--rw-r--r--   0        0        0     1028 2024-03-29 15:38:21.246936 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/config_db.py
--rw-r--r--   0        0        0      182 2024-03-29 15:38:21.247467 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/container_templates_response.py
--rw-r--r--   0        0        0      986 2024-03-29 15:38:21.248085 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/create_app_output.py
--rw-r--r--   0        0        0      991 2024-03-29 15:38:21.248628 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/delete_evaluation.py
--rw-r--r--   0        0        0      986 2024-03-29 15:38:21.249104 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/docker_env_vars.py
--rw-r--r--   0        0        0     1176 2024-03-29 15:38:21.249534 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/environment_output.py
--rw-r--r--   0        0        0     1376 2024-03-29 15:38:21.249971 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/evaluation.py
--rw-r--r--   0        0        0     1497 2024-03-29 15:38:21.250499 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario.py
--rw-r--r--   0        0        0     1027 2024-03-29 15:38:21.251140 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_input.py
--rw-r--r--   0        0        0     1014 2024-03-29 15:38:21.251815 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_output.py
--rw-r--r--   0        0        0     1033 2024-03-29 15:38:21.252247 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_result.py
--rw-r--r--   0        0        0     1102 2024-03-29 15:38:21.252717 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/evaluation_status_enum.py
--rw-r--r--   0        0        0      644 2024-03-29 15:38:21.253129 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/evaluation_type.py
--rw-r--r--   0        0        0      971 2024-03-29 15:38:21.253545 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/evaluation_webhook.py
--rw-r--r--   0        0        0     1046 2024-03-29 15:38:21.254100 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/evaluator.py
--rw-r--r--   0        0        0     1124 2024-03-29 15:38:21.254598 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/evaluator_config.py
--rw-r--r--   0        0        0     1136 2024-03-29 15:38:21.255072 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/feedback.py
--rw-r--r--   0        0        0     1063 2024-03-29 15:38:21.255549 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/get_config_reponse.py
--rw-r--r--   0        0        0     1060 2024-03-29 15:38:21.256152 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/http_validation_error.py
--rw-r--r--   0        0        0     1305 2024-03-29 15:38:21.256706 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation.py
--rw-r--r--   0        0        0     1580 2024-03-29 15:38:21.257151 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario.py
--rw-r--r--   0        0        0     1006 2024-03-29 15:38:21.257665 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_input.py
--rw-r--r--   0        0        0     1010 2024-03-29 15:38:21.258161 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_output.py
--rw-r--r--   0        0        0      134 2024-03-29 15:38:21.258634 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_score.py
--rw-r--r--   0        0        0      140 2024-03-29 15:38:21.259047 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_update_score.py
--rw-r--r--   0        0        0     1048 2024-03-29 15:38:21.259555 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/image.py
--rw-r--r--   0        0        0      965 2024-03-29 15:38:21.260000 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/invite_request.py
--rw-r--r--   0        0        0     1095 2024-03-29 15:38:21.260474 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/list_api_keys_output.py
--rw-r--r--   0        0        0     1045 2024-03-29 15:38:21.260976 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/llm_run_rate_limit.py
--rw-r--r--   0        0        0     1009 2024-03-29 15:38:21.261472 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/new_testset.py
--rw-r--r--   0        0        0     1181 2024-03-29 15:38:21.261911 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/organization.py
--rw-r--r--   0        0        0      981 2024-03-29 15:38:21.262371 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/organization_output.py
--rw-r--r--   0        0        0      996 2024-03-29 15:38:21.262822 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/result.py
--rw-r--r--   0        0        0     1117 2024-03-29 15:38:21.263320 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/simple_evaluation_output.py
--rw-r--r--   0        0        0     1546 2024-03-29 15:38:21.263903 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/span.py
--rw-r--r--   0        0        0     1037 2024-03-29 15:38:21.264526 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/template.py
--rw-r--r--   0        0        0     1189 2024-03-29 15:38:21.265123 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/template_image_info.py
--rw-r--r--   0        0        0     1088 2024-03-29 15:38:21.265659 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/test_set_output_response.py
--rw-r--r--   0        0        0     1004 2024-03-29 15:38:21.266314 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/test_set_simple_response.py
--rw-r--r--   0        0        0     1353 2024-03-29 15:38:21.266828 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/trace.py
--rw-r--r--   0        0        0      953 2024-03-29 15:38:21.267207 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/uri.py
--rw-r--r--   0        0        0     1086 2024-03-29 15:38:21.267670 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-03-29 15:38:21.268112 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     1031 2024-03-29 15:38:21.268517 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/variant_action.py
--rw-r--r--   0        0        0      511 2024-03-29 15:38:21.268961 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/variant_action_enum.py
--rw-r--r--   0        0        0    19667 2024-04-02 20:00:54.885983 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/client.py
--rw-r--r--   0        0        0       94 2024-03-29 15:38:21.269971 chainlo-1.1.416/chainlo/agenta_cli/agenta/client/exceptions.py
--rw-r--r--   0        0        0      732 2024-03-29 15:38:21.270473 chainlo-1.1.416/chainlo/agenta_cli/agenta/config.py
--rw-r--r--   0        0        0      245 2024-04-04 15:17:30.727889 chainlo-1.1.416/chainlo/agenta_cli/agenta/config.toml
--rw-r--r--   0        0        0      317 2024-03-29 15:38:21.272321 chainlo-1.1.416/chainlo/agenta_cli/agenta/docker/docker-assets/Dockerfile.cloud.template
--rw-r--r--   0        0        0      291 2024-04-03 22:53:43.117295 chainlo-1.1.416/chainlo/agenta_cli/agenta/docker/docker-assets/Dockerfile.template
--rw-r--r--   0        0        0      102 2024-03-29 15:38:21.273161 chainlo-1.1.416/chainlo/agenta_cli/agenta/docker/docker-assets/README.md
--rwxr-xr-x   0        0        0       75 2024-04-02 21:38:18.446443 chainlo-1.1.416/chainlo/agenta_cli/agenta/docker/docker-assets/entrypoint.sh
--rw-r--r--   0        0        0      112 2024-04-02 20:23:24.001250 chainlo-1.1.416/chainlo/agenta_cli/agenta/docker/docker-assets/lambda_function.py
--rw-r--r--   0        0        0      280 2024-04-02 20:23:49.555521 chainlo-1.1.416/chainlo/agenta_cli/agenta/docker/docker-assets/main.py
--rw-r--r--   0        0        0     3561 2024-04-02 20:00:54.887775 chainlo-1.1.416/chainlo/agenta_cli/agenta/docker/docker_utils.py
--rw-r--r--   0        0        0      565 2024-03-29 15:38:21.275737 chainlo-1.1.416/chainlo/agenta_cli/agenta/sdk/__init__.py
--rw-r--r--   0        0        0    15514 2024-04-06 01:02:59.748843 chainlo-1.1.416/chainlo/agenta_cli/agenta/sdk/agenta_decorator.py
--rw-r--r--   0        0        0     8063 2024-04-02 20:00:55.228132 chainlo-1.1.416/chainlo/agenta_cli/agenta/sdk/agenta_init.py
--rw-r--r--   0        0        0      901 2024-03-29 15:38:21.277386 chainlo-1.1.416/chainlo/agenta_cli/agenta/sdk/context.py
--rw-r--r--   0        0        0      269 2024-03-29 15:38:21.277737 chainlo-1.1.416/chainlo/agenta_cli/agenta/sdk/router.py
--rw-r--r--   0        0        0     4658 2024-03-29 15:38:21.278086 chainlo-1.1.416/chainlo/agenta_cli/agenta/sdk/types.py
--rw-r--r--   0        0        0      389 2024-04-02 20:23:10.241942 chainlo-1.1.416/chainlo/agenta_cli/agenta/sdk/utils/globals.py
--rw-r--r--   0        0        0     5877 2024-03-29 15:38:21.279477 chainlo-1.1.416/chainlo/agenta_cli/agenta/sdk/utils/helper/openai_cost.py
--rw-r--r--   0        0        0     1278 2024-03-29 15:38:21.279853 chainlo-1.1.416/chainlo/agenta_cli/agenta/sdk/utils/preinit.py
--rw-r--r--   0        0        0      308 2024-03-29 15:38:21.281309 chainlo-1.1.416/chainlo/agenta_cli/agenta/templates/compose_email/README.md
--rw-r--r--   0        0        0     2384 2024-03-29 15:38:21.281686 chainlo-1.1.416/chainlo/agenta_cli/agenta/templates/compose_email/app.py
--rw-r--r--   0        0        0       70 2024-03-29 15:38:21.282049 chainlo-1.1.416/chainlo/agenta_cli/agenta/templates/compose_email/env.example
--rw-r--r--   0        0        0       23 2024-03-29 15:38:21.282449 chainlo-1.1.416/chainlo/agenta_cli/agenta/templates/compose_email/requirements.txt
--rw-r--r--   0        0        0       47 2024-03-29 15:38:21.282787 chainlo-1.1.416/chainlo/agenta_cli/agenta/templates/compose_email/template.toml
--rw-r--r--   0        0        0      308 2024-03-29 15:38:21.283477 chainlo-1.1.416/chainlo/agenta_cli/agenta/templates/extract_data_to_json/README.md
--rw-r--r--   0        0        0     1320 2024-03-29 15:38:21.283896 chainlo-1.1.416/chainlo/agenta_cli/agenta/templates/extract_data_to_json/app.py
--rw-r--r--   0        0        0       70 2024-03-29 15:38:21.284271 chainlo-1.1.416/chainlo/agenta_cli/agenta/templates/extract_data_to_json/env.example
--rw-r--r--   0        0        0       23 2024-03-29 15:38:21.284661 chainlo-1.1.416/chainlo/agenta_cli/agenta/templates/extract_data_to_json/requirements.txt
--rw-r--r--   0        0        0       60 2024-03-29 15:38:21.285035 chainlo-1.1.416/chainlo/agenta_cli/agenta/templates/extract_data_to_json/template.toml
--rw-r--r--   0        0        0      308 2024-03-29 15:38:21.285928 chainlo-1.1.416/chainlo/agenta_cli/agenta/templates/simple_prompt/README.md
--rw-r--r--   0        0        0     1258 2024-04-03 22:59:21.919707 chainlo-1.1.416/chainlo/agenta_cli/agenta/templates/simple_prompt/app.py
--rw-r--r--   0        0        0       70 2024-03-29 15:38:21.286665 chainlo-1.1.416/chainlo/agenta_cli/agenta/templates/simple_prompt/env.example
--rw-r--r--   0        0        0       24 2024-04-02 15:18:01.855024 chainlo-1.1.416/chainlo/agenta_cli/agenta/templates/simple_prompt/requirements.txt
--rw-r--r--   0        0        0       60 2024-03-29 15:38:21.287420 chainlo-1.1.416/chainlo/agenta_cli/agenta/templates/simple_prompt/template.toml
--rw-r--r--   0        0        0     1078 2024-04-01 00:20:31.300954 chainlo-1.1.416/chainlo/agenta_cli/pyproject.toml-ex
--rw-r--r--   0        0        0        0 2024-03-29 15:38:21.289373 chainlo-1.1.416/chainlo/agenta_cli/requirements.txt
--rw-r--r--   0        0        0      580 2024-03-29 15:38:21.290495 chainlo-1.1.416/chainlo/agenta_cli/tests/example_projects/simple_langchain/app.py
--rw-r--r--   0        0        0       31 2024-03-29 15:38:21.290969 chainlo-1.1.416/chainlo/agenta_cli/tests/example_projects/simple_langchain/requirements.txt
--rw-r--r--   0        0        0      411 2024-03-29 15:38:21.292434 chainlo-1.1.416/chainlo/agenta_cli/tests/example_projects/test2/README.md
--rw-r--r--   0        0        0     3294 2024-03-29 15:38:21.293249 chainlo-1.1.416/chainlo/agenta_cli/tests/example_projects/test2/agenta.py
--rw-r--r--   0        0        0      580 2024-03-29 15:38:21.294048 chainlo-1.1.416/chainlo/agenta_cli/tests/example_projects/test2/app.py
--rw-r--r--   0        0        0       51 2024-03-29 15:38:21.294746 chainlo-1.1.416/chainlo/agenta_cli/tests/example_projects/test2/config.toml
--rw-r--r--   0        0        0      187 2024-03-29 15:38:21.295361 chainlo-1.1.416/chainlo/agenta_cli/tests/example_projects/test2/main.py
--rw-r--r--   0        0        0       31 2024-03-29 15:38:21.295991 chainlo-1.1.416/chainlo/agenta_cli/tests/example_projects/test2/requirements.txt
--rw-r--r--   0        0        0     2677 2024-04-02 20:00:55.227808 chainlo-1.1.416/chainlo/auth.py
--rw-r--r--   0        0        0     1359 2024-04-02 20:00:55.227793 chainlo-1.1.416/chainlo/cache.py
--rw-r--r--   0        0        0      875 2024-04-02 20:00:55.227834 chainlo-1.1.416/chainlo/chat_settings.py
--rw-r--r--   0        0        0     4989 2024-04-07 00:03:06.911430 chainlo-1.1.416/chainlo/cli/__init__.py
--rw-r--r--   0        0        0      717 2024-03-28 12:59:00.279324 chainlo-1.1.416/chainlo/cli/utils.py
--rw-r--r--   0        0        0    13496 2024-04-06 23:44:16.214790 chainlo-1.1.416/chainlo/config.py
--rw-r--r--   0        0        0     2471 2024-04-02 20:00:55.227752 chainlo-1.1.416/chainlo/context.py
--rw-r--r--   0        0        0     8887 2024-04-02 13:46:34.758455 chainlo-1.1.416/chainlo/copilot/dist/assets/logo_dark-2a3cf740.svg
--rw-r--r--   0        0        0     8889 2024-04-02 13:46:34.756788 chainlo-1.1.416/chainlo/copilot/dist/assets/logo_light-b078e7bc.svg
--rw-r--r--   0        0        0  7013566 2024-04-02 13:46:34.752958 chainlo-1.1.416/chainlo/copilot/dist/index.js
--rw-r--r--   0        0        0    14716 2024-04-02 20:00:55.191849 chainlo-1.1.416/chainlo/data/__init__.py
--rw-r--r--   0        0        0      460 2024-04-02 20:00:54.932738 chainlo-1.1.416/chainlo/data/acl.py
--rw-r--r--   0        0        0    10157 2024-04-02 20:00:55.227734 chainlo-1.1.416/chainlo/element.py
--rw-r--r--   0        0        0    12170 2024-04-02 20:00:55.227715 chainlo-1.1.416/chainlo/emitter.py
--rw-r--r--   0        0        0  3071160 2024-04-02 13:46:34.734588 chainlo-1.1.416/chainlo/frontend/dist/assets/index-7bc2ef31.js
--rw-r--r--   0        0        0     6605 2024-04-02 13:46:34.736982 chainlo-1.1.416/chainlo/frontend/dist/assets/index-d088547c.css
--rw-r--r--   0        0        0     8887 2024-04-02 13:46:34.736163 chainlo-1.1.416/chainlo/frontend/dist/assets/logo_dark-2a3cf740.svg
--rw-r--r--   0        0        0     8889 2024-04-02 13:46:34.735648 chainlo-1.1.416/chainlo/frontend/dist/assets/logo_light-b078e7bc.svg
--rw-r--r--   0        0        0  3763471 2024-04-02 13:46:34.739499 chainlo-1.1.416/chainlo/frontend/dist/assets/react-plotly-70086d41.js
--rw-r--r--   0        0        0     6455 2024-04-02 13:46:34.741377 chainlo-1.1.416/chainlo/frontend/dist/favicon.svg
--rw-r--r--   0        0        0     1005 2024-04-02 13:46:34.731871 chainlo-1.1.416/chainlo/frontend/dist/index.html
--rw-r--r--   0        0        0      216 2024-04-02 20:00:55.228246 chainlo-1.1.416/chainlo/haystack/__init__.py
--rw-r--r--   0        0        0     5205 2024-04-02 20:00:55.191778 chainlo-1.1.416/chainlo/haystack/callbacks.py
--rw-r--r--   0        0        0     3015 2024-04-02 20:00:54.885954 chainlo-1.1.416/chainlo/hello.py
--rw-r--r--   0        0        0     4879 2024-04-02 20:00:54.885927 chainlo-1.1.416/chainlo/input_widget.py
--rw-r--r--   0        0        0      216 2024-04-02 20:00:55.171891 chainlo-1.1.416/chainlo/langchain/__init__.py
--rw-r--r--   0        0        0    20518 2024-04-02 20:00:55.171912 chainlo-1.1.416/chainlo/langchain/callbacks.py
--rw-r--r--   0        0        0      815 2024-04-02 20:00:55.171857 chainlo-1.1.416/chainlo/langflow/__init__.py
--rw-r--r--   0        0        0      226 2024-04-02 20:00:55.171832 chainlo-1.1.416/chainlo/llama_index/__init__.py
--rw-r--r--   0        0        0     6075 2024-04-02 20:00:55.134912 chainlo-1.1.416/chainlo/llama_index/callbacks.py
--rw-r--r--   0        0        0      373 2024-03-28 12:59:00.282615 chainlo-1.1.416/chainlo/logger.py
--rw-r--r--   0        0        0     2024 2024-04-02 20:00:55.227774 chainlo-1.1.416/chainlo/markdown.py
--rw-r--r--   0        0        0    17674 2024-04-02 20:00:55.227695 chainlo-1.1.416/chainlo/message.py
--rw-r--r--   0        0        0    17458 2024-04-02 20:00:55.227664 chainlo-1.1.416/chainlo/oauth_providers.py
--rw-r--r--   0        0        0     1998 2024-04-02 20:00:54.975014 chainlo-1.1.416/chainlo/openai/__init__.py
--rw-r--r--   0        0        0       80 2024-03-28 12:59:00.283801 chainlo-1.1.416/chainlo/playground/__init__.py
--rw-r--r--   0        0        0     1031 2024-04-02 20:00:54.974932 chainlo-1.1.416/chainlo/playground/config.py
--rw-r--r--   0        0        0     3854 2024-04-02 20:00:54.974863 chainlo-1.1.416/chainlo/playground/provider.py
--rw-r--r--   0        0        0      236 2024-03-28 12:59:00.284521 chainlo-1.1.416/chainlo/playground/providers/__init__.py
--rw-r--r--   0        0        0     3493 2024-04-02 20:00:54.974475 chainlo-1.1.416/chainlo/playground/providers/anthropic.py
--rw-r--r--   0        0        0     2127 2024-04-02 20:00:54.954439 chainlo-1.1.416/chainlo/playground/providers/huggingface.py
--rw-r--r--   0        0        0     3100 2024-04-02 20:00:54.932814 chainlo-1.1.416/chainlo/playground/providers/langchain.py
--rw-r--r--   0        0        0    12395 2024-04-02 20:00:54.952587 chainlo-1.1.416/chainlo/playground/providers/openai.py
--rw-r--r--   0        0        0     5081 2024-04-02 20:00:54.887826 chainlo-1.1.416/chainlo/playground/providers/vertexai.py
--rw-r--r--   0        0        0        0 2024-03-28 12:59:00.285429 chainlo-1.1.416/chainlo/py.typed
--rw-r--r--   0        0        0      295 2024-03-28 12:59:00.285564 chainlo-1.1.416/chainlo/secret.py
--rw-r--r--   0        0        0    22586 2024-04-07 01:16:42.223923 chainlo-1.1.416/chainlo/server.py
--rw-r--r--   0        0        0     8837 2024-04-02 20:00:55.227631 chainlo-1.1.416/chainlo/session.py
--rw-r--r--   0        0        0     9834 2024-04-02 20:00:55.228438 chainlo-1.1.416/chainlo/socket.py
--rw-r--r--   0        0        0    12742 2024-04-02 20:00:55.227568 chainlo-1.1.416/chainlo/step.py
--rw-r--r--   0        0        0     1234 2024-04-02 20:00:55.191939 chainlo-1.1.416/chainlo/sync.py
--rw-r--r--   0        0        0     3058 2024-04-02 20:00:55.191900 chainlo-1.1.416/chainlo/telemetry.py
--rw-r--r--   0        0        0     6252 2024-03-28 12:59:00.286806 chainlo-1.1.416/chainlo/translations/de.json
--rw-r--r--   0        0        0     4514 2024-03-28 12:59:00.287261 chainlo-1.1.416/chainlo/translations/en-US.json
--rw-r--r--   0        0        0     4614 2024-03-28 12:59:00.287519 chainlo-1.1.416/chainlo/translations/pt-BR.json
--rw-r--r--   0        0        0     3376 2024-04-02 20:00:55.191876 chainlo-1.1.416/chainlo/types.py
--rw-r--r--   0        0        0      619 2024-03-28 12:59:00.287957 chainlo-1.1.416/chainlo/user.py
--rw-r--r--   0        0        0     1367 2024-04-02 20:00:55.228294 chainlo-1.1.416/chainlo/user_session.py
--rw-r--r--   0        0        0     2568 2024-04-02 20:00:55.191815 chainlo-1.1.416/chainlo/utils.py
--rw-r--r--   0        0        0      196 2024-03-28 12:59:00.288410 chainlo-1.1.416/chainlo/version.py
--rw-r--r--   0        0        0     2371 2024-04-07 01:17:21.337245 chainlo-1.1.416/pyproject.toml
--rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 chainlo-1.1.416/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-28 12:59:00.277858 chainlo-1.1.417/README.md
+-rw-r--r--   0        0        0     9640 2024-04-02 18:01:22.602103 chainlo-1.1.417/chainlo/__init__.py
+-rw-r--r--   0        0        0       85 2024-04-02 18:00:53.775192 chainlo-1.1.417/chainlo/__main__.py
+-rw-r--r--   0        0        0     1408 2024-04-02 20:00:55.227821 chainlo-1.1.417/chainlo/action.py
+-rw-r--r--   0        0        0    26017 2024-03-29 15:38:21.217731 chainlo-1.1.417/chainlo/agenta_cli/README.md
+-rw-r--r--   0        0        0      493 2024-03-29 15:38:21.221195 chainlo-1.1.417/chainlo/agenta_cli/agenta/__init__.py
+-rw-r--r--   0        0        0      493 2024-04-02 20:00:55.228018 chainlo-1.1.417/chainlo/agenta_cli/agenta/cli/evaluation_commands.py
+-rw-r--r--   0        0        0     6237 2024-04-02 20:00:55.228164 chainlo-1.1.417/chainlo/agenta_cli/agenta/cli/helper.py
+-rw-r--r--   0        0        0     9530 2024-04-02 20:00:54.885868 chainlo-1.1.417/chainlo/agenta_cli/agenta/cli/main.py
+-rw-r--r--   0        0        0     1336 2024-04-02 20:00:55.228042 chainlo-1.1.417/chainlo/agenta_cli/agenta/cli/telemetry.py
+-rw-r--r--   0        0        0    16972 2024-04-02 20:00:55.228192 chainlo-1.1.417/chainlo/agenta_cli/agenta/cli/variant_commands.py
+-rw-r--r--   0        0        0     1312 2024-04-02 20:00:55.228061 chainlo-1.1.417/chainlo/agenta_cli/agenta/cli/variant_configs.py
+-rw-r--r--   0        0        0     2756 2024-03-29 15:38:21.228131 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/Readme.md
+-rw-r--r--   0        0        0        0 2024-03-29 15:38:21.228597 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/__init__.py
+-rw-r--r--   0        0        0     2505 2024-04-02 20:00:54.885886 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/api.py
+-rw-r--r--   0        0        0      623 2024-03-29 15:38:21.229938 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/api_models.py
+-rw-r--r--   0        0        0     2666 2024-03-29 15:38:21.231650 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/__init__.py
+-rw-r--r--   0        0        0   259068 2024-03-29 15:38:21.233513 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/client.py
+-rw-r--r--   0        0        0      519 2024-03-29 15:38:21.234601 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/core/__init__.py
+-rw-r--r--   0        0        0      440 2024-03-29 15:38:21.235211 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/core/api_error.py
+-rw-r--r--   0        0        0      972 2024-03-29 15:38:21.235881 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/core/client_wrapper.py
+-rw-r--r--   0        0        0     1069 2024-03-29 15:38:21.236559 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/core/datetime_utils.py
+-rw-r--r--   0        0        0     3825 2024-03-29 15:38:21.237211 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-03-29 15:38:21.237761 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      170 2024-03-29 15:38:21.239005 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-03-29 15:38:21.239732 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0     4008 2024-03-29 15:38:21.241610 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/__init__.py
+-rw-r--r--   0        0        0      211 2024-03-29 15:38:21.242318 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/add_variant_from_base_and_config_response.py
+-rw-r--r--   0        0        0     1083 2024-03-29 15:38:21.243231 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/aggregated_result.py
+-rw-r--r--   0        0        0      974 2024-03-29 15:38:21.243870 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/app.py
+-rw-r--r--   0        0        0     1268 2024-03-29 15:38:21.244420 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output.py
+-rw-r--r--   0        0        0     1394 2024-03-29 15:38:21.245000 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output_extended.py
+-rw-r--r--   0        0        0     1075 2024-03-29 15:38:21.245538 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/app_variant_revision.py
+-rw-r--r--   0        0        0      983 2024-03-29 15:38:21.246051 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/base_output.py
+-rw-r--r--   0        0        0     1061 2024-03-29 15:38:21.246493 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/body_import_testset.py
+-rw-r--r--   0        0        0     1028 2024-03-29 15:38:21.246936 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/config_db.py
+-rw-r--r--   0        0        0      182 2024-03-29 15:38:21.247467 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/container_templates_response.py
+-rw-r--r--   0        0        0      986 2024-03-29 15:38:21.248085 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/create_app_output.py
+-rw-r--r--   0        0        0      991 2024-03-29 15:38:21.248628 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/delete_evaluation.py
+-rw-r--r--   0        0        0      986 2024-03-29 15:38:21.249104 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/docker_env_vars.py
+-rw-r--r--   0        0        0     1176 2024-03-29 15:38:21.249534 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/environment_output.py
+-rw-r--r--   0        0        0     1376 2024-03-29 15:38:21.249971 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/evaluation.py
+-rw-r--r--   0        0        0     1497 2024-03-29 15:38:21.250499 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario.py
+-rw-r--r--   0        0        0     1027 2024-03-29 15:38:21.251140 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_input.py
+-rw-r--r--   0        0        0     1014 2024-03-29 15:38:21.251815 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_output.py
+-rw-r--r--   0        0        0     1033 2024-03-29 15:38:21.252247 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_result.py
+-rw-r--r--   0        0        0     1102 2024-03-29 15:38:21.252717 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/evaluation_status_enum.py
+-rw-r--r--   0        0        0      644 2024-03-29 15:38:21.253129 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/evaluation_type.py
+-rw-r--r--   0        0        0      971 2024-03-29 15:38:21.253545 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/evaluation_webhook.py
+-rw-r--r--   0        0        0     1046 2024-03-29 15:38:21.254100 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/evaluator.py
+-rw-r--r--   0        0        0     1124 2024-03-29 15:38:21.254598 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/evaluator_config.py
+-rw-r--r--   0        0        0     1136 2024-03-29 15:38:21.255072 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/feedback.py
+-rw-r--r--   0        0        0     1063 2024-03-29 15:38:21.255549 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/get_config_reponse.py
+-rw-r--r--   0        0        0     1060 2024-03-29 15:38:21.256152 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/http_validation_error.py
+-rw-r--r--   0        0        0     1305 2024-03-29 15:38:21.256706 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation.py
+-rw-r--r--   0        0        0     1580 2024-03-29 15:38:21.257151 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario.py
+-rw-r--r--   0        0        0     1006 2024-03-29 15:38:21.257665 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_input.py
+-rw-r--r--   0        0        0     1010 2024-03-29 15:38:21.258161 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_output.py
+-rw-r--r--   0        0        0      134 2024-03-29 15:38:21.258634 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_score.py
+-rw-r--r--   0        0        0      140 2024-03-29 15:38:21.259047 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_update_score.py
+-rw-r--r--   0        0        0     1048 2024-03-29 15:38:21.259555 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/image.py
+-rw-r--r--   0        0        0      965 2024-03-29 15:38:21.260000 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/invite_request.py
+-rw-r--r--   0        0        0     1095 2024-03-29 15:38:21.260474 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/list_api_keys_output.py
+-rw-r--r--   0        0        0     1045 2024-03-29 15:38:21.260976 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/llm_run_rate_limit.py
+-rw-r--r--   0        0        0     1009 2024-03-29 15:38:21.261472 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/new_testset.py
+-rw-r--r--   0        0        0     1181 2024-03-29 15:38:21.261911 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/organization.py
+-rw-r--r--   0        0        0      981 2024-03-29 15:38:21.262371 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/organization_output.py
+-rw-r--r--   0        0        0      996 2024-03-29 15:38:21.262822 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/result.py
+-rw-r--r--   0        0        0     1117 2024-03-29 15:38:21.263320 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/simple_evaluation_output.py
+-rw-r--r--   0        0        0     1546 2024-03-29 15:38:21.263903 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/span.py
+-rw-r--r--   0        0        0     1037 2024-03-29 15:38:21.264526 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/template.py
+-rw-r--r--   0        0        0     1189 2024-03-29 15:38:21.265123 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/template_image_info.py
+-rw-r--r--   0        0        0     1088 2024-03-29 15:38:21.265659 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/test_set_output_response.py
+-rw-r--r--   0        0        0     1004 2024-03-29 15:38:21.266314 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/test_set_simple_response.py
+-rw-r--r--   0        0        0     1353 2024-03-29 15:38:21.266828 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/trace.py
+-rw-r--r--   0        0        0      953 2024-03-29 15:38:21.267207 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/uri.py
+-rw-r--r--   0        0        0     1086 2024-03-29 15:38:21.267670 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-03-29 15:38:21.268112 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     1031 2024-03-29 15:38:21.268517 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/variant_action.py
+-rw-r--r--   0        0        0      511 2024-03-29 15:38:21.268961 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/variant_action_enum.py
+-rw-r--r--   0        0        0    19667 2024-04-02 20:00:54.885983 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/client.py
+-rw-r--r--   0        0        0       94 2024-03-29 15:38:21.269971 chainlo-1.1.417/chainlo/agenta_cli/agenta/client/exceptions.py
+-rw-r--r--   0        0        0      732 2024-03-29 15:38:21.270473 chainlo-1.1.417/chainlo/agenta_cli/agenta/config.py
+-rw-r--r--   0        0        0      245 2024-04-04 15:17:30.727889 chainlo-1.1.417/chainlo/agenta_cli/agenta/config.toml
+-rw-r--r--   0        0        0      317 2024-03-29 15:38:21.272321 chainlo-1.1.417/chainlo/agenta_cli/agenta/docker/docker-assets/Dockerfile.cloud.template
+-rw-r--r--   0        0        0      291 2024-04-03 22:53:43.117295 chainlo-1.1.417/chainlo/agenta_cli/agenta/docker/docker-assets/Dockerfile.template
+-rw-r--r--   0        0        0      102 2024-03-29 15:38:21.273161 chainlo-1.1.417/chainlo/agenta_cli/agenta/docker/docker-assets/README.md
+-rwxr-xr-x   0        0        0       75 2024-04-02 21:38:18.446443 chainlo-1.1.417/chainlo/agenta_cli/agenta/docker/docker-assets/entrypoint.sh
+-rw-r--r--   0        0        0      112 2024-04-02 20:23:24.001250 chainlo-1.1.417/chainlo/agenta_cli/agenta/docker/docker-assets/lambda_function.py
+-rw-r--r--   0        0        0      280 2024-04-02 20:23:49.555521 chainlo-1.1.417/chainlo/agenta_cli/agenta/docker/docker-assets/main.py
+-rw-r--r--   0        0        0     3561 2024-04-02 20:00:54.887775 chainlo-1.1.417/chainlo/agenta_cli/agenta/docker/docker_utils.py
+-rw-r--r--   0        0        0      565 2024-03-29 15:38:21.275737 chainlo-1.1.417/chainlo/agenta_cli/agenta/sdk/__init__.py
+-rw-r--r--   0        0        0    15514 2024-04-06 01:02:59.748843 chainlo-1.1.417/chainlo/agenta_cli/agenta/sdk/agenta_decorator.py
+-rw-r--r--   0        0        0     8063 2024-04-02 20:00:55.228132 chainlo-1.1.417/chainlo/agenta_cli/agenta/sdk/agenta_init.py
+-rw-r--r--   0        0        0      901 2024-03-29 15:38:21.277386 chainlo-1.1.417/chainlo/agenta_cli/agenta/sdk/context.py
+-rw-r--r--   0        0        0      269 2024-03-29 15:38:21.277737 chainlo-1.1.417/chainlo/agenta_cli/agenta/sdk/router.py
+-rw-r--r--   0        0        0     4658 2024-03-29 15:38:21.278086 chainlo-1.1.417/chainlo/agenta_cli/agenta/sdk/types.py
+-rw-r--r--   0        0        0      389 2024-04-02 20:23:10.241942 chainlo-1.1.417/chainlo/agenta_cli/agenta/sdk/utils/globals.py
+-rw-r--r--   0        0        0     5877 2024-03-29 15:38:21.279477 chainlo-1.1.417/chainlo/agenta_cli/agenta/sdk/utils/helper/openai_cost.py
+-rw-r--r--   0        0        0     1278 2024-03-29 15:38:21.279853 chainlo-1.1.417/chainlo/agenta_cli/agenta/sdk/utils/preinit.py
+-rw-r--r--   0        0        0      308 2024-03-29 15:38:21.281309 chainlo-1.1.417/chainlo/agenta_cli/agenta/templates/compose_email/README.md
+-rw-r--r--   0        0        0     2384 2024-03-29 15:38:21.281686 chainlo-1.1.417/chainlo/agenta_cli/agenta/templates/compose_email/app.py
+-rw-r--r--   0        0        0       70 2024-03-29 15:38:21.282049 chainlo-1.1.417/chainlo/agenta_cli/agenta/templates/compose_email/env.example
+-rw-r--r--   0        0        0       23 2024-03-29 15:38:21.282449 chainlo-1.1.417/chainlo/agenta_cli/agenta/templates/compose_email/requirements.txt
+-rw-r--r--   0        0        0       47 2024-03-29 15:38:21.282787 chainlo-1.1.417/chainlo/agenta_cli/agenta/templates/compose_email/template.toml
+-rw-r--r--   0        0        0      308 2024-03-29 15:38:21.283477 chainlo-1.1.417/chainlo/agenta_cli/agenta/templates/extract_data_to_json/README.md
+-rw-r--r--   0        0        0     1320 2024-03-29 15:38:21.283896 chainlo-1.1.417/chainlo/agenta_cli/agenta/templates/extract_data_to_json/app.py
+-rw-r--r--   0        0        0       70 2024-03-29 15:38:21.284271 chainlo-1.1.417/chainlo/agenta_cli/agenta/templates/extract_data_to_json/env.example
+-rw-r--r--   0        0        0       23 2024-03-29 15:38:21.284661 chainlo-1.1.417/chainlo/agenta_cli/agenta/templates/extract_data_to_json/requirements.txt
+-rw-r--r--   0        0        0       60 2024-03-29 15:38:21.285035 chainlo-1.1.417/chainlo/agenta_cli/agenta/templates/extract_data_to_json/template.toml
+-rw-r--r--   0        0        0      308 2024-03-29 15:38:21.285928 chainlo-1.1.417/chainlo/agenta_cli/agenta/templates/simple_prompt/README.md
+-rw-r--r--   0        0        0     1258 2024-04-03 22:59:21.919707 chainlo-1.1.417/chainlo/agenta_cli/agenta/templates/simple_prompt/app.py
+-rw-r--r--   0        0        0       70 2024-03-29 15:38:21.286665 chainlo-1.1.417/chainlo/agenta_cli/agenta/templates/simple_prompt/env.example
+-rw-r--r--   0        0        0       24 2024-04-02 15:18:01.855024 chainlo-1.1.417/chainlo/agenta_cli/agenta/templates/simple_prompt/requirements.txt
+-rw-r--r--   0        0        0       60 2024-03-29 15:38:21.287420 chainlo-1.1.417/chainlo/agenta_cli/agenta/templates/simple_prompt/template.toml
+-rw-r--r--   0        0        0     1078 2024-04-01 00:20:31.300954 chainlo-1.1.417/chainlo/agenta_cli/pyproject.toml-ex
+-rw-r--r--   0        0        0        0 2024-03-29 15:38:21.289373 chainlo-1.1.417/chainlo/agenta_cli/requirements.txt
+-rw-r--r--   0        0        0      580 2024-03-29 15:38:21.290495 chainlo-1.1.417/chainlo/agenta_cli/tests/example_projects/simple_langchain/app.py
+-rw-r--r--   0        0        0       31 2024-03-29 15:38:21.290969 chainlo-1.1.417/chainlo/agenta_cli/tests/example_projects/simple_langchain/requirements.txt
+-rw-r--r--   0        0        0      411 2024-03-29 15:38:21.292434 chainlo-1.1.417/chainlo/agenta_cli/tests/example_projects/test2/README.md
+-rw-r--r--   0        0        0     3294 2024-03-29 15:38:21.293249 chainlo-1.1.417/chainlo/agenta_cli/tests/example_projects/test2/agenta.py
+-rw-r--r--   0        0        0      580 2024-03-29 15:38:21.294048 chainlo-1.1.417/chainlo/agenta_cli/tests/example_projects/test2/app.py
+-rw-r--r--   0        0        0       51 2024-03-29 15:38:21.294746 chainlo-1.1.417/chainlo/agenta_cli/tests/example_projects/test2/config.toml
+-rw-r--r--   0        0        0      187 2024-03-29 15:38:21.295361 chainlo-1.1.417/chainlo/agenta_cli/tests/example_projects/test2/main.py
+-rw-r--r--   0        0        0       31 2024-03-29 15:38:21.295991 chainlo-1.1.417/chainlo/agenta_cli/tests/example_projects/test2/requirements.txt
+-rw-r--r--   0        0        0     2677 2024-04-02 20:00:55.227808 chainlo-1.1.417/chainlo/auth.py
+-rw-r--r--   0        0        0     1359 2024-04-02 20:00:55.227793 chainlo-1.1.417/chainlo/cache.py
+-rw-r--r--   0        0        0      875 2024-04-02 20:00:55.227834 chainlo-1.1.417/chainlo/chat_settings.py
+-rw-r--r--   0        0        0     4997 2024-04-14 19:24:39.525370 chainlo-1.1.417/chainlo/cli/__init__.py
+-rw-r--r--   0        0        0      717 2024-03-28 12:59:00.279324 chainlo-1.1.417/chainlo/cli/utils.py
+-rw-r--r--   0        0        0    13496 2024-04-06 23:44:16.214790 chainlo-1.1.417/chainlo/config.py
+-rw-r--r--   0        0        0     2471 2024-04-02 20:00:55.227752 chainlo-1.1.417/chainlo/context.py
+-rw-r--r--   0        0        0     8887 2024-04-02 13:46:34.758455 chainlo-1.1.417/chainlo/copilot/dist/assets/logo_dark-2a3cf740.svg
+-rw-r--r--   0        0        0     8889 2024-04-02 13:46:34.756788 chainlo-1.1.417/chainlo/copilot/dist/assets/logo_light-b078e7bc.svg
+-rw-r--r--   0        0        0  7013566 2024-04-02 13:46:35.752958 chainlo-1.1.417/chainlo/copilot/dist/index.js
+-rw-r--r--   0        0        0    14716 2024-04-02 20:00:55.191849 chainlo-1.1.417/chainlo/data/__init__.py
+-rw-r--r--   0        0        0      460 2024-04-02 20:00:54.932738 chainlo-1.1.417/chainlo/data/acl.py
+-rw-r--r--   0        0        0    10157 2024-04-02 20:00:55.227734 chainlo-1.1.417/chainlo/element.py
+-rw-r--r--   0        0        0    12170 2024-04-02 20:00:55.227715 chainlo-1.1.417/chainlo/emitter.py
+-rw-r--r--   0        0        0  3071160 2024-04-02 13:46:34.734588 chainlo-1.1.417/chainlo/frontend/dist/assets/index-7bc2ef31.js
+-rw-r--r--   0        0        0     6605 2024-04-02 13:46:34.736982 chainlo-1.1.417/chainlo/frontend/dist/assets/index-d088547c.css
+-rw-r--r--   0        0        0     8887 2024-04-02 13:46:34.736163 chainlo-1.1.417/chainlo/frontend/dist/assets/logo_dark-2a3cf740.svg
+-rw-r--r--   0        0        0     8889 2024-04-02 13:46:34.735648 chainlo-1.1.417/chainlo/frontend/dist/assets/logo_light-b078e7bc.svg
+-rw-r--r--   0        0        0  3763471 2024-04-02 13:46:34.739499 chainlo-1.1.417/chainlo/frontend/dist/assets/react-plotly-70086d41.js
+-rw-r--r--   0        0        0     6455 2024-04-02 13:46:34.741377 chainlo-1.1.417/chainlo/frontend/dist/favicon.svg
+-rw-r--r--   0        0        0     1005 2024-04-02 13:46:34.731871 chainlo-1.1.417/chainlo/frontend/dist/index.html
+-rw-r--r--   0        0        0      216 2024-04-02 20:00:55.228246 chainlo-1.1.417/chainlo/haystack/__init__.py
+-rw-r--r--   0        0        0     5205 2024-04-02 20:00:55.191778 chainlo-1.1.417/chainlo/haystack/callbacks.py
+-rw-r--r--   0        0        0     3015 2024-04-02 20:00:54.885954 chainlo-1.1.417/chainlo/hello.py
+-rw-r--r--   0        0        0     4879 2024-04-02 20:00:54.885927 chainlo-1.1.417/chainlo/input_widget.py
+-rw-r--r--   0        0        0      216 2024-04-02 20:00:55.171891 chainlo-1.1.417/chainlo/langchain/__init__.py
+-rw-r--r--   0        0        0    20518 2024-04-02 20:00:55.171912 chainlo-1.1.417/chainlo/langchain/callbacks.py
+-rw-r--r--   0        0        0      815 2024-04-02 20:00:55.171857 chainlo-1.1.417/chainlo/langflow/__init__.py
+-rw-r--r--   0        0        0      226 2024-04-02 20:00:55.171832 chainlo-1.1.417/chainlo/llama_index/__init__.py
+-rw-r--r--   0        0        0     6075 2024-04-02 20:00:55.134912 chainlo-1.1.417/chainlo/llama_index/callbacks.py
+-rw-r--r--   0        0        0      373 2024-03-28 12:59:00.282615 chainlo-1.1.417/chainlo/logger.py
+-rw-r--r--   0        0        0     1488 2024-04-14 19:13:03.255606 chainlo-1.1.417/chainlo/markdown.py
+-rw-r--r--   0        0        0    17674 2024-04-02 20:00:55.227695 chainlo-1.1.417/chainlo/message.py
+-rw-r--r--   0        0        0    17458 2024-04-02 20:00:55.227664 chainlo-1.1.417/chainlo/oauth_providers.py
+-rw-r--r--   0        0        0     1998 2024-04-02 20:00:54.975014 chainlo-1.1.417/chainlo/openai/__init__.py
+-rw-r--r--   0        0        0       80 2024-03-28 12:59:00.283801 chainlo-1.1.417/chainlo/playground/__init__.py
+-rw-r--r--   0        0        0     1031 2024-04-02 20:00:54.974932 chainlo-1.1.417/chainlo/playground/config.py
+-rw-r--r--   0        0        0     3854 2024-04-02 20:00:54.974863 chainlo-1.1.417/chainlo/playground/provider.py
+-rw-r--r--   0        0        0      236 2024-03-28 12:59:00.284521 chainlo-1.1.417/chainlo/playground/providers/__init__.py
+-rw-r--r--   0        0        0     3493 2024-04-02 20:00:54.974475 chainlo-1.1.417/chainlo/playground/providers/anthropic.py
+-rw-r--r--   0        0        0     2127 2024-04-02 20:00:54.954439 chainlo-1.1.417/chainlo/playground/providers/huggingface.py
+-rw-r--r--   0        0        0     3100 2024-04-02 20:00:54.932814 chainlo-1.1.417/chainlo/playground/providers/langchain.py
+-rw-r--r--   0        0        0    12395 2024-04-02 20:00:54.952587 chainlo-1.1.417/chainlo/playground/providers/openai.py
+-rw-r--r--   0        0        0     5081 2024-04-02 20:00:54.887826 chainlo-1.1.417/chainlo/playground/providers/vertexai.py
+-rw-r--r--   0        0        0        0 2024-03-28 12:59:00.285429 chainlo-1.1.417/chainlo/py.typed
+-rw-r--r--   0        0        0      295 2024-03-28 12:59:00.285564 chainlo-1.1.417/chainlo/secret.py
+-rw-r--r--   0        0        0    22586 2024-04-07 01:16:42.223923 chainlo-1.1.417/chainlo/server.py
+-rw-r--r--   0        0        0     8837 2024-04-02 20:00:55.227631 chainlo-1.1.417/chainlo/session.py
+-rw-r--r--   0        0        0     9834 2024-04-02 20:00:55.228438 chainlo-1.1.417/chainlo/socket.py
+-rw-r--r--   0        0        0    12742 2024-04-02 20:00:55.227568 chainlo-1.1.417/chainlo/step.py
+-rw-r--r--   0        0        0     1234 2024-04-02 20:00:55.191939 chainlo-1.1.417/chainlo/sync.py
+-rw-r--r--   0        0        0     3058 2024-04-02 20:00:55.191900 chainlo-1.1.417/chainlo/telemetry.py
+-rw-r--r--   0        0        0     6252 2024-03-28 12:59:00.286806 chainlo-1.1.417/chainlo/translations/de.json
+-rw-r--r--   0        0        0     4514 2024-03-28 12:59:00.287261 chainlo-1.1.417/chainlo/translations/en-US.json
+-rw-r--r--   0        0        0     4614 2024-03-28 12:59:00.287519 chainlo-1.1.417/chainlo/translations/pt-BR.json
+-rw-r--r--   0        0        0     3376 2024-04-02 20:00:55.191876 chainlo-1.1.417/chainlo/types.py
+-rw-r--r--   0        0        0      619 2024-03-28 12:59:00.287957 chainlo-1.1.417/chainlo/user.py
+-rw-r--r--   0        0        0     1367 2024-04-02 20:00:55.228294 chainlo-1.1.417/chainlo/user_session.py
+-rw-r--r--   0        0        0     2568 2024-04-02 20:00:55.191815 chainlo-1.1.417/chainlo/utils.py
+-rw-r--r--   0        0        0      196 2024-03-28 12:59:00.288410 chainlo-1.1.417/chainlo/version.py
+-rw-r--r--   0        0        0     2371 2024-04-14 20:44:55.429236 chainlo-1.1.417/pyproject.toml
+-rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 chainlo-1.1.417/PKG-INFO
```

### Comparing `chainlo-1.1.416/chainlo/__init__.py` & `chainlo-1.1.417/chainlo/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/action.py` & `chainlo-1.1.417/chainlo/action.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/README.md` & `chainlo-1.1.417/chainlo/agenta_cli/README.md`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/cli/helper.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/cli/helper.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/cli/main.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/cli/main.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/cli/telemetry.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/cli/telemetry.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/cli/variant_commands.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/cli/variant_commands.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/cli/variant_configs.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/cli/variant_configs.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/Readme.md` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/Readme.md`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/api.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/api.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/api_models.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/api_models.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/__init__.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/client.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/client.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/core/__init__.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/core/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/core/client_wrapper.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/core/datetime_utils.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/core/jsonable_encoder.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/__init__.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/aggregated_result.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/aggregated_result.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/app.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/app.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output_extended.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output_extended.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/app_variant_revision.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/app_variant_revision.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/base_output.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/base_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/body_import_testset.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/body_import_testset.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/config_db.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/config_db.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/create_app_output.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/create_app_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/delete_evaluation.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/delete_evaluation.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/docker_env_vars.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/docker_env_vars.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/environment_output.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/environment_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/evaluation.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/evaluation.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_input.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_input.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_output.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_result.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_result.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/evaluation_status_enum.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/evaluation_status_enum.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/evaluation_type.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/evaluation_type.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/evaluation_webhook.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/evaluation_webhook.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/evaluator.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/evaluator.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/evaluator_config.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/evaluator_config.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/feedback.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/feedback.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/get_config_reponse.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/get_config_reponse.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/http_validation_error.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_input.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_input.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_output.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/image.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/image.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/invite_request.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/invite_request.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/list_api_keys_output.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/list_api_keys_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/llm_run_rate_limit.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/llm_run_rate_limit.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/new_testset.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/new_testset.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/organization.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/organization.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/organization_output.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/organization_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/result.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/result.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/simple_evaluation_output.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/simple_evaluation_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/span.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/span.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/template.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/template.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/template_image_info.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/template_image_info.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/test_set_output_response.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/test_set_output_response.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/test_set_simple_response.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/test_set_simple_response.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/trace.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/trace.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/uri.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/uri.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/validation_error.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/backend/types/variant_action.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/backend/types/variant_action.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/client/client.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/client/client.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/config.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/config.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/docker/docker_utils.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/docker/docker_utils.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/sdk/__init__.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/sdk/agenta_decorator.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/sdk/agenta_decorator.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/sdk/agenta_init.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/sdk/agenta_init.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/sdk/context.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/sdk/context.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/sdk/types.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/sdk/types.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/sdk/utils/helper/openai_cost.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/sdk/utils/helper/openai_cost.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/sdk/utils/preinit.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/sdk/utils/preinit.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/templates/compose_email/app.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/templates/compose_email/app.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/templates/extract_data_to_json/app.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/templates/extract_data_to_json/app.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/agenta/templates/simple_prompt/app.py` & `chainlo-1.1.417/chainlo/agenta_cli/agenta/templates/simple_prompt/app.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/pyproject.toml-ex` & `chainlo-1.1.417/chainlo/agenta_cli/pyproject.toml-ex`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/tests/example_projects/simple_langchain/app.py` & `chainlo-1.1.417/chainlo/agenta_cli/tests/example_projects/simple_langchain/app.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/tests/example_projects/test2/agenta.py` & `chainlo-1.1.417/chainlo/agenta_cli/tests/example_projects/test2/agenta.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/agenta_cli/tests/example_projects/test2/app.py` & `chainlo-1.1.417/chainlo/agenta_cli/tests/example_projects/test2/app.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/auth.py` & `chainlo-1.1.417/chainlo/auth.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/cache.py` & `chainlo-1.1.417/chainlo/cache.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/chat_settings.py` & `chainlo-1.1.417/chainlo/chat_settings.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/cli/__init__.py` & `chainlo-1.1.417/chainlo/cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,26 +63,26 @@
 
     # Initialize the LangChain cache if installed and enabled
     init_lc_cache()
 
     log_level = "debug" if config.run.debug else "error"
 
     print("el config el koullll ", config)
-    print("config.root_path", config.project.root_path)
-    _root_path = config.project.root_path
-    print("root_path", _root_path)
+    # print("config.root_path", config.project.root_path)
+    # _root_path = config.project.root_path
+    # print("root_path", _root_path)
     # Start the server
     async def start():
         _config = uvicorn.Config(
             app,
             host=host,
             port=port,
             log_level=log_level,
             ws_per_message_deflate=ws_per_message_deflate,
-            root_path=_root_path,
+            # root_path=_root_path,
         )
         server = uvicorn.Server(_config)
         await server.serve()
     print("Starting server Yal Fouuuuuuuu !!!!!!!!!")
     # Run the asyncio event loop instead of uvloop to enable re entrance
     asyncio.run(start())
     # uvicorn.run(app, host=host, port=port, log_level=log_level)
```

### Comparing `chainlo-1.1.416/chainlo/cli/utils.py` & `chainlo-1.1.417/chainlo/cli/utils.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/config.py` & `chainlo-1.1.417/chainlo/config.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/context.py` & `chainlo-1.1.417/chainlo/context.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/copilot/dist/assets/logo_dark-2a3cf740.svg` & `chainlo-1.1.417/chainlo/copilot/dist/assets/logo_dark-2a3cf740.svg`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/copilot/dist/assets/logo_light-b078e7bc.svg` & `chainlo-1.1.417/chainlo/copilot/dist/assets/logo_light-b078e7bc.svg`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/copilot/dist/index.js` & `chainlo-1.1.417/chainlo/copilot/dist/index.js`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/data/__init__.py` & `chainlo-1.1.417/chainlo/data/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/element.py` & `chainlo-1.1.417/chainlo/element.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/emitter.py` & `chainlo-1.1.417/chainlo/emitter.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/frontend/dist/assets/index-7bc2ef31.js` & `chainlo-1.1.417/chainlo/frontend/dist/assets/index-7bc2ef31.js`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/frontend/dist/assets/index-d088547c.css` & `chainlo-1.1.417/chainlo/frontend/dist/assets/index-d088547c.css`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/frontend/dist/assets/logo_dark-2a3cf740.svg` & `chainlo-1.1.417/chainlo/frontend/dist/assets/logo_dark-2a3cf740.svg`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/frontend/dist/assets/logo_light-b078e7bc.svg` & `chainlo-1.1.417/chainlo/frontend/dist/assets/logo_light-b078e7bc.svg`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/frontend/dist/assets/react-plotly-70086d41.js` & `chainlo-1.1.417/chainlo/frontend/dist/assets/react-plotly-70086d41.js`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/frontend/dist/favicon.svg` & `chainlo-1.1.417/chainlo/frontend/dist/favicon.svg`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/frontend/dist/index.html` & `chainlo-1.1.417/chainlo/frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/haystack/callbacks.py` & `chainlo-1.1.417/chainlo/haystack/callbacks.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/hello.py` & `chainlo-1.1.417/chainlo/hello.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/input_widget.py` & `chainlo-1.1.417/chainlo/input_widget.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/langchain/callbacks.py` & `chainlo-1.1.417/chainlo/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/langflow/__init__.py` & `chainlo-1.1.417/chainlo/langflow/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/llama_index/callbacks.py` & `chainlo-1.1.417/chainlo/llama_index/callbacks.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/markdown.py` & `chainlo-1.1.417/chainlo/markdown.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 import os
 
 from chainlo.logger import logger
 
 # Default chainlit.md file created if none exists
-DEFAULT_MARKDOWN_STR = """# Welcome to Chainlit! 🚀🤖
+DEFAULT_MARKDOWN_STR = """# Welcome to Aladin Assistants! 🚀🤖
 
-Hi there, Developer! 👋 We're excited to have you on board. Chainlit is a powerful tool designed to help you prototype, debug and share applications built on top of LLMs.
+Hi there, Developer! 👋 We're excited to have you on board. Aladin Assistants is a powerful tool designed to help you prototype, debug and share applications built on top of LLMs.
 
-## Useful Links 🔗
-
-- **Documentation:** Get started with our comprehensive [Chainlit Documentation](https://docs.chainlit.io) 📚
-- **Discord Community:** Join our friendly [Chainlit Discord](https://discord.gg/k73SQ3FyUh) to ask questions, share your projects, and connect with other developers! 💬
-
-We can't wait to see what you create with Chainlit! Happy coding! 💻😊
-
-## Welcome screen
-
-To modify the welcome screen, edit the `chainlit.md` file at the root of your project. If you do not want a welcome screen, just leave this file empty.
 """
 
 
 def init_markdown(root: str):
     """Initialize the chainlit.md file if it doesn't exist."""
     chainlit_md_file = os.path.join(root, "chainlit.md")
```

### Comparing `chainlo-1.1.416/chainlo/message.py` & `chainlo-1.1.417/chainlo/message.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/oauth_providers.py` & `chainlo-1.1.417/chainlo/oauth_providers.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/openai/__init__.py` & `chainlo-1.1.417/chainlo/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/playground/config.py` & `chainlo-1.1.417/chainlo/playground/config.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/playground/provider.py` & `chainlo-1.1.417/chainlo/playground/provider.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/playground/providers/anthropic.py` & `chainlo-1.1.417/chainlo/playground/providers/anthropic.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/playground/providers/huggingface.py` & `chainlo-1.1.417/chainlo/playground/providers/huggingface.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/playground/providers/langchain.py` & `chainlo-1.1.417/chainlo/playground/providers/langchain.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/playground/providers/openai.py` & `chainlo-1.1.417/chainlo/playground/providers/openai.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/playground/providers/vertexai.py` & `chainlo-1.1.417/chainlo/playground/providers/vertexai.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/server.py` & `chainlo-1.1.417/chainlo/server.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/session.py` & `chainlo-1.1.417/chainlo/session.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/socket.py` & `chainlo-1.1.417/chainlo/socket.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/step.py` & `chainlo-1.1.417/chainlo/step.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/sync.py` & `chainlo-1.1.417/chainlo/sync.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/telemetry.py` & `chainlo-1.1.417/chainlo/telemetry.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/translations/de.json` & `chainlo-1.1.417/chainlo/translations/de.json`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/translations/en-US.json` & `chainlo-1.1.417/chainlo/translations/en-US.json`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/translations/pt-BR.json` & `chainlo-1.1.417/chainlo/translations/pt-BR.json`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/types.py` & `chainlo-1.1.417/chainlo/types.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/user.py` & `chainlo-1.1.417/chainlo/user.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/user_session.py` & `chainlo-1.1.417/chainlo/user_session.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/chainlo/utils.py` & `chainlo-1.1.417/chainlo/utils.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.1.416/pyproject.toml` & `chainlo-1.1.417/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainlo"
-version = "1.1.416"
+version = "1.1.417"
 keywords = ['LLM', 'Agents', 'gen ai', 'chat ui', 'chatbot ui', 'openai', 'copilot', 'langchain', 'conversational ai']
 description = "Build Conversational AI."
 authors = ["Chainlo"]
 license = "Apache-2.0 license"
 repository = "https://github.com/Chainlit/chainlit"
 readme = "README.md"
 exclude = [
```

### Comparing `chainlo-1.1.416/PKG-INFO` & `chainlo-1.1.417/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlo
-Version: 1.1.416
+Version: 1.1.417
 Summary: Build Conversational AI.
 Home-page: https://github.com/Chainlit/chainlit
 License: Apache-2.0 license
 Keywords: LLM,Agents,gen ai,chat ui,chatbot ui,openai,copilot,langchain,conversational ai
 Author: Chainlo
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
```


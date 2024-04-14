# Comparing `tmp/solutions_builder-1.17.9.tar.gz` & `tmp/solutions_builder-1.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solutions_builder-1.17.9.tar", max compression
+gzip compressed data, was "solutions_builder-1.18.0.tar", max compression
```

## Comparing `solutions_builder-1.17.9.tar` & `solutions_builder-1.18.0.tar`

### file list

```diff
@@ -1,203 +1,237 @@
--rw-r--r--   0        0        0    11358 2022-06-28 21:05:37.723277 solutions_builder-1.17.9/LICENSE
--rw-r--r--   0        0        0     5262 2023-08-10 18:49:50.184543 solutions_builder-1.17.9/README.md
--rw-r--r--   0        0        0     1150 2023-08-16 18:07:12.485985 solutions_builder-1.17.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.622568 solutions_builder-1.17.9/solutions_builder/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.622645 solutions_builder-1.17.9/solutions_builder/cli/__init__.py
--rw-r--r--   0        0        0     7197 2023-08-10 18:49:50.185421 solutions_builder-1.17.9/solutions_builder/cli/cli.py
--rw-r--r--   0        0        0     4630 2023-08-10 18:10:06.462083 solutions_builder-1.17.9/solutions_builder/cli/cli_utils.py
--rw-r--r--   0        0        0     6961 2023-08-10 19:12:36.858975 solutions_builder-1.17.9/solutions_builder/cli/component.py
--rw-r--r--   0        0        0     6145 2023-08-11 17:53:15.272636 solutions_builder-1.17.9/solutions_builder/cli/infra.py
--rw-r--r--   0        0        0     2620 2023-08-14 04:15:33.013020 solutions_builder-1.17.9/solutions_builder/cli/set.py
--rw-r--r--   0        0        0     1416 2023-07-31 19:26:06.133259 solutions_builder-1.17.9/solutions_builder/cli/template.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.624032 solutions_builder-1.17.9/solutions_builder/copier_extensions/__init__.py
--rw-r--r--   0        0        0     5205 2023-08-10 18:49:50.185864 solutions_builder-1.17.9/solutions_builder/copier_extensions/sb_helpers.py
--rw-r--r--   0        0        0        0 2023-08-10 19:20:40.337609 solutions_builder-1.17.9/solutions_builder/fragments/skaffold_template/copier.yaml
--rw-r--r--   0        0        0      101 2023-07-31 15:22:50.624510 solutions_builder-1.17.9/solutions_builder/module_template/.st/module_answers/{{'{{component_name}}'}}.yaml
--rw-r--r--   0        0        0      766 2023-07-31 15:22:50.624649 solutions_builder-1.17.9/solutions_builder/module_template/README.md
--rw-r--r--   0        0        0      865 2023-08-10 18:49:50.186207 solutions_builder-1.17.9/solutions_builder/module_template/copier.yaml
--rw-r--r--   0        0        0       89 2023-07-31 15:22:50.625018 solutions_builder-1.17.9/solutions_builder/module_template/docs/components/{{'{{component_name}}'}}.md
--rw-r--r--   0        0        0     1135 2023-08-10 18:49:50.186419 solutions_builder-1.17.9/solutions_builder/module_template/template_copier.yaml
--rw-r--r--   0        0        0     3878 2023-07-31 19:26:06.134447 solutions_builder-1.17.9/solutions_builder/module_template/{{"{{'.github' if use_github_action}}"}}/workflows/{{"unit_test_linter_{{component_name}}"}}.yaml
--rw-r--r--   0        0        0      566 2023-07-31 15:22:50.625671 solutions_builder-1.17.9/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/Dockerfile
--rw-r--r--   0        0        0      109 2023-07-31 15:22:50.625798 solutions_builder-1.17.9/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/requirements.txt
--rw-r--r--   0        0        0     3204 2023-07-31 15:22:50.625960 solutions_builder-1.17.9/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/skaffold.yaml
--rw-r--r--   0        0        0      590 2023-07-31 19:26:06.135288 solutions_builder-1.17.9/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/src/main.py
--rw-r--r--   0        0        0       81 2023-07-31 15:22:50.626261 solutions_builder-1.17.9/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/st_module.yaml
--rw-r--r--   0        0        0      736 2023-07-31 19:26:06.135779 solutions_builder-1.17.9/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/backend.tf
--rw-r--r--   0        0        0      636 2023-07-31 19:26:06.136084 solutions_builder-1.17.9/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/main.tf
--rw-r--r--   0        0        0      836 2023-07-31 19:26:06.136404 solutions_builder-1.17.9/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/providers.tf
--rw-r--r--   0        0        0      777 2023-07-31 19:26:06.137072 solutions_builder-1.17.9/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/terraform.tfvars
--rw-r--r--   0        0        0      858 2023-07-31 19:26:06.137649 solutions_builder-1.17.9/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/variables.tf
--rw-r--r--   0        0        0       80 2023-08-07 16:00:17.013007 solutions_builder-1.17.9/solutions_builder/modules/restful_service/.sb/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1363 2023-07-31 15:22:50.627536 solutions_builder-1.17.9/solutions_builder/modules/restful_service/README.md
--rw-r--r--   0        0        0      545 2023-07-31 15:22:50.627695 solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/Dockerfile
--rw-r--r--   0        0        0     1257 2023-07-31 15:22:50.628306 solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/README.md
--rw-r--r--   0        0        0      215 2023-07-31 15:22:50.628605 solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/manifests/cloudrun-service.yaml
--rw-r--r--   0        0        0       77 2023-07-31 15:22:50.628881 solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/requirements-test.txt
--rw-r--r--   0        0        0       98 2023-07-31 15:22:50.629046 solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/requirements.txt
--rw-r--r--   0        0        0     2974 2023-07-31 15:22:50.629209 solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/skaffold.yaml
--rw-r--r--   0        0        0      862 2023-07-31 19:26:06.138139 solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/src/config.py
--rw-r--r--   0        0        0     1711 2023-07-31 19:26:06.138427 solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/src/main.py
--rw-r--r--   0        0        0     1664 2023-07-31 19:26:06.138760 solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.629799 solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/__init__.py
--rw-r--r--   0        0        0     3876 2023-07-31 19:26:06.139176 solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py
--rw-r--r--   0        0        0     1222 2023-07-31 19:26:06.139854 solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.630283 solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/src/utils/__init__.py
--rw-r--r--   0        0        0     1232 2023-07-31 15:22:50.630545 solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml
--rw-r--r--   0        0        0      197 2023-07-31 15:22:50.630703 solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/kustomization.yaml
--rw-r--r--   0        0        0       60 2023-07-31 15:22:50.630849 solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/properties.env
--rw-r--r--   0        0        0      229 2023-07-31 15:22:50.630997 solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/service.yaml
--rw-r--r--   0        0        0      421 2023-07-31 15:22:50.631183 solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/hpa.yaml
--rw-r--r--   0        0        0      103 2023-07-31 15:22:50.631328 solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/kustomization.yaml
--rw-r--r--   0        0        0     2305 2023-08-10 18:49:50.186880 solutions_builder-1.17.9/solutions_builder/modules/restful_service/copier.yaml
--rw-r--r--   0        0        0      120 2023-07-31 15:22:50.631626 solutions_builder-1.17.9/solutions_builder/modules/restful_service/docs/components/{{component_name}}.md
--rw-r--r--   0        0        0       92 2023-07-31 15:22:50.631734 solutions_builder-1.17.9/solutions_builder/modules/restful_service/skaffold.yaml.patch
--rw-r--r--   0        0        0      263 2023-07-31 15:22:50.631945 solutions_builder-1.17.9/solutions_builder/modules/restful_service/terraform/stages/{{'3-httplb-cloudrun' if cloudrun_neg}}/{{component_name}}_neg.tf
--rw-r--r--   0        0        0     3223 2023-07-31 15:22:50.632152 solutions_builder-1.17.9/solutions_builder/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py
--rw-r--r--   0        0        0     3269 2023-07-31 15:22:50.632352 solutions_builder-1.17.9/solutions_builder/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
--rw-r--r--   0        0        0       80 2023-08-07 16:00:17.013263 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/.sb/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1572 2023-07-31 15:22:50.632676 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/README.md
--rw-r--r--   0        0        0      545 2023-07-31 15:22:50.632822 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/Dockerfile
--rw-r--r--   0        0        0      215 2023-07-31 15:22:50.632992 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/manifests/cloudrun-service.yaml
--rw-r--r--   0        0        0       77 2023-07-31 15:22:50.633061 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/requirements-test.txt
--rw-r--r--   0        0        0      143 2023-07-31 15:22:50.633183 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/requirements.txt
--rw-r--r--   0        0        0     3193 2023-07-31 15:22:50.633333 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/skaffold.yaml
--rw-r--r--   0        0        0      942 2023-07-31 19:26:06.140161 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/config.py
--rw-r--r--   0        0        0     1751 2023-07-31 19:26:06.140436 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/main.py
--rw-r--r--   0        0        0     1550 2023-07-31 19:26:06.140868 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/models/task.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.633781 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/__init__.py
--rw-r--r--   0        0        0     5195 2023-07-31 19:26:06.141312 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/tasks.py
--rw-r--r--   0        0        0     1196 2023-07-31 19:26:06.141730 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/schemas/task.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.634163 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.634237 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/__init__.py
--rw-r--r--   0        0        0      430 2023-07-31 15:22:50.634359 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/example.yaml
--rw-r--r--   0        0        0     1348 2023-07-31 15:22:50.634473 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow.py
--rw-r--r--   0        0        0     1138 2023-07-31 15:22:50.634593 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow_test.py
--rw-r--r--   0        0        0     1232 2023-07-31 15:22:50.634791 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/deployment.yaml
--rw-r--r--   0        0        0      197 2023-07-31 15:22:50.634913 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/kustomization.yaml
--rw-r--r--   0        0        0       97 2023-07-31 15:22:50.635030 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/properties.env
--rw-r--r--   0        0        0      229 2023-07-31 15:22:50.635163 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/service.yaml
--rw-r--r--   0        0        0      421 2023-07-31 15:22:50.635357 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/hpa/hpa.yaml
--rw-r--r--   0        0        0      103 2023-07-31 15:22:50.635506 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/hpa/kustomization.yaml
--rw-r--r--   0        0        0     2667 2023-08-10 18:49:50.187221 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/copier.yaml
--rw-r--r--   0        0        0       71 2023-07-31 15:22:50.635866 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/docs/components/{{component_name}}.md
--rw-r--r--   0        0        0       92 2023-07-31 15:22:50.635986 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/skaffold.yaml.patch
--rw-r--r--   0        0        0      719 2023-07-31 19:26:06.142418 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/backend.tf
--rw-r--r--   0        0        0     2693 2023-07-31 19:26:06.142972 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/main.tf
--rw-r--r--   0        0        0      930 2023-07-31 19:26:06.143419 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/providers.tf
--rw-r--r--   0        0        0     1280 2023-07-31 19:26:06.143751 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/terraform.tfvars
--rw-r--r--   0        0        0     2076 2023-07-31 19:26:06.144059 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/variables.tf
--rw-r--r--   0        0        0     3851 2023-07-31 19:26:06.144531 solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
--rw-r--r--   0        0        0       80 2023-08-07 16:00:17.013512 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke/.sb/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1374 2023-08-10 18:49:50.187691 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke/copier.yaml
--rw-r--r--   0        0        0      794 2023-07-31 15:22:50.637941 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke/docs/components/{{component_name}}.md
--rw-r--r--   0        0        0      701 2023-07-31 19:26:06.144964 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/backend.tf
--rw-r--r--   0        0        0     1568 2023-07-31 19:26:06.145601 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/iam.tf
--rw-r--r--   0        0        0     2486 2023-07-31 19:26:06.145978 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/main.tf
--rw-r--r--   0        0        0     1783 2023-07-31 19:26:06.146393 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/providers.tf
--rw-r--r--   0        0        0      268 2023-07-31 15:22:50.639380 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/terraform.tfvars
--rw-r--r--   0        0        0     1553 2023-07-31 19:26:06.146871 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/variables.tf
--rw-r--r--   0        0        0       80 2023-08-07 16:00:17.014089 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/.sb/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     2306 2023-08-10 18:49:50.188092 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/copier.yaml
--rw-r--r--   0        0        0      181 2023-08-11 19:05:30.220409 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/frontend_config.yaml
--rw-r--r--   0        0        0      658 2023-07-31 15:22:50.641933 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/ingress.yaml
--rw-r--r--   0        0        0      145 2023-07-31 15:22:50.642056 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/kustomization.yaml
--rw-r--r--   0        0        0      185 2023-07-31 15:22:50.642172 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/managed_cert.yaml
--rw-r--r--   0        0        0      378 2023-07-31 15:22:50.642293 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/ingress/skaffold.yaml
--rw-r--r--   0        0        0       59 2023-08-03 16:02:48.218741 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/skaffold.yaml.patch
--rw-r--r--   0        0        0     1560 2023-08-08 20:33:13.355918 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/main.tf
--rw-r--r--   0        0        0      670 2023-07-31 19:26:06.147738 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/outputs.tf
--rw-r--r--   0        0        0     1264 2023-07-31 19:26:06.148024 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/variables.tf
--rw-r--r--   0        0        0      709 2023-07-31 19:26:06.148386 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/backend.tf
--rw-r--r--   0        0        0     1568 2023-07-31 19:26:06.148713 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/iam.tf
--rw-r--r--   0        0        0     1695 2023-07-31 19:26:06.149003 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/main.tf
--rw-r--r--   0        0        0     1877 2023-07-31 19:26:06.149312 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/providers.tf
--rw-r--r--   0        0        0      480 2023-07-31 15:22:50.643659 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/terraform.tfvars
--rw-r--r--   0        0        0     1802 2023-07-31 19:26:06.149801 solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/variables.tf
--rw-r--r--   0        0        0       80 2023-07-31 15:22:50.644034 solutions_builder-1.17.9/solutions_builder/modules/terraform_httplb_cloudrun/.st/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1048 2023-08-10 18:49:50.188374 solutions_builder-1.17.9/solutions_builder/modules/terraform_httplb_cloudrun/copier.yaml
--rw-r--r--   0        0        0      834 2023-07-31 19:26:06.150138 solutions_builder-1.17.9/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf
--rw-r--r--   0        0        0     2760 2023-07-31 15:22:50.644547 solutions_builder-1.17.9/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf
--rw-r--r--   0        0        0      670 2023-07-31 19:26:06.150553 solutions_builder-1.17.9/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf
--rw-r--r--   0        0        0     1298 2023-07-31 19:26:06.151001 solutions_builder-1.17.9/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf
--rw-r--r--   0        0        0       81 2023-07-31 15:22:50.644903 solutions_builder-1.17.9/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/st_module.yaml
--rw-r--r--   0        0        0      196 2023-07-31 15:22:50.645021 solutions_builder-1.17.9/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/terraform.tfvars
--rw-r--r--   0        0        0     1984 2023-07-31 19:26:06.151475 solutions_builder-1.17.9/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf
--rw-r--r--   0        0        0       90 2023-07-31 15:22:50.645285 solutions_builder-1.17.9/solutions_builder/requirements.txt
--rw-r--r--   0        0        0    68957 2023-07-31 15:22:50.645771 solutions_builder-1.17.9/solutions_builder/template_root/.github/assets/setup_local.png
--rw-r--r--   0        0        0   239307 2023-07-31 15:22:50.647206 solutions_builder-1.17.9/solutions_builder/template_root/.github/assets/skaffold_dev_terminal.png
--rw-r--r--   0        0        0     2639 2023-07-31 15:22:50.647454 solutions_builder-1.17.9/solutions_builder/template_root/.github/workflows/deployment_cloudrun_dev.yaml
--rw-r--r--   0        0        0     2690 2023-07-31 15:22:50.647592 solutions_builder-1.17.9/solutions_builder/template_root/.github/workflows/deployment_gke_dev.yaml
--rw-r--r--   0        0        0     5786 2023-08-07 16:00:17.015359 solutions_builder-1.17.9/solutions_builder/template_root/.github/workflows/e2e_cloudrun_api_test.yaml
--rw-r--r--   0        0        0     8049 2023-08-07 16:00:17.015808 solutions_builder-1.17.9/solutions_builder/template_root/.github/workflows/e2e_gke_api_test.yaml
--rw-r--r--   0        0        0     3131 2023-07-31 15:22:50.648490 solutions_builder-1.17.9/solutions_builder/template_root/.github/workflows/unit_test_linter_common.yaml
--rw-r--r--   0        0        0      471 2023-07-31 15:22:50.648622 solutions_builder-1.17.9/solutions_builder/template_root/.gitignore
--rw-r--r--   0        0        0    14552 2023-07-31 15:22:50.648747 solutions_builder-1.17.9/solutions_builder/template_root/.pylintrc
--rw-r--r--   0        0        0     1760 2023-08-11 17:16:46.809461 solutions_builder-1.17.9/solutions_builder/template_root/README.md
--rw-r--r--   0        0        0      398 2023-07-31 15:22:50.649329 solutions_builder-1.17.9/solutions_builder/template_root/components/README.md
--rw-r--r--   0        0        0      211 2023-07-31 15:22:50.649479 solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile
--rw-r--r--   0        0        0      395 2023-07-31 15:22:50.649633 solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile.unittest
--rw-r--r--   0        0        0       77 2023-07-31 15:22:50.649720 solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/requirements-test.txt
--rw-r--r--   0        0        0      131 2023-07-31 15:22:50.649904 solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/requirements.txt
--rw-r--r--   0        0        0      571 2023-07-31 15:22:50.650164 solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/skaffold.yaml
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.650248 solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/__init__.py
--rw-r--r--   0        0        0      831 2023-07-31 19:26:06.151862 solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/config.py
--rw-r--r--   0        0        0      695 2023-07-31 19:26:06.153743 solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/db_client.py
--rw-r--r--   0        0        0       35 2023-07-31 15:22:50.650730 solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/README.md
--rw-r--r--   0        0        0       91 2023-07-31 15:22:50.650873 solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/__init__.py
--rw-r--r--   0        0        0     1376 2023-07-31 19:26:06.154070 solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/example.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.651072 solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/__init__.py
--rw-r--r--   0        0        0      754 2023-07-31 19:26:06.154613 solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/bq_client_fixture.py
--rw-r--r--   0        0        0     1006 2023-07-31 19:26:06.155093 solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/client_with_emulator.py
--rw-r--r--   0        0        0     2243 2023-07-31 19:26:06.155755 solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/firestore_emulator.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.651579 solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/__init__.py
--rw-r--r--   0        0        0     1002 2023-07-31 19:26:06.156062 solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/logging_handler.py
--rw-r--r--   0        0        0     2434 2023-08-11 17:19:54.149563 solutions_builder-1.17.9/solutions_builder/template_root/copier.yaml
--rw-r--r--   0        0        0       97 2023-07-31 15:22:50.652011 solutions_builder-1.17.9/solutions_builder/template_root/firebase.json
--rw-r--r--   0        0        0      359 2023-08-07 16:00:17.016290 solutions_builder-1.17.9/solutions_builder/template_root/sb.yaml
--rw-r--r--   0        0        0       98 2023-07-31 15:22:50.652089 solutions_builder-1.17.9/solutions_builder/template_root/setup.cfg
--rw-r--r--   0        0        0      215 2023-07-31 15:22:50.652207 solutions_builder-1.17.9/solutions_builder/template_root/skaffold.yaml
--rw-r--r--   0        0        0      921 2023-07-31 19:26:06.156495 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/cloudbuild/main.tf
--rw-r--r--   0        0        0      730 2023-07-31 19:26:06.157029 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/cloudbuild/variables.tf
--rw-r--r--   0        0        0     3585 2023-07-31 19:26:06.157569 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/cloudrun/main.tf
--rw-r--r--   0        0        0     1178 2023-07-31 19:26:06.158072 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/cloudrun/variables.tf
--rw-r--r--   0        0        0     5024 2023-07-31 19:26:06.158367 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/compute_backend/main.tf
--rw-r--r--   0        0        0      190 2023-07-31 15:22:50.653603 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/compute_backend/outputs.tf
--rw-r--r--   0        0        0     1186 2023-07-31 19:26:06.158842 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/compute_backend/providers.tf
--rw-r--r--   0        0        0     1601 2023-07-31 19:26:06.159185 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/compute_backend/variables.tf
--rw-r--r--   0        0        0     2364 2023-07-31 19:26:06.159491 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/firebase/main.tf
--rw-r--r--   0        0        0     1194 2023-07-31 19:26:06.160029 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/firebase/variables.tf
--rw-r--r--   0        0        0     3860 2023-07-31 19:26:06.160499 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/gke/main.tf
--rw-r--r--   0        0        0      832 2023-07-31 19:26:06.160786 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/gke/outputs.tf
--rw-r--r--   0        0        0     3453 2023-08-14 04:19:27.140460 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/gke/variables.tf
--rw-r--r--   0        0        0     3012 2023-08-07 16:00:17.017038 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/ingress_nginx/main.tf
--rw-r--r--   0        0        0      692 2023-07-31 19:26:06.161609 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/ingress_nginx/outputs.tf
--rw-r--r--   0        0        0     1087 2023-07-31 19:26:06.161883 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/ingress_nginx/variables.tf
--rw-r--r--   0        0        0      827 2023-07-31 19:26:06.162157 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/project_services/main.tf
--rw-r--r--   0        0        0      774 2023-07-31 19:26:06.162534 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/project_services/variables.tf
--rw-r--r--   0        0        0      953 2023-07-31 19:26:06.162825 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/service_account/main.tf
--rw-r--r--   0        0        0     1037 2023-07-31 19:26:06.163149 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/service_account/variables.tf
--rw-r--r--   0        0        0     1529 2023-07-31 19:26:06.163558 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/terraform_cicd/main.tf
--rw-r--r--   0        0        0      678 2023-07-31 19:26:06.163969 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/terraform_cicd/variables.tf
--rw-r--r--   0        0        0     1333 2023-07-31 19:26:06.164360 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/vpc_network/main.tf
--rw-r--r--   0        0        0     1269 2023-07-31 19:26:06.164825 solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/vpc_network/variables.tf
--rw-r--r--   0        0        0     2306 2023-08-07 16:00:17.017595 solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/1-bootstrap/main.tf
--rw-r--r--   0        0        0      730 2023-07-31 19:26:06.165370 solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/1-bootstrap/output.tf
--rw-r--r--   0        0        0       66 2023-07-31 15:22:50.656645 solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/1-bootstrap/terraform.tfvars
--rw-r--r--   0        0        0     1071 2023-07-31 19:26:06.165664 solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/1-bootstrap/variables.tf
--rw-r--r--   0        0        0      826 2023-07-31 19:26:06.166236 solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/2-foundation/backend.tf
--rw-r--r--   0        0        0     1435 2023-08-13 18:48:27.395950 solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/2-foundation/firestore_setup.tf
--rw-r--r--   0        0        0     1568 2023-07-31 19:26:06.166512 solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/2-foundation/iam.tf
--rw-r--r--   0        0        0      823 2023-08-13 18:29:37.464423 solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/2-foundation/identity_platform.tf
--rw-r--r--   0        0        0     4662 2023-08-13 18:50:52.233727 solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/2-foundation/main.tf
--rw-r--r--   0        0        0      991 2023-07-31 19:26:06.167766 solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/2-foundation/outputs.tf
--rw-r--r--   0        0        0      921 2023-08-10 18:49:50.189868 solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/2-foundation/providers.tf
--rw-r--r--   0        0        0      670 2023-08-11 17:04:02.459409 solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/2-foundation/terraform.tfvars
--rw-r--r--   0        0        0     2707 2023-08-13 18:44:19.906640 solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/2-foundation/variables.tf
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.657846 solutions_builder-1.17.9/solutions_builder/template_root/tests/__init__.py
--rw-r--r--   0        0        0     1386 2023-08-11 17:18:05.788947 solutions_builder-1.17.9/solutions_builder/template_root/tests/e2e/e2e_utils.py
--rwxr-xr-x   0        0        0      952 2023-08-11 17:19:05.627205 solutions_builder-1.17.9/solutions_builder/template_root/utils/disable_org_policies.sh
--rwxr-xr-x   0        0        0      990 2023-07-31 19:26:06.169251 solutions_builder-1.17.9/solutions_builder/template_root/utils/init_env_vars.sh
--rw-r--r--   0        0        0       81 2023-07-31 15:22:50.658645 solutions_builder-1.17.9/solutions_builder/template_root/{{_copier_conf.answers_file}}
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.658746 solutions_builder-1.17.9/solutions_builder/tests/__init__.py
--rw-r--r--   0        0        0     6376 1970-01-01 00:00:00.000000 solutions_builder-1.17.9/PKG-INFO
+-rw-r--r--   0        0        0    11358 2022-06-28 21:05:37.723277 solutions_builder-1.18.0/LICENSE
+-rw-r--r--   0        0        0     5636 2024-04-14 21:46:23.164280 solutions_builder-1.18.0/README.md
+-rw-r--r--   0        0        0     1148 2024-04-14 20:49:54.057476 solutions_builder-1.18.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.724132 solutions_builder-1.18.0/solutions_builder/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.730627 solutions_builder-1.18.0/solutions_builder/cli/__init__.py
+-rw-r--r--   0        0        0    10056 2024-04-14 21:44:15.880745 solutions_builder-1.18.0/solutions_builder/cli/cli.py
+-rw-r--r--   0        0        0      773 2024-03-25 03:04:07.741379 solutions_builder-1.18.0/solutions_builder/cli/cli_constants.py
+-rw-r--r--   0        0        0     4810 2024-03-25 03:04:07.748052 solutions_builder-1.18.0/solutions_builder/cli/cli_utils.py
+-rw-r--r--   0        0        0     7362 2024-04-14 21:37:17.430667 solutions_builder-1.18.0/solutions_builder/cli/component.py
+-rw-r--r--   0        0        0     6347 2024-04-14 21:02:16.843261 solutions_builder-1.18.0/solutions_builder/cli/infra.py
+-rw-r--r--   0        0        0     2567 2024-04-14 21:02:48.815027 solutions_builder-1.18.0/solutions_builder/cli/set.py
+-rw-r--r--   0        0        0     1429 2024-04-14 21:03:11.981839 solutions_builder-1.18.0/solutions_builder/cli/template.py
+-rw-r--r--   0        0        0     5828 2024-04-14 21:03:17.359957 solutions_builder-1.18.0/solutions_builder/cli/vars.py
+-rw-r--r--   0        0        0     3942 2024-03-25 03:04:07.751131 solutions_builder-1.18.0/solutions_builder/cli/vars_test.py
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.752671 solutions_builder-1.18.0/solutions_builder/copier_extensions/__init__.py
+-rw-r--r--   0        0        0     1563 2024-03-25 03:04:07.756910 solutions_builder-1.18.0/solutions_builder/copier_extensions/context.py
+-rw-r--r--   0        0        0     6126 2024-03-25 03:04:07.757820 solutions_builder-1.18.0/solutions_builder/copier_extensions/sb_helpers.py
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.760026 solutions_builder-1.18.0/solutions_builder/fragments/skaffold_template/copier.yaml
+-rw-r--r--   0        0        0      101 2024-03-25 03:04:07.760859 solutions_builder-1.18.0/solutions_builder/module_template/.st/module_answers/{{'{{component_name}}'}}.yaml
+-rw-r--r--   0        0        0      766 2024-03-25 03:04:07.761736 solutions_builder-1.18.0/solutions_builder/module_template/README.md
+-rw-r--r--   0        0        0      865 2024-03-25 03:04:07.762000 solutions_builder-1.18.0/solutions_builder/module_template/copier.yaml
+-rw-r--r--   0        0        0       89 2024-03-25 03:04:07.762719 solutions_builder-1.18.0/solutions_builder/module_template/docs/components/{{'{{component_name}}'}}.md
+-rw-r--r--   0        0        0     1135 2024-03-25 03:04:07.763039 solutions_builder-1.18.0/solutions_builder/module_template/template_copier.yaml
+-rw-r--r--   0        0        0     3878 2024-03-25 03:04:07.765629 solutions_builder-1.18.0/solutions_builder/module_template/{{"{{'.github' if use_github_action}}"}}/workflows/{{"unit_test_linter_{{component_name}}"}}.yaml
+-rw-r--r--   0        0        0      566 2024-03-25 03:04:07.767359 solutions_builder-1.18.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/Dockerfile
+-rw-r--r--   0        0        0      109 2024-03-25 03:04:07.767845 solutions_builder-1.18.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/requirements.txt
+-rw-r--r--   0        0        0     3204 2024-03-25 03:04:07.768208 solutions_builder-1.18.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/skaffold.yaml
+-rw-r--r--   0        0        0      590 2024-03-25 03:04:07.768754 solutions_builder-1.18.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/src/main.py
+-rw-r--r--   0        0        0       81 2024-03-25 03:04:07.769062 solutions_builder-1.18.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/st_module.yaml
+-rw-r--r--   0        0        0      736 2024-03-25 03:04:07.771134 solutions_builder-1.18.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/backend.tf
+-rw-r--r--   0        0        0      636 2024-03-25 03:04:07.771582 solutions_builder-1.18.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/main.tf
+-rw-r--r--   0        0        0      836 2024-03-25 03:04:07.772094 solutions_builder-1.18.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/providers.tf
+-rw-r--r--   0        0        0      777 2024-03-25 03:04:07.772440 solutions_builder-1.18.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/terraform.tfvars
+-rw-r--r--   0        0        0      858 2024-03-25 03:04:07.772726 solutions_builder-1.18.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/variables.tf
+-rw-r--r--   0        0        0       80 2024-03-25 03:04:07.775721 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/.sb/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0      545 2024-03-25 03:04:07.777691 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/Dockerfile
+-rw-r--r--   0        0        0     1300 2024-03-25 03:04:07.778047 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/README.md
+-rw-r--r--   0        0        0       77 2024-03-25 03:04:07.778421 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/requirements-test.txt
+-rw-r--r--   0        0        0       98 2024-03-25 03:04:07.778741 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/requirements.txt
+-rw-r--r--   0        0        0     2974 2024-03-25 03:04:07.779722 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/skaffold.yaml
+-rw-r--r--   0        0        0     1610 2024-04-14 20:43:56.364650 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/src/main.py
+-rw-r--r--   0        0        0      903 2024-03-25 03:04:07.780746 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/src/routes/sample.py
+-rw-r--r--   0        0        0     1232 2024-03-25 03:04:07.781845 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml
+-rw-r--r--   0        0        0      197 2024-03-25 03:04:07.782124 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/kustomization.yaml
+-rw-r--r--   0        0        0       60 2024-03-25 03:04:07.783108 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/properties.env
+-rw-r--r--   0        0        0      229 2024-03-25 03:04:07.783376 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/service.yaml
+-rw-r--r--   0        0        0      421 2024-03-25 03:04:07.783937 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/hpa.yaml
+-rw-r--r--   0        0        0      103 2024-03-25 03:04:07.784849 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/kustomization.yaml
+-rw-r--r--   0        0        0      215 2024-03-25 03:04:07.785391 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'manifests' if deploy_cloudrun else ''}}/cloudrun-service.yaml
+-rw-r--r--   0        0        0       92 2024-03-25 03:04:07.785799 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/skaffold.yaml.patch
+-rw-r--r--   0        0        0     2095 2024-03-25 03:04:07.786572 solutions_builder-1.18.0/solutions_builder/modules/blank_service/copier.yaml
+-rw-r--r--   0        0        0       80 2024-03-25 03:04:07.787312 solutions_builder-1.18.0/solutions_builder/modules/restful_service/.sb/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     1363 2024-03-25 03:04:07.787571 solutions_builder-1.18.0/solutions_builder/modules/restful_service/README.md
+-rw-r--r--   0        0        0      545 2024-03-25 03:04:07.788965 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/Dockerfile
+-rw-r--r--   0        0        0     1309 2024-03-25 03:04:07.789227 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/README.md
+-rw-r--r--   0        0        0       77 2024-03-25 03:04:07.789564 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/requirements-test.txt
+-rw-r--r--   0        0        0       98 2024-03-25 03:04:07.789873 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/requirements.txt
+-rw-r--r--   0        0        0     2974 2024-03-25 03:04:07.790203 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/skaffold.yaml
+-rw-r--r--   0        0        0      862 2024-03-25 03:04:07.791788 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/config.py
+-rw-r--r--   0        0        0     1711 2024-03-25 03:04:07.792135 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/main.py
+-rw-r--r--   0        0        0     1725 2024-04-14 20:43:56.364892 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.793877 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/__init__.py
+-rw-r--r--   0        0        0     3876 2024-03-25 03:04:07.796299 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py
+-rw-r--r--   0        0        0     1222 2024-03-25 03:04:07.796775 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.797162 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/utils/__init__.py
+-rw-r--r--   0        0        0     1232 2024-03-25 03:04:07.797870 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml
+-rw-r--r--   0        0        0      197 2024-03-25 03:04:07.798184 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/kustomization.yaml
+-rw-r--r--   0        0        0       60 2024-03-25 03:04:07.798460 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/properties.env
+-rw-r--r--   0        0        0      229 2024-03-25 03:04:07.798769 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/service.yaml
+-rw-r--r--   0        0        0      421 2024-03-25 03:04:07.799347 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/hpa.yaml
+-rw-r--r--   0        0        0      103 2024-03-25 03:04:07.799631 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/kustomization.yaml
+-rw-r--r--   0        0        0      215 2024-03-25 03:04:07.800125 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'manifests' if deploy_cloudrun else ''}}/cloudrun-service.yaml
+-rw-r--r--   0        0        0     2305 2024-03-25 03:04:07.803460 solutions_builder-1.18.0/solutions_builder/modules/restful_service/copier.yaml
+-rw-r--r--   0        0        0      120 2024-03-25 03:04:07.804550 solutions_builder-1.18.0/solutions_builder/modules/restful_service/docs/components/{{component_name}}.md
+-rw-r--r--   0        0        0       92 2024-03-25 03:04:07.804816 solutions_builder-1.18.0/solutions_builder/modules/restful_service/skaffold.yaml.patch
+-rw-r--r--   0        0        0      263 2024-03-25 03:04:07.806500 solutions_builder-1.18.0/solutions_builder/modules/restful_service/terraform/stages/{{'3-httplb-cloudrun' if cloudrun_neg}}/{{component_name}}_neg.tf
+-rw-r--r--   0        0        0     3223 2024-03-25 03:04:07.808817 solutions_builder-1.18.0/solutions_builder/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py
+-rw-r--r--   0        0        0     3269 2024-03-25 03:04:07.809387 solutions_builder-1.18.0/solutions_builder/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
+-rw-r--r--   0        0        0       80 2024-03-25 03:04:07.811569 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/.sb/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     1572 2024-03-25 03:04:07.811814 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/README.md
+-rw-r--r--   0        0        0      545 2024-03-25 03:04:07.813321 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/Dockerfile
+-rw-r--r--   0        0        0      215 2024-03-25 03:04:07.813936 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/manifests/cloudrun-service.yaml
+-rw-r--r--   0        0        0       77 2024-03-25 03:04:07.814203 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/requirements-test.txt
+-rw-r--r--   0        0        0      143 2024-03-25 03:04:07.814453 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/requirements.txt
+-rw-r--r--   0        0        0     3193 2024-03-25 03:04:07.814770 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/skaffold.yaml
+-rw-r--r--   0        0        0      942 2024-03-25 03:04:07.816878 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/config.py
+-rw-r--r--   0        0        0     1751 2024-03-25 03:04:07.817133 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/main.py
+-rw-r--r--   0        0        0     1550 2024-03-25 03:04:07.818717 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/models/task.py
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.819395 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/__init__.py
+-rw-r--r--   0        0        0     5195 2024-03-25 03:04:07.822303 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/tasks.py
+-rw-r--r--   0        0        0     1196 2024-03-25 03:04:07.823423 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/schemas/task.py
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.823723 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.824495 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/__init__.py
+-rw-r--r--   0        0        0      430 2024-03-25 03:04:07.825744 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/example.yaml
+-rw-r--r--   0        0        0     1348 2024-03-25 03:04:07.827789 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow.py
+-rw-r--r--   0        0        0     1138 2024-03-25 03:04:07.828088 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow_test.py
+-rw-r--r--   0        0        0     1232 2024-03-25 03:04:07.828856 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/deployment.yaml
+-rw-r--r--   0        0        0      197 2024-03-25 03:04:07.829109 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/kustomization.yaml
+-rw-r--r--   0        0        0       97 2024-03-25 03:04:07.829359 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/properties.env
+-rw-r--r--   0        0        0      229 2024-03-25 03:04:07.829594 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/service.yaml
+-rw-r--r--   0        0        0      421 2024-03-25 03:04:07.829956 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/hpa/hpa.yaml
+-rw-r--r--   0        0        0      103 2024-03-25 03:04:07.830168 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/hpa/kustomization.yaml
+-rw-r--r--   0        0        0     2667 2024-03-25 03:04:07.830370 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/copier.yaml
+-rw-r--r--   0        0        0       71 2024-03-25 03:04:07.830981 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/docs/components/{{component_name}}.md
+-rw-r--r--   0        0        0       92 2024-03-25 03:04:07.831165 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/skaffold.yaml.patch
+-rw-r--r--   0        0        0      719 2024-03-25 03:04:07.833442 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/backend.tf
+-rw-r--r--   0        0        0     2693 2024-03-25 03:04:07.833738 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/main.tf
+-rw-r--r--   0        0        0      930 2024-03-25 03:04:07.834108 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/providers.tf
+-rw-r--r--   0        0        0     1320 2024-03-25 03:04:07.834369 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/terraform.tfvars
+-rw-r--r--   0        0        0     2076 2024-03-25 03:04:07.834641 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/variables.tf
+-rw-r--r--   0        0        0     3851 2024-03-25 03:04:07.835330 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
+-rw-r--r--   0        0        0       80 2024-03-25 03:04:07.836211 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/.sb/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     1374 2024-03-25 03:04:07.836431 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/copier.yaml
+-rw-r--r--   0        0        0      784 2024-03-25 03:04:07.837033 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/docs/components/{{component_name}}.md
+-rw-r--r--   0        0        0      763 2024-03-25 03:04:07.837791 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/backend.tf
+-rw-r--r--   0        0        0     1568 2024-03-25 03:04:07.838178 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/iam.tf
+-rw-r--r--   0        0        0     2486 2024-03-25 03:04:07.838410 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/main.tf
+-rw-r--r--   0        0        0     1783 2024-03-25 03:04:07.838671 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/providers.tf
+-rw-r--r--   0        0        0      308 2024-03-25 03:04:07.838982 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/terraform.tfvars
+-rw-r--r--   0        0        0     1553 2024-03-25 03:04:07.839201 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/variables.tf
+-rw-r--r--   0        0        0       80 2024-03-25 03:04:07.839951 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/.sb/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0      946 2024-03-25 03:04:07.840151 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/copier.yaml
+-rw-r--r--   0        0        0      650 2024-03-25 03:04:07.840804 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/docs/components/{{component_name}}.md
+-rw-r--r--   0        0        0      763 2024-03-25 03:04:07.841462 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/backend.tf
+-rw-r--r--   0        0        0     1490 2024-03-25 03:04:07.841826 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/main.tf
+-rw-r--r--   0        0        0     1002 2024-03-25 03:04:07.842816 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/providers.tf
+-rw-r--r--   0        0        0      138 2024-03-25 03:04:07.843058 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/terraform.tfvars
+-rw-r--r--   0        0        0     1140 2024-03-25 03:04:07.843413 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/variables.tf
+-rw-r--r--   0        0        0       80 2024-03-25 03:04:07.845118 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/.sb/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     2396 2024-03-25 03:04:07.845466 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/copier.yaml
+-rw-r--r--   0        0        0      181 2024-03-25 03:04:07.846354 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/frontend_config.yaml
+-rw-r--r--   0        0        0      658 2024-03-25 03:04:07.846642 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/ingress.yaml
+-rw-r--r--   0        0        0      145 2024-03-25 03:04:07.846979 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/kustomization.yaml
+-rw-r--r--   0        0        0      225 2024-03-25 03:04:07.847261 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/managed_cert.yaml
+-rw-r--r--   0        0        0      378 2024-03-25 03:04:07.852866 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/ingress/skaffold.yaml
+-rw-r--r--   0        0        0       59 2024-03-25 03:04:07.853875 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/skaffold.yaml.patch
+-rw-r--r--   0        0        0     1695 2024-03-25 03:04:07.858750 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/main.tf
+-rw-r--r--   0        0        0      670 2024-03-25 03:04:07.859082 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/outputs.tf
+-rw-r--r--   0        0        0     1264 2024-03-25 03:04:07.860615 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/variables.tf
+-rw-r--r--   0        0        0      752 2024-04-14 20:43:56.365155 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/backend.tf
+-rw-r--r--   0        0        0     1568 2024-03-25 03:04:07.861621 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/iam.tf
+-rw-r--r--   0        0        0     1695 2024-03-25 03:04:07.861857 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/main.tf
+-rw-r--r--   0        0        0     1877 2024-03-25 03:04:07.862898 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/providers.tf
+-rw-r--r--   0        0        0      520 2024-03-25 03:04:07.863221 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/terraform.tfvars
+-rw-r--r--   0        0        0     1802 2024-03-25 03:04:07.863461 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/variables.tf
+-rw-r--r--   0        0        0       80 2024-03-25 03:04:07.864843 solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/.sb/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     1048 2024-03-25 03:04:07.865072 solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/copier.yaml
+-rw-r--r--   0        0        0      877 2024-04-14 20:43:56.365414 solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf
+-rw-r--r--   0        0        0     2760 2024-03-25 03:04:07.866341 solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf
+-rw-r--r--   0        0        0      670 2024-03-25 03:04:07.866546 solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf
+-rw-r--r--   0        0        0     1298 2024-03-25 03:04:07.866888 solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf
+-rw-r--r--   0        0        0       81 2024-03-25 03:04:07.867470 solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/st_module.yaml
+-rw-r--r--   0        0        0      236 2024-03-25 03:04:07.867794 solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/terraform.tfvars
+-rw-r--r--   0        0        0     1984 2024-03-25 03:04:07.868153 solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf
+-rw-r--r--   0        0        0       90 2024-03-25 03:04:07.868658 solutions_builder-1.18.0/solutions_builder/requirements.txt
+-rw-r--r--   0        0        0    68957 2024-03-25 03:04:07.870229 solutions_builder-1.18.0/solutions_builder/template_root/.github/assets/setup_local.png
+-rw-r--r--   0        0        0   239307 2024-03-25 03:04:07.870988 solutions_builder-1.18.0/solutions_builder/template_root/.github/assets/skaffold_dev_terminal.png
+-rw-r--r--   0        0        0     2637 2024-03-25 03:04:07.871475 solutions_builder-1.18.0/solutions_builder/template_root/.github/workflows/deployment_cloudrun_dev.yaml
+-rw-r--r--   0        0        0     2688 2024-03-25 03:04:07.871683 solutions_builder-1.18.0/solutions_builder/template_root/.github/workflows/deployment_gke_dev.yaml
+-rw-r--r--   0        0        0     5784 2024-03-25 03:04:07.872126 solutions_builder-1.18.0/solutions_builder/template_root/.github/workflows/e2e_cloudrun_api_test.yaml
+-rw-r--r--   0        0        0     8047 2024-03-25 03:04:07.874328 solutions_builder-1.18.0/solutions_builder/template_root/.github/workflows/e2e_gke_api_test.yaml
+-rw-r--r--   0        0        0     3129 2024-03-25 03:04:07.874720 solutions_builder-1.18.0/solutions_builder/template_root/.github/workflows/unit_test_linter_common.yaml
+-rw-r--r--   0        0        0      471 2024-03-25 03:04:07.875041 solutions_builder-1.18.0/solutions_builder/template_root/.gitignore
+-rw-r--r--   0        0        0    14552 2024-03-25 03:04:07.876082 solutions_builder-1.18.0/solutions_builder/template_root/.pylintrc
+-rw-r--r--   0        0        0     4878 2024-03-25 03:04:07.876530 solutions_builder-1.18.0/solutions_builder/template_root/README.md
+-rw-r--r--   0        0        0      398 2024-03-25 03:04:07.876998 solutions_builder-1.18.0/solutions_builder/template_root/components/README.md
+-rw-r--r--   0        0        0      893 2024-03-25 03:04:07.877867 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile
+-rw-r--r--   0        0        0     1101 2024-03-25 03:04:07.878112 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile.unittest
+-rw-r--r--   0        0        0      111 2024-03-25 03:04:07.878424 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/requirements-test.txt
+-rw-r--r--   0        0        0      240 2024-03-25 03:04:07.878829 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/requirements.txt
+-rw-r--r--   0        0        0      571 2024-03-25 03:04:07.879408 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/skaffold.yaml
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.880848 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/__init__.py
+-rw-r--r--   0        0        0      831 2024-03-25 03:04:07.881462 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/config.py
+-rw-r--r--   0        0        0      695 2024-03-25 03:04:07.881658 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/db_client.py
+-rw-r--r--   0        0        0       35 2024-03-25 03:04:07.882687 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/README.md
+-rw-r--r--   0        0        0       91 2024-03-25 03:04:07.882932 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/__init__.py
+-rw-r--r--   0        0        0     1376 2024-03-25 03:04:07.884644 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/example.py
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.885395 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/__init__.py
+-rw-r--r--   0        0        0      754 2024-03-25 03:04:07.887849 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/bq_client_fixture.py
+-rw-r--r--   0        0        0     1006 2024-03-25 03:04:07.888076 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/client_with_emulator.py
+-rw-r--r--   0        0        0     2243 2024-03-25 03:04:07.888314 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/firestore_emulator.py
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.889468 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/__init__.py
+-rw-r--r--   0        0        0     1002 2024-03-25 03:04:07.891212 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/logging_handler.py
+-rw-r--r--   0        0        0     2500 2024-03-25 03:04:07.891459 solutions_builder-1.18.0/solutions_builder/template_root/copier.yaml
+-rw-r--r--   0        0        0       97 2024-03-25 03:04:07.891699 solutions_builder-1.18.0/solutions_builder/template_root/firebase.json
+-rw-r--r--   0        0        0      484 2024-04-14 21:44:49.817394 solutions_builder-1.18.0/solutions_builder/template_root/sb.yaml
+-rw-r--r--   0        0        0       98 2024-03-25 03:04:07.892621 solutions_builder-1.18.0/solutions_builder/template_root/setup.cfg
+-rw-r--r--   0        0        0      215 2024-03-25 03:04:07.893127 solutions_builder-1.18.0/solutions_builder/template_root/skaffold.yaml
+-rw-r--r--   0        0        0      921 2024-03-25 03:04:07.894470 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/cloudbuild/main.tf
+-rw-r--r--   0        0        0      730 2024-03-25 03:04:07.894809 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/cloudbuild/variables.tf
+-rw-r--r--   0        0        0     3585 2024-03-25 03:04:07.895330 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/cloudrun/main.tf
+-rw-r--r--   0        0        0     1178 2024-03-25 03:04:07.895611 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/cloudrun/variables.tf
+-rw-r--r--   0        0        0     5024 2024-03-25 03:04:07.896165 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/compute_backend/main.tf
+-rw-r--r--   0        0        0      190 2024-03-25 03:04:07.896402 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/compute_backend/outputs.tf
+-rw-r--r--   0        0        0     1186 2024-03-25 03:04:07.896659 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/compute_backend/providers.tf
+-rw-r--r--   0        0        0     1601 2024-03-25 03:04:07.896925 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/compute_backend/variables.tf
+-rw-r--r--   0        0        0     2364 2024-03-25 03:04:07.897379 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/firebase/main.tf
+-rw-r--r--   0        0        0     1194 2024-03-25 03:04:07.897631 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/firebase/variables.tf
+-rw-r--r--   0        0        0     3868 2024-03-25 03:04:07.898055 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/gke/main.tf
+-rw-r--r--   0        0        0      832 2024-03-25 03:04:07.898338 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/gke/outputs.tf
+-rw-r--r--   0        0        0     3453 2024-03-25 03:04:07.898588 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/gke/variables.tf
+-rw-r--r--   0        0        0     3012 2024-03-25 03:04:07.899082 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/ingress_nginx/main.tf
+-rw-r--r--   0        0        0      692 2024-03-25 03:04:07.899396 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/ingress_nginx/outputs.tf
+-rw-r--r--   0        0        0     1087 2024-03-25 03:04:07.899720 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/ingress_nginx/variables.tf
+-rw-r--r--   0        0        0      827 2024-03-25 03:04:07.900599 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/project_services/main.tf
+-rw-r--r--   0        0        0      774 2024-03-25 03:04:07.900949 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/project_services/variables.tf
+-rw-r--r--   0        0        0      953 2024-03-25 03:04:07.901558 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/service_account/main.tf
+-rw-r--r--   0        0        0     1037 2024-03-25 03:04:07.902536 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/service_account/variables.tf
+-rw-r--r--   0        0        0     1529 2024-03-25 03:04:07.905914 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/terraform_cicd/main.tf
+-rw-r--r--   0        0        0      678 2024-03-25 03:04:07.906314 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/terraform_cicd/variables.tf
+-rw-r--r--   0        0        0     1333 2024-03-25 03:04:07.906938 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/vpc_network/main.tf
+-rw-r--r--   0        0        0     1269 2024-03-25 03:04:07.907328 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/vpc_network/variables.tf
+-rw-r--r--   0        0        0     2561 2024-03-25 03:04:07.908063 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/0-jumphost/bastion_startup.sh
+-rw-r--r--   0        0        0     3593 2024-03-25 03:04:07.909125 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/0-jumphost/main.tf
+-rw-r--r--   0        0        0      178 2024-03-25 03:04:07.909456 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/0-jumphost/terraform.tfvars
+-rw-r--r--   0        0        0      782 2024-03-25 03:04:07.910038 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/0-jumphost/variables.tf
+-rw-r--r--   0        0        0     2873 2024-03-25 03:04:07.910583 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/1-bootstrap/main.tf
+-rw-r--r--   0        0        0      730 2024-03-25 03:04:07.910858 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/1-bootstrap/output.tf
+-rw-r--r--   0        0        0       86 2024-03-25 03:04:07.911144 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/1-bootstrap/terraform.tfvars
+-rw-r--r--   0        0        0     1071 2024-03-25 03:04:07.911400 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/1-bootstrap/variables.tf
+-rw-r--r--   0        0        0      869 2024-04-14 20:43:56.365662 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/backend.tf
+-rw-r--r--   0        0        0     1669 2024-03-25 03:04:07.912198 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/firestore_setup.tf
+-rw-r--r--   0        0        0     1568 2024-03-25 03:04:07.912485 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/iam.tf
+-rw-r--r--   0        0        0     1032 2024-03-25 03:04:07.912743 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/identity_platform.tf
+-rw-r--r--   0        0        0     4602 2024-03-25 03:04:07.913103 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/main.tf
+-rw-r--r--   0        0        0      991 2024-03-25 03:04:07.913405 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/outputs.tf
+-rw-r--r--   0        0        0      921 2024-03-25 03:04:07.913735 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/providers.tf
+-rw-r--r--   0        0        0      724 2024-03-25 03:04:07.914076 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/terraform.tfvars
+-rw-r--r--   0        0        0     2839 2024-03-25 03:04:07.914408 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/variables.tf
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.914895 solutions_builder-1.18.0/solutions_builder/template_root/tests/__init__.py
+-rw-r--r--   0        0        0     1386 2024-03-25 03:04:07.915482 solutions_builder-1.18.0/solutions_builder/template_root/tests/e2e/e2e_utils.py
+-rwxr-xr-x   0        0        0      952 2024-03-25 03:04:07.915993 solutions_builder-1.18.0/solutions_builder/template_root/utils/disable_org_policies.sh
+-rwxr-xr-x   0        0        0      990 2024-03-25 03:04:07.916378 solutions_builder-1.18.0/solutions_builder/template_root/utils/init_env_vars.sh
+-rwxr-xr-x   0        0        0     1845 2024-03-25 03:04:07.917312 solutions_builder-1.18.0/solutions_builder/template_root/utils/setup_ksa.sh
+-rw-r--r--   0        0        0       81 2024-03-25 03:04:07.917579 solutions_builder-1.18.0/solutions_builder/template_root/{{_copier_conf.answers_file}}
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.917901 solutions_builder-1.18.0/solutions_builder/tests/__init__.py
+-rw-r--r--   0        0        0     6730 1970-01-01 00:00:00.000000 solutions_builder-1.18.0/PKG-INFO
```

### Comparing `solutions_builder-1.17.9/LICENSE` & `solutions_builder-1.18.0/LICENSE`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/README.md` & `solutions_builder-1.18.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,148 +6,171 @@
 ## TL;DR
 
 Solutions Builder is a boilerplate template for building repeatable
 solutions with the best practices in architecture on Google Cloud, including GKE
 clusters, Cloud Run, Test Automation, CI/CD, as well as development process.
 
 This template provides built-in and ready-to-ship modules including:
-* Easy-to-deploy [Terraform](https://www.terraform.io/) boilerplate modules
-* Container-based microservices, can be deployed to a Kubernetes cluster or Cloud Run.
-* Unified deployment using Skaffold.
-* Automatically generated API documentation with Swagger UI.
-* CI/CD deployment (with Github Actions).
-* Cloud Run templates.
+
+- Easy-to-deploy [Terraform](https://www.terraform.io/) boilerplate modules
+- Container-based microservices, can be deployed to a Kubernetes cluster or Cloud Run.
+- Unified deployment using Skaffold.
+- Automatically generated API documentation with Swagger UI.
+- CI/CD deployment (with GitHub Actions).
+- Cloud Run templates.
 
 ## Roadmap
 
-Please see [Feature Requests in the Github issue list](https://github.com/GoogleCloudPlatform/solutions-builder/issues?q=is%3Aopen+is%3Aissue+label%3A%22feature+request%22).
+Please see [Feature Requests in the GitHub issue list](https://github.com/GoogleCloudPlatform/solutions-builder/issues?q=is%3Aopen+is%3Aissue+label%3A%22feature+request%22).
 
 ## Prerequisite
 
-| Tool | Required Version | Installation |
-|---|---|---|
-| Python     | &gt;= 3.9     | |
-| gcloud CLI | Latest        | https://cloud.google.com/sdk/docs/install |
-| Terraform  | &gt;= v1.3.7  | https://developer.hashicorp.com/terraform/downloads |
-| Skaffold   | &gt;= v2.4.0  | https://skaffold.dev/docs/install/ |
+| Tool       | Required Version | Installation                                        |
+| ---------- | ---------------- | --------------------------------------------------- |
+| Python     | &gt;= 3.11       |                                                     |
+| gcloud CLI | Latest           | https://cloud.google.com/sdk/docs/install           |
+| Terraform  | &gt;= v1.3.7     | https://developer.hashicorp.com/terraform/downloads |
+| Skaffold   | &gt;= v2.4.0     | https://skaffold.dev/docs/install/                  |
 
 [Optional] If you plan to deploy services on a GKE cluster, please install the following:
 
-| Tool | Required Version | Installation |
-|---|---|---|
-| Kustomize   | &gt;= v5.0.0 | https://kubectl.docs.kubernetes.io/installation/kustomize/ |
+| Tool      | Required Version | Installation                                               |
+| --------- | ---------------- | ---------------------------------------------------------- |
+| Kustomize | &gt;= v5.0.0     | https://kubectl.docs.kubernetes.io/installation/kustomize/ |
 
 ## Installing Solutions Builder CLI
 
 With `pip`:
+
 ```
 pip install solutions-builder
 ```
 
 With `pipx`:
+
 ```
 pip install --user pipx
 pipx install solutions-builder
 ```
 
 ## Quick Start
 
 This quick start steps will do the following:
+
 - Create a new GCP project and initialize Cloud foundation.
 - Add a RESTful API service for managing Todo list.
 - Deploy the service to Cloud Run.
 
 Set up GCP project
+
 ```
 export PROJECT_ID=my-solution-gcp-id
 
 # (Optional) Create a new GCP project. You can also use an existing GCP project.
 gcloud projects create $PROJECT_ID
 
 # Set gcloud CLI to the GCP project.
 gcloud config set project $PROJECT_ID
 ```
 
 Generate a new solution folder.
+
 ```
 sb new my-solution
 ```
 
 This will prompt options and variables:
+
 ```
 🎤 What is your project name? (Spaces are allowed.)
    my-solution
 🎤 What is your Google Cloud project ID?
    my-solution-gcp-id
 🎤 What is your Google Cloud project number?
    12345678
 🎤 Which Google Cloud region?
    us-central1
 🎤 Use GCS Bucket for Terraform backend?
    Yes
 ```
 
 Go to the newly created project folder
+
 ```
 cd my-solution
 sb infra apply 1-bootstrap
 ```
 
 Initialize Cloud infrastructure
+
 - Option 1: (Recommended) Log in to the jump host and run the following command(s) in the solution folder.
 - Option 2: Run the following commands in your local machine.
+
 ```
 sb infra apply 2-foundation
 ```
 
 Add a RESTful API service with **Todo** data model to this solution.
+
 ```
-sb components add restful_service
+sb components add -t restful_service todo_service
 ```
 
 Fill details in the prompt:
+
 - Component name: **todo_service**
 - Resource name: **todo-service**
 - Relative path: **todo-service**
 - GCP region: **us-central1**
 - Data model name: **todo**
 - Add Cloud Run to deployment methods: **yes**
 - Create network endpoint group (NEG) for serverless ingress: **yes**
 - Default deploy method? (cloudrun or gke): **Cloud Run**
 
-Add a HTTP Load Balancer for Cloud Run service(s)
+Add an HTTP Load Balancer for Cloud Run service(s)
+
 ```
-sb add component terraform_httplb_cloudrun
+sb components add -t terraform_httplb_cloudrun terraform_httplb_cloudrun
 sb infra apply 3-httplb-cloudrun
 ```
 
 Build and deploy
+
 ```
 sb deploy
 ```
+
 - See other deployment options in [solutions_builder/modules](solutions_builder/modules).
 
+## CLI Usage
+
+For more information on how to use the CLI, please refer to the [CLI_USAGE.md](docs/CLI_USAGE.md).
 
 ## Additional Documentations
 
 You can find more documentations in [docs](docs) folder. In a nutshell, it covers the following:
+
 - [INSTALLATION.md](docs/INSTALLATION.md) - The overall installation guide.
 - [DEVELOPMENT.md](docs/DEVELOPMENT.md) - Development guide and code submission process.
 - [TROUBLESHOOTING.md](docs/TROUBLESHOOTING.md) - Development guide and code submission process.
 
-In the [docs/components](docs/components/) folder, it contains a few more guidance based on each component/feature available in this template.
-- [gke.md](docs/components/gke.md) covers the overall developmeng guidance on Google Kubernetes Engine.
+In the [docs/components](docs/components) folder, it contains a few more guidance based on each component/feature available in this template.
+
+- [gke.md](docs/components/gke.md) covers the overall development guidance on Google Kubernetes Engine.
 - [cloudrun.md](docs/components/cloudrun.md) covers the guidance if you want to deploy microservice to Cloud Run.
 
 ## FAQ
+
 - Who are the target audience/users for this Solutions Builder?
+
   - A: Any engineering team to start a new solution development project.
 
 - Can I choose to deploy microservice just to Cloud Run?
-  - A: Yes, please refer to [Setting up Google Cloud Project](README.md#setting-up-google-cloud-project) in this README.md to choose where to deploy microservices. Or you can refer to [INSTALLATION.md](docs/INSTALLATION.md) for more details.
+
+  - A: Yes, please refer to [INSTALLATION Guide](docs/INSTALLATION.md) for more details.
 
 - Can I use this template for non-Google or multi-Cloud environments?
-  - A: We design this Solutions Builder to work 100% out of the box with Google Cloud products. However you could customize the solution to meet your needs on multi-Cloud environment. See [Why Google Cloud](https://cloud.google.com/why-google-cloud) for details.
+  - A: We design this Solutions Builder to work 100% out of the box with Google Cloud products. However, you could customize the solution to meet your needs on multi-Cloud environment. See [Why Google Cloud](https://cloud.google.com/why-google-cloud) for details.
 
 ## Troubleshoot
 
-See [TROUBLESHOOTING.md](docs/TROUBLESHOOTING.md) for details.
+See [TROUBLESHOOTING Guide](docs/TROUBLESHOOTING.md) for details.
```

### Comparing `solutions_builder-1.17.9/pyproject.toml` & `solutions_builder-1.18.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solutions-builder"
-version = "1.17.9"
+version = "1.18.0"
 description = "A solution framework to generate a project with built-in structure and modules"
 authors = ["Jon Chen <jonchen@google.com>"]
 license = "Apache"
 readme = "README.md"
 homepage = "https://github.com/GoogleCloudPlatform/solutions-builder"
 repository = "https://github.com/GoogleCloudPlatform/solutions-builder"
 packages = [
@@ -15,32 +15,32 @@
   "**/.terraform/**/*",
   "**/.terraform/providers/**/*",
   "**/.terraform.lock.hcl",
   "**/__pycache__/**/*"
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
-copier = "^7.2.0"
+python = ">=3.9,<4.0"
+copier = ">=9.2.0"
 pyyaml = "^6.0"
-typer = "^0.9.0"
+typer = ">=0.9.0"
 jinja2-time = "^0.2.0"
 copier-templates-extensions = "^0.3.0"
 pathlib = "^1.0.1"
 jinja2 = "^3.1.2"
 jinja2-strcase = "^0.0.2"
-pydantic = "<=1.10.12"
+pydantic = ">=2"
 
 [tool.poetry.group.dev.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.9,<4.0"
 copier-templates-extensions = "^0.3.0"
-copier = "^7.2.0"
+copier = ">=9.2.0"
 PyYAML = "^6.0"
 jinja2-time = "^0.2.0"
-typer = "^0.9.0"
+typer = ">=0.9.0"
 
 [tool.poetry.scripts]
 sb = "solutions_builder.cli.cli:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `solutions_builder-1.17.9/solutions_builder/cli/cli.py` & `solutions_builder-1.18.0/solutions_builder/cli/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,32 +10,35 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import typer, traceback, os
+import typer
+import traceback
+import os
 import importlib.metadata
 from typing import Optional
 from typing_extensions import Annotated
-from copier import run_auto
-from .component import component_app
+from copier import run_copy
+from .component import component_app, list as components_list
 from .infra import infra_app
 from .template import template_app
-from .set import set_app
+from .set import set_app, project_id as set_project_id
+from .vars import vars_app
 from .cli_utils import *
+from .cli_constants import DEBUG, PLACEHOLDER_VALUES
 
 __version__ = importlib.metadata.version("solutions-builder")
 DEFAULT_DEPLOY_PROFILE = "default-deploy"
 
 app = typer.Typer(
     add_completion=False,
-    help=
-    "Solutions Builder CLI. See https://github.com/GoogleCloudPlatform/solutions-builder for details."
+    help="Solutions Builder CLI. See https://github.com/GoogleCloudPlatform/solutions-builder for details."
 )
 app.add_typer(component_app,
               name="components",
               help="Add or update components.")
 app.add_typer(component_app,
               name="component",
               help="Add or update components.")
@@ -44,14 +47,17 @@
               help="Manage infrastructure (terraform).")
 app.add_typer(template_app,
               name="template",
               help="Create or update module templates.")
 app.add_typer(set_app,
               name="set",
               help="Set properties to an existing solution folder.")
+app.add_typer(vars_app,
+              name="vars",
+              help="Set variables in an existing solutions-builder folder.")
 
 
 # Create a new solution
 @app.command()
 def new(folder_name,
         output_dir: Annotated[Optional[str], typer.Argument()] = ".",
         template_path=None,
@@ -69,15 +75,15 @@
 
   if os.path.exists(output_path):
     raise FileExistsError(f"Solution folder {output_path} already exists.")
 
   # Copy template_root to destination.
   print(f"template_path = {template_path}")
   answers_dict["folder_name"] = folder_name
-  run_auto(template_path, output_path, data=answers_dict)
+  run_copy(template_path, output_path, data=answers_dict, unsafe=True)
 
   print_success(f"Complete. New solution folder created at {output_path}.\n")
 
 
 # Update a solution
 @app.command()
 def update(solution_path: Annotated[Optional[str],
@@ -90,152 +96,227 @@
     solution_path = "."
 
   validate_solution_folder(solution_path)
 
   if not os.path.exists(solution_path):
     raise FileNotFoundError(f"Solution folder {solution_path} does not exist.")
 
-  confirm(
-      f"\nThis will update solution root folder at '{solution_path}'. Continue?"
-  )
+  confirm_msg = "This will update the current solution folder. Continue?"
+  if solution_path != ".":
+    confirm_msg = "This will update solution root folder at " \
+        "'{solution_path}'. Continue?"
+  confirm(confirm_msg)
 
   # Copy template_root to destination, excluding skaffold.yaml.
   orig_sb_yaml = read_yaml(f"{solution_path}/sb.yaml")
 
   if not template_path:
     current_dir = os.path.dirname(__file__)
     template_path = f"{current_dir}/../template_root"
     if not os.path.exists(template_path):
       raise FileNotFoundError(f"{template_path} does not exist.")
-  worker = run_auto(template_path,
+
+  worker = run_copy(template_path,
                     solution_path,
-                    exclude=["skaffold.yaml", "sb.yaml"])
+                    exclude=["skaffold.yaml", "sb.yaml"],
+                    unsafe=True)
   answers = worker.answers.last
 
   # Restore some fields in sb.yaml.
   sb_yaml = read_yaml(f"{solution_path}/sb.yaml")
   sb_yaml["created_at"] = orig_sb_yaml["created_at"]
   sb_yaml["components"] = orig_sb_yaml["components"]
   write_yaml(f"{solution_path}/sb.yaml", sb_yaml)
 
   print_success(f"Complete. Solution folder updated at {solution_path}.\n")
 
 
 # Build and deploy services.
 @app.command()
-def deploy(profile: str = DEFAULT_DEPLOY_PROFILE,
-           component: str = None,
-           dev: Optional[bool] = False,
-           solution_path: Annotated[Optional[str],
-                                    typer.Argument()] = ".",
-           yes: Optional[bool] = False):
+def deploy(
+        profile: Annotated[str, typer.Option(
+          "--profile", "-p")] = DEFAULT_DEPLOY_PROFILE,
+        component: Annotated[str, typer.Option(
+          "--component", "-c", "-m")] = None,
+        namespace: Annotated[str, typer.Option("--namespace", "-n")] = None,
+        dev: Optional[bool] = False,
+        solution_path: Annotated[Optional[str],
+                                 typer.Argument()] = ".",
+        skaffold_args: Optional[str] = "",
+        yes: Optional[bool] = False):
   """
   Build and deploy services.
   """
   validate_solution_folder(solution_path)
 
   sb_yaml = read_yaml(f"{solution_path}/sb.yaml")
-  project_id = sb_yaml["project_id"]
+  global_variables = sb_yaml.get("global_variables", {})
+
+  # Get project_id from sb.yaml.
+  project_id = global_variables.get("project_id", None)
+  assert project_id, "project_id is not set in 'global_variables' in sb.yaml."
+
+  # Check namespace
+  deploy_config = sb_yaml.get("deploy", {})
+  if deploy_config.get("require_namespace") not in [None, False, ""] \
+          and not namespace:
+    assert namespace, "Please set namespace with --namespace or -n"
+
+  if project_id in PLACEHOLDER_VALUES:
+    project_id = None
+    while not project_id:
+      project_id = input("Please set the GCP project ID: ")
+    print()
+    set_project_id(project_id)
+
+    # Reload sb.yaml
+    sb_yaml = read_yaml(f"{solution_path}/sb.yaml")
+    global_variables = sb_yaml.get("global_variables", {})
+
+  # Get terraform_gke component settings.
   terraform_gke = sb_yaml["components"].get("terraform_gke")
+  env_vars = {
+    "PROJECT_ID": project_id,
+  }
   commands = []
 
   if component:
     component_flag = f" -m {component} "
   else:
     component_flag = ""
 
+  port_forwarding_flag = ""
   if dev:
     skaffold_command = "skaffold dev"
+    port_forwarding_flag = "--port-forward"
   else:
     skaffold_command = "skaffold run"
 
   if terraform_gke:
     cluster_name = terraform_gke["cluster_name"]
     region = terraform_gke["gcp_region"]
     commands.append(
         f"gcloud container clusters get-credentials {cluster_name} --region {region} --project {project_id}"
     )
 
+  # Set Skaffold namespace
+  namespace_flag = f"-n {namespace}" if namespace else ""
+
+  # Add skaffold command.
   commands.append(
-      f"{skaffold_command} -p {profile} {component_flag} --default-repo=\"gcr.io/{project_id}\""
+      f"{skaffold_command} -p {profile} {component_flag} {namespace_flag} --default-repo=\"gcr.io/{project_id}\" {skaffold_args} {port_forwarding_flag}"
   )
-  print("This will build and deploy all services using the command below:")
+  print("This will build and deploy all services using the command "
+        "and variables below:")
   for command in commands:
-    print_highlight(f"- {command}")
-  confirm("\nThis may take a few minutes. Continue?", skip=yes)
+    print_success(f"- {command}")
 
-  for command in commands:
-    exec_shell(command, working_dir=solution_path)
+  namespace_str = namespace or "default"
+  print("\nnamespace:")
+  print_success(f"- {namespace_str}")
+
+  print("\nenvironment variables:")
+  env_var_str = ""
+  for key, value in env_vars.items():
+    print_success(f"- {key}={value}")
+    env_var_str += f"{key}={value} "
+
+  print("\nglobal_variables in sb.yaml:")
+  for key, value in sb_yaml.get("global_variables", {}).items():
+    print_success(f"- {key}: {value}")
 
+  print()
+  confirm("This may take a few minutes. Continue?", skip=yes)
+
+  for command in commands:
+    exec_shell(env_var_str + command, working_dir=solution_path)
 
 # Destory deployment.
+
+
 @app.command()
 def delete(profile: str = DEFAULT_DEPLOY_PROFILE,
-           component: str = None,
+           component: Annotated[str, typer.Option(
+             "--component", "-c", "-m")] = None,
+           namespace: Annotated[str, typer.Option("--namespace", "-n")] = None,
            solution_path: Annotated[Optional[str],
                                     typer.Argument()] = ".",
            yes: Optional[bool] = False):
   """
   Delete deployment.
   """
   validate_solution_folder(solution_path)
 
   sb_yaml = read_yaml(f"{solution_path}/sb.yaml")
-  project_id = sb_yaml["project_id"]
+  global_variables = sb_yaml.get("global_variables", {})
+
+  # Get project_id from sb.yaml.
+  project_id = global_variables.get("project_id", None)
+  assert project_id, "project_id is not set in 'global_variables' in sb.yaml."
 
   if component:
     component_flag = f" -m {component} "
   else:
     component_flag = ""
 
-  command = f"skaffold delete -p {profile} {component_flag} --default-repo=\"gcr.io/{project_id}\""
+  # Set Skaffold namespace
+  namespace_flag = f"-n {namespace}" if namespace else ""
+
+  command = f"skaffold delete -p {profile} {component_flag} {namespace_flag} --default-repo=\"gcr.io/{project_id}\""
   print("This will DELETE deployed services using the command below:")
   print_highlight(command)
   confirm("\nThis may take a few minutes. Continue?", default=False, skip=yes)
   exec_shell(command, working_dir=solution_path)
 
 
 @app.command()
 def info(solution_path: Annotated[Optional[str],
-                                    typer.Argument()] = "."):
+                                  typer.Argument()] = "."):
   """
   Print info from ./sb.yaml.
   """
   sb_yaml = read_yaml(f"{solution_path}/sb.yaml")
-  print(f"Printing info of the solution folder at '{solution_path}'\n")
+  print(f"Printing info of the solution folder at '{solution_path}/'\n")
 
-  for key, value in sb_yaml.items():
-    if key not in ["components", "_metadata"]:
-      print(f"{key}: {value}")
+  # Global variables
+  print("global_variables in sb.yaml:")
+  for key, value in sb_yaml.get("global_variables", {}).items():
+    print(f"- {key}: {value}")
   print()
 
-  print(f"Installed components:")
-  for key, value in sb_yaml["components"].items():
-    print(f" - {key}")
-  print()
+  # List of installed components.
+  components_list()
 
 
 @app.command()
 def version():
   """
   Print version.
   """
   print(f"Solutions Builder v{__version__}")
   raise typer.Exit()
 
 
 def main():
   try:
-    print_highlight(f"Solutions Builder (version " +
+    print_highlight("Solutions Builder (version " +
                     typer.style(__version__, fg=typer.colors.CYAN, bold=True) +
                     ")\n")
     app()
     print()
 
   except Exception as e:
-    if os.getenv("DEBUG", False):
+    if DEBUG:
       traceback.print_exc()
-    print_error(e)
+      print_error(f"Error: {e}")
+    else:
+      print_error(f"Error: {e}")
+      print("\nTip: try adding 'SB_DEBUG=true' to your environment variables to get more details.")
+      print("E.g. SB_DEBUG=true sb new your-project\n")
+
+    return -1
+
+  return 0
 
 
 if __name__ == "__main__":
   main()
```

### Comparing `solutions_builder-1.17.9/solutions_builder/cli/cli_utils.py` & `solutions_builder-1.18.0/solutions_builder/cli/cli_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,19 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import os, yaml, typer, subprocess, re
+import os
+import yaml
+import typer
+import subprocess
+import re
 
 
 def confirm(msg, skip=False, default=True):
   if not skip:
     typer.confirm(msg, abort=True, default=default)
 
 
@@ -100,16 +104,16 @@
 
 # Execute shell commands
 def exec_shell(command, working_dir=".", stop_when_error=True, stdout=None):
   proc = subprocess.Popen(command, cwd=working_dir, shell=True, stdout=stdout)
   exit_status = proc.wait()
 
   if exit_status != 0 and stop_when_error:
-    raise Exception(
-        f"Error when running command: {command} (working_dir={working_dir})")
+    raise RuntimeError(
+        f"Error occurs when running command: {command} (working_dir={working_dir})")
 
   return exit_status
 
 
 # Execute shell commands
 def exec_output(command, working_dir=".", stop_when_error=True):
   output = subprocess.check_output(command,
@@ -134,16 +138,22 @@
 def list_subfolders(path):
   modules = get_immediate_subdirectories(path)
   for module_name in sorted(modules):
     print_highlight(f"- {module_name}")
   print()
 
 
+def list_component_templates():
+  current_dir = os.path.dirname(__file__)
+  path = current_dir + "/../modules"
+  list_subfolders(path)
+
+
 def check_git_url(url):
-  regex_str = "((git|ssh|http(s)?)|(git@[\w\.]+))(:(//)?)([\w\.@\:/\-~]+)(\.git)(/)?"
+  regex_str = "((git|ssh|http(s)?)|(git@[\\w\\.]+))(:(//)?)([\\w\\.\\@\\:/\\-~]+)(\\.git)(/)?"
   regex = re.compile(regex_str)
   match = regex.match(url)
   return match is not None
 
 
 def get_answers_dict(data):
   if data:
```

### Comparing `solutions_builder-1.17.9/solutions_builder/cli/component.py` & `solutions_builder-1.18.0/solutions_builder/cli/component.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,154 +11,162 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import typer
-import traceback
 from typing import Optional
 from typing_extensions import Annotated
-from copier import run_auto
+from copier import run_copy
 from .cli_utils import *
 
 component_app = typer.Typer()
 
 
 @component_app.command()
 def add(component_name,
+        component_template: Annotated[str,
+                                      typer.Option("--template", "-t")] = None,
         solution_path: Annotated[Optional[str],
                                  typer.Argument()] = ".",
         yes: Optional[bool] = False,
         answers=None):
   validate_solution_folder(solution_path)
+
+  # Check if component_template is empty.
+  if not component_template:
+    print("Missing component_template. Please set --template or -t with one "
+          " of the component templates:")
+    list_component_templates()
+    return
+
   confirm(
-      f"This will add component '{component_name}' to '{solution_path}'. " +
-      "Continue?",
+      f"This will add component '{component_name}' to "
+      f"{solution_path}/components folder. Continue?",
       skip=yes)
 
   answers_dict = get_answers_dict(answers)
-  process_component("add", component_name, solution_path, data=answers_dict)
+  process_component("add",
+                    component_name, component_template,
+                    solution_path, data=answers_dict)
   print_success(
       f"Complete. Component {component_name} added to solution at {solution_path}\n"
   )
 
 
 @component_app.command()
 def update(component_name,
            solution_path: Annotated[Optional[str],
                                     typer.Argument()] = ".",
            yes: Optional[bool] = False,
            answers=None):
   validate_solution_folder(solution_path)
   confirm(
-      f"This will update the existing component '{component_name}' in '{solution_path}'. "
-      + "Continue?",
+      f"This will update '{component_name}' in "
+      f"'{solution_path}/components'. Continue?",
       skip=yes)
 
+  sb_yaml = read_yaml(f"{solution_path}/sb.yaml")
+  components = sb_yaml.get("components", {})
+  component_dict = components.get(component_name, {})
+  component_template = component_dict.get("component_template")
+
   answers_dict = get_answers_dict(answers)
   process_component("update",
                     component_name,
+                    component_template,
                     solution_path,
                     data=answers_dict,
                     use_existing_answers=yes)
   print_success(
       f"Complete. Component {component_name} updated to solution at {solution_path}\n"
   )
 
 
-@component_app.command()
-def init(component_name,
-          solution_path: Annotated[Optional[str],
-                                  typer.Argument()] = ".",
-          yes: Optional[bool] = False):
-
-  pass
-
-@component_app.command()
-def fix_skaffold(component_name,
-          solution_path: Annotated[Optional[str],
-                                  typer.Argument()] = ".",
-          yes: Optional[bool] = False):
-
-  pass
-
 def update_component_to_root_yaml(component_name, answers, solution_path):
   # Update Solution root YAML with new component name.
   solution_yaml_dict = read_yaml(f"{solution_path}/sb.yaml") or {}
   components = solution_yaml_dict["components"] or {}
   components[component_name] = answers
   solution_yaml_dict["components"] = components
   write_yaml(f"{solution_path}/sb.yaml", solution_yaml_dict)
 
 
 def process_component(method,
                       component_name,
+                      component_template,
                       solution_path,
                       data={},
                       use_existing_answers=False):
+
+  assert component_template, f"component_template is not empty."
+
   destination_path = "."
   current_dir = os.path.dirname(__file__)
   answers_file = None
 
   # Get basic info from root sb.yaml.
-  root_st_yaml = read_yaml(f"{solution_path}/sb.yaml")
+  sb_yaml = read_yaml(f"{solution_path}/sb.yaml")
+  global_variables = sb_yaml.get("global_variables", {})
   component_answers = {}
 
   # If the component name is a Git URL, use the URL as-is in copier.
-  if check_git_url(component_name):
-    print(f"Loading component from remote Git URL: {component_name}")
-    template_path = component_name
+  if check_git_url(component_template):
+    print(f"Loading component from remote Git URL: {component_template}")
+    template_path = component_template
 
   # Otherwise, try to locate the component in local modules/ folder.
   else:
-
     if method == "update":
       data["component_name"] = component_name
-      if component_name not in root_st_yaml["components"]:
+      if component_name not in sb_yaml["components"]:
         raise NameError(
             f"Component {component_name} is not defined in the root yaml 'sb.yaml' file."
         )
-      component_answers = root_st_yaml["components"][component_name]
+      component_answers = sb_yaml["components"][component_name]
       component_template = component_answers["component_template"]
       template_path = f"{current_dir}/../modules/{component_template}"
       answers_file = f".st/module_answers/{component_name}.yaml"
 
       # Use existing answer values in data, skipping the prompt.
       if use_existing_answers:
         answers_yaml = read_yaml(answers_file)
         for key, value in answers_yaml.items():
           data[key] = value
 
     else:
-      component_template = component_name
       template_path = f"{current_dir}/../modules/{component_template}"
       if not os.path.exists(template_path):
         raise FileNotFoundError(
-            f"Component {component_name} does not exist in modules folder.")
+            f"Component {component_template} does not exist in modules folder.")
 
     # Get destination_path defined in copier.yaml
     copier_dict = get_copier_yaml(template_path)
     destination_path = solution_path + "/" + copier_dict["_metadata"].get(
         "destination_path")
     destination_path = destination_path.replace("//", "/")
 
-  data["project_id"] = root_st_yaml["project_id"]
-  data["project_number"] = root_st_yaml["project_number"]
+  data["component_name"] = component_name
+  data["project_id"] = global_variables["project_id"]
+  data["project_number"] = global_variables["project_number"]
   data["solution_path"] = solution_path
+  data["template_path"] = template_path
 
   # Run copier with data.
-  worker = run_auto(template_path,
+  worker = run_copy(template_path,
                     destination_path,
                     data=data,
-                    answers_file=answers_file)
+                    answers_file=answers_file,
+                    unsafe=True)
 
   # Get answer values inputed by user.
   answers = worker.answers.user
-  for key, value in worker.answers.default.items():
+
+  for key, value in worker.answers.user_defaults.items():
     if key not in answers:
       answers[key] = component_answers.get(key) or value
   answers["component_template"] = component_template
   answers["destination_path"] = copier_dict["_metadata"].get(
       "destination_path")
 
   # Update component's answer back to sb.yaml.
@@ -173,28 +181,28 @@
     new_yaml["requires"] = dedupe(new_yaml["requires"])
     write_yaml(f"{solution_path}/{patch_file}", new_yaml)
     os.remove(f"{solution_path}/{patch_file}.patch")
 
   print()
 
 # List installed components.
+
+
 @component_app.command()
-def list(solution_path: Annotated[Optional[str], typer.Argument()] = ".", ):
-  root_st_yaml = read_yaml(f"{solution_path}/sb.yaml")
-  components = root_st_yaml.get("components", [])
-  print("Installed components:\n")
+def list(solution_path: Annotated[Optional[str], typer.Argument()] = "."):
+  sb_yaml = read_yaml(f"{solution_path}/sb.yaml")
+  components = sb_yaml.get("components", [])
+  print("Installed components:")
   for component_name, properties in components.items():
     typer.echo(
         typer.style(f"- {component_name} ", fg=typer.colors.WHITE, bold=True) +
         typer.style(f"(from: {properties['component_template']})",
                     fg=typer.colors.BLACK,
                     bold=True))
   print()
 
 
 # List available components to add.
 @component_app.command()
 def available():
-  current_dir = os.path.dirname(__file__)
-  path = current_dir + "/../modules"
   print("Available components to add:\n")
-  list_subfolders(path)
+  list_component_templates()
```

### Comparing `solutions_builder-1.17.9/solutions_builder/cli/infra.py` & `solutions_builder-1.18.0/solutions_builder/cli/infra.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import typer, time
+import typer
+import time
 from typing import Optional
 from typing_extensions import Annotated
-from copier import run_auto
 from .cli_utils import *
 
 infra_app = typer.Typer()
 
 
 def get_impersonate_clause(impersonate, impersonate_email, project_id):
   impersonate_clause = ""
@@ -44,16 +44,17 @@
 
   if not yes:
     auto_approve_flag = ""
   else:
     auto_approve_flag = "-auto-approve"
 
   # Get project ID from the existing root yaml.
-  st_yaml = read_yaml(f"{solution_path}/sb.yaml")
-  project_id = st_yaml["project_id"]
+  sb_yaml = read_yaml(f"{solution_path}/sb.yaml")
+  global_variables = sb_yaml.get("global_variables", {})
+  project_id = global_variables["project_id"]
 
   confirm(f"""
   This will initialize the solution with the following steps:
   - Set gcloud project to '{project_id}'
   - Run terraform init and apply in 'bootstrap' stage.
   - Run terraform init and apply in 'foundation' stage.
 
@@ -105,23 +106,25 @@
   This will initialize the solution with the following steps:
   - Run terraform init and apply in '{stage}' stage.
 
   This will take a few minutes. Continue?""",
           skip=yes)
 
   # Get project_id
-  st_yaml = read_yaml(f"{solution_path}/sb.yaml")
-  project_id = st_yaml["project_id"]
+  sb_yaml = read_yaml(f"{solution_path}/sb.yaml")
+  global_variables = sb_yaml.get("global_variables", {})
+  project_id = global_variables["project_id"]
 
   # Get impersonate service account email
   env_var_clause = get_impersonate_clause(impersonate, impersonate_email,
                                           project_id)
   unclock_clause = " -unlock=false" if unlock else ""
   working_dir = f"{solution_path}/terraform/stages/{stage}"
-  exec_shell(f"{env_var_clause} terraform init {unclock_clause}", working_dir=working_dir)
+  exec_shell(f"{env_var_clause} terraform init {unclock_clause}",
+             working_dir=working_dir)
   exec_shell(f"{env_var_clause} terraform apply {auto_approve_flag} {unclock_clause}",
              working_dir=working_dir)
   exec_shell(f"{env_var_clause} terraform output > tf_output.tfvars",
              working_dir=working_dir)
 
 
 # Project bootstrap and foundation.
@@ -151,23 +154,25 @@
   confirm(f"""
   WARNING! This will destory all resources created by 'terraform/{stage}'.
 
   This will take a few minutes. Continue?""",
           skip=yes)
 
   # Get project ID from the existing root yaml.
-  st_yaml = read_yaml(f"{solution_path}/sb.yaml")
-  project_id = st_yaml["project_id"]
+  sb_yaml = read_yaml(f"{solution_path}/sb.yaml")
+  global_variables = sb_yaml.get("global_variables", {})
+  project_id = global_variables["project_id"]
 
   # Get impersonate service account email
   env_var_clause = get_impersonate_clause(impersonate, impersonate_email,
                                           project_id)
   unclock_clause = " -unlock=false" if unlock else ""
   working_dir = f"{solution_path}/terraform/stages/{stage}"
-  exec_shell(f"{env_var_clause} terraform init {unclock_clause}", working_dir=working_dir)
+  exec_shell(f"{env_var_clause} terraform init {unclock_clause}",
+             working_dir=working_dir)
   exec_shell(f"{env_var_clause} terraform destroy {auto_approve_flag} {unclock_clause}",
              working_dir=working_dir)
 
 
 @infra_app.command()
 def list(solution_path: Annotated[Optional[str], typer.Argument()] = "."):
   print("Available infra stagse:\n")
```

### Comparing `solutions_builder-1.17.9/solutions_builder/cli/set.py` & `solutions_builder-1.18.0/solutions_builder/cli/set.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 """
 
 import typer
 import glob
 import pathlib
 from typing import Optional
 from typing_extensions import Annotated
-from copier import run_auto
 from .cli_utils import *
+from .vars import set_var
 
 set_app = typer.Typer()
 
 INCLUDE_PATTERNS = [
     "*.yaml", "*.yml", "*.env", "*.tfvars", "*.tf", "*.sh", "*.md"
 ]
 EXCLUDE_PATTERNS = ["**/.terraform/**/*.*", "**/node_modules/**/*.*"]
@@ -33,47 +33,42 @@
 @set_app.command()
 def project_id(
     new_project_id,
     solution_path: Annotated[Optional[str], typer.Argument()] = ".",
     yes: Optional[bool] = False,
 ):
   validate_solution_folder(solution_path)
-  root_st_yaml = read_yaml(f"{solution_path}/sb.yaml")
-  old_project_id = root_st_yaml.get("project_id")
+  sb_yaml = read_yaml(f"{solution_path}/sb.yaml")
+  global_variables = sb_yaml.get("global_variables", {})
+
+  old_project_id = global_variables.get("project_id")
+  old_project_number = global_variables.get("project_number")
   assert old_project_id, "project_id does not exist in sb.yaml"
 
   confirm(
       f"This will replace all project-id '{old_project_id}' to '{new_project_id}' in folder '{solution_path}'. "
       + "Continue?",
       skip=yes)
 
   # Update Root sb.yaml
-  root_st_yaml["project_id"] = new_project_id
-  root_st_yaml["project_number"] = int(get_project_number(new_project_id))
-  write_yaml(f"{solution_path}/sb.yaml", root_st_yaml)
+  new_project_number = get_project_number(new_project_id)
+  assert new_project_number, "Unable to receive project number for project " \
+                             f"'{new_project_id}'. Does this GCP project exist?"
+
+  global_variables["project_id"] = new_project_id
+  global_variables["project_number"] = new_project_number
+  sb_yaml["global_variables"] = global_variables
+  write_yaml(f"{solution_path}/sb.yaml", sb_yaml)
 
   # Update copier answers
   copier_yaml = read_yaml(f"{solution_path}/.copier-answers.yml")
   copier_yaml["project_id"] = new_project_id
   copier_yaml["project_number"] = int(get_project_number(new_project_id))
   write_yaml(f"{solution_path}/.copier-answers.yml", copier_yaml)
 
-  file_set = set()
-  # Adding includes.
-  for pattern in INCLUDE_PATTERNS:
-    file_list = pathlib.Path(solution_path).rglob(f"{pattern}")
-    file_set.update(set([str(x) for x in file_list]))
-
-  # Removing excludes.
-  for pattern in EXCLUDE_PATTERNS:
-    file_list = pathlib.Path(solution_path).rglob(f"{pattern}")
-    file_set = file_set - set([str(x) for x in file_list])
-
-  for filename in list(file_set):
-    with open(filename, "r") as file:
-      filedata = file.read()
-      filedata = re.sub(old_project_id, new_project_id, filedata)
-    with open(filename, "w") as file:
-      file.write(filedata)
+  set_var("project_id", new_project_id)
+  set_var("project_number", new_project_number)
 
   print(
       f"\nReplaced project_id from '{old_project_id}' to '{new_project_id}'.")
+  print(
+      f"Replaced project_number from '{old_project_number}' to '{new_project_number}'.\n")
```

### Comparing `solutions_builder-1.17.9/solutions_builder/cli/template.py` & `solutions_builder-1.18.0/solutions_builder/cli/template.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 limitations under the License.
 """
 
 import typer
 import traceback
 from typing import Optional
 from typing_extensions import Annotated
-from copier import run_auto
+from copier import run_copy
 from .cli_utils import *
 
 template_app = typer.Typer()
 
 
 @template_app.command()
 def new(module_name,
@@ -35,10 +35,10 @@
   if not module_template_path:
     current_dir = os.path.dirname(__file__)
     module_template_path = f"{current_dir}/../module_template"
 
   answers_dict = get_answers_dict(answers)
   answers_dict["module_name"] = module_name
   module_path = f"{modules_folder}/{module_name}"
-  run_auto(module_template_path, module_path, data=answers_dict)
+  run_copy(module_template_path, module_path, data=answers_dict, unsafe=True)
 
   print_success(f"Complete. New module folder created at {module_path}.\n")
```

### Comparing `solutions_builder-1.17.9/solutions_builder/copier_extensions/sb_helpers.py` & `solutions_builder-1.18.0/solutions_builder/copier_extensions/sb_helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,68 +21,95 @@
 
 # Read YAML file and convert to a dict.
 def read_yaml(filepath):
   with open(filepath) as f:
     data = yaml.safe_load(f)
   return data
 
+def print_indent(text, offest=6):
+  text = " " * offest + text
+  print(text)
+
 
 # Execute shell commands
-def exec_output(command, working_dir=".", stop_when_error=True):
-  output = subprocess.check_output(command,
-                                   cwd=working_dir,
-                                   shell=True,
-                                   text=True)
-  return output
+def exec_output(command, working_dir=".", stop_when_error=False):
+  try:
+    output = subprocess.check_output(command,
+                                    stderr=subprocess.STDOUT,
+                                    cwd=working_dir,
+                                    shell=True,
+                                    text=True)
+  except subprocess.CalledProcessError as e:
+    # print("Status : FAIL", e.returncode, e.output)
+    raise e
+
+  else:
+    return output
 
 
 def exec_gcloud_output(command, working_dir="."):
   output = ""
-  try:
-    output = exec_output(command)
-  except Exception as e:
-    print(f"Error: {e}")
-    output = ""
-
+  output = exec_output(command)
   output = output.strip()
   return output
 
 
 def get_project_number(project_id):
   """
     Get GCP project number based on project_id using gcloud command.
     """
-  print(f"    (Retrieving project number for {project_id}...)")
+  print_indent(f"(Retrieving project number for {project_id}...)")
   command = f"gcloud projects describe {project_id} --format='value(projectNumber)'"
-  project_number = exec_gcloud_output(command)
-  project_number = project_number.strip()
-  if not project_number.isnumeric():
+  try:
+    project_number = exec_gcloud_output(command)
+    project_number = project_number.strip()
+
+    if not project_number.isnumeric():
+      print_indent(f"project_number is not numeric: {project_number}")
+      return ""
+
+  except subprocess.CalledProcessError as e:
+    print_indent(f"{e.output}")
+    print_indent(f"Unable to retrieve project_number for '{project_id}'. GCP project '{project_id}' may not exist on GCP yet.\n")
     return ""
 
-  return project_number
+  else:
+    return project_number
 
 
 def get_existing_firestore(project_id):
   """
     Get boolean whether to initialize Firestore.
     """
-  print(f"   (Retrieving Firestore databases list...)")
+  print_indent(f"(Retrieving Firestore databases list...)")
   command = f"gcloud alpha firestore databases list --format='value(databases[0].name)' --project='{project_id}' --quiet"
-  database_name = exec_gcloud_output(command)
-  return database_name
 
+  try:
+    database_name = exec_gcloud_output(command)
+    return database_name
+
+  except subprocess.CalledProcessError as e:
+    print_indent(f"Unable to retrieve default Firestore database name for '{project_id}'. GCP project '{project_id}' may not exist on GCP yet.\n")
+    return ""
 
 def get_current_user(project_id):
   """
     Get current authenticated gcloud user.
     """
   print(f"   (Retrieving current authenticated gcloud user...)")
   command = f"gcloud config list account --format 'value(core.account)' | head -n 1"
-  email = exec_gcloud_output(command)
-  return email
+
+  try:
+    email = exec_gcloud_output(command)
+    return email
+
+  except subprocess.CalledProcessError as e:
+    print_indent(f"{e.output}")
+    print_indent(f"Unable to retrieve current authenticated gcloud user.")
+    return ""
 
 
 def get_cloud_run_services(project_id):
   """
     Get all deployed Cloud Run services.
     """
   print(f"   (Retrieving existing Cloud Run services for {project_id}...)")
```

### Comparing `solutions_builder-1.17.9/solutions_builder/module_template/README.md` & `solutions_builder-1.18.0/solutions_builder/module_template/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/module_template/copier.yaml` & `solutions_builder-1.18.0/solutions_builder/module_template/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/module_template/template_copier.yaml` & `solutions_builder-1.18.0/solutions_builder/module_template/template_copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/module_template/{{"{{'.github' if use_github_action}}"}}/workflows/{{"unit_test_linter_{{component_name}}"}}.yaml` & `solutions_builder-1.18.0/solutions_builder/module_template/{{"{{'.github' if use_github_action}}"}}/workflows/{{"unit_test_linter_{{component_name}}"}}.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/Dockerfile` & `solutions_builder-1.18.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/skaffold.yaml` & `solutions_builder-1.18.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/src/main.py` & `solutions_builder-1.18.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/src/main.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/backend.tf` & `solutions_builder-1.18.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/main.tf` & `solutions_builder-1.18.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/providers.tf` & `solutions_builder-1.18.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/terraform.tfvars` & `solutions_builder-1.18.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/terraform.tfvars`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/variables.tf` & `solutions_builder-1.18.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/restful_service/README.md` & `solutions_builder-1.18.0/solutions_builder/modules/restful_service/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/Dockerfile` & `solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/skaffold.yaml` & `solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/src/config.py` & `solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/config.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/src/main.py` & `solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/main.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py` & `solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,12 +46,13 @@
   status = TextField()
   created_at = DateTime()
   modified_at = DateTime()
 
   @classmethod
   def find_by_id(cls, id):
     try:
-      {{data_model}} = {{data_model | capitalize}}.collection.get(id)
+      {{data_model}} = {{data_model | capitalize}}.collection.get(
+          DATABASE_PREFIX + "{{data_model_plural}}" + "/" + id)
     except ReferenceDocNotExist:
       return None
 
     return {{data_model}}
```

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py` & `solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py` & `solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml` & `solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/restful_service/copier.yaml` & `solutions_builder-1.18.0/solutions_builder/modules/restful_service/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py` & `solutions_builder-1.18.0/solutions_builder/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml` & `solutions_builder-1.18.0/solutions_builder/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/README.md` & `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/Dockerfile` & `solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/skaffold.yaml` & `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/config.py` & `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/config.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/main.py` & `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/main.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/models/task.py` & `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/models/task.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/tasks.py` & `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/tasks.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/schemas/task.py` & `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/schemas/task.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow.py` & `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow_test.py` & `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow_test.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/deployment.yaml` & `solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/copier.yaml` & `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/backend.tf` & `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/main.tf` & `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/providers.tf` & `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/terraform.tfvars` & `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/terraform.tfvars`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,16 @@
  *
  */
 
 # TODO: Add Terraform variable with Jinja variables below.
 # Note for modules: Jinja variables are defined in copier.yaml.
 
 
-project_id                 = "{{project_id}}"
-region                     = "{{gcp_region}}"
+project_id                 = "{{project_id}}" # sb-var:project_id
+region                     = "{{gcp_region}}" # sb-var:gcp_region
 task_pubsub_topic          = "{{task_pubsub_topic}}"
 message_retention_duration = "{{pubsub_message_retention_duration}}"
 eventarc_trigger_name      = "{{eventarc_trigger_name}}"
 eventarc_cloudrun_service  = "{{eventarc_cloudrun_service}}"
 eventarc_gke_cluster       = "{{eventarc_gke_cluster}}"
 eventarc_gke_namespace     = "{{eventarc_gke_namespace}}"
 eventarc_gke_path          = "{{eventarc_gke_path}}"
```

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/variables.tf` & `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/task_dispatch_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml` & `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_gke/copier.yaml` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/copier.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   type: str
   help: What is the name of this component (snake_case)?
   default: terraform_gke
 
 terraform_stage_name:
   type: str
   help: Terraform stage name?
-  default: 2-gke
+  default: 3-gke
 
 resource_name:
   type: str
   help: Ingress resource name (lower case, alphanumeric characters, '-')?
   default: gke-ingress
 
 gcp_region:
@@ -34,15 +34,15 @@
   help: Kubernetes version?
   default: latest
   # See https://cloud.google.com/kubernetes-engine/docs/release-notes-stable
 
 node_machine_type:
   type: str
   help: GKE Node machine type (Compute Engine)?
-  default: n1-standard-4
+  default: n2-standard-2
 
 private_cluster:
   type: bool
   help: Private cluster?
   default: true
 
 _answers_file: ".st/module_answers/{{component_name}}.yaml"
```

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_gke/docs/components/{{component_name}}.md` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/docs/components/{{component_name}}.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # Module: Terraform GKE Stage
 
-This module defines a Terraform GKE setup stage named "2-gke".
+This module defines a Terraform GKE setup stage named "3-gke".
 
 Main components after setup:
-- ./terraform/stage/2-gke
+- ./terraform/stage/3-gke
 
 ## Setup
 
-Run `st components add [COMPONENT_NAME]` to add this module.
+Run `sb components add [COMPONENT_NAME]` to add this module.
 ```
 cd my-solution-folder
-st components add terraform_gke .
+sb components add terraform_gke .
 ```
 
 Fill in the variables.
 ```
 🎤 What is the name of this terraform stage?
-   2-gke
+   3-gke
 🎤 Which Google Cloud region?
    us-central1
 🎤 Kubernetes version?
-   1.24.11-gke.1000
+   latest
 🎤 Allow domains for CORS? (comma-seperated)
    http://localhost:4200,http://localhost:3000
 🎤 Cert Issuer Email
    my_name@example.com
 
 ...
 
 Complete. Component terraform_gke added to solution at .
 ```
 
 Initialize the terraform stage using `st init --stage=[STAGE_NAME]`
 ```
-st init --stage=2-gke
+sb init --stage=3-gke
 ```
 
 ## Development
 
 ## FAQ
```

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/backend.tf` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf`

 * *Files 10% similar despite different names*

```diff
@@ -12,12 +12,15 @@
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
 terraform {
+  {% if terraform_backend_gcs == true -%}
   backend "gcs" {
-    bucket = "{{project_id}}-tfstate"
-    prefix = "stage/2-gke"
+    # Uncomment below and specify a GCS bucket for TF state.
+    bucket = "{{project_id}}-tfstate" # sb-var:project_id:{{project_id}}-tfstate
+    prefix = "stage/3-ingress-serverless"
   }
+  {%- endif %}
 }
```

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/iam.tf` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/iam.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/main.tf` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/providers.tf` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/variables.tf` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/variables.tf`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
   type        = string
   description = "Kubernetes version. See https://cloud.google.com/kubernetes-engine/docs/release-notes-stable"
 }
 
 variable "node_machine_type" {
   type        = string
   description = "VM machine time"
-  default     = "n1-standard-4"
+  default     = "n2-standard-2"
 }
 
 variable "private_cluster" {
   type        = bool
   description = "Whether to use private nodes"
   default     = true
 }
```

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/copier.yaml` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/copier.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 # questions
 component_name:
   type: str
   help: What is the name of this component?
   default: terraform_gke_ingress
   validator: "{% if not component_name %}Required{% endif %}"
 
+terraform_stage_name:
+  type: str
+  help: Terraform stage name?
+  default: 3-gke-ingress
+
 resource_name:
   type: str
   help: Resource name for ingress configs?
   default: gke-ingress
   validator: "{% if not resource_name %}Required{% endif %}"
 
 loadbalancer_name:
```

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/ingress.yaml` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/ingress.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/main.tf` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/main.tf`

 * *Files 9% similar despite different names*

```diff
@@ -40,17 +40,19 @@
   count        = var.external_ip_address == null ? 1 : 0
   project      = var.project_id
   name         = "gke-ingress-ip"
   address_type = "EXTERNAL"
 }
 
 resource "google_compute_managed_ssl_certificate" "managed_certificate" {
-  provider = google-beta
+  # Prevent managed cert from deploying if no domains
+  count = ((length(var.domains) == 1) && (var.domains[0] == "None")) ? 0 : 1
 
-  name = var.managed_cert_name
+  provider = google-beta
+  name     = var.managed_cert_name
   managed {
     domains = var.domains
   }
 }
 
 resource "google_compute_ssl_policy" "gke-ingress-ssl-policy" {
   name            = "gke-ingress-ssl-policy"
```

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/outputs.tf` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/variables.tf` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/backend.tf` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/backend.tf`

 * *Files 12% similar despite different names*

```diff
@@ -13,11 +13,11 @@
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
 terraform {
   backend "gcs" {
-    bucket = "{{project_id}}-tfstate"
-    prefix = "stage/3-gke-ingress"
+    bucket = "{{project_id}}-tfstate" # sb-var:project_id:{{project_id}}-tfstate
+    prefix = "stage/{{terraform_stage_name}}"
   }
 }
```

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/iam.tf` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/iam.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/main.tf` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/providers.tf` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/variables.tf` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_httplb_cloudrun/copier.yaml` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/backend.tf`

 * *Files 12% similar despite different names*

```diff
@@ -15,12 +15,12 @@
  *
  */
 
 terraform {
   {% if terraform_backend_gcs == true -%}
   backend "gcs" {
     # Uncomment below and specify a GCS bucket for TF state.
-    bucket = "{{project_id}}-tfstate"
-    prefix = "stage/3-ingress-serverless"
+    bucket = "{{project_id}}-tfstate" # sb-var:project_id:{{project_id}}-tfstate
+    prefix = "stage/2-foundation"
   }
   {%- endif %}
 }
```

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/.github/assets/setup_local.png` & `solutions_builder-1.18.0/solutions_builder/template_root/.github/assets/setup_local.png`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/.github/assets/skaffold_dev_terminal.png` & `solutions_builder-1.18.0/solutions_builder/template_root/.github/assets/skaffold_dev_terminal.png`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/.github/workflows/deployment_cloudrun_dev.yaml` & `solutions_builder-1.18.0/solutions_builder/template_root/.github/workflows/deployment_cloudrun_dev.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   workflow_dispatch:
 
 env:
   PROJECT_ID: {{project_id}}
   REGION: {{gcp_region}}
   ENV: dev
 
-# copoier:raw {% raw %}
+# copier:raw {% raw %}
 jobs:
   build_common:
     name: Build Common image
     runs-on: ubuntu-latest
     steps:
       - name: Check out repository
         uses: actions/checkout@v3
@@ -81,8 +81,8 @@
           _CLOUD_RUN_SERVICE_NAME="${{ matrix.target-folder[1] }}",\
           _PROJECT_ID="${{ env.PROJECT_ID }}",\
           _REGION="${{ env.REGION }}",\
           _REPOSITORY="cloudrun",\
           _IMAGE="${{ matrix.target-folder[1] }}",\
           _SERVICE_ACCOUNT="deployment-${{ env.ENV }}@${{ env.PROJECT_ID }}.iam.gserviceaccount.com"
 
-# copoier:endraw {% endraw %}
+# copier:endraw {% endraw %}
```

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/.github/workflows/deployment_gke_dev.yaml` & `solutions_builder-1.18.0/solutions_builder/template_root/.github/workflows/deployment_gke_dev.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   SKAFFOLD_NAMESPACE: default
   GKE_CLUSTER: main-cluster
   GKE_REGION: {{gcp_region}}
   KUSTOMIZE_VERSION: 4.1.3
   SKAFFOLD_VERSION: 2.0.3
   SKAFFOLD_CACHE_GCS: gs://{{project_id}}.appspot.com/skaffold/cache
 
-# copoier:raw {% raw %}
+# copier:raw {% raw %}
 jobs:
   deploy_backends:
     name: Deploy microservices to GKE cluster
     runs-on: ubuntu-latest
     steps:
       - name: Check out repository
         uses: actions/checkout@v3
@@ -78,8 +78,8 @@
           --add-skaffold-labels=false
 
       - name: Upload Skaffold cache
         if: always()
         run: |
           gsutil cp ~/.skaffold/cache $SKAFFOLD_CACHE_GCS
 
-# copoier:endraw {% endraw %}
+# copier:endraw {% endraw %}
```

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/.github/workflows/e2e_cloudrun_api_test.yaml` & `solutions_builder-1.18.0/solutions_builder/template_root/.github/workflows/e2e_cloudrun_api_test.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
       - ".github/workflows/e2e_cloudrun_api_tesb.yaml"
   workflow_dispatch:
 env:
   PROJECT_ID: {{project_id}}
   REGION: {{gcp_region}}
   ENV: dev
 
-# copoier:raw {% raw %}
+# copier:raw {% raw %}
 jobs:
   build_common:
     name: Build Common image
     runs-on: ubuntu-latest
     steps:
       - name: Check out repository
         uses: actions/checkout@v3
@@ -164,8 +164,8 @@
 
       - name: Delete CloudRun service
         run: |
           PR_NUMBER=$(jq --raw-output .pull_request.number "$GITHUB_EVENT_PATH")
           SERVICE_NAME_PREFIX=e2e-pr${PR_NUMBER}-
           gcloud run services delete ${SERVICE_NAME_PREFIX}${{ matrix.cloudrun-services }} --region=${{ env.REGION }} --quiet
 
-# copoier:endraw {% endraw %}
+# copier:endraw {% endraw %}
```

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/.github/workflows/e2e_gke_api_test.yaml` & `solutions_builder-1.18.0/solutions_builder/template_root/.github/workflows/e2e_gke_api_test.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   SKAFFOLD_NAMESPACE: default
   GKE_CLUSTER: main-cluster
   GKE_ZONE: {{gcp_region}}
   KUSTOMIZE_VERSION: 4.1.3
   SKAFFOLD_VERSION: 2.0.3
   SKAFFOLD_CACHE_GCS: gs://{{project_id}}.appspot.com/skaffold/cache
 
-# copoier:raw {% raw %}
+# copier:raw {% raw %}
 jobs:
   deploy:
     name: Deploy all microservices in PR namespace
     runs-on: ubuntu-latest
     steps:
       - name: Check out repository
         uses: actions/checkout@v3
@@ -224,8 +224,8 @@
       - name: Delete all deployments and namespace
         run: |
           PR_NUMBER=$(jq --raw-output .pull_request.number "$GITHUB_EVENT_PATH")
           NAMESPACE=e2e-pr-$PR_NUMBER
           skaffold delete --namespace $NAMESPACE
           kubectl delete namespace $NAMESPACE
 
-# copoier:endraw {% endraw %}
+# copier:endraw {% endraw %}
```

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/.github/workflows/unit_test_linter_common.yaml` & `solutions_builder-1.18.0/solutions_builder/template_root/.github/workflows/unit_test_linter_common.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       - ".github/workflows/unit_test_linter_common.yaml"
       - ".pylintrc"
   workflow_dispatch:
 
 env:
   PROJECT_ID: {{project_id}}
 
-# copoier:raw {% raw %}
+# copier:raw {% raw %}
 jobs:
   unit-test:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version: [3.9]
@@ -91,8 +91,8 @@
 
       - name: Lint with pylint
         run: |
           BASE_DIR=$(pwd)
           cd ${{ matrix.target-folder }}/src
           python -m pylint $(git ls-files '*.py') --rcfile=$BASE_DIR/.pylintrc
 
-# copoier:endraw {% endraw %}
+# copier:endraw {% endraw %}
```

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/.pylintrc` & `solutions_builder-1.18.0/solutions_builder/template_root/.pylintrc`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/skaffold.yaml` & `solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/config.py` & `solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/config.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/db_client.py` & `solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/db_client.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/example.py` & `solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/example.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/bq_client_fixture.py` & `solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/bq_client_fixture.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/client_with_emulator.py` & `solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/client_with_emulator.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/firestore_emulator.py` & `solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/firestore_emulator.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/logging_handler.py` & `solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/logging_handler.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/copier.yaml` & `solutions_builder-1.18.0/solutions_builder/template_root/copier.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -11,35 +11,46 @@
 project_id:
   type: str
   help: What is your Google Cloud project ID?
   default: "{{folder_name}}"
 
 project_number:
   type: str
-  help: What is your Google Cloud project number?
+  help: What is your Google Cloud project number? (Leave it as empty if the project hasn't created yet.)
   default: "{{project_id | get_project_number}}"
 
 gcp_region:
   type: str
   help: Which Google Cloud region?
   default: us-central1
 
+use_jump_host:
+  type: bool
+  help: Use a jump-host for running terraform foundations?
+  default: true
+
+jump_host_zone:
+  type: str
+  help: Google Cloud zone for creating the jump host?
+  default: us-central1-a
+  when: "{{use_jump_host}}"
+
 has_common:
   type: bool
   help: Include a common container image for shared libraries, data models, utils, etc?
   default: true
 
 terraform_backend_gcs:
   type: bool
   help: Use GCS Bucket for Terraform backend?
   default: true
 
 advanced_settings:
   type: bool
-  help: Show advanced settings (VPC, Storage region, etc)?
+  help: Show advanced settings (VPC, Storage, Region, etc)?
   default: false
 
 create_vpc_network:
   type: bool
   help: Create a default VPC Network?
   default: true
   when: "{{advanced_settings}}"
@@ -76,20 +87,14 @@
 
 secondary_service_ip_cidr_range:
   type: str
   help: Secondary service ranges?
   default: 10.2.0.0/16
   when: "{{advanced_settings and create_vpc_network}}"
 
-existing_firestore_name:
-  type: str
-  help: Existing Firestore path? (e.g. projects/{{project_id}}/databases/(default))
-  default: "{{project_id | get_existing_firestore}}"
-  when: "{{advanced_settings and create_vpc_network}}"
-
 _templates_suffix: ""
 
 _exclude:
   - "copier.yaml"
   - ".terraform*"
   - ".tmp"
   - ".venv"
```

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/cloudbuild/main.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/cloudbuild/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/cloudbuild/variables.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/cloudbuild/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/cloudrun/main.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/cloudrun/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/cloudrun/variables.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/cloudrun/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/compute_backend/main.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/compute_backend/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/compute_backend/providers.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/compute_backend/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/compute_backend/variables.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/compute_backend/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/firebase/main.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/firebase/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/firebase/variables.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/firebase/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/gke/main.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/gke/main.tf`

 * *Files 1% similar despite different names*

```diff
@@ -80,17 +80,17 @@
   create_duration = "120s"
 }
 
 module "cloud-nat" {
   count                              = var.enable_private_nodes ? 1 : 0
   source                             = "terraform-google-modules/cloud-nat/google"
   version                            = "~> 1.2"
-  name                               = format("%s-%s-nat", var.project_id, var.region)
+  name                               = format("%s-%s-gke-nat", var.project_id, var.region)
   create_router                      = true
-  router                             = format("%s-%s-router", var.project_id, var.region)
+  router                             = format("%s-%s-gke-router", var.project_id, var.region)
   project_id                         = var.project_id
   region                             = var.region
   network                            = var.vpc_network
   source_subnetwork_ip_ranges_to_nat = var.source_subnetwork_ip_ranges_to_nat
   log_config_enable                  = true
   log_config_filter                  = "ERRORS_ONLY"
 }
```

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/gke/outputs.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/gke/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/gke/variables.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/gke/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/ingress_nginx/main.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/ingress_nginx/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/ingress_nginx/outputs.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/ingress_nginx/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/ingress_nginx/variables.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/ingress_nginx/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/project_services/main.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/project_services/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/project_services/variables.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/project_services/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/service_account/main.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/service_account/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/service_account/variables.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/service_account/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/terraform_cicd/main.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/terraform_cicd/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/terraform_cicd/variables.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/terraform_cicd/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/vpc_network/main.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/vpc_network/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/modules/vpc_network/variables.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/vpc_network/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/1-bootstrap/output.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/1-bootstrap/output.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/1-bootstrap/variables.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/1-bootstrap/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/2-foundation/backend.tf` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/backend.tf`

 * *Files 24% similar despite different names*

```diff
@@ -12,15 +12,12 @@
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
 terraform {
-  {% if terraform_backend_gcs == true -%}
   backend "gcs" {
-    # Uncomment below and specify a GCS bucket for TF state.
-    bucket = "{{project_id}}-tfstate"
-    prefix = "stage/2-foundation"
+    bucket = "{{project_id}}-tfstate" # sb-var:project_id:{{project_id}}-tfstate
+    prefix = "stage/3-gke-ingress"
   }
-  {%- endif %}
 }
```

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/2-foundation/firestore_setup.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/firestore_setup.tf`

 * *Files 11% similar despite different names*

```diff
@@ -35,15 +35,18 @@
 }
 
 resource "google_project_service" "firestore" {
   project = var.project_id
   service = "firestore.googleapis.com"
 }
 
+# Only create a new Firestore database if choosing a different
+# Firestore database name other than (default).
 resource "google_firestore_database" "database" {
   depends_on = [google_project_service.firestore]
+  count      = ((var.firestore_database_name != "" && var.firestore_database_name != "(default)") ? 1 : 0)
 
   project     = var.project_id
   location_id = var.firestore_location_id
-  name        = "(default)"
+  name        = var.firestore_database_name
   type        = "FIRESTORE_NATIVE"
 }
```

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/2-foundation/iam.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/iam.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/2-foundation/identity_platform.tf` & `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/backend.tf`

 * *Files 15% similar despite different names*

```diff
@@ -11,17 +11,13 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
-resource "google_apikeys_key" "idp_api_key" {
-  name         = "idp-api-key"
-  display_name = "API Key for Identity Platform"
-
-  restrictions {
-    api_targets {
-      service = "identitytoolkit.googleapis.com"
-    }
+terraform {
+  backend "gcs" {
+    bucket = "{{project_id}}-tfstate" # sb-var:project_id:{{project_id}}-tfstate
+    prefix = "stage/{{terraform_stage_name}}"
   }
 }
```

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/2-foundation/main.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/main.tf`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     "aiplatform.googleapis.com",           # Vertex AI
     "apikeys.googleapis.com",              # API Keys
     "appengine.googleapis.com",            # AppEngine
     "artifactregistry.googleapis.com",     # Artifact Registry
     "bigquery.googleapis.com",             # BigQuery
     "bigquerydatatransfer.googleapis.com", # BigQuery Data Transfer
     "cloudbuild.googleapis.com",           # Cloud Build
-    "compute.googleapis.com",              # Compute Engine
     "container.googleapis.com",            # Google Kubernetes Engine
     "containerregistry.googleapis.com",    # Google Container Registry
     "dataflow.googleapis.com",             # Cloud Dataflow
     "eventarc.googleapis.com",             # Event Arc
     "firebase.googleapis.com",             # Firebase
     "firestore.googleapis.com",            # Firestore
     "iam.googleapis.com",                  # Cloud IAM
```

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/2-foundation/outputs.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/2-foundation/providers.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/terraform/stages/2-foundation/variables.tf` & `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/variables.tf`

 * *Files 14% similar despite different names*

```diff
@@ -109,7 +109,13 @@
 }
 
 variable "firestore_location_id" {
   type        = string
   description = "Firestore Dataset location. Available values: nam5 or eur3"
   default     = "nam5"
 }
+
+variable "firestore_database_name" {
+  type        = string
+  description = "Firestore Dataset name"
+  default     = "(default)"
+}
```

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/tests/e2e/e2e_utils.py` & `solutions_builder-1.18.0/solutions_builder/template_root/tests/e2e/e2e_utils.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/utils/disable_org_policies.sh` & `solutions_builder-1.18.0/solutions_builder/template_root/utils/disable_org_policies.sh`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/solutions_builder/template_root/utils/init_env_vars.sh` & `solutions_builder-1.18.0/solutions_builder/template_root/utils/init_env_vars.sh`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.9/PKG-INFO` & `solutions_builder-1.18.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: solutions-builder
-Version: 1.17.9
+Version: 1.18.0
 Summary: A solution framework to generate a project with built-in structure and modules
 Home-page: https://github.com/GoogleCloudPlatform/solutions-builder
 License: Apache
 Author: Jon Chen
 Author-email: jonchen@google.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: copier (>=7.2.0,<8.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: copier (>=9.2.0)
 Requires-Dist: copier-templates-extensions (>=0.3.0,<0.4.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jinja2-strcase (>=0.0.2,<0.0.3)
 Requires-Dist: jinja2-time (>=0.2.0,<0.3.0)
 Requires-Dist: pathlib (>=1.0.1,<2.0.0)
-Requires-Dist: pydantic (<=1.10.12)
+Requires-Dist: pydantic (>=2)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: typer (>=0.9.0)
 Project-URL: Repository, https://github.com/GoogleCloudPlatform/solutions-builder
 Description-Content-Type: text/markdown
 
 # Google Cloud Solutions Builder
 
 **A solution framework to generate a new project with built-in structure and modules
 to accelerate your project setup.**
@@ -33,148 +33,172 @@
 ## TL;DR
 
 Solutions Builder is a boilerplate template for building repeatable
 solutions with the best practices in architecture on Google Cloud, including GKE
 clusters, Cloud Run, Test Automation, CI/CD, as well as development process.
 
 This template provides built-in and ready-to-ship modules including:
-* Easy-to-deploy [Terraform](https://www.terraform.io/) boilerplate modules
-* Container-based microservices, can be deployed to a Kubernetes cluster or Cloud Run.
-* Unified deployment using Skaffold.
-* Automatically generated API documentation with Swagger UI.
-* CI/CD deployment (with Github Actions).
-* Cloud Run templates.
+
+- Easy-to-deploy [Terraform](https://www.terraform.io/) boilerplate modules
+- Container-based microservices, can be deployed to a Kubernetes cluster or Cloud Run.
+- Unified deployment using Skaffold.
+- Automatically generated API documentation with Swagger UI.
+- CI/CD deployment (with GitHub Actions).
+- Cloud Run templates.
 
 ## Roadmap
 
-Please see [Feature Requests in the Github issue list](https://github.com/GoogleCloudPlatform/solutions-builder/issues?q=is%3Aopen+is%3Aissue+label%3A%22feature+request%22).
+Please see [Feature Requests in the GitHub issue list](https://github.com/GoogleCloudPlatform/solutions-builder/issues?q=is%3Aopen+is%3Aissue+label%3A%22feature+request%22).
 
 ## Prerequisite
 
-| Tool | Required Version | Installation |
-|---|---|---|
-| Python     | &gt;= 3.9     | |
-| gcloud CLI | Latest        | https://cloud.google.com/sdk/docs/install |
-| Terraform  | &gt;= v1.3.7  | https://developer.hashicorp.com/terraform/downloads |
-| Skaffold   | &gt;= v2.4.0  | https://skaffold.dev/docs/install/ |
+| Tool       | Required Version | Installation                                        |
+| ---------- | ---------------- | --------------------------------------------------- |
+| Python     | &gt;= 3.11       |                                                     |
+| gcloud CLI | Latest           | https://cloud.google.com/sdk/docs/install           |
+| Terraform  | &gt;= v1.3.7     | https://developer.hashicorp.com/terraform/downloads |
+| Skaffold   | &gt;= v2.4.0     | https://skaffold.dev/docs/install/                  |
 
 [Optional] If you plan to deploy services on a GKE cluster, please install the following:
 
-| Tool | Required Version | Installation |
-|---|---|---|
-| Kustomize   | &gt;= v5.0.0 | https://kubectl.docs.kubernetes.io/installation/kustomize/ |
+| Tool      | Required Version | Installation                                               |
+| --------- | ---------------- | ---------------------------------------------------------- |
+| Kustomize | &gt;= v5.0.0     | https://kubectl.docs.kubernetes.io/installation/kustomize/ |
 
 ## Installing Solutions Builder CLI
 
 With `pip`:
+
 ```
 pip install solutions-builder
 ```
 
 With `pipx`:
+
 ```
 pip install --user pipx
 pipx install solutions-builder
 ```
 
 ## Quick Start
 
 This quick start steps will do the following:
+
 - Create a new GCP project and initialize Cloud foundation.
 - Add a RESTful API service for managing Todo list.
 - Deploy the service to Cloud Run.
 
 Set up GCP project
+
 ```
 export PROJECT_ID=my-solution-gcp-id
 
 # (Optional) Create a new GCP project. You can also use an existing GCP project.
 gcloud projects create $PROJECT_ID
 
 # Set gcloud CLI to the GCP project.
 gcloud config set project $PROJECT_ID
 ```
 
 Generate a new solution folder.
+
 ```
 sb new my-solution
 ```
 
 This will prompt options and variables:
+
 ```
 🎤 What is your project name? (Spaces are allowed.)
    my-solution
 🎤 What is your Google Cloud project ID?
    my-solution-gcp-id
 🎤 What is your Google Cloud project number?
    12345678
 🎤 Which Google Cloud region?
    us-central1
 🎤 Use GCS Bucket for Terraform backend?
    Yes
 ```
 
 Go to the newly created project folder
+
 ```
 cd my-solution
 sb infra apply 1-bootstrap
 ```
 
 Initialize Cloud infrastructure
+
 - Option 1: (Recommended) Log in to the jump host and run the following command(s) in the solution folder.
 - Option 2: Run the following commands in your local machine.
+
 ```
 sb infra apply 2-foundation
 ```
 
 Add a RESTful API service with **Todo** data model to this solution.
+
 ```
-sb components add restful_service
+sb components add -t restful_service todo_service
 ```
 
 Fill details in the prompt:
+
 - Component name: **todo_service**
 - Resource name: **todo-service**
 - Relative path: **todo-service**
 - GCP region: **us-central1**
 - Data model name: **todo**
 - Add Cloud Run to deployment methods: **yes**
 - Create network endpoint group (NEG) for serverless ingress: **yes**
 - Default deploy method? (cloudrun or gke): **Cloud Run**
 
-Add a HTTP Load Balancer for Cloud Run service(s)
+Add an HTTP Load Balancer for Cloud Run service(s)
+
 ```
-sb add component terraform_httplb_cloudrun
+sb components add -t terraform_httplb_cloudrun terraform_httplb_cloudrun
 sb infra apply 3-httplb-cloudrun
 ```
 
 Build and deploy
+
 ```
 sb deploy
 ```
+
 - See other deployment options in [solutions_builder/modules](solutions_builder/modules).
 
+## CLI Usage
+
+For more information on how to use the CLI, please refer to the [CLI_USAGE.md](docs/CLI_USAGE.md).
 
 ## Additional Documentations
 
 You can find more documentations in [docs](docs) folder. In a nutshell, it covers the following:
+
 - [INSTALLATION.md](docs/INSTALLATION.md) - The overall installation guide.
 - [DEVELOPMENT.md](docs/DEVELOPMENT.md) - Development guide and code submission process.
 - [TROUBLESHOOTING.md](docs/TROUBLESHOOTING.md) - Development guide and code submission process.
 
-In the [docs/components](docs/components/) folder, it contains a few more guidance based on each component/feature available in this template.
-- [gke.md](docs/components/gke.md) covers the overall developmeng guidance on Google Kubernetes Engine.
+In the [docs/components](docs/components) folder, it contains a few more guidance based on each component/feature available in this template.
+
+- [gke.md](docs/components/gke.md) covers the overall development guidance on Google Kubernetes Engine.
 - [cloudrun.md](docs/components/cloudrun.md) covers the guidance if you want to deploy microservice to Cloud Run.
 
 ## FAQ
+
 - Who are the target audience/users for this Solutions Builder?
+
   - A: Any engineering team to start a new solution development project.
 
 - Can I choose to deploy microservice just to Cloud Run?
-  - A: Yes, please refer to [Setting up Google Cloud Project](README.md#setting-up-google-cloud-project) in this README.md to choose where to deploy microservices. Or you can refer to [INSTALLATION.md](docs/INSTALLATION.md) for more details.
+
+  - A: Yes, please refer to [INSTALLATION Guide](docs/INSTALLATION.md) for more details.
 
 - Can I use this template for non-Google or multi-Cloud environments?
-  - A: We design this Solutions Builder to work 100% out of the box with Google Cloud products. However you could customize the solution to meet your needs on multi-Cloud environment. See [Why Google Cloud](https://cloud.google.com/why-google-cloud) for details.
+  - A: We design this Solutions Builder to work 100% out of the box with Google Cloud products. However, you could customize the solution to meet your needs on multi-Cloud environment. See [Why Google Cloud](https://cloud.google.com/why-google-cloud) for details.
 
 ## Troubleshoot
 
-See [TROUBLESHOOTING.md](docs/TROUBLESHOOTING.md) for details.
+See [TROUBLESHOOTING Guide](docs/TROUBLESHOOTING.md) for details.
+
```


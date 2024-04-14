# Comparing `tmp/lungo_cli-0.2.3.tar.gz` & `tmp/lungo_cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lungo_cli-0.2.3.tar", max compression
+gzip compressed data, was "lungo_cli-0.3.0.tar", max compression
```

## Comparing `lungo_cli-0.2.3.tar` & `lungo_cli-0.3.0.tar`

### file list

```diff
@@ -1,228 +1,276 @@
--rw-r--r--   0        0        0     1075 2024-02-15 20:41:34.767178 lungo_cli-0.2.3/LICENSE
--rw-r--r--   0        0        0     2396 2024-02-15 20:41:34.767178 lungo_cli-0.2.3/README.md
--rw-r--r--   0        0        0     1139 2024-02-15 20:41:34.767178 lungo_cli-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-15 20:41:34.767178 lungo_cli-0.2.3/src/lungo_cli/__init__.py
--rw-r--r--   0        0        0        0 2024-02-15 20:41:34.767178 lungo_cli-0.2.3/src/lungo_cli/app/__init__.py
--rw-r--r--   0        0        0     1129 2024-02-15 20:41:34.767178 lungo_cli-0.2.3/src/lungo_cli/app/main.py
--rw-r--r--   0        0        0     1301 2024-02-15 20:41:34.767178 lungo_cli-0.2.3/src/lungo_cli/app/state.py
--rw-r--r--   0        0        0        0 2024-02-15 20:41:34.767178 lungo_cli-0.2.3/src/lungo_cli/commands/__init__.py
--rw-r--r--   0        0        0      806 2024-02-15 20:41:34.767178 lungo_cli-0.2.3/src/lungo_cli/commands/base.py
--rw-r--r--   0        0        0      434 2024-02-15 20:41:34.767178 lungo_cli-0.2.3/src/lungo_cli/commands/check.py
--rw-r--r--   0        0        0      960 2024-02-15 20:41:34.767178 lungo_cli-0.2.3/src/lungo_cli/commands/down.py
--rw-r--r--   0        0        0     1890 2024-02-15 20:41:34.767178 lungo_cli-0.2.3/src/lungo_cli/commands/up.py
--rw-r--r--   0        0        0        0 2024-02-15 20:41:34.767178 lungo_cli-0.2.3/src/lungo_cli/core/__init__.py
--rw-r--r--   0        0        0    11170 2024-02-15 20:41:34.767178 lungo_cli-0.2.3/src/lungo_cli/core/app.py
--rw-r--r--   0        0        0     6202 2024-02-15 20:41:34.767178 lungo_cli-0.2.3/src/lungo_cli/core/console.py
--rw-r--r--   0        0        0      741 2024-02-15 20:41:34.767178 lungo_cli-0.2.3/src/lungo_cli/core/constants.py
--rw-r--r--   0        0        0     6828 2024-02-15 20:41:34.767178 lungo_cli-0.2.3/src/lungo_cli/core/container.py
--rw-r--r--   0        0        0     3855 2024-02-15 20:41:34.767178 lungo_cli-0.2.3/src/lungo_cli/core/context.py
--rw-r--r--   0        0        0    10097 2024-02-15 20:41:34.767178 lungo_cli-0.2.3/src/lungo_cli/core/database.py
--rw-r--r--   0        0        0     5101 2024-02-15 20:41:34.767178 lungo_cli-0.2.3/src/lungo_cli/core/file.py
--rw-r--r--   0        0        0     2599 2024-02-15 20:41:34.767178 lungo_cli-0.2.3/src/lungo_cli/core/network.py
--rw-r--r--   0        0        0     1701 2024-02-15 20:41:34.767178 lungo_cli-0.2.3/src/lungo_cli/core/renderer.py
--rw-r--r--   0        0        0     5890 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/core/storage.py
--rw-r--r--   0        0        0        0 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/helpers/__init__.py
--rw-r--r--   0        0        0      786 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/helpers/common.py
--rw-r--r--   0        0        0     1571 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/helpers/crypto.py
--rw-r--r--   0        0        0     1057 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/helpers/format.py
--rw-r--r--   0        0        0        0 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/models/__init__.py
--rw-r--r--   0        0        0     1215 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/models/base.py
--rw-r--r--   0        0        0     3451 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/models/config.py
--rw-r--r--   0        0        0      906 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/models/context.py
--rw-r--r--   0        0        0     1837 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/models/users.py
--rw-r--r--   0        0        0        0 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/__init__.py
--rw-r--r--   0        0        0    12849 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/compose.yaml.jinja
--rw-r--r--   0        0        0     1197 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/filebrowser/config_export.yaml
--rw-r--r--   0        0        0      156 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/filebrowser/settings.yaml
--rw-r--r--   0        0        0     1354 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/filebrowser/users_export.yaml.jinja
--rw-r--r--   0        0        0     2731 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/jupyterhub/config.py.jinja
--rw-r--r--   0        0        0      362 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/keto/config.yaml.jinja
--rw-r--r--   0        0        0     1733 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/kratos/config.yaml.jinja
--rw-r--r--   0        0        0    14238 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.body.gotmpl.jinja
--rw-r--r--   0        0        0      410 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.body.plaintext.gotmpl.jinja
--rw-r--r--   0        0        0       50 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.subject.gotmpl.jinja
--rw-r--r--   0        0        0     2633 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/kratos/user.schema.json
--rw-r--r--   0        0        0     1270 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx/conf.d/default.conf.jinja
--rw-r--r--   0        0        0       92 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx/custom.d/jit.conf
--rw-r--r--   0        0        0     1310 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx/sites/filebrowser.conf.jinja
--rw-r--r--   0        0        0     1203 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx/sites/jupyterhub.conf.jinja
--rw-r--r--   0        0        0      911 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx/sites/oathkeeper.conf
--rw-r--r--   0        0        0     1170 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx/sites/privatebin.conf.jinja
--rw-r--r--   0        0        0     1403 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx/sites/rstudio.conf.jinja
--rw-r--r--   0        0        0      411 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx/sites/xray.conf.jinja
--rw-r--r--   0        0        0      712 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx/snippets/auth.conf
--rw-r--r--   0        0        0      592 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx/snippets/proxy.conf
--rw-r--r--   0        0        0      848 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx/snippets/upstreams.conf.jinja
--rw-r--r--   0        0        0     2185 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx_gateway/conf.d/default.conf.jinja
--rw-r--r--   0        0        0       92 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx_gateway/custom.d/jit.conf
--rw-r--r--   0        0        0       90 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx_gateway/snippets/certificate.conf
--rw-r--r--   0        0        0     1586 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx_gateway/snippets/proxy.conf.jinja
--rw-r--r--   0        0        0     1609 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx_gateway/snippets/rate_limiting.conf.jinja
--rw-r--r--   0        0        0     1400 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/oathkeeper/access_rules.yaml.jinja
--rw-r--r--   0        0        0     1641 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/oathkeeper/config.yaml.jinja
--rw-r--r--   0        0        0     7466 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/privatebin/conf.php.jinja
--rw-r--r--   0        0        0      765 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/privatebin/site.conf
--rw-r--r--   0        0        0      103 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/rstudio/rserver.conf
--rw-r--r--   0        0        0       30 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/rstudio/rsession.conf
--rw-r--r--   0        0        0     1177 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/config/xray/config.json.jinja
--rw-r--r--   0        0        0      686 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/dockerfiles/filebrowser.Dockerfile.jinja
--rw-r--r--   0        0        0     1121 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/dockerfiles/jupyterhub.Dockerfile.jinja
--rw-r--r--   0        0        0      474 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/dockerfiles/keto_admin/compose.yaml.jinja
--rw-r--r--   0        0        0      819 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/dockerfiles/kratos_admin/compose.yaml.jinja
--rw-r--r--   0        0        0      857 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/dockerfiles/nginx.Dockerfile.jinja
--rw-r--r--   0        0        0      404 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/dockerfiles/privatebin.Dockerfile.jinja
--rw-r--r--   0        0        0      925 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/dockerfiles/rstudio.Dockerfile.jinja
--rw-r--r--   0        0        0     7464 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/excluded/config.yaml
--rw-r--r--   0        0        0       82 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/excluded/kratos/secrets.yaml.jinja
--rw-r--r--   0        0        0     1999 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/excluded/users.yaml
--rw-r--r--   0        0        0      426 2024-02-15 20:41:35.231176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/.editorconfig
--rw-r--r--   0        0        0       93 2024-02-15 20:41:35.223176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/.git
--rw-r--r--   0        0        0      519 2024-02-15 20:41:35.231176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/.gitattributes
--rw-r--r--   0        0        0      128 2024-02-15 20:41:35.231176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CODEOWNERS
--rw-r--r--   0        0        0      121 2024-02-15 20:41:35.231176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     5476 2024-02-15 20:41:35.231176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      323 2024-02-15 20:41:35.231176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/.github/FUNDING.yml
--rw-r--r--   0        0        0      105 2024-02-15 20:41:35.231176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/.github/dependabot.yml
--rw-r--r--   0        0        0      958 2024-02-15 20:41:35.231176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/auto-merge.yml
--rw-r--r--   0        0        0      322 2024-02-15 20:41:35.231176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1284 2024-02-15 20:41:35.231176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/server.yml
--rw-r--r--   0        0        0       91 2024-02-15 20:41:35.231176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/.gitignore
--rw-r--r--   0        0        0    41306 2024-02-15 20:41:35.231176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/CHANGELOG.md
--rw-r--r--   0        0        0     1043 2024-02-15 20:41:35.231176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/LICENSE.txt
--rw-r--r--   0        0        0     4817 2024-02-15 20:41:35.231176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/README.md
--rw-r--r--   0        0        0      763 2024-02-15 20:41:35.231176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/.default.conf
--rw-r--r--   0        0        0      932 2024-02-15 20:41:35.231176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/no-ssl.default.conf
--rw-r--r--   0        0        0     1434 2024-02-15 20:41:35.231176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/example.com.conf
--rw-r--r--   0        0        0     1133 2024-02-15 20:41:35.231176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/no-ssl.example.com.conf
--rw-r--r--   0        0        0      314 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/basic.conf
--rw-r--r--   0        0        0      739 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/requests.conf
--rw-r--r--   0        0        0      761 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/resource_timing.conf
--rw-r--r--   0        0        0      385 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/errors/custom_errors.conf
--rw-r--r--   0        0        0     1706 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/security_file_access.conf
--rw-r--r--   0        0        0      701 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_filename-based_cache_busting.conf
--rw-r--r--   0        0        0      685 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_svgz-compression.conf
--rw-r--r--   0        0        0     1029 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/character_encodings.conf
--rw-r--r--   0        0        0      650 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/media_types.conf
--rw-r--r--   0        0        0     1198 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/content-security-policy.conf
--rw-r--r--   0        0        0     2102 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/cross-origin-policy.conf
--rw-r--r--   0        0        0     1121 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/permissions-policy.conf
--rw-r--r--   0        0        0     1135 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/referrer-policy.conf
--rw-r--r--   0        0        0      396 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/server_software_information.conf
--rw-r--r--   0        0        0     2008 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/strict-transport-security.conf
--rw-r--r--   0        0        0      871 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-content-type-options.conf
--rw-r--r--   0        0        0     1800 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-frame-options.conf
--rw-r--r--   0        0        0     1136 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/certificate_files.conf
--rw-r--r--   0        0        0     1235 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ocsp_stapling.conf
--rw-r--r--   0        0        0      797 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_balanced.conf
--rw-r--r--   0        0        0     1818 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_strict.conf
--rw-r--r--   0        0        0     1880 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ssl_engine.conf
--rw-r--r--   0        0        0     2202 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-control.conf
--rw-r--r--   0        0        0     1484 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-file-descriptors.conf
--rw-r--r--   0        0        0     2220 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache_expiration.conf
--rw-r--r--   0        0        0     2049 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/compression.conf
--rw-r--r--   0        0        0     1435 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/content_transformation.conf
--rw-r--r--   0        0        0      732 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_brotli.conf
--rw-r--r--   0        0        0      572 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_gzip.conf
--rw-r--r--   0        0        0     5775 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/mime.types
--rw-r--r--   0        0        0     7293 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/nginx.conf
--rw-r--r--   0        0        0      399 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/default.conf
--rw-r--r--   0        0        0      678 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/secure.server.localhost.conf
--rw-r--r--   0        0        0      782 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/server.localhost.conf
--rw-r--r--   0        0        0      126 2024-02-15 20:41:35.235176 lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/www-server.localhost.conf
--rw-r--r--   0        0        0      167 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/web/.dockerignore
--rw-r--r--   0        0        0      160 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/web/.eslintignore
--rw-r--r--   0        0        0      702 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/web/.eslintrc.cjs
--rw-r--r--   0        0        0       19 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/web/.npmrc
--rw-r--r--   0        0        0      160 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/web/.prettierignore
--rw-r--r--   0        0        0      351 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/web/.prettierrc
--rw-r--r--   0        0        0      411 2024-02-15 20:41:34.771178 lungo_cli-0.2.3/src/lungo_cli/resources/web/Dockerfile.jinja
--rw-r--r--   0        0        0    40315 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/assets/schemas/keto.openapi.json
--rw-r--r--   0        0        0   274746 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/assets/schemas/kratos.openapi.json
--rw-r--r--   0        0        0     1763 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/package.json
--rw-r--r--   0        0        0    98280 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/pnpm-lock.yaml
--rw-r--r--   0        0        0      264 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/postcss.config.cjs
--rw-r--r--   0        0        0      270 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/app.d.ts
--rw-r--r--   0        0        0      378 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/app.html
--rw-r--r--   0        0        0     1875 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/app.pcss
--rw-r--r--   0        0        0      248 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/hooks.server.ts
--rw-r--r--   0        0        0     2483 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/actions.ts
--rw-r--r--   0        0        0     5750 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/components/AppShell.svelte
--rw-r--r--   0        0        0      657 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/components/Avatar.svelte
--rw-r--r--   0        0        0     1140 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/components/CodeBlock.svelte
--rw-r--r--   0        0        0     7083 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/components/FormBuilder.svelte
--rw-r--r--   0        0        0      477 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/components/HeroFrame.svelte
--rw-r--r--   0        0        0      618 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/components/LoadingIndicator.svelte
--rw-r--r--   0        0        0     1395 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/components/NavRail.svelte
--rw-r--r--   0        0        0      822 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/components/PasswordInput.svelte
--rw-r--r--   0        0        0     6300 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/components/PatchedInlineFrame.svelte
--rw-r--r--   0        0        0     2032 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/components/SwappableIcon.svelte
--rw-r--r--   0        0        0     2901 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/components/ThemeSelector.svelte
--rw-r--r--   0        0        0      686 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/components/index.ts
--rw-r--r--   0        0        0      551 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/constants.ts
--rw-r--r--   0        0        0     2166 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/Account.svelte
--rw-r--r--   0        0        0      414 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/BaseIcon.svelte
--rw-r--r--   0        0        0      432 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/Check.svelte
--rw-r--r--   0        0        0     1031 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/Close.svelte
--rw-r--r--   0        0        0     1337 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/DarkMode.svelte
--rw-r--r--   0        0        0      427 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/Expand.svelte
--rw-r--r--   0        0        0      783 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/FolderOutline.svelte
--rw-r--r--   0        0        0      725 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/FolderSolid.svelte
--rw-r--r--   0        0        0      522 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/Fullscreen.svelte
--rw-r--r--   0        0        0     2016 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/Jupyter.svelte
--rw-r--r--   0        0        0     3326 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/LightMode.svelte
--rw-r--r--   0        0        0      617 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/Logout.svelte
--rw-r--r--   0        0        0     1182 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/Menu.svelte
--rw-r--r--   0        0        0     2124 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/NetworkLock.svelte
--rw-r--r--   0        0        0      691 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/NoteOutline.svelte
--rw-r--r--   0        0        0      663 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/NoteSolid.svelte
--rw-r--r--   0        0        0     1888 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/ProxyOutline.svelte
--rw-r--r--   0        0        0     1799 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/ProxySolid.svelte
--rw-r--r--   0        0        0     1811 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/RStudioOutline.svelte
--rw-r--r--   0        0        0     1554 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/RStudioSolid.svelte
--rw-r--r--   0        0        0     1707 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/Reset.svelte
--rw-r--r--   0        0        0     2164 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/Settings.svelte
--rw-r--r--   0        0        0     1328 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/TerminalOutline.svelte
--rw-r--r--   0        0        0     1302 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/TerminalSolid.svelte
--rw-r--r--   0        0        0     1861 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/VisibilityOff.svelte
--rw-r--r--   0        0        0     1476 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/VisibilityOn.svelte
--rw-r--r--   0        0        0     1572 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/index.ts
--rw-r--r--   0        0        0     3707 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/server/api.ts
--rw-r--r--   0        0        0      421 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/server/constants.ts
--rw-r--r--   0        0        0      160 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/server/types.ts
--rw-r--r--   0        0        0      758 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/server/utils.ts
--rw-r--r--   0        0        0     1397 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/stores.ts
--rw-r--r--   0        0        0     1307 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/types/common.ts
--rw-r--r--   0        0        0      317 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/types/index.ts
--rw-r--r--   0        0        0    26759 2024-02-15 20:41:34.775178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/types/keto.d.ts
--rw-r--r--   0        0        0   276139 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/types/kratos.d.ts
--rw-r--r--   0        0        0      532 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/types/user.d.ts
--rw-r--r--   0        0        0     2514 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/utils.ts
--rw-r--r--   0        0        0      179 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(account)/+layout.svelte
--rw-r--r--   0        0        0     4712 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(account)/account/+page.server.ts
--rw-r--r--   0        0        0      322 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(account)/account/+page.svelte
--rw-r--r--   0        0        0     6757 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(account)/login/+page.server.ts
--rw-r--r--   0        0        0      518 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(account)/login/+page.svelte
--rw-r--r--   0        0        0      416 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(account)/logout/+server.ts
--rw-r--r--   0        0        0     5184 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(account)/recover/+page.server.ts
--rw-r--r--   0        0        0      356 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(account)/recover/+page.svelte
--rw-r--r--   0        0        0      353 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(apps)/+layout.svelte
--rw-r--r--   0        0        0     1075 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(apps)/+page.svelte
--rw-r--r--   0        0        0      535 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(apps)/app/+layout.server.ts
--rw-r--r--   0        0        0      136 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(apps)/app/+page.server.ts
--rw-r--r--   0        0        0      110 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(apps)/app/[...url]/+page.svelte
--rw-r--r--   0        0        0     1406 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(apps)/app/jupyterhub/+layout.server.ts
--rw-r--r--   0        0        0      110 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(apps)/app/jupyterhub/[...url]/+page.svelte
--rw-r--r--   0        0        0     2322 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(apps)/app/rstudio/+layout.server.ts
--rw-r--r--   0        0        0      110 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(apps)/app/rstudio/[...url]/+page.svelte
--rw-r--r--   0        0        0      399 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(apps)/app/xray/+page.server.ts
--rw-r--r--   0        0        0     6965 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(apps)/app/xray/+page.svelte
--rw-r--r--   0        0        0      969 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/+error.svelte
--rw-r--r--   0        0        0     3071 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/+layout.server.ts
--rw-r--r--   0        0        0      847 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/+layout.svelte
--rw-r--r--   0        0        0   146031 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/static/cover.jpg
--rw-r--r--   0        0        0    25573 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/static/favicon.png
--rw-r--r--   0        0        0      295 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/svelte.config.js
--rw-r--r--   0        0        0     1835 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/tailwind.config.cjs
--rw-r--r--   0        0        0      601 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/tsconfig.json
--rw-r--r--   0        0        0      145 2024-02-15 20:41:34.779178 lungo_cli-0.2.3/src/lungo_cli/resources/web/vite.config.ts
--rw-r--r--   0        0        0     3399 1970-01-01 00:00:00.000000 lungo_cli-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-04-14 19:09:33.552501 lungo_cli-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2410 2024-04-14 19:09:33.552501 lungo_cli-0.3.0/README.md
+-rw-r--r--   0        0        0     1116 2024-04-14 19:09:33.552501 lungo_cli-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-14 19:09:33.552501 lungo_cli-0.3.0/src/lungo_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 19:09:33.552501 lungo_cli-0.3.0/src/lungo_cli/app/__init__.py
+-rw-r--r--   0        0        0     1264 2024-04-14 19:09:33.552501 lungo_cli-0.3.0/src/lungo_cli/app/main.py
+-rw-r--r--   0        0        0     1551 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/app/state.py
+-rw-r--r--   0        0        0        0 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/commands/__init__.py
+-rw-r--r--   0        0        0      743 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/commands/base.py
+-rw-r--r--   0        0        0      478 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/commands/check.py
+-rw-r--r--   0        0        0      922 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/commands/down.py
+-rw-r--r--   0        0        0     1244 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/commands/install.py
+-rw-r--r--   0        0        0     3370 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/commands/list.py
+-rw-r--r--   0        0        0     1241 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/commands/uninstall.py
+-rw-r--r--   0        0        0     2705 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/commands/up.py
+-rw-r--r--   0        0        0        0 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/__init__.py
+-rw-r--r--   0        0        0    12436 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/app.py
+-rw-r--r--   0        0        0     5973 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/console.py
+-rw-r--r--   0        0        0      569 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/constants.py
+-rw-r--r--   0        0        0     7390 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/container.py
+-rw-r--r--   0        0        0     3174 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/context.py
+-rw-r--r--   0        0        0    10206 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/database.py
+-rw-r--r--   0        0        0     5978 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/file.py
+-rw-r--r--   0        0        0     2599 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/network.py
+-rw-r--r--   0        0        0    11815 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/plugin.py
+-rw-r--r--   0        0        0     2452 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/renderer.py
+-rw-r--r--   0        0        0     5901 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/storage.py
+-rw-r--r--   0        0        0        0 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/helpers/__init__.py
+-rw-r--r--   0        0        0     1275 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/helpers/common.py
+-rw-r--r--   0        0        0     1873 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/helpers/crypto.py
+-rw-r--r--   0        0        0     1071 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/helpers/format.py
+-rw-r--r--   0        0        0        0 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/models/__init__.py
+-rw-r--r--   0        0        0     1002 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/models/base.py
+-rw-r--r--   0        0        0     2876 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/models/config.py
+-rw-r--r--   0        0        0      482 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/models/context.py
+-rw-r--r--   0        0        0      588 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/models/plugin.py
+-rw-r--r--   0        0        0     1865 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/models/users.py
+-rw-r--r--   0        0        0        0 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/__init__.py
+-rw-r--r--   0        0        0      686 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/Dockerfile.jinja
+-rw-r--r--   0        0        0      280 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/README.md
+-rw-r--r--   0        0        0     1958 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/compose/compose.yaml.jinja
+-rw-r--r--   0        0        0     1197 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/config/config_export.yaml
+-rw-r--r--   0        0        0      156 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/config/settings.yaml
+-rw-r--r--   0        0        0     1354 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/config/users_export.yaml.jinja
+-rw-r--r--   0        0        0     1254 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/nginx/site.conf.jinja
+-rw-r--r--   0        0        0      125 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/nginx/upstream.conf.jinja
+-rw-r--r--   0        0        0      864 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/oathkeeper/access_rules.yaml.jinja
+-rw-r--r--   0        0        0      485 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/plugin.py
+-rw-r--r--   0        0        0      792 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/web/lib/icons/FolderOutline.svelte
+-rw-r--r--   0        0        0      734 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/web/lib/icons/FolderSolid.svelte
+-rw-r--r--   0        0        0      100 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/web/routes/[...url]/+page.svelte
+-rw-r--r--   0        0        0     1121 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/Dockerfile.jinja
+-rw-r--r--   0        0        0      427 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/README.md
+-rw-r--r--   0        0        0     1457 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/compose/compose.yaml.jinja
+-rw-r--r--   0        0        0     2734 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/config/config.py.jinja
+-rw-r--r--   0        0        0     1148 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/nginx/site.conf.jinja
+-rw-r--r--   0        0        0      124 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/nginx/upstream.conf.jinja
+-rw-r--r--   0        0        0     1624 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/plugin.py
+-rw-r--r--   0        0        0       20 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/web/dependencies.txt
+-rw-r--r--   0        0        0     2025 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/web/lib/icons/Jupyter.svelte
+-rw-r--r--   0        0        0       76 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/web/lib/server/constants.server.ts
+-rw-r--r--   0        0        0      144 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/web/lib/server/constants.server.ts.jinja
+-rw-r--r--   0        0        0     1204 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/web/routes/+layout.server.ts
+-rw-r--r--   0        0        0      100 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/web/routes/[...url]/+page.svelte
+-rw-r--r--   0        0        0      384 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/Dockerfile.jinja
+-rw-r--r--   0        0        0      275 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/README.md
+-rw-r--r--   0        0        0      494 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/compose/compose.yaml.jinja
+-rw-r--r--   0        0        0     7466 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/config/conf.php.jinja
+-rw-r--r--   0        0        0      765 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/config/site.conf
+-rw-r--r--   0        0        0     1115 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/nginx/site.conf.jinja
+-rw-r--r--   0        0        0      124 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/nginx/upstream.conf.jinja
+-rw-r--r--   0        0        0      865 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/oathkeeper/access_rules.yaml.jinja
+-rw-r--r--   0        0        0      691 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/plugin.py
+-rw-r--r--   0        0        0      700 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/web/lib/icons/NoteOutline.svelte
+-rw-r--r--   0        0        0      672 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/web/lib/icons/NoteSolid.svelte
+-rw-r--r--   0        0        0      100 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/web/routes/[...url]/+page.svelte
+-rw-r--r--   0        0        0      925 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/Dockerfile.jinja
+-rw-r--r--   0        0        0      418 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/README.md
+-rw-r--r--   0        0        0     1305 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/compose/compose.yaml.jinja
+-rw-r--r--   0        0        0      103 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/config/rserver.conf
+-rw-r--r--   0        0        0       30 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/config/rsession.conf
+-rw-r--r--   0        0        0     1351 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/nginx/site.conf.jinja
+-rw-r--r--   0        0        0      121 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/nginx/upstream.conf.jinja
+-rw-r--r--   0        0        0     1309 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/plugin.py
+-rw-r--r--   0        0        0       20 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/web/dependencies.txt
+-rw-r--r--   0        0        0     1820 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/web/lib/icons/RStudioOutline.svelte
+-rw-r--r--   0        0        0     1563 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/web/lib/icons/RStudioSolid.svelte
+-rw-r--r--   0        0        0       70 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/web/lib/server/constants.server.ts
+-rw-r--r--   0        0        0      132 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/web/lib/server/constants.server.ts.jinja
+-rw-r--r--   0        0        0     2118 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/web/routes/+layout.server.ts
+-rw-r--r--   0        0        0      100 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/web/routes/[...url]/+page.svelte
+-rw-r--r--   0        0        0      991 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/README.md
+-rw-r--r--   0        0        0      502 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/compose/compose.yaml.jinja
+-rw-r--r--   0        0        0     1174 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/config/config.json.jinja
+-rw-r--r--   0        0        0      362 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/nginx/site.conf.jinja
+-rw-r--r--   0        0        0      118 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/nginx/upstream.conf.jinja
+-rw-r--r--   0        0        0     1588 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/plugin.py
+-rw-r--r--   0        0        0       33 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/dependencies.txt
+-rw-r--r--   0        0        0     1594 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/lib/components/CodeBlock.svelte
+-rw-r--r--   0        0        0     2133 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/lib/icons/NetworkLock.svelte
+-rw-r--r--   0        0        0     1897 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/lib/icons/ProxyOutline.svelte
+-rw-r--r--   0        0        0     1808 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/lib/icons/ProxySolid.svelte
+-rw-r--r--   0        0        0      205 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/lib/server/constants.server.ts
+-rw-r--r--   0        0        0      437 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/lib/server/constants.server.ts.jinja
+-rw-r--r--   0        0        0      775 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/routes/+page.server.ts
+-rw-r--r--   0        0        0     6649 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/routes/+page.svelte
+-rw-r--r--   0        0        0        0 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/__init__.py
+-rw-r--r--   0        0        0     5623 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/assets/config_references/config.yaml
+-rw-r--r--   0        0        0     1995 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/assets/config_references/users.yaml
+-rw-r--r--   0        0        0     6798 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/compose.yaml.jinja
+-rw-r--r--   0        0        0      363 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/keto/config.yaml.jinja
+-rw-r--r--   0        0        0     2116 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/config.yaml.jinja
+-rw-r--r--   0        0        0    14236 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/email_templates/login_code/valid/email.body.gotmpl.jinja
+-rw-r--r--   0        0        0      408 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/email_templates/login_code/valid/email.body.plaintext.gotmpl.jinja
+-rw-r--r--   0        0        0       51 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/email_templates/login_code/valid/email.subject.gotmpl.jinja
+-rw-r--r--   0        0        0    14238 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.body.gotmpl.jinja
+-rw-r--r--   0        0        0      410 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.body.plaintext.gotmpl.jinja
+-rw-r--r--   0        0        0       50 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.subject.gotmpl.jinja
+-rw-r--r--   0        0        0     2801 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/user.schema.json
+-rw-r--r--   0        0        0     1281 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx/conf.d/default.conf.jinja
+-rw-r--r--   0        0        0       92 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx/custom.d/jit.conf
+-rw-r--r--   0        0        0      203 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx/sites/apps.conf.jinja
+-rw-r--r--   0        0        0      911 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx/sites/oathkeeper.conf
+-rw-r--r--   0        0        0      712 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx/snippets/auth.conf
+-rw-r--r--   0        0        0      592 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx/snippets/proxy.conf
+-rw-r--r--   0        0        0      375 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx/snippets/upstreams.conf.jinja
+-rw-r--r--   0        0        0     2257 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx_gateway/conf.d/default.conf.jinja
+-rw-r--r--   0        0        0       92 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx_gateway/custom.d/jit.conf
+-rw-r--r--   0        0        0       90 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx_gateway/snippets/certificate.conf
+-rw-r--r--   0        0        0     1586 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx_gateway/snippets/proxy.conf.jinja
+-rw-r--r--   0        0        0     1609 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx_gateway/snippets/rate_limiting.conf.jinja
+-rw-r--r--   0        0        0     1303 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/oathkeeper/access_rules.yaml.jinja
+-rw-r--r--   0        0        0     1634 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/oathkeeper/config.yaml.jinja
+-rw-r--r--   0        0        0      474 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/dockerfiles/keto_admin/compose.yaml.jinja
+-rw-r--r--   0        0        0      820 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/dockerfiles/kratos_admin/compose.yaml.jinja
+-rw-r--r--   0        0        0      859 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/dockerfiles/nginx.Dockerfile.jinja
+-rw-r--r--   0        0        0       82 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/excluded/kratos/secrets.yaml.jinja
+-rw-r--r--   0        0        0      426 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.editorconfig
+-rw-r--r--   0        0        0       93 2024-04-14 19:09:33.992508 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.git
+-rw-r--r--   0        0        0      519 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.gitattributes
+-rw-r--r--   0        0        0      128 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CODEOWNERS
+-rw-r--r--   0        0        0      121 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     5476 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      323 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/FUNDING.yml
+-rw-r--r--   0        0        0      105 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/dependabot.yml
+-rw-r--r--   0        0        0      958 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/auto-merge.yml
+-rw-r--r--   0        0        0      322 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1284 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/server.yml
+-rw-r--r--   0        0        0       91 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.gitignore
+-rw-r--r--   0        0        0    41306 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/CHANGELOG.md
+-rw-r--r--   0        0        0     1043 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/LICENSE.txt
+-rw-r--r--   0        0        0     4817 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/README.md
+-rw-r--r--   0        0        0      763 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/.default.conf
+-rw-r--r--   0        0        0      932 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/no-ssl.default.conf
+-rw-r--r--   0        0        0     1434 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/example.com.conf
+-rw-r--r--   0        0        0     1133 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/no-ssl.example.com.conf
+-rw-r--r--   0        0        0      314 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/basic.conf
+-rw-r--r--   0        0        0      739 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/requests.conf
+-rw-r--r--   0        0        0      761 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/resource_timing.conf
+-rw-r--r--   0        0        0      385 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/errors/custom_errors.conf
+-rw-r--r--   0        0        0     1706 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/security_file_access.conf
+-rw-r--r--   0        0        0      701 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_filename-based_cache_busting.conf
+-rw-r--r--   0        0        0      685 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_svgz-compression.conf
+-rw-r--r--   0        0        0     1029 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/character_encodings.conf
+-rw-r--r--   0        0        0      650 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/media_types.conf
+-rw-r--r--   0        0        0     1198 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/content-security-policy.conf
+-rw-r--r--   0        0        0     2102 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/cross-origin-policy.conf
+-rw-r--r--   0        0        0     1121 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/permissions-policy.conf
+-rw-r--r--   0        0        0     1135 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/referrer-policy.conf
+-rw-r--r--   0        0        0      396 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/server_software_information.conf
+-rw-r--r--   0        0        0     2008 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/strict-transport-security.conf
+-rw-r--r--   0        0        0      871 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-content-type-options.conf
+-rw-r--r--   0        0        0     1800 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-frame-options.conf
+-rw-r--r--   0        0        0     1136 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/certificate_files.conf
+-rw-r--r--   0        0        0     1235 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ocsp_stapling.conf
+-rw-r--r--   0        0        0      797 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_balanced.conf
+-rw-r--r--   0        0        0     1818 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_strict.conf
+-rw-r--r--   0        0        0     1880 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ssl_engine.conf
+-rw-r--r--   0        0        0     2202 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-control.conf
+-rw-r--r--   0        0        0     1484 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-file-descriptors.conf
+-rw-r--r--   0        0        0     2220 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache_expiration.conf
+-rw-r--r--   0        0        0     2049 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/compression.conf
+-rw-r--r--   0        0        0     1435 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/content_transformation.conf
+-rw-r--r--   0        0        0      732 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_brotli.conf
+-rw-r--r--   0        0        0      572 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_gzip.conf
+-rw-r--r--   0        0        0     5775 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/mime.types
+-rw-r--r--   0        0        0     7293 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/nginx.conf
+-rw-r--r--   0        0        0      399 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/default.conf
+-rw-r--r--   0        0        0      678 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/secure.server.localhost.conf
+-rw-r--r--   0        0        0      782 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/server.localhost.conf
+-rw-r--r--   0        0        0      126 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/www-server.localhost.conf
+-rw-r--r--   0        0        0      161 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/web/.dockerignore
+-rw-r--r--   0        0        0      160 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/web/.eslintignore
+-rw-r--r--   0        0        0      702 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/web/.eslintrc.cjs
+-rw-r--r--   0        0        0       19 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/web/.npmrc
+-rw-r--r--   0        0        0      160 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/web/.prettierignore
+-rw-r--r--   0        0        0      351 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/web/.prettierrc
+-rw-r--r--   0        0        0      773 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/web/Dockerfile.jinja
+-rw-r--r--   0        0        0    40573 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/assets/schemas/keto.openapi.json
+-rw-r--r--   0        0        0   300951 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/assets/schemas/kratos.openapi.json
+-rw-r--r--   0        0        0     1728 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/package.json
+-rw-r--r--   0        0        0   115548 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/pnpm-lock.yaml
+-rw-r--r--   0        0        0      264 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/postcss.config.cjs
+-rw-r--r--   0        0        0      304 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/app.d.ts
+-rw-r--r--   0        0        0      352 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/app.html
+-rw-r--r--   0        0        0     1736 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/app.pcss
+-rw-r--r--   0        0        0      248 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/hooks.server.ts
+-rw-r--r--   0        0        0     3137 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/actions.ts
+-rw-r--r--   0        0        0   146031 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/assets/cover.jpg
+-rw-r--r--   0        0        0     1713 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/AccountDropdown.svelte
+-rw-r--r--   0        0        0     5068 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/AppShell.svelte
+-rw-r--r--   0        0        0     7325 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/FormBuilder.svelte
+-rw-r--r--   0        0        0      556 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/HeroFrame.svelte
+-rw-r--r--   0        0        0      618 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/LoadingIndicator.svelte
+-rw-r--r--   0        0        0     1525 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/NavRail.svelte
+-rw-r--r--   0        0        0      887 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/PasswordInput.svelte
+-rw-r--r--   0        0        0     6343 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/PatchedIFrame.svelte
+-rw-r--r--   0        0        0      608 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/SwappableIcon.svelte
+-rw-r--r--   0        0        0     1691 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/ThemeSelector.svelte
+-rw-r--r--   0        0        0     1719 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/ThemeSelectorDropdown.svelte
+-rw-r--r--   0        0        0      566 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/index.ts
+-rw-r--r--   0        0        0      237 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/constants.ts
+-rw-r--r--   0        0        0     2166 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Account.svelte
+-rw-r--r--   0        0        0      414 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/BaseIcon.svelte
+-rw-r--r--   0        0        0      432 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Check.svelte
+-rw-r--r--   0        0        0     1031 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Close.svelte
+-rw-r--r--   0        0        0     1337 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/DarkMode.svelte
+-rw-r--r--   0        0        0      427 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Expand.svelte
+-rw-r--r--   0        0        0      522 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Fullscreen.svelte
+-rw-r--r--   0        0        0     3326 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/LightMode.svelte
+-rw-r--r--   0        0        0      617 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Logout.svelte
+-rw-r--r--   0        0        0     1182 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Menu.svelte
+-rw-r--r--   0        0        0     1259 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/QuestionMark.svelte
+-rw-r--r--   0        0        0     1707 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Reset.svelte
+-rw-r--r--   0        0        0     2164 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Settings.svelte
+-rw-r--r--   0        0        0     1861 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/VisibilityOff.svelte
+-rw-r--r--   0        0        0     1476 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/VisibilityOn.svelte
+-rw-r--r--   0        0        0      836 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/index.ts
+-rw-r--r--   0        0        0      158 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/server/constants.ts
+-rw-r--r--   0        0        0      906 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/server/utils/api.ts
+-rw-r--r--   0        0        0       98 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/server/utils/index.ts
+-rw-r--r--   0        0        0      109 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/server/utils/stubs.ts
+-rw-r--r--   0        0        0      480 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/server/utils/stubs.ts.jinja
+-rw-r--r--   0        0        0     2312 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/stores.ts
+-rw-r--r--   0        0        0      307 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/types/common.ts
+-rw-r--r--   0        0        0      247 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/types/index.ts
+-rw-r--r--   0        0        0    31445 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/types/keto.d.ts
+-rw-r--r--   0        0        0   298809 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/types/kratos.d.ts
+-rw-r--r--   0        0        0      511 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/types/user.d.ts
+-rw-r--r--   0        0        0     2463 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/utils/api.ts
+-rw-r--r--   0        0        0      483 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/utils/app.ts
+-rw-r--r--   0        0        0     2348 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/utils/common.ts
+-rw-r--r--   0        0        0      316 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/utils/index.ts
+-rw-r--r--   0        0        0      225 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/utils/stubs.ts
+-rw-r--r--   0        0        0     1130 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/utils/stubs.ts.jinja
+-rw-r--r--   0        0        0      289 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/+layout.svelte
+-rw-r--r--   0        0        0     4621 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/account/+page.server.ts
+-rw-r--r--   0        0        0      335 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/account/+page.svelte
+-rw-r--r--   0        0        0     6932 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/login/+page.server.ts
+-rw-r--r--   0        0        0      590 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/login/+page.svelte
+-rw-r--r--   0        0        0      367 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/logout/+server.ts
+-rw-r--r--   0        0        0     5081 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/recover/+page.server.ts
+-rw-r--r--   0        0        0      369 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/recover/+page.svelte
+-rw-r--r--   0        0        0      463 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(apps)/+layout.svelte
+-rw-r--r--   0        0        0     1277 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(apps)/+page.svelte
+-rw-r--r--   0        0        0      448 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(apps)/app/+layout.server.ts
+-rw-r--r--   0        0        0      130 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(apps)/app/+page.server.ts
+-rw-r--r--   0        0        0     1008 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/+error.svelte
+-rw-r--r--   0        0        0     2327 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/+layout.server.ts
+-rw-r--r--   0        0        0      963 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/+layout.svelte
+-rw-r--r--   0        0        0    25573 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/static/favicon.png
+-rw-r--r--   0        0        0      276 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/svelte.config.js
+-rw-r--r--   0        0        0     1835 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/tailwind.config.cjs
+-rw-r--r--   0        0        0      601 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/tsconfig.json
+-rw-r--r--   0        0        0      219 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/vite.config.ts
+-rw-r--r--   0        0        0     3385 1970-01-01 00:00:00.000000 lungo_cli-0.3.0/PKG-INFO
```

### Comparing `lungo_cli-0.2.3/LICENSE` & `lungo_cli-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/README.md` & `lungo_cli-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 <br>
 
 ## Features
 
 - **Complete configurability** - manage everything declaratively through YAML files
 - **Seamless interoperability** - access all applications via a single sign-on portal
-- **Batteries included** - benefit from a diverse range of applications
+- **Batteries included** - extend functionality with both built-in and custom plugins
 - **Containerized solution** - designed to operate in a rootless Docker environment
 - **Security by default** - use HTTPS and secure server settings across the system
 
 ## Installation
 
 The recommended way to install Lungo is via [pipx](https://pypa.github.io/pipx/):
```

#### html2text {}

```diff
@@ -4,27 +4,27 @@
                                      ************
   A user-friendly home lab setup designed for small-to-mid-scale on-premises
                                    hosting.
                          _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_:_ _M_I_T_]
 
 ## Features - **Complete configurability** - manage everything declaratively
 through YAML files - **Seamless interoperability** - access all applications
-via a single sign-on portal - **Batteries included** - benefit from a diverse
-range of applications - **Containerized solution** - designed to operate in a
-rootless Docker environment - **Security by default** - use HTTPS and secure
-server settings across the system ## Installation The recommended way to
-install Lungo is via [pipx](https://pypa.github.io/pipx/): ```bash pipx install
-lungo-cli ``` Note that Lungo is built upon [Docker Compose](https://
-github.com/docker/compose). Before proceeding, please ensure that Docker is
-installed on your machine. Alternatively, you can use [Podman Compose](https://
-github.com/containers/podman-compose) with [Podman](https://podman.io/). You
-can also [use Docker Compose with Podman](https://fedoramagazine.org/use-
-docker-compose-with-podman-to-orchestrate-containers-on-fedora/). For
-instructions on setting up these tools, please refer to their respective
-documentation. ## Quickstart Copy the example configuration files to the
-platform-specific configuration directory. For example, on Linux, you can use
-the following command: ```bash mkdir -p ~/.config/lungo cp examples/
+via a single sign-on portal - **Batteries included** - extend functionality
+with both built-in and custom plugins - **Containerized solution** - designed
+to operate in a rootless Docker environment - **Security by default** - use
+HTTPS and secure server settings across the system ## Installation The
+recommended way to install Lungo is via [pipx](https://pypa.github.io/pipx/):
+```bash pipx install lungo-cli ``` Note that Lungo is built upon [Docker
+Compose](https://github.com/docker/compose). Before proceeding, please ensure
+that Docker is installed on your machine. Alternatively, you can use [Podman
+Compose](https://github.com/containers/podman-compose) with [Podman](https://
+podman.io/). You can also [use Docker Compose with Podman](https://
+fedoramagazine.org/use-docker-compose-with-podman-to-orchestrate-containers-on-
+fedora/). For instructions on setting up these tools, please refer to their
+respective documentation. ## Quickstart Copy the example configuration files to
+the platform-specific configuration directory. For example, on Linux, you can
+use the following command: ```bash mkdir -p ~/.config/lungo cp examples/
 * ~/.config/lungo ``` Edit the configuration files according to your
 preferences. Then, launch the Lungo service by running the following command:
 ```bash lungo up ``` ## Documentation For more information, please refer to the
 [documentation](https://raymond-u.github.io/lungo/). ## License This project is
 licensed under the MIT License. See [LICENSE](LICENSE) for details.
```

### Comparing `lungo_cli-0.2.3/pyproject.toml` & `lungo_cli-0.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 [tool.black]
 line-length = 120
 
 [tool.poetry]
 name = "lungo-cli"
-version = "0.2.3"
+version = "0.3.0"
 description = "A user-friendly home lab setup designed for small-to-mid-scale on-premises hosting."
 authors = ["raymond-u <36328498+raymond-u@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/raymond-u/lungo"
 documentation = "https://raymond-u.github.io/lungo/"
 keywords = ["homelab", "self-host"]
 packages = [{ include = "lungo_cli", from = "src" }]
 
 [tool.poetry.dependencies]
-python = "^3.11"
-cryptography = "^42.0.2"
-importlib-resources = "^6.0.1"
+python = "^3.12"
+aenum = "^3.1.15"
+cryptography = "^42.0.5"
 jinja2 = "^3.1.3"
+packaging = "^24.0"
 platformdirs = "^4.2.0"
-pydantic = { extras = ["email"], version = "^2.6.1" }
-pydantic-yaml = "^1.2.1"
+pydantic = { extras = ["email"], version = "^2.6.4" }
+pydantic-yaml = "^1.3.0"
 requests = "^2.31.0"
-typer = { extras = ["all"], version = "^0.9.0" }
+typer = "^0.12.3"
 
 [tool.poetry.group.dev.dependencies]
-black = "^24.2.0"
+black = "^24.4.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mike = "^2.0.0"
 mkdocs-glightbox = "^0.3.7"
-mkdocs-material = "^9.5.9"
+mkdocs-material = "^9.5.17"
 mkdocs-typer = "^0.0.3"
 
 [tool.poetry.scripts]
 lungo = "lungo_cli.app.main:app_wrapper"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/app/main.py` & `lungo_cli-0.3.0/src/lungo_cli/app/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from typing import Annotated
 
 from typer import Exit, Option, Typer
 
 from .state import console
-from ..commands import check, down, up
+from ..commands import check, down, install, list, uninstall, up
 from ..core.constants import APP_NAME, APP_NAME_CAPITALIZED
 from ..helpers.common import get_app_version
 
 app = Typer(
     context_settings={"help_option_names": ["-h", "--help"]},
     no_args_is_help=True,
     pretty_exceptions_show_locals=False,
     rich_markup_mode="rich",
 )
 
 app.command("check")(check.main)
 app.command("up")(up.main)
 app.command("down")(down.main)
+app.command("list")(list.main)
+app.command("install")(install.main)
+app.command("uninstall")(uninstall.main)
 
 
 def app_wrapper():
     app()
 
 
 def version_callback(value: bool):
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/app/state.py` & `lungo_cli-0.3.0/src/lungo_cli/app/state.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from ..core.app import AppManager
 from ..core.console import Console
 from ..core.container import Container
 from ..core.context import ContextManager
 from ..core.database import AccountManager
 from ..core.file import FileUtils
 from ..core.network import HttpApiClient
+from ..core.plugin import PluginManager
 from ..core.renderer import Renderer
 from ..core.storage import Storage
 
 _console = Console()
+_client = HttpApiClient(_console)
 _file_utils = FileUtils(_console)
 _storage = Storage(_console, _file_utils)
 _context_manager = ContextManager(_console, _file_utils, _storage)
-_container = Container(_console, _file_utils, _storage, _context_manager)
-_account_manager = AccountManager(_console, _file_utils, _storage, HttpApiClient(_console), _container)
-_renderer = Renderer(_console, _file_utils, _storage)
-_app_manager = AppManager(_console, _file_utils, _storage, _context_manager, _account_manager, _renderer)
+_container = Container(_console, _context_manager, _file_utils, _storage)
+_plugin_manager = PluginManager(_console, _context_manager, _file_utils, _storage)
+_renderer = Renderer(_console, _context_manager, _file_utils, _storage)
+_account_manager = AccountManager(_client, _console, _container, _file_utils, _storage)
+_app_manager = AppManager(
+    _account_manager, _console, _context_manager, _file_utils, _plugin_manager, _renderer, _storage
+)
 
 
 def console() -> Console:
     return _console
 
 
 def file_utils() -> FileUtils:
@@ -34,17 +39,21 @@
     return _context_manager
 
 
 def container() -> Container:
     return _container
 
 
-def account_manager() -> AccountManager:
-    return _account_manager
+def plugin_manager() -> PluginManager:
+    return _plugin_manager
 
 
 def renderer() -> Renderer:
     return _renderer
 
 
+def account_manager() -> AccountManager:
+    return _account_manager
+
+
 def app_manager() -> AppManager:
     return _app_manager
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/commands/base.py` & `lungo_cli-0.3.0/src/lungo_cli/commands/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from pathlib import Path
-from typing import Annotated, Optional
+from typing import Annotated, Final, Optional
 
 from typer import Option
 
-config_dir_type = Annotated[
+ConfigDirType: Final = Annotated[
     Optional[Path], Option("--config-dir", "-c", help="Path to the configuration directory.", show_default=False)
 ]
-dev_type = Annotated[bool, Option("--dev", help="Use the development configuration.", show_default=False)]
-force_init_type = Annotated[bool, Option("--force-init", help="Do a fresh initialization.", show_default=False)]
-remove_lock_type = Annotated[bool, Option("--remove-lock", help="Remove the lock file.", show_default=False)]
-quiet_type = Annotated[bool, Option("--quiet", "-q", help="Suppress all output except for errors.", show_default=False)]
-verbosity_type = Annotated[int, Option("--verbose", "-v", count=True, help="Increase verbosity.", show_default=False)]
+DevType: Final = Annotated[bool, Option("--dev", help="Use the development configuration.", show_default=False)]
+ForceInitType: Final = Annotated[bool, Option("--force-init", help="Do a fresh initialization.", show_default=False)]
+QuietType: Final = Annotated[
+    bool, Option("--quiet", "-q", help="Suppress all output except for errors.", show_default=False)
+]
+VerbosityType: Final = Annotated[
+    int, Option("--verbose", "-v", count=True, help="Increase verbosity.", show_default=False)
+]
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/commands/down.py` & `lungo_cli-0.3.0/src/lungo_cli/commands/install.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,44 @@
-from typing import Annotated, Optional
+from typing import Annotated
 
-from typer import Option
+from typer import Argument
 
-from .base import config_dir_type, dev_type, quiet_type, verbosity_type
-from ..app.state import app_manager, console, container
-from ..core.constants import APP_NAME_CAPITALIZED
-from ..models.base import EContainer
+from .base import ConfigDirType, DevType, QuietType, VerbosityType
+from ..app.state import app_manager, console, plugin_manager
+from ..helpers.format import format_input
 
 
 def main(
-    container_tool: Annotated[
-        Optional[EContainer], Option("--container-tool", help="Container management tool to use.", show_default=False)
-    ] = None,
-    config_dir: config_dir_type = None,
-    dev: dev_type = False,
-    quiet: quiet_type = False,
-    verbosity: verbosity_type = 0,
-):
+    args: Annotated[
+        list[str],
+        Argument(
+            help="Names of the plugins to add.",
+            show_default=False,
+        ),
+    ],
+    config_dir: ConfigDirType = None,
+    dev: DevType = False,
+    quiet: QuietType = False,
+    verbosity: VerbosityType = 0,
+) -> None:
     """
-    Stop the service.
+    Install or upgrade plugins.
     """
-    app_manager().process_args(config_dir, quiet, verbosity)
-    app_manager().load_config()
-    app_manager().process_args_deferred(dev)
+    app_manager().process_cli_options(config_dir, dev, quiet, verbosity)
+    app_manager().load_core_config()
 
-    container().set_preferred_tool(container_tool)
+    count = 0
 
-    with console().status("Stopping the service..."):
-        container().down()
+    for arg in args:
+        plugin_cls = next((x for x in plugin_manager().installable_plugin_classes if x.config.name == arg), None)
 
-    console().print(f"{APP_NAME_CAPITALIZED} stopped.")
+        if plugin_cls is None:
+            console().print_warning(f"Plugin {format_input(arg)} not found or not installable. Skipping it.")
+            continue
+
+        if plugin_manager().add_plugin(plugin_cls):
+            count += 1
+
+    if count == 1:
+        console().print("1 plugin added successfully.")
+    elif count > 1:
+        console().print(f"{count} plugins added successfully.")
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/commands/up.py` & `lungo_cli-0.3.0/src/lungo_cli/commands/up.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,71 @@
 from typing import Annotated, Optional
 
-from typer import Option
+from typer import Exit, Option
 
-from .base import config_dir_type, dev_type, force_init_type, quiet_type, remove_lock_type, verbosity_type
-from ..app.state import app_manager, console, container, context_manager
+from .base import ConfigDirType, DevType, ForceInitType, QuietType, VerbosityType
+from ..app.state import app_manager, console, container, context_manager, file_utils, storage
 from ..core.constants import APP_NAME, APP_NAME_CAPITALIZED
-from ..helpers.format import format_command, format_link
+from ..helpers.common import port_is_available
+from ..helpers.format import format_command, format_input, format_link
 from ..models.base import EContainer
 
 
 def main(
-    build_only: Annotated[bool, Option("--build-only", help="Only build the container.", show_default=False)] = False,
+    build_only: Annotated[bool, Option("--build-only", help="Only build the containers.", show_default=False)] = False,
     container_tool: Annotated[
         Optional[EContainer], Option("--container-tool", help="Container management tool to use.", show_default=False)
     ] = None,
-    config_dir: config_dir_type = None,
-    dev: dev_type = False,
-    force_init: force_init_type = False,
-    remove_lock: remove_lock_type = False,
-    quiet: quiet_type = False,
-    verbosity: verbosity_type = 0,
+    render_only: Annotated[
+        bool, Option("--render-only", help="Only render the templates.", show_default=False)
+    ] = False,
+    force_init: ForceInitType = False,
+    remove_lock: Annotated[bool, Option("--remove-lock", help="Remove the lock file.", show_default=False)] = False,
+    config_dir: ConfigDirType = None,
+    dev: DevType = False,
+    quiet: QuietType = False,
+    verbosity: VerbosityType = 0,
 ):
     """
     Start the service.
     """
-    app_manager().process_args(config_dir, quiet, verbosity)
-    app_manager().load_config()
-    app_manager().process_args_deferred(dev, force_init, remove_lock)
+    app_manager().process_cli_options(config_dir, dev, quiet, verbosity, force_init)
+    app_manager().load_full_config()
+
+    if remove_lock:
+        file_utils().remove(storage().lock_file)
 
     app_manager().update_app_data()
-    app_manager().ensure_port_availability()
+
+    if render_only:
+        return
 
     container().set_preferred_tool(container_tool)
 
     if build_only:
         with console().status(
-            "Building the container (it may take up to an hour depending on the internet connection)..."
+            "Building containers (could take a few minutes, depending on the internet connection)..."
         ):
             container().build()
 
         console().print("Build completed.")
     else:
+        http_port = context_manager().config.network.http.port
+        https_port = context_manager().config.network.https.port
+
+        if context_manager().config.network.http.enabled and not port_is_available(http_port):
+            console().print_error(f"Port {format_input(http_port)} is in use.")
+            raise Exit(code=1)
+
+        if not port_is_available(https_port):
+            console().print_error(f"Port {format_input(https_port)} is in use.")
+            raise Exit(code=1)
+
         with console().status(
-            "Starting the service (building may take up to an hour depending on the internet connection)..."
+            "Starting the service (could take a few minutes, depending on the internet connection)..."
         ):
             container().up()
 
         console().print(
             f"{APP_NAME_CAPITALIZED} is now available at {format_link(context_manager().base_url)}. "
-            f"To stop it, run {format_command(APP_NAME, 'down')}."
+            f"To stop it, run {format_command(APP_NAME, 'down', '--dev' if context_manager().dev else '')}."
         )
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/core/app.py` & `lungo_cli-0.3.0/src/lungo_cli/core/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,174 +1,103 @@
 import os
 from os import PathLike
 from pathlib import Path
-from uuid import uuid1
 
-from importlib_resources import as_file, files
 from typer import Exit
 
 from .console import Console
 from .constants import PACKAGE_NAME
 from .context import ContextManager
 from .database import AccountManager
 from .file import FileUtils
+from .plugin import PluginManager
 from .renderer import Renderer
 from .storage import Storage
-from ..helpers.common import get_app_version, get_file_permissions, port_is_available
-from ..helpers.crypto import generate_random_hex, generate_self_signed_cert
+from ..helpers.common import get_app_version, get_file_permissions
+from ..helpers.crypto import generate_random_hex, generate_self_signed_cert, hash_text
 from ..helpers.format import format_input, format_path
 from ..models.base import EApp
-from ..models.config import Config
+from ..models.config import Config, CoreConfig
 from ..models.users import Users
 
 
 class AppManager:
+    """Manager for the application."""
+
     def __init__(
         self,
+        account_manager: AccountManager,
         console: Console,
-        file_utils: FileUtils,
-        storage: Storage,
         context_manager: ContextManager,
-        account_manager: AccountManager,
+        file_utils: FileUtils,
+        plugin_manager: PluginManager,
         renderer: Renderer,
+        storage: Storage,
     ):
+        self.account_manager = account_manager
         self.console = console
-        self.file_utils = file_utils
-        self.storage = storage
         self.context_manager = context_manager
-        self.account_manager = account_manager
+        self.file_utils = file_utils
+        self.plugin_manager = plugin_manager
         self.renderer = renderer
+        self.storage = storage
+
+        self.force_init = False
 
-    def process_args(self, config_dir: str | PathLike[str] | None, quiet: bool, verbosity: int) -> None:
+    def process_cli_options(
+        self, config_dir: str | PathLike[str] | None, dev: bool, quiet: bool, verbosity: int, force_init: bool = False
+    ) -> None:
         """Process common arguments."""
         if config_dir:
             if not Path(config_dir).is_dir():
                 self.console.print_error(f"{format_path(config_dir)} is not a directory.")
                 raise Exit(code=1)
 
             self.storage.config_dir = Path(config_dir).resolve()
 
-        if quiet:
-            self.console.set_log_level(-1)
-        else:
-            self.console.set_log_level(verbosity)
-
-    def process_args_deferred(self, dev: bool, force_init: bool = False, remove_lock: bool = False) -> None:
-        """Process common arguments that need to be processed after the configuration is loaded."""
         if dev:
             self.console.set_log_level(1)
             self.storage.storage_version = "dev"
             self.context_manager.dev = True
+            self.force_init = True
 
-        if force_init:
-            self.file_utils.remove(self.storage.bundled_dir)
-
-        if remove_lock:
-            self.file_utils.remove(self.storage.lock_file)
-
-    def copy_app_resources(self, src: str | PathLike[str], dst: str | PathLike[str]) -> None:
-        """Copy resources from the package to the destination directory."""
-        with as_file(files(f"{PACKAGE_NAME}.resources")) as resources:
-            self.file_utils.copy(resources / src, dst)
-
-    def generate_config_hash(self) -> str:
-        """Generate a hash of the configuration files."""
-        return (
-            f"v{get_app_version()}"
-            + f"+{self.file_utils.hash_sha256(self.storage.config_file)}"
-            + f"+{self.file_utils.hash_sha256(self.storage.users_file)}"
-        )
-
-    def update_app_data(self) -> None:
-        """Ensure that all the application data exists and is up-to-date."""
-        config_hash = self.generate_config_hash()
-
-        with self.console.status("Updating storage..."):
-            self.storage.validate()
-            self.storage.create_dirs()
-
-            if (
-                not self.storage.init_file.is_file()
-                or self.file_utils.read_text(self.storage.init_file) != config_hash
-                or not self.storage.bundled_dir.is_dir()
-                or self.context_manager.dev
-            ):
-                self.console.print_info("Updating bundled data...")
-                self.copy_app_resources(".", self.storage.bundled_dir)
-                self.file_utils.change_mode(self.storage.bundled_dir, 0o700)
-                self.file_utils.remove(self.storage.init_file)
-
-            if not self.storage.nginx_gateway_cert_file.is_file() or not self.storage.nginx_gateway_key_file.is_file():
-                self.console.print_info("Generating self-signed certificate...")
-                cert, key = generate_self_signed_cert()
-                self.file_utils.write_bytes(self.storage.nginx_gateway_cert_file, cert)
-                self.file_utils.write_bytes(self.storage.nginx_gateway_key_file, key, True)
-
-            if not self.storage.kratos_secrets_file.is_file():
-                self.console.print_info("Generating Kratos secrets...")
-                self.renderer.render(
-                    self.storage.template_kratos_secrets_rel,
-                    self.storage.kratos_secrets_file,
-                    secret_cookie=generate_random_hex(),
-                )
-                self.file_utils.change_mode(self.storage.kratos_secrets_file, 0o600)
-
-            if not self.storage.jupyterhub_cookie_secret_file.is_file():
-                self.console.print_info("Generating JupyterHub cookie secret...")
-                self.file_utils.write_text(self.storage.jupyterhub_cookie_secret_file, generate_random_hex(), True)
-
-            if not self.storage.jupyterhub_password_file.is_file():
-                self.console.print_info("Generating JupyterHub password...")
-                self.file_utils.write_text(self.storage.jupyterhub_password_file, generate_random_hex(), True)
-
-            if not self.storage.rstudio_password_file.is_file():
-                self.console.print_info("Generating RStudio password...")
-                self.file_utils.write_text(self.storage.rstudio_password_file, generate_random_hex(), True)
-
-            if not self.storage.xray_salt_file.is_file():
-                self.console.print_info("Generating Xray salt...")
-                self.file_utils.write_text(self.storage.xray_salt_file, str(uuid1()), True)
-
-        with self.console.status("Updating database..."):
-            if not self.storage.init_file.is_file():
-                self.renderer.render_all(self.context_manager.context)
-                self.account_manager.update(self.context_manager.config, self.context_manager.users)
-
-                self.file_utils.write_text(self.storage.init_file, config_hash)
-
-    def ensure_port_availability(self) -> None:
-        """Ensure that ports used by the application are available."""
-        if self.context_manager.config.network.http.enabled and not port_is_available(
-            self.context_manager.config.network.http.port
-        ):
-            self.console.print_error(f"Port {format_input(self.context_manager.config.network.http.port)} is in use.")
-            raise Exit(code=1)
+        if quiet:
+            self.console.set_log_level(-1)
+        else:
+            self.console.set_log_level(verbosity)
 
-        if not port_is_available(self.context_manager.config.network.https.port):
-            self.console.print_error(f"Port {format_input(self.context_manager.config.network.https.port)} is in use.")
-            raise Exit(code=1)
+        if force_init:
+            self.force_init = True
 
-    def load_config(self) -> None:
-        """Load the configuration files into the context manager."""
+    def load_core_config(self) -> None:
+        """Load the core part of the configuration file that is critical to set up the application."""
         files_missing = False
 
         if not self.storage.config_file.is_file():
             self.console.print_error(
                 f"{format_path(self.storage.config_file.name)} not found. "
-                "A template will be created, please read the manual to learn how to configure it."
+                "A template has been created in place of the missing file."
+            )
+            self.file_utils.copy_package_resources(
+                f"{PACKAGE_NAME}.resources",
+                self.storage.template_config_rel,
+                self.storage.config_file,
             )
-            self.copy_app_resources(self.storage.template_config_rel, self.storage.config_file)
             files_missing = True
 
         if not self.storage.users_file.is_file():
             self.console.print_error(
                 f"{format_path(self.storage.users_file.name)} not found. "
-                "A template will be created, please read the manual to learn how to configure it."
+                "A template has been created in place of the missing file."
+            )
+            self.file_utils.copy_package_resources(
+                f"{PACKAGE_NAME}.resources",
+                self.storage.template_users_rel,
+                self.storage.users_file,
             )
-            self.copy_app_resources(self.storage.template_users_rel, self.storage.users_file)
             files_missing = True
 
         if files_missing:
             raise Exit(code=1)
 
         if (permission := get_file_permissions(self.storage.config_file))[1:] != "00":
             self.console.print_warning(
@@ -177,28 +106,36 @@
             )
         if (permission := get_file_permissions(self.storage.users_file))[1:] != "00":
             self.console.print_warning(
                 f"{format_path(self.storage.users_file)} should not be readable or writable by other users "
                 f"(recommended permission: 600, current permission: {permission})."
             )
 
+        core_config = self.file_utils.parse_yaml(self.storage.config_file, CoreConfig)
+
+        if core_config.directories.cache_dir:
+            self.storage.cache_dir = core_config.directories.cache_dir.resolve()
+        if core_config.directories.data_dir:
+            self.storage.data_dir = core_config.directories.data_dir.resolve()
+
+    def load_full_config(self) -> None:
+        """Load the full configuration files into the context manager."""
+        self.load_core_config()
+        self.plugin_manager.extend_models()
+
         config = self.file_utils.parse_yaml(self.storage.config_file, Config)
         users = self.file_utils.parse_yaml(self.storage.users_file, Users)
 
-        if config.directories.cache_dir:
-            self.storage.cache_dir = config.directories.cache_dir.resolve()
-        if config.directories.data_dir:
-            self.storage.data_dir = config.directories.data_dir.resolve()
-
         self.verify_config(config, users)
 
         self.context_manager.config = config
         self.context_manager.users = users
 
     def verify_config(self, config: Config, users: Users) -> None:
+        """Verify the configuration files."""
         shared_dirs = list(map(lambda x: x.name, config.directories.shared_dirs))
         anonymous_account_exists = False
 
         for account in users.accounts:
             if account.username == "anonymous":
                 self.console.print_info(
                     f"Found username {format_input('anonymous')}. "
@@ -227,17 +164,123 @@
             if config.rules.privileges.unregistered.allowed_apps == "all":
                 self.console.print_error(
                     "An anonymous account is required when the unregistered role has access to all applications."
                 )
                 raise Exit(code=1)
 
             for allowed_app in config.rules.privileges.unregistered.allowed_apps:
-                # Pydantic does not distinguish between a string and a enum value
-                if type(allowed_app) is str:
-                    allowed_app = EApp(allowed_app)
-
-                if allowed_app in (EApp.FILEBROWSER, EApp.JUPYTERHUB, EApp.RSTUDIO):
+                # Pydantic does not distinguish between a string and an enum value
+                if type(allowed_app) is EApp:
+                    allowed_app = allowed_app.value
+
+                if next(
+                    (
+                        plugin_cls.config.require_account
+                        for plugin_cls in self.plugin_manager.compatible_plugin_classes
+                        if plugin_cls.config.name == allowed_app
+                    ),
+                    False,
+                ):
                     self.console.print_error(
                         "An anonymous account is required when the unregistered role "
                         "has access to applications that require an account."
                     )
                     raise Exit(code=1)
+
+    def generate_config_hash(self) -> str:
+        """Generate a hash of the configuration files."""
+        ordered_plugins = sorted(self.plugin_manager.compatible_plugin_classes, key=lambda x: x.config.name)
+
+        return hash_text(
+            "+".join(
+                [
+                    f"v{get_app_version()}",
+                    *(
+                        map(
+                            lambda x: f"{x.config.name}{f'v{x.config.version}' if x.config.version else ''}",
+                            ordered_plugins,
+                        )
+                    ),
+                    self.file_utils.hash_sha256(self.storage.config_file),
+                    self.file_utils.hash_sha256(self.storage.users_file),
+                ]
+            )
+        )
+
+    def update_app_data(self) -> None:
+        """Ensure that all the application data exists and is up-to-date."""
+        config_hash = self.generate_config_hash()
+
+        with self.console.status("Updating app data..."):
+            self.storage.validate()
+
+            if (
+                self.force_init
+                or not self.storage.bundled_dir.is_dir()
+                or not self.storage.init_file.is_file()
+                or self.file_utils.read_text(self.storage.init_file) != config_hash
+            ):
+                self.console.print_info("Updating bundled resources...")
+
+                # Backup the installed plugins directory if it exists
+                if self.storage.installed_plugins_dir.is_dir():
+                    self.file_utils.move(self.storage.installed_plugins_dir, self.storage.cache_plugins_dir)
+
+                self.file_utils.copy_package_resources(f"{PACKAGE_NAME}.resources", ".", self.storage.bundled_dir)
+
+                if self.storage.cache_plugins_dir.is_dir():
+                    self.file_utils.move(self.storage.cache_plugins_dir, self.storage.installed_plugins_dir)
+
+                self.file_utils.change_mode(self.storage.bundled_dir, 0o700)
+                self.file_utils.remove(self.storage.init_file)
+
+            if not self.storage.nginx_gateway_cert_file.is_file() or not self.storage.nginx_gateway_key_file.is_file():
+                self.console.print_info("Generating self-signed certificate...")
+                cert, key = generate_self_signed_cert()
+                self.file_utils.write_bytes(self.storage.nginx_gateway_cert_file, cert)
+                self.file_utils.write_bytes(self.storage.nginx_gateway_key_file, key, True)
+
+            # Remove the socket file every time to avoid binding issues
+            self.file_utils.remove(self.storage.nginx_gateway_socket_file)
+
+            if not self.storage.kratos_secrets_file.is_file():
+                self.console.print_info("Generating Kratos secrets...")
+                self.renderer.render(
+                    self.storage.template_kratos_secrets_rel,
+                    self.storage.kratos_secrets_file,
+                    secret_cookie=generate_random_hex(),
+                )
+                self.file_utils.change_mode(self.storage.kratos_secrets_file, 0o600)
+
+            self.plugin_manager.initialize_plugins()
+
+            if not self.storage.init_file.is_file():
+                for plugin in self.plugin_manager.plugins:
+                    self.renderer.render_plugin(plugin)
+                    self.context_manager.plugin_outputs.append(plugin.output)
+
+                self.renderer.render_main()
+                self.account_manager.update(self.context_manager.config, self.context_manager.users)
+
+                # Delay copying the web files until the templates have all been rendered
+                for plugin in self.plugin_manager.plugins:
+                    for web_dir in (self.storage.installed_plugins_dir / plugin.config.name / "web").iterdir():
+                        if web_dir.name == "lib":
+                            dst_prefix = self.storage.bundled_dir / "web" / "src" / "lib" / "plugins"
+                            self.file_utils.copy(web_dir, dst_prefix / plugin.config.name)
+                        elif web_dir.name == "routes":
+                            dst_prefix = self.storage.bundled_dir / "web" / "src" / "routes" / "(apps)" / "app"
+                            self.file_utils.copy(web_dir, dst_prefix / plugin.config.name)
+
+                if self.context_manager.config.branding.cover:
+                    self.file_utils.copy(
+                        self.context_manager.config.branding.cover,
+                        self.storage.bundled_dir / "web" / "src" / "lib" / "assets" / "cover.jpg",
+                    )
+
+                if self.context_manager.config.branding.logo:
+                    self.file_utils.copy(
+                        self.context_manager.config.branding.logo,
+                        self.storage.bundled_dir / "web" / "static" / "favicon.png",
+                    )
+
+                self.file_utils.write_text(self.storage.init_file, config_hash)
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/core/console.py` & `lungo_cli-0.3.0/src/lungo_cli/core/console.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from contextlib import nullcontext
-from enum import Enum
-from typing import Any, Callable, TypeVar
+from enum import auto, Enum, IntEnum
+from typing import Any, Callable
 
 from rich import console
 from rich.prompt import Confirm, Prompt
 from rich.status import Status
 
-TEnum = TypeVar("TEnum", bound=Enum)
 
-
-class LogLevels(int, Enum):
+class LogLevels(IntEnum):
     """Log levels for console output."""
 
-    TRACE = 0
-    DEBUG = 1
-    INFO = 2
-    WARNING = 3
-    ERROR = 4
+    TRACE = auto()
+    DEBUG = auto()
+    INFO = auto()
+    WARNING = auto()
+    ERROR = auto()
 
 
 class Console:
     """Console for text output."""
 
     def __init__(self):
         self.is_empty = True
@@ -28,81 +26,76 @@
         self.epilogue = []
         self.log_level = LogLevels.INFO
         self.stdout = console.Console()
 
     def set_log_level(self, verbosity: int):
         if verbosity <= -1:
             self.log_level = LogLevels.WARNING
-        elif verbosity == 0:
-            self.log_level = LogLevels.INFO
         elif verbosity == 1:
             self.log_level = LogLevels.DEBUG
         elif verbosity >= 2:
             self.log_level = LogLevels.TRACE
 
     def ensure_newline(self):
         if self.need_newline:
             self.need_newline = False
             print()
 
         self.is_empty = False
 
-    def request_for_newline(self):
+    def request_newline(self):
         if not self.is_empty:
             self.need_newline = True
 
     def print(self, *args: Any, epilogue: bool = False, **kwargs: Any):
-        if self.log_level.value > LogLevels.INFO.value:
-            return
-
         kwargs["highlight"] = kwargs.get("highlight", False)
 
         if epilogue:
             self.epilogue.append((args, kwargs))
         else:
             self.ensure_newline()
             self.stdout.print(*args, **kwargs)
 
     def print_trace(self, *args: Any, **kwargs: Any):
-        if self.log_level.value > LogLevels.TRACE.value:
+        if self.log_level > LogLevels.TRACE:
             return
 
         kwargs["highlight"] = kwargs.get("highlight", False)
         self.stdout.print("[TRACE]", *args, **kwargs)
 
     def print_debug(self, *args: Any, **kwargs: Any):
-        if self.log_level.value > LogLevels.DEBUG.value:
+        if self.log_level > LogLevels.DEBUG:
             return
 
         kwargs["highlight"] = kwargs.get("highlight", False)
         self.stdout.print("[DEBUG]", *args, **kwargs)
 
     def print_info(self, *args: Any, **kwargs: Any):
-        if self.log_level.value > LogLevels.INFO.value:
+        if self.log_level > LogLevels.INFO:
             return
 
         kwargs["highlight"] = kwargs.get("highlight", False)
         self.stdout.print("[INFO]", *args, **kwargs)
 
     def print_warning(self, *args: Any, **kwargs: Any):
-        if self.log_level.value > LogLevels.WARNING.value:
+        if self.log_level > LogLevels.WARNING:
             return
 
         kwargs["highlight"] = kwargs.get("highlight", False)
         self.stdout.print("[bold yellow][WARNING][/bold yellow]", *args, **kwargs)
 
     def print_error(self, *args: Any, **kwargs: Any):
-        if self.log_level.value > LogLevels.ERROR.value:
+        if self.log_level > LogLevels.ERROR:
             return
 
         kwargs["highlight"] = kwargs.get("highlight", False)
         self.stdout.print("[bold red][ERROR][/bold red]", *args, **kwargs)
 
     def show_epilogue(self):
-        self.request_for_newline()
+        self.request_newline()
         self.ensure_newline()
 
         for args, kwargs in self.epilogue:
             self.stdout.print(*args, **kwargs)
 
         self.epilogue.clear()
 
@@ -159,15 +152,15 @@
             if Prompt.ask(**kwargs) == answer:
                 break
             else:
                 self.print_warning("Passwords do not match. Please try again.")
 
         return answer
 
-    def ask_for_enum(self, prompt: str, enum: type[TEnum], default: TEnum | None = None, **kwargs: Any) -> TEnum:
+    def ask_for_enum[T: Enum](self, prompt: str, enum: type[T], default: T | None = None, **kwargs: Any) -> T:
         self.ensure_newline()
 
         kwargs["prompt"] = f"[bold]{prompt}[/bold]"
         kwargs["choices"] = [e.value for e in enum]
         kwargs["default"] = default.value if default else None
 
         while not (answer := Prompt.ask(**kwargs)):
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/core/container.py` & `lungo_cli-0.3.0/src/lungo_cli/core/container.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,51 +6,62 @@
 from .console import Console
 from .constants import APP_NAME_CAPITALIZED, DOCKER_COMPOSE_URL, DOCKER_URL, PODMAN_COMPOSE_URL, PODMAN_URL
 from .context import ContextManager
 from .file import FileUtils
 from .storage import Storage
 from ..helpers.common import program_exists
 from ..helpers.format import format_command, format_link, format_program
-from ..models.base import EContainer, EService
+from ..models.base import EApp, EContainer, ECoreService
 
 _docker = format_program("Docker")
 _docker_link = format_link(DOCKER_URL, _docker)
 _docker_compose = format_program("Docker Compose")
 _docker_compose_link = format_link(DOCKER_COMPOSE_URL, _docker_compose)
 _podman = format_program("Podman")
 _podman_link = format_link(PODMAN_URL, _podman)
 _podman_compose = format_program("Podman Compose")
 _podman_compose_link = format_link(PODMAN_COMPOSE_URL, _podman_compose)
 
 
 class Container:
     """Communicate with the container management tool."""
 
-    def __init__(self, console: Console, file_utils: FileUtils, storage: Storage, context_manager: ContextManager):
+    def __init__(self, console: Console, context_manager: ContextManager, file_utils: FileUtils, storage: Storage):
         self.console = console
+        self.context_manager = context_manager
         self.file_utils = file_utils
         self.storage = storage
-        self.context_manager = context_manager
+
         self.preferred_tool = None
         self.tool = None
 
     def set_preferred_tool(self, tool: EContainer | None) -> None:
         self.preferred_tool = tool
 
     def run_shell_command(self, *command: str, cwd: str | PathLike[str] | None = None) -> None:
         command = list(filter(None, command))
 
         try:
-            subprocess.run(
-                command,
-                check=True,
-                cwd=cwd or self.storage.bundled_dir,
-                stderr=subprocess.DEVNULL,
-                stdout=subprocess.DEVNULL,
-            )
+            if self.context_manager.dev:
+                with subprocess.Popen(
+                    command,
+                    stdout=subprocess.PIPE,
+                    stderr=subprocess.STDOUT,
+                    cwd=cwd or self.storage.bundled_dir,
+                ) as process:
+                    for line in process.stdout:
+                        self.console.print(line.decode("utf8"))
+            else:
+                subprocess.run(
+                    command,
+                    stdout=subprocess.DEVNULL,
+                    stderr=subprocess.DEVNULL,
+                    cwd=cwd or self.storage.bundled_dir,
+                    check=True,
+                )
         except Exception as e:
             self.console.print_error(f"Failed to run command {format_command(*command)} ({e}).")
             raise Exit(code=1)
 
     def choose_tool(self) -> EContainer:
         if self.tool:
             return self.tool
@@ -105,43 +116,47 @@
             else:
                 self.console.print_error(f"Neither {_docker_compose_link} nor {_podman_compose_link} is installed.")
                 raise Exit(code=1)
         else:
             self.console.print_error(f"Neither {_docker_link} nor {_podman_link} is installed.")
             raise Exit(code=1)
 
-    def build(self, working_dir: str | PathLike[str] | None = None, service: EService | None = None) -> None:
+    def build(self, working_dir: str | PathLike[str] | None = None, service: EApp | ECoreService | None = None) -> None:
         match self.choose_tool():
             case EContainer.DOCKER:
                 self.run_shell_command("docker", "compose", "build", service.value if service else "", cwd=working_dir)
             case EContainer.DOCKER_COMPOSE:
                 self.run_shell_command("docker-compose", "build", service.value if service else "", cwd=working_dir)
             case EContainer.PODMAN_COMPOSE:
                 self.run_shell_command("podman-compose", "build", service.value if service else "", cwd=working_dir)
 
     def up(self, working_dir: str | PathLike[str] | None = None) -> None:
         if self.storage.lock_file.is_file():
             self.console.print_error(
-                f"An existing instance of {APP_NAME_CAPITALIZED} is running. Please stop it before proceeding. "
-                f"Or, you can remove the restriction forcibly by using the {format_command('--remove-lock')} option."
+                f"An existing instance of {APP_NAME_CAPITALIZED} is running. Please stop it before proceeding, "
+                f"or use the {format_command('--remove-lock')} flag."
             )
             raise Exit(code=1)
 
         tool = self.choose_tool()
 
         if not working_dir:
             self.file_utils.create(self.storage.lock_file)
 
-        match tool:
-            case EContainer.DOCKER:
-                self.run_shell_command("docker", "compose", "up", "-d", "--build", cwd=working_dir)
-            case EContainer.DOCKER_COMPOSE:
-                self.run_shell_command("docker-compose", "up", "-d", "--build", cwd=working_dir)
-            case EContainer.PODMAN_COMPOSE:
-                self.run_shell_command("podman-compose", "up", "-d", "--build", cwd=working_dir)
+        try:
+            match tool:
+                case EContainer.DOCKER:
+                    self.run_shell_command("docker", "compose", "up", "-d", "--build", cwd=working_dir)
+                case EContainer.DOCKER_COMPOSE:
+                    self.run_shell_command("docker-compose", "up", "-d", "--build", cwd=working_dir)
+                case EContainer.PODMAN_COMPOSE:
+                    self.run_shell_command("podman-compose", "up", "-d", "--build", cwd=working_dir)
+        except Exception:
+            self.file_utils.remove(self.storage.lock_file)
+            raise
 
     def down(self, working_dir: str | PathLike[str] | None = None) -> None:
         match self.choose_tool():
             case EContainer.DOCKER:
                 self.run_shell_command("docker", "compose", "down", cwd=working_dir)
             case EContainer.DOCKER_COMPOSE:
                 self.run_shell_command("docker-compose", "down", cwd=working_dir)
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/core/database.py` & `lungo_cli-0.3.0/src/lungo_cli/core/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 from ..models.users import Users
 
 
 class AccountManager:
     """Validate and update user accounts."""
 
     def __init__(
-        self, console: Console, file_utils: FileUtils, storage: Storage, client: HttpApiClient, container: Container
+        self, client: HttpApiClient, console: Console, container: Container, file_utils: FileUtils, storage: Storage
     ):
+        self.client = client
         self.console = console
+        self.container = container
         self.file_utils = file_utils
         self.storage = storage
-        self.client = client
-        self.container = container
 
     def update(self, config: Config, users: Users) -> None:
         # Ensure that the container can always be started even if it failed last time
         self.container.down(self.storage.service_keto_admin_dir)
         self.container.down(self.storage.service_kratos_admin_dir)
 
         self.container.up(self.storage.service_keto_admin_dir)
@@ -78,15 +78,15 @@
             },
         ]
 
         enabled_apps = []
 
         app: EApp
         for app in EApp:
-            if getattr(config.modules, app.value).enabled:
+            if getattr(config.plugins, app.value).enabled:
                 enabled_apps.append(app)
                 data.append(
                     {
                         "action": "insert",
                         "relation_tuple": {
                             "namespace": "app",
                             "object": app.value,
@@ -110,15 +110,15 @@
                             "relation": "access",
                             "subject_set": {"namespace": "role", "object": role, "relation": "member"},
                         },
                     },
                 )
             else:
                 for allowed_app in privilege.allowed_apps:
-                    # Pydantic does not distinguish between a string and a enum value
+                    # Pydantic does not distinguish between a string and an enum value
                     if type(allowed_app) is str:
                         allowed_app = EApp(allowed_app)
 
                     if allowed_app in enabled_apps:
                         data.append(
                             {
                                 "action": "insert",
@@ -157,15 +157,15 @@
                             "relation": "access",
                             "subject_id": account.username,
                         },
                     },
                 )
             else:
                 for allowed_app in account.extra.allowed_apps:
-                    # Pydantic does not distinguish between a string and a enum value
+                    # Pydantic does not distinguish between a string and an enum value
                     if type(allowed_app) is str:
                         allowed_app = EApp(allowed_app)
 
                     if allowed_app in enabled_apps:
                         data.append(
                             {
                                 "action": "insert",
@@ -188,14 +188,15 @@
 
         accounts = users.accounts[:]
 
         # It makes no sense for the anonymous account to be managed by Kratos
         if anonymous_account := next(filter(lambda x: x.username == "anonymous", accounts), None):
             accounts.remove(anonymous_account)
 
+        # This endpoint by default returns the first 250 accounts, but should be enough for most use cases
         for old_account in self.client.get(f"{KRATOS_ADMIN_API_BASE_URL}/admin/identities"):
             if new_account := next(filter(lambda x: x.username == old_account["traits"]["username"], accounts), None):
                 # Update the account
                 accounts.remove(new_account)
                 data = []
 
                 if old_account["state"] != (state := ("active" if new_account.enabled else "inactive")):
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/core/file.py` & `lungo_cli-0.3.0/src/lungo_cli/core/file.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-import hashlib
 import shutil
+from importlib.resources import as_file, files
 from os import PathLike
 from pathlib import Path
-from typing import Type, TypeVar
 
 from pydantic import BaseModel, ValidationError
 from pydantic_yaml import parse_yaml_file_as
 from typer import Exit
 
 from .console import Console
-from ..helpers.format import format_path
-
-T = TypeVar("T", bound=BaseModel)
+from ..helpers.crypto import hash_stream
+from ..helpers.format import format_input, format_path
 
 
 class FileUtils:
-    """File utilities."""
+    """Utility class for file operations."""
 
     def __init__(self, console: Console):
         self.console = console
 
     def create(self, path: str | PathLike[str]) -> None:
         path = Path(path)
 
@@ -35,54 +33,76 @@
 
         try:
             path.mkdir(parents=True, exist_ok=True)
         except Exception as e:
             self.console.print_error(f"Failed to create {format_path(path.name)} ({e}).")
             raise Exit(code=1)
 
-    def copy(self, src: str | PathLike[str], dst: str | PathLike[str]) -> None:
+    def copy(self, src: str | PathLike[str], dst: str | PathLike[str], merge: bool = False) -> None:
         src = Path(src)
         dst = Path(dst)
 
         try:
             self.create_dir(dst.parent)
-            self.remove(dst)
+
+            if not merge:
+                self.remove(dst)
 
             if src.is_dir():
-                shutil.copytree(src, dst)
+                shutil.copytree(src, dst, dirs_exist_ok=True)
             elif src.is_file():
                 shutil.copy(src, dst)
             else:
                 self.console.print_error(f"{format_path(src.name)} is not a file or directory.")
                 raise Exit(code=1)
         except Exception as e:
             self.console.print_error(f"Failed to copy {format_path(src.name)} to {format_path(dst.name)} ({e}).")
             raise Exit(code=1)
 
-    def copy_to(self, src: str | PathLike[str], dst_dir: str | PathLike[str]) -> None:
+    def move(self, src: str | PathLike[str], dst: str | PathLike[str], merge: bool = False) -> None:
         src = Path(src)
-        dst_dir = Path(dst_dir)
+        dst = Path(dst)
+
+        try:
+            self.create_dir(dst.parent)
+
+            if not merge:
+                self.remove(dst)
 
-        self.copy(src, dst_dir / src.name)
+            shutil.move(src, dst)
+        except Exception as e:
+            self.console.print_error(f"Failed to move {format_path(src.name)} to {format_path(dst.name)} ({e}).")
+            raise Exit(code=1)
 
     def remove(self, path: str | PathLike[str]) -> None:
         path = Path(path)
 
         try:
             if path.is_dir():
                 shutil.rmtree(path)
             elif path.is_file():
                 path.unlink()
         except Exception as e:
             self.console.print_error(f"Failed to remove {format_path(path.name)} ({e}).")
             raise Exit(code=1)
 
-    def read_text(self, path: str | PathLike[str]) -> str:
+    def copy_package_resources(self, package: str, src: str | PathLike[str], dst: str | PathLike[str]) -> None:
+        try:
+            with as_file(files(package)) as package_dir:
+                self.copy(package_dir / src, dst)
+        except Exception as e:
+            self.console.print_error(f"Failed to copy resources from {format_input(package)} ({e}).")
+            raise Exit(code=1)
+
+    def read_text(self, path: str | PathLike[str], not_exist_ok: bool = False) -> str:
         path = Path(path)
 
+        if not path.is_file() and not_exist_ok:
+            return ""
+
         try:
             return path.read_text()
         except Exception as e:
             self.console.print_error(f"Failed to read {format_path(path.name)} ({e}).")
             raise Exit(code=1)
 
     def write_bytes(self, path: str | PathLike[str], data: bytes, secret: bool = False) -> None:
@@ -121,20 +141,20 @@
             raise Exit(code=1)
 
     def hash_sha256(self, path: str | PathLike[str]) -> str:
         path = Path(path)
 
         try:
             with open(path, "rb") as f:
-                return hashlib.file_digest(f, "sha256").hexdigest()
+                return hash_stream(f)
         except Exception as e:
             self.console.print_error(f"Failed to hash {format_path(path.name)} ({e}).")
             raise Exit(code=1)
 
-    def parse_yaml(self, path: str | PathLike[str], model: Type[T]) -> T:
+    def parse_yaml[T: BaseModel](self, path: str | PathLike[str], model: type[T]) -> T:
         """Parse a YAML file as a Pydantic model."""
         try:
             return parse_yaml_file_as(model, path)
         except ValidationError as e:
             error_msg = f"Failed to parse {format_path(path)}."
 
             for error in e.errors():
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/core/network.py` & `lungo_cli-0.3.0/src/lungo_cli/core/network.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/core/storage.py` & `lungo_cli-0.3.0/src/lungo_cli/core/storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 from platformdirs import user_cache_path, user_config_path, user_data_path
 from typer import Exit
 
 from .console import Console
 from .constants import APP_AUTHOR, APP_NAME, STORAGE_PREFIX, STORAGE_VERSION
 from .file import FileUtils
 from ..helpers.format import format_path
-from ..models.base import EService
+from ..models.base import EApp, ECoreService
 
 
 class Storage:
     """Contain all the paths used by the application."""
 
     def __init__(self, console: Console, file_utils: FileUtils):
         self.console = console
         self.file_utils = file_utils
+
         self._storage_version = STORAGE_VERSION
         self._cache_dir = user_cache_path(APP_NAME, APP_AUTHOR)
         self._config_dir = user_config_path(APP_NAME, APP_AUTHOR)
         self._data_dir = user_data_path(APP_NAME, APP_AUTHOR)
 
     @property
     def storage_version(self) -> str:
@@ -88,14 +89,30 @@
         return Path("managed")
 
     @property
     def excluded_rel(self) -> Path:
         return Path("excluded")
 
     @property
+    def plugins_rel(self) -> Path:
+        return Path("plugins")
+
+    @property
+    def cache_plugins_dir(self) -> Path:
+        return self.cache_latest_dir / self.plugins_rel
+
+    @property
+    def custom_plugins_dir(self) -> Path:
+        return self.config_dir / self.plugins_rel
+
+    @property
+    def installed_plugins_dir(self) -> Path:
+        return self.bundled_dir / self.plugins_rel
+
+    @property
     def config_file(self) -> Path:
         return self._config_dir / "config.yaml"
 
     @property
     def users_file(self) -> Path:
         return self._config_dir / "users.yaml"
 
@@ -113,51 +130,39 @@
 
     @property
     def service_kratos_admin_dir(self) -> Path:
         return self.bundled_dir / "dockerfiles" / "kratos_admin"
 
     @property
     def template_config_rel(self) -> Path:
-        return self.excluded_rel / "config.yaml"
+        return Path("assets") / "config_references" / "config.yaml"
 
     @property
     def template_users_rel(self) -> Path:
-        return self.excluded_rel / "users.yaml"
+        return Path("assets") / "config_references" / "users.yaml"
 
     @property
     def template_kratos_secrets_rel(self) -> Path:
         return self.excluded_rel / "kratos" / "secrets.yaml.jinja"
 
     @property
     def nginx_gateway_cert_file(self) -> Path:
         return self.generated_dir / "nginx_gateway" / "lungo.crt"
 
     @property
     def nginx_gateway_key_file(self) -> Path:
         return self.generated_dir / "nginx_gateway" / "lungo.key"
 
     @property
-    def kratos_secrets_file(self) -> Path:
-        return self.generated_dir / "kratos" / "secrets.yaml"
-
-    @property
-    def jupyterhub_cookie_secret_file(self) -> Path:
-        return self.generated_dir / "jupyterhub" / "cookie_secret"
-
-    @property
-    def jupyterhub_password_file(self) -> Path:
-        return self.generated_dir / "jupyterhub" / "password"
+    def nginx_gateway_socket_file(self) -> Path:
+        return self.managed_dir / "nginx_gateway" / "sockets" / "nginx.sock"
 
     @property
-    def rstudio_password_file(self) -> Path:
-        return self.generated_dir / "rstudio" / "password"
-
-    @property
-    def xray_salt_file(self) -> Path:
-        return self.generated_dir / "xray" / "salt"
+    def kratos_secrets_file(self) -> Path:
+        return self.generated_dir / "kratos" / "secrets.yaml"
 
     def validate(self) -> None:
         if self.data_latest_dir.is_dir():
             return
 
         largest_version = -1
 
@@ -168,27 +173,24 @@
 
                 if version_number > largest_version:
                     largest_version = version_number
 
         if largest_version >= 0:
             self.migrate(self.data_dir / f"{STORAGE_PREFIX}{largest_version}")
 
+        # Always make sure the directories exist
+        app: EApp | ECoreService
+        for app in *EApp, *ECoreService:
+            self.file_utils.create_dir(self.cache_latest_dir / app.value)
+            self.file_utils.change_mode(self.cache_latest_dir / app.value, 0o700)
+            self.file_utils.create_dir(self.managed_dir / app.value)
+            self.file_utils.change_mode(self.managed_dir / app.value, 0o700)
+
     def migrate(self, from_: str | PathLike[str]) -> None:
         self.console.print_info(f"Migrating storage from {format_path(Path(from_).name)}...")
 
         # FIXME: use `unshare` to copy the files generated by the container to avoid permission issues
         try:
             self.file_utils.copy(from_ / self.generated_rel, self.generated_dir)
             self.file_utils.copy(from_ / self.managed_rel, self.managed_dir)
         except Exit:
             ...
-
-    def create_dirs(self) -> None:
-        app: EService
-        for app in EService:
-            self.file_utils.create_dir(self.cache_latest_dir / app.value)
-            self.file_utils.change_mode(self.cache_latest_dir / app.value, 0o700)
-            self.file_utils.create_dir(self.managed_dir / app.value)
-            self.file_utils.change_mode(self.managed_dir / app.value, 0o700)
-
-        # Allow the non-root container user to write
-        self.file_utils.change_mode(self.managed_dir / EService.PRIVATEBIN.value, 0o777)
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/helpers/crypto.py` & `lungo_cli-0.3.0/src/lungo_cli/helpers/crypto.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import hashlib
 from datetime import datetime, timedelta, UTC
 from secrets import token_hex
+from typing import BinaryIO
 
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import rsa
 
 from ..core.constants import APP_NAME_CAPITALIZED
@@ -38,7 +40,17 @@
 
     return cert_pem, key_pem
 
 
 def generate_random_hex() -> str:
     """Generate a random hex string."""
     return token_hex(32)
+
+
+def hash_stream(f: BinaryIO) -> str:
+    """Hash a stream using SHA-256."""
+    return hashlib.file_digest(f, "sha256").hexdigest()
+
+
+def hash_text(text: str) -> str:
+    """Hash a text using SHA-256."""
+    return hashlib.sha256(text.encode()).hexdigest()
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/helpers/format.py` & `lungo_cli-0.3.0/src/lungo_cli/helpers/format.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 from os import PathLike
 
 
 def format_command(*value: str) -> str:
     """Format a shell command for console output."""
-    return f"[green]{' '.join(value)}[/green]"
+    return f"[green]{' '.join(filter(None, value))}[/green]"
 
 
 def format_program(value: str) -> str:
     """Format a program name for console output."""
     return f"[cyan]{value}[/cyan]"
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/models/config.py` & `lungo_cli-0.3.0/src/lungo_cli/models/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 from datetime import timedelta
 from ipaddress import IPv4Address, IPv4Network
 
-from pydantic import DirectoryPath, EmailStr, field_validator, FilePath, NewPath, PositiveInt
+from pydantic import (
+    ConfigDict,
+    DirectoryPath,
+    EmailStr,
+    field_validator,
+    FilePath,
+    NewPath,
+    NonNegativeInt,
+    PositiveInt,
+)
 
-from .base import AllowedApps, Base, EApp, FileName, Port
+from .base import AllowedAppsType, Base, FileNameType, PortType
 from ..core.constants import APP_NAME_CAPITALIZED
 
 
 class Branding(Base):
     name: str = APP_NAME_CAPITALIZED
     subtitle: list[str] = ["a hug in a mug", "a poetry of aroma", "a quiet solitude", "a whisper of inspiration"]
     cover: FilePath | None = None
     logo: FilePath | None = None
 
 
 class SharedDir(Base):
-    name: FileName
+    name: FileNameType
     source: DirectoryPath | FilePath
     read_only: bool = False
 
     # noinspection PyNestedDecorators
     @field_validator("name")
     @classmethod
     def name_field_validator(cls, v: str) -> str:
@@ -35,77 +44,47 @@
     data_dir: DirectoryPath | NewPath | None = None
     users_dir: DirectoryPath | NewPath
     shared_dirs: list[SharedDir] = []
 
 
 class Http(Base):
     enabled: bool = True
-    port: Port = 80
+    port: PortType = 80
 
 
 class Tls(Base):
     cert: FilePath
     key: FilePath
 
 
 class Https(Base):
-    port: Port = 443
+    port: PortType = 443
     tls: Tls | None = None
 
 
-class FileBrowserSettings(Base):
-    enabled: bool = True
-
-
-class JupyterHubSettings(Base):
-    enabled: bool = True
-    password: str | None = None
-
-
-class PrivateBinSettings(Base):
-    enabled: bool = True
-
-
-class RStudioSettings(Base):
-    enabled: bool = True
-    password: str | None = None
-
-
-class XraySettings(Base):
-    enabled: bool = True
-    domain_whitelist: list[str] = []
-    domain_keyword_whitelist: list[str] = []
-    domain_suffix_whitelist: list[str] = []
-    ip_range_whitelist: list[IPv4Network] = []
-
-
-class Modules(Base):
-    filebrowser: FileBrowserSettings = FileBrowserSettings()
-    jupyterhub: JupyterHubSettings = JupyterHubSettings()
-    privatebin: PrivateBinSettings = PrivateBinSettings()
-    rstudio: RStudioSettings = RStudioSettings()
-    xray: XraySettings = XraySettings()
-
-
 class Network(Base):
     hostname: str
     subnet: IPv4Network = IPv4Network("192.168.2.0/24")
     trusted_proxies: list[IPv4Address] = []
     http: Http = Http()
     https: Https = Https()
 
 
+class Plugins(Base):
+    model_config = ConfigDict(extra="ignore")
+
+
 class Privilege(Base):
-    allowed_apps: AllowedApps
+    allowed_apps: AllowedAppsType
 
 
 class Privileges(Base):
     unregistered: Privilege = Privilege(allowed_apps=[])
-    guest: Privilege = Privilege(allowed_apps=[EApp.FILEBROWSER, EApp.PRIVATEBIN])
-    user: Privilege = Privilege(allowed_apps=[EApp.JUPYTERHUB, EApp.RSTUDIO])
+    guest: Privilege = Privilege(allowed_apps=[])
+    user: Privilege = Privilege(allowed_apps=[])
     admin: Privilege = Privilege(allowed_apps="all")
 
 
 class Rules(Base):
     privileges: Privileges = Privileges()
 
 
@@ -116,28 +95,35 @@
 
 
 class Session(Base):
     lifetime: timedelta = timedelta(days=1)
 
 
 class Security(Base):
+    max_body_size: NonNegativeInt = 0
     rate_limiting: RateLimiting = RateLimiting()
     session: Session = Session()
 
 
 class Smtp(Base):
     host: str
-    port: Port
+    port: PortType
     username: str
     password: str
     name: str = APP_NAME_CAPITALIZED
     sender: EmailStr
 
 
+class CoreConfig(Base):
+    model_config = ConfigDict(extra="ignore")
+
+    directories: Directories
+
+
 class Config(Base):
     branding: Branding = Branding()
     directories: Directories
-    modules: Modules = Modules()
     network: Network
+    plugins: Plugins = Plugins()
     rules: Rules = Rules()
     security: Security = Security()
     smtp: Smtp
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/models/users.py` & `lungo_cli-0.3.0/src/lungo_cli/models/users.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from typing import Self
 
 from pydantic import DirectoryPath, EmailStr, field_validator, model_validator, NewPath
 
-from .base import AllowedApps, Base, ERole, NameStr, Username
+from .base import AllowedAppsType, Base, ERole, NameStrType, UsernameType
 from .config import SharedDir
 
 
 class Name(Base):
-    first: NameStr
-    last: NameStr
+    first: NameStrType
+    last: NameStrType
 
 
 class Extra(Base):
-    allowed_apps: AllowedApps = []
+    allowed_apps: AllowedAppsType = []
     user_dir: DirectoryPath | NewPath | None = None
     shared_dirs: list[SharedDir] = []
 
 
 class Account(Base):
     enabled: bool = True
-    username: Username
+    username: UsernameType
     name: Name
     email: EmailStr
     role: ERole
     extra: Extra = Extra()
 
     @model_validator(mode="after")
     def account_model_validator(self) -> Self:
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/config/filebrowser/config_export.yaml` & `lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/config/config_export.yaml`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/config/filebrowser/users_export.yaml.jinja` & `lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/config/users_export.yaml.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/config/jupyterhub/config.py.jinja` & `lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/config/config.py.jinja`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 c.JupyterHub.db_url = 'sqlite:///db.sqlite3?mode=rwc'
 
 ## The class to use for spawning single-user servers
 c.JupyterHub.spawner_class = 'jupyterhub.spawner.LocalProcessSpawner'
 
 ## Downstream proxy IP addresses to trust
 c.JupyterHub.trusted_downstream_ips = [
-    '{{ ip_addresses.nginx }}',
+    '{{ ip_addresses['nginx'] }}',
     {% for proxy in config.network.trusted_proxies %}
     '{{ proxy }}',
     {% endfor %}
 ]
 
 ## Upgrade the database automatically on start
 c.JupyterHub.upgrade_db = True
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/config/kratos/config.yaml.jinja` & `lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/config.yaml.jinja`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% set network = config.network %}
 {% set security = config.security %}
 {% set smtp = config.smtp %}
 
-dsn: 'sqlite:///var/lib/kratos/db.sqlite3?_fk=true&mode=rwc'
+dsn: 'sqlite:////var/lib/kratos/db.sqlite3?_fk=true&mode=rwc'
 
 serve:
   public:
     port: 80
     base_url: '{{ base_url }}'
   admin:
     port: 8080
@@ -45,26 +45,34 @@
       notify_unknown_recipients: false
       after:
         hooks:
           - hook: revoke_active_sessions
   methods:
     code:
       enabled: true
+      passwordless_enabled: true
     password:
       enabled: true
     profile:
       enabled: false
 
 courier:
   smtp:
     connection_uri: 'smtp://{{ smtp.username|urlencode }}:{{ smtp.password }}@{{ smtp.host }}:{{ smtp.port }}/'
     from_address: '{{ smtp.sender }}'
     from_name: '{{ smtp.name }}'
     local_name: '{{ network.hostname }}'
   templates:
+    login_code:
+      valid:
+        email:
+          subject: 'file:///etc/kratos/email_templates/login_code/valid/email.subject.gotmpl'
+          body:
+            html: 'file:///etc/kratos/email_templates/login_code/valid/email.body.gotmpl'
+            plaintext: 'file:///etc/kratos/email_templates/login_code/valid/email.body.plaintext.gotmpl'
     recovery_code:
       valid:
         email:
           subject: 'file:///etc/kratos/email_templates/recovery_code/valid/email.subject.gotmpl'
           body:
             html: 'file:///etc/kratos/email_templates/recovery_code/valid/email.body.gotmpl'
             plaintext: 'file:///etc/kratos/email_templates/recovery_code/valid/email.body.plaintext.gotmpl'
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.body.gotmpl.jinja` & `lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.body.gotmpl.jinja`

 * *Files 0% similar despite different names*

```diff
@@ -363,15 +363,15 @@
                                style="width: 570px; -premailer-width: 570px; -premailer-cellpadding: 0; -premailer-cellspacing: 0; text-align: center; margin: 0 auto; padding: 0;">
                             <tr>
                                 <td class="content-cell" align="center"
                                     style="word-break: break-word; font-family: &quot;Nunito Sans&quot;, Helvetica, Arial, sans-serif; font-size: 16px; padding: 32px 0;">
                                     <p class="f-fallback sub align-center"
                                        style="font-size: 14px; line-height: 1.625; text-align: center; color: #6B6E76; margin: 0;"
                                        align="center">
-                                        © 2023 {{ config.branding.name }}. All rights reserved.
+                                        © 2024 {{ config.branding.name }}. All rights reserved.
                                     </p>
                                 </td>
                             </tr>
                         </table>
                     </td>
                 </tr>
             </table>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
 Recover your account
                                        _{_{_ _c_o_n_f_i_g_._b_r_a_n_d_i_n_g_._n_a_m_e_ _}_}
 ************ HHii {{%% rraaww %%}}{{{{ ..IIddeennttiittyy..ttrraaiittss..nnaammee..ffiirrsstt }}}}{{%% eennddrraaww %%}},, ************
 Please use the code below to validate your identity. If you didn't request one,
 please feel free to ignore this email.
                    {% raw %} {{ .RecoveryCode }}{% endraw %}
 This code will expire in one hour.
-               © 2023 {{ config.branding.name }}. All rights reserved.
+               © 2024 {{ config.branding.name }}. All rights reserved.
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/config/kratos/user.schema.json` & `lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/user.schema.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999932183159722%*

 * *Differences: {"'properties'": "{'traits': {'properties': {'email': {'ory.sh/kratos': {'credentials': {'code': "*

 * *                 "OrderedDict([('identifier', True), ('via', 'email')])}}}}}}"}*

```diff
@@ -4,14 +4,18 @@
         "traits": {
             "additionalProperties": false,
             "properties": {
                 "email": {
                     "format": "email",
                     "ory.sh/kratos": {
                         "credentials": {
+                            "code": {
+                                "identifier": true,
+                                "via": "email"
+                            },
                             "password": {
                                 "identifier": true
                             },
                             "totp": {
                                 "account_name": true
                             },
                             "webauthn": {
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx/conf.d/default.conf.jinja` & `lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx/conf.d/default.conf.jinja`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # Use dedicated writable paths for temporary files
 client_body_temp_path /var/run/nginx/nginx-client-body;
 proxy_temp_path       /var/run/nginx/nginx-proxy;
 fastcgi_temp_path     /var/run/nginx/nginx-fastcgi;
 uwsgi_temp_path       /var/run/nginx/nginx-uwsgi;
 scgi_temp_path        /var/run/nginx/nginx-scgi;
 
-# Support uploading large files
-client_max_body_size 128m;
+# Body size is already checked by the gateway
+client_max_body_size 0;
 
 # Support forwarding websocket connections
 map $http_upgrade $connection_upgrade {
     default Upgrade;
     ""      "";
 }
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx/sites/filebrowser.conf.jinja` & `lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/nginx/site.conf.jinja`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 {% set APP_NAME = 'filebrowser' %}
 
-{% if config.modules.filebrowser.enabled %}
 location = /app/{{ APP_NAME }} {
     include snippets/proxy.conf;
     include snippets/auth.conf;
 
     if ($arg_iframe) {
         return 307 $http_x_forwarded_proto://$http_x_forwarded_host/app/{{ APP_NAME }}/?$args;
     }
@@ -42,8 +41,7 @@
 location @{{ APP_NAME }} {
     include snippets/proxy.conf;
     include snippets/auth.conf;
 
     proxy_pass http://{{ APP_NAME }}$escaped_uri?$filtered_args;
     proxy_redirect ~*^(?:https?://[^/]+)?/app/{{ APP_NAME }}([^?]*)\??(.*)$ $http_x_forwarded_proto://$http_x_forwarded_host/app/{{ APP_NAME }}$1?iframe=1&$2;
 }
-{% endif %}
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx/sites/jupyterhub.conf.jinja` & `lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/nginx/site.conf.jinja`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 {% set APP_NAME = 'jupyterhub' %}
 
-{% if config.modules.jupyterhub.enabled %}
 location = /app/{{ APP_NAME }} {
     include snippets/proxy.conf;
     include snippets/auth.conf;
 
     if ($arg_iframe) {
         return 307 $http_x_forwarded_proto://$http_x_forwarded_host/app/{{ APP_NAME }}/?$args;
     }
@@ -36,8 +35,7 @@
 location @{{ APP_NAME }} {
     include snippets/proxy.conf;
     include snippets/auth.conf;
 
     proxy_pass http://{{ APP_NAME }}$escaped_uri?$filtered_args;
     proxy_redirect ~*^(?:https?://[^/]+)?/app/{{ APP_NAME }}([^?]*)\??(.*)$ $http_x_forwarded_proto://$http_x_forwarded_host/app/{{ APP_NAME }}$1?iframe=1&$2;
 }
-{% endif %}
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx/sites/oathkeeper.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx/sites/oathkeeper.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx/sites/privatebin.conf.jinja` & `lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/nginx/site.conf.jinja`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 {% set APP_NAME = 'privatebin' %}
 
-{% if config.modules.privatebin.enabled %}
 location = /app/{{ APP_NAME }} {
     include snippets/proxy.conf;
     include snippets/auth.conf;
 
     if ($arg_iframe) {
         return 307 $http_x_forwarded_proto://$http_x_forwarded_host/app/{{ APP_NAME }}/?$args;
     }
@@ -35,8 +34,7 @@
     # Break into two lines to avoid regex capturing group being overwritten
     rewrite ^ $escaped_uri?$filtered_args?;
     rewrite ^/app/{{ APP_NAME }}/(.*)$ /$1 break;
 
     proxy_pass http://{{ APP_NAME }};
     proxy_redirect ~*^(?:https?://[^/]+)?/app/{{ APP_NAME }}([^?]*)\??(.*)$ $http_x_forwarded_proto://$http_x_forwarded_host/app/{{ APP_NAME }}?iframe=1&$2;
 }
-{% endif %}
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx/sites/rstudio.conf.jinja` & `lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/nginx/site.conf.jinja`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 {% set APP_NAME = 'rstudio' %}
 
-{% if config.modules.rstudio.enabled %}
 location = /app/{{ APP_NAME }} {
     include snippets/proxy.conf;
     include snippets/auth.conf;
 
     if ($arg_iframe) {
         return 307 $http_x_forwarded_proto://$http_x_forwarded_host/app/{{ APP_NAME }}/?$args;
     }
@@ -41,8 +40,7 @@
     rewrite ^ $escaped_uri?$filtered_args?;
     rewrite ^/app/{{ APP_NAME }}/(.*)$ /$1 break;
 
     proxy_set_header X-RStudio-Root-Path /app/{{ APP_NAME }};
     proxy_pass http://{{ APP_NAME }};
     proxy_redirect ~*^(?:https?://[^/]+)?/app/{{ APP_NAME }}([^?]*)\??(.*)$ $http_x_forwarded_proto://$http_x_forwarded_host/app/{{ APP_NAME }}$1?iframe=1&$2;
 }
-{% endif %}
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx/snippets/auth.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx/snippets/auth.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx/snippets/proxy.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx/snippets/proxy.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx_gateway/conf.d/default.conf.jinja` & `lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx_gateway/conf.d/default.conf.jinja`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 client_body_temp_path /var/run/nginx/nginx-client-body;
 proxy_temp_path       /var/run/nginx/nginx-proxy;
 fastcgi_temp_path     /var/run/nginx/nginx-fastcgi;
 uwsgi_temp_path       /var/run/nginx/nginx-uwsgi;
 scgi_temp_path        /var/run/nginx/nginx-scgi;
 
 # Support uploading large files
-client_max_body_size 128m;
+client_max_body_size {{ '0' if security.max_body_size == 0 else security.max_body_size ~ 'm' }};
 
 # Support forwarding websocket connections
 map $http_upgrade $connection_upgrade {
     default Upgrade;
     ""      "";
 }
 
@@ -35,16 +35,17 @@
         return 301 wss://$host$request_uri;
     }
 
     return 301 https://$host$request_uri;
 }
 
 server {
-    listen [::]:443 ssl http2 default_server;
-    listen 443 ssl http2 default_server;
+    listen [::]:443 ssl default_server;
+    listen 443 ssl default_server;
+    http2 on;
 
     include h5bp/tls/ssl_engine.conf;
     include h5bp/tls/ocsp_stapling.conf;
     include h5bp/tls/policy_balanced.conf;
 
     include snippets/certificate.conf;
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx_gateway/snippets/proxy.conf.jinja` & `lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx_gateway/snippets/proxy.conf.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/config/nginx_gateway/snippets/rate_limiting.conf.jinja` & `lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx_gateway/snippets/rate_limiting.conf.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/config/oathkeeper/access_rules.yaml.jinja` & `lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/oathkeeper/access_rules.yaml.jinja`

 * *Files 16% similar despite different names*

```diff
@@ -27,53 +27,25 @@
     handler: allow
   mutators:
     - handler: noop
   errors:
     - handler: json
 {% endset %}
 
-- id: apps
-  match:
-    url: '{{ base_url }}app/<(?!filebrowser|privatebin)[^/]*><.*>'
-    methods:
-      {{ ALL }}
-  {{ AUTH }}
-
-- id: filebrowser-private
-  match:
-    url: '{{ base_url }}app/<filebrowser><(?!/(?:api/public|share|static)/).*>'
-    methods:
-      {{ ALL }}
-  {{ AUTH }}
-
-- id: filebrowser-public
-  match:
-    url: '{{ base_url }}app/filebrowser<(?=/(?:api/public|share|static)/).*>'
-    methods:
-      {{ ALL }}
-  {{ PASS }}
-
 - id: privatebin-private
   match:
-    url: '{{ base_url }}app/<privatebin><.*>'
+    url: '{{ base_url }}app/<privatebin><(?:$|/).*>'
     methods:
       - POST
       - DELETE
       - PATCH
       - PUT
       - HEAD
       - OPTIONS
   {{ AUTH }}
 
 - id: privatebin-public
   match:
-    url: '{{ base_url }}app/privatebin<.*>'
+    url: '{{ base_url }}app/privatebin<(?:$|/).*>'
     methods:
       - GET
   {{ PASS }}
-
-- id: catch-all
-  match:
-    url: '{{ base_url }}<(?!app/).*>'
-    methods:
-      {{ ALL }}
-  {{ PASS }}
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/config/oathkeeper/config.yaml.jinja` & `lungo_cli-0.3.0/src/lungo_cli/resources/config/oathkeeper/config.yaml.jinja`

 * *Files 15% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     enabled: true
     config:
       subject: anonymous
 
   cookie_session:
     enabled: true
     config:
-      check_session_url: 'http://{{ ip_addresses.kratos }}:80/sessions/whoami'
+      check_session_url: 'http://{{ ip_addresses['kratos'] }}:80/sessions/whoami'
       preserve_path: true
       extra_from: '@this'
       subject_from: 'identity.id'
       only:
         - 'lungo_session'
 
   noop:
@@ -46,15 +46,15 @@
 
 authorizers:
   allow:
     enabled: true
   remote_json:
     enabled: true
     config:
-      remote: 'http://{{ ip_addresses.keto }}:80/relation-tuples/check'
+      remote: 'http://{{ ip_addresses['keto'] }}:80/relation-tuples/check'
       payload: >-
         {% raw %}
         {
           "namespace": "app",
           "object": "{{ printIndex .MatchContext.RegexpCaptureGroups 0 }}",
           "relation": "access",
           "subject_id": "{{ if .Extra.identity }}{{ .Extra.identity.traits.username }}{{ else }}{{ .Subject }}{{ end }}"
@@ -64,15 +64,15 @@
 mutators:
   noop:
     enabled: true
   header:
     enabled: true
     config:
       headers:
-        X-Remote-User: {% raw %}"{{ if .Extra.identity }}{{ .Extra.identity.traits.username }}{{ else }}{{ .Subject }}{{ end }}"{% endraw %}
+        X-Remote-User: '{{ '{{ if .Extra.identity }}{{ .Extra.identity.traits.username }}{{ else }}{{ .Subject }}{{ end }}' }}'
 
 errors:
   handlers:
     json:
       enabled: true
       config:
         verbose: true
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/config/privatebin/conf.php.jinja` & `lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/config/conf.php.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/config/privatebin/site.conf` & `lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/config/site.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/config/xray/config.json.jinja` & `lungo_cli-0.3.0/src/lungo_cli/plugins/xray/config/config.json.jinja`

 * *Files 14% similar despite different names*

```diff
@@ -10,16 +10,16 @@
             "protocol": "vless",
             "listen": "0.0.0.0",
             "port": 80,
             "settings": {
                 "clients": [
                     {% for account in xray_accounts %}
                     {
-                        "email": "{{ account.email }}",
-                        "id": "{{ account.id|string }}"
+                        "email": "{{ account[0] }}",
+                        "id": "{{ account[1]|string }}"
                     }
                     {{- '' if loop.last else ',' }}
                     {% endfor %}
                 ],
                 "decryption": "none"
             },
             "streamSettings": {
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/dockerfiles/filebrowser.Dockerfile.jinja` & `lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/dockerfiles/jupyterhub.Dockerfile.jinja` & `lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/Dockerfile.jinja`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-{% set JUPYTERHUB_VER = '4.0.2' %}
-{% set JUPYTERLAB_VER = '4.1.1' %}
+{% set JUPYTERHUB_VER = '4.1.5' %}
+{% set JUPYTERLAB_VER = '4.1.6' %}
 
 FROM docker.io/jupyterhub/jupyterhub:{{ JUPYTERHUB_VER }}
 RUN python3 -m pip install --no-cache-dir --upgrade setuptools pip && \
     python3 -m pip install --no-cache-dir 'jupyterlab=={{ JUPYTERLAB_VER }}' && \
     {% for account in users.accounts %}
         {% if account.role == 'admin' %}
     useradd --no-log-init -g root -G sudo -m -s /usr/bin/bash '{{ account.username }}' && \
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/dockerfiles/kratos_admin/compose.yaml.jinja` & `lungo_cli-0.3.0/src/lungo_cli/resources/dockerfiles/kratos_admin/compose.yaml.jinja`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% set KRATOS_VER = 'v1.0.0' %}
+{% set KRATOS_VER = 'v1.1.0' %}
 
 services:
   kratos_admin:
     container_name: kratos_admin
     hostname: kratos_admin
 
     image: 'docker.io/oryd/kratos:{{ KRATOS_VER }}'
@@ -17,15 +17,15 @@
       - '3940:8080'
 
     volumes:
       - '../../config/kratos:/etc/kratos:ro'
       - '{{ app_dirs.managed_dir }}/kratos:/var/lib/kratos:rw'
 
     environment:
-      - DSN=sqlite:///var/lib/kratos/db.sqlite3?_fk=true&mode=rwc
+      - DSN=sqlite:////var/lib/kratos/db.sqlite3?_fk=true&mode=rwc
     secrets:
       - source: KRATOS_SECRETS
         target: /etc/kratos/secrets.yaml
 
 secrets:
   KRATOS_SECRETS:
     file: '{{ app_dirs.generated_dir }}/kratos/secrets.yaml'
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/dockerfiles/nginx.Dockerfile.jinja` & `lungo_cli-0.3.0/src/lungo_cli/resources/dockerfiles/nginx.Dockerfile.jinja`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-{% set NGINX_VER = '1.21.4.3-alpine-apk' %}
+{% set NGINX_VER = '1.25.3.1-alpine-apk' %}
 
 FROM docker.io/openresty/openresty:{{ NGINX_VER }}
 RUN adduser -D -H -S www-data && \
-    apk --update add logrotate && \
+    apk add --no-cache logrotate && \
     printf '%s\n' >/etc/logrotate.d/nginx \
         '/var/log/nginx/*.log {' \
         '    daily' \
         '    compress' \
         '    delaycompress' \
         '    rotate 30' \
         '    missingok' \
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/dockerfiles/rstudio.Dockerfile.jinja` & `lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/Dockerfile.jinja`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% set RSTUDIO_VER = '4.3.2' %}
+{% set RSTUDIO_VER = '4.3.3' %}
 
 FROM docker.io/rocker/verse:{{ RSTUDIO_VER }}
 RUN : && \
     {% for account in users.accounts %}
         {% if account.role == 'admin' %}
     useradd --no-log-init -g root -G sudo -m -s /usr/bin/bash '{{ account.username }}' && \
         {% else %}
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/excluded/config.yaml` & `lungo_cli-0.3.0/src/lungo_cli/resources/assets/config_references/config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -70,99 +70,14 @@
 #         # Whether to mount the directory as read-only or not
 #         # Type: boolean
 #         # Default: false
 #         # Required: no
 #         read_only: true
 
 # ========
-# modules:
-# ========
-
-#   # Settings for the File Browser module
-#   filebrowser:
-
-#     # Enable or disable the module
-#     # Type: boolean
-#     # Default: true
-#     # Required: no
-#     enabled: true
-
-#   # Settings for the JupyterHub module
-#   jupyterhub:
-
-#     # Enable or disable the module
-#     # Type: boolean
-#     # Default: true
-#     # Required: no
-#     enabled: true
-
-#     # Password for users inside the container
-#     # Type: string
-#     # Default: (randomly generated)
-#     # Required: no
-#     password: passwd
-
-#   # Settings for the PrivateBin module
-#   privatebin:
-
-#     # Enable or disable the module
-#     # Type: boolean
-#     # Default: true
-#     # Required: no
-#     enabled: true
-
-#   # Settings for the RStudio module
-#   rstudio:
-
-#     # Enable or disable the module
-#     # Type: boolean
-#     # Default: true
-#     # Required: no
-#     enabled: true
-
-#     # Password for users inside the container
-#     # Type: string
-#     # Default: (randomly generated)
-#     # Required: no
-#     password: passwd
-
-#   # Settings for the Xray module
-#   xray:
-
-#     # Enable or disable the module
-#     # Type: boolean
-#     # Default: true
-#     # Required: no
-#     enabled: true
-
-#     # Domain whitelist (used only as a template for configuring the proxy client)
-#     # Type: array
-#     # Default: [ ]
-#     # Required: no
-#     domain_whitelist: [ ]
-
-#     # Domain keyword whitelist (used only as a template for configuring the proxy client)
-#     # Type: array
-#     # Default: [ ]
-#     # Required: no
-#     domain_keyword_whitelist: [ ]
-
-#     # Domain suffix whitelist (used only as a template for configuring the proxy client)
-#     # Type: array
-#     # Default: [ ]
-#     # Required: no
-#     domain_suffix_whitelist: [ ]
-
-#     # IP range whitelist (used only as a template for configuring the proxy client)
-#     # Type: array
-#     # Default: [ ]
-#     # Required: no
-#     ip_range_whitelist: [ ]
-
-# ========
 # network:
 # ========
 
 #   # Hostname of the website
 #   # Type: string
 #   # Default: none
 #   # Required: yes
@@ -215,14 +130,18 @@
 
 #       # Path to the TLS private key
 #       # Type: path
 #       # Default: none
 #       # Required: no
 #       key: /etc/ssl/private/self-signed.key
 
+# ========
+# plugins:
+# ========
+
 # ======
 # rules:
 # ======
 
 #   # Privileges of each role (privileges are inherited from roles above)
 #   privileges:
 
@@ -236,68 +155,72 @@
 #       allowed_apps: [ ]
 
 #     # For guest users
 #     guest:
 
 #       # Allowed apps, or 'all' to allow all apps
 #       # Type: 'all' | array
-#       # Default: ['filebrowser', 'privatebin']
+#       # Default: [ ]
 #       # Required: no
-#       allowed_apps:
-#         - filebrowser
+#       allowed_apps: [ ]
 
 #     # For regular users
 #     user:
 
 #       # Allowed apps, or 'all' to allow all apps
 #       # Type: 'all' | array
-#       # Default: ['jupyterhub', 'rstudio']
+#       # Default: [ ]
 #       # Required: no
-#       allowed_apps:
-#         - rstudio
+#       allowed_apps: [ ]
 
 #     # For administrators
 #     admin:
 
 #       # Allowed apps, or 'all' to allow all apps
 #       # Type: 'all' | array
 #       # Default: 'all'
 #       # Required: no
 #       allowed_apps: all
 
 # =========
 # security:
 # =========
 
+#   # Maximum size of the request body allowed in megabytes (or 0 for unlimited)
+#   # Type: integer
+#   # Default: 0
+#   # Required: no
+#   max_body_size: 0
+
 #   # Rate limiting settings
 #   rate_limiting:
 
 #     # Enable or disable rate limiting
 #     # Type: boolean
 #     # Default: false
 #     # Required: no
 #     enabled: false
 
 #     # Maximum number of requests in the given time window
-#     # Type: int
+#     # Type: integer
 #     # Default: 5
 #     # Required: no
 #     max_requests: 5
 
 #     # Time window (in seconds, or a string describing a time span in ISO 8601 format)
-#     # Type: int | string
+#     # Type: integer | string
 #     # Default: 'PT1H'
 #     # Required: no
 #     time_window: 'PT1H'
 
 #   # Session settings
 #   session:
 
 #     # Session lifetime (in seconds, or a string describing a time span in ISO 8601 format)
-#     # Type: int | string
+#     # Type: integer | string
 #     # Default: 'P1DT'
 #     # Required: no
 #     lifetime: 'P1DT'
 
 # =====
 # smtp:
 # =====
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/excluded/users.yaml` & `lungo_cli-0.3.0/src/lungo_cli/resources/assets/config_references/users.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 #       extra:
 
 #         # Allowed apps besides those defined in the role, or 'all' to allow all apps
 #         # Type: 'all' | array
 #         # Default: [ ]
 #         # Required: no
 #         allowed_apps:
-#           - rstudio
+#           - all
 
 #         # Override user directory
 #         # Type: path
 #         # Default: none
 #         # Required: no
 #         user_dir: /mnt/somewhere/someone
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/.gitattributes` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.gitattributes`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CONTRIBUTING.md` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/auto-merge.yml` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/auto-merge.yml`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/server.yml` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/server.yml`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/CHANGELOG.md` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/LICENSE.txt` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/README.md` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/README.md`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/.default.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/.default.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/no-ssl.default.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/no-ssl.default.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/example.com.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/example.com.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/no-ssl.example.com.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/no-ssl.example.com.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/requests.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/requests.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/resource_timing.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/resource_timing.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/security_file_access.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/security_file_access.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_filename-based_cache_busting.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_filename-based_cache_busting.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_svgz-compression.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_svgz-compression.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/character_encodings.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/character_encodings.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/media_types.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/media_types.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/content-security-policy.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/content-security-policy.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/cross-origin-policy.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/cross-origin-policy.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/permissions-policy.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/permissions-policy.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/referrer-policy.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/referrer-policy.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/strict-transport-security.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/strict-transport-security.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-content-type-options.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-content-type-options.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-frame-options.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-frame-options.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/certificate_files.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/certificate_files.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ocsp_stapling.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ocsp_stapling.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_balanced.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_balanced.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_strict.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_strict.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ssl_engine.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ssl_engine.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-control.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-control.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-file-descriptors.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-file-descriptors.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache_expiration.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache_expiration.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/compression.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/compression.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/content_transformation.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/content_transformation.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_brotli.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_brotli.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_gzip.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_gzip.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/mime.types` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/mime.types`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/nginx.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/nginx.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/secure.server.localhost.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/secure.server.localhost.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/server.localhost.conf` & `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/server.localhost.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/.eslintrc.cjs` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/.eslintrc.cjs`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/assets/schemas/keto.openapi.json` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/assets/schemas/keto.openapi.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.997055431547619%*

 * *Differences: {"'components'": "{'schemas': {'DefaultError': OrderedDict(), 'unexpectedError': "*

 * *                 "OrderedDict([('type', 'string')])}}",*

 * * "'paths'": "{'/health/alive': {'get': {'responses': {'default': OrderedDict([('content', "*

 * *            "OrderedDict([('text/plain', OrderedDict([('schema', OrderedDict([('type', "*

 * *            "'string')]))]))])), ('description', 'Unexpected error')]), delete: ['500']}}}, "*

 * *            "'/health/ready': {'get': {'responses': {'default': OrderedDict([('content', "*

 * *        […]*

```diff
@@ -2,14 +2,15 @@
     "components": {
         "responses": {
             "emptyResponse": {
                 "description": "Empty responses are sent when, for example, resources are deleted. The HTTP status code for empty responses is typically 204."
             }
         },
         "schemas": {
+            "DefaultError": {},
             "ParseError": {
                 "properties": {
                     "end": {
                         "$ref": "#/components/schemas/SourcePosition"
                     },
                     "message": {
                         "type": "string"
@@ -385,14 +386,17 @@
                 "required": [
                     "namespace",
                     "object",
                     "relation"
                 ],
                 "type": "object"
             },
+            "unexpectedError": {
+                "type": "string"
+            },
             "version": {
                 "properties": {
                     "version": {
                         "description": "Version is the service's version.",
                         "type": "string"
                     }
                 },
@@ -632,23 +636,23 @@
                                     ],
                                     "type": "object"
                                 }
                             }
                         },
                         "description": "Ory Keto is ready to accept connections."
                     },
-                    "500": {
+                    "default": {
                         "content": {
-                            "application/json": {
+                            "text/plain": {
                                 "schema": {
-                                    "$ref": "#/components/schemas/genericError"
+                                    "type": "string"
                                 }
                             }
                         },
-                        "description": "genericError"
+                        "description": "Unexpected error"
                     }
                 },
                 "summary": "Check HTTP Server Status",
                 "tags": [
                     "metadata"
                 ]
             }
@@ -694,14 +698,24 @@
                                         "errors"
                                     ],
                                     "type": "object"
                                 }
                             }
                         },
                         "description": "Ory Kratos is not yet ready to accept requests."
+                    },
+                    "default": {
+                        "content": {
+                            "text/plain": {
+                                "schema": {
+                                    "type": "string"
+                                }
+                            }
+                        },
+                        "description": "Unexpected error"
                     }
                 },
                 "summary": "Check HTTP Server and Database Status",
                 "tags": [
                     "metadata"
                 ]
             }
@@ -1023,15 +1037,14 @@
                 ]
             },
             "post": {
                 "description": "To learn how relationship tuples and the check works, head over to [the documentation](https://www.ory.sh/docs/keto/concepts/api-overview).",
                 "operationId": "postCheckPermissionOrError",
                 "parameters": [
                     {
-                        "description": "nolint:deadcode,unused",
                         "in": "query",
                         "name": "max-depth",
                         "schema": {
                             "format": "int64",
                             "type": "integer"
                         }
                     }
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/assets/schemas/kratos.openapi.json` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/assets/schemas/kratos.openapi.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9983708449818184%*

 * *Differences: {"'components'": "{'schemas': {'OAuth2Client': {'properties': {'client_id': {'description': 'OAuth "*

 * *                 '2.0 Client ID  The ID is immutable. If no ID is provided, a UUID4 will be '*

 * *                 "generated.'}, 'token_endpoint_auth_method': {'description': 'OAuth 2.0 Token "*

 * *                 'Endpoint Authentication Method  Requested Client Authentication method for the '*

 * *                 'Token Endpoint. The options are:  `client_secret_basic`: (default) Send '*

 * *                 '`client_id` […]*

```diff
@@ -115,14 +115,18 @@
             "NullUUID": {
                 "format": "uuid4",
                 "nullable": true,
                 "type": "string"
             },
             "OAuth2Client": {
                 "properties": {
+                    "access_token_strategy": {
+                        "description": "OAuth 2.0 Access Token Strategy  AccessTokenStrategy is the strategy used to generate access tokens. Valid options are `jwt` and `opaque`. `jwt` is a bad idea, see https://www.ory.sh/docs/hydra/advanced#json-web-tokens Setting the stragegy here overrides the global setting in `strategies.access_token`.",
+                        "type": "string"
+                    },
                     "allowed_cors_origins": {
                         "items": {
                             "type": "string"
                         },
                         "type": "array"
                     },
                     "audience": {
@@ -152,15 +156,15 @@
                         "type": "string"
                     },
                     "client_credentials_grant_access_token_lifespan": {
                         "description": "Specify a time duration in milliseconds, seconds, minutes, hours.",
                         "type": "string"
                     },
                     "client_id": {
-                        "description": "OAuth 2.0 Client ID  The ID is autogenerated and immutable.",
+                        "description": "OAuth 2.0 Client ID  The ID is immutable. If no ID is provided, a UUID4 will be generated.",
                         "type": "string"
                     },
                     "client_name": {
                         "description": "OAuth 2.0 Client Name  The human-readable name of the client to be presented to the end-user during authorization.",
                         "type": "string"
                     },
                     "client_secret": {
@@ -285,20 +289,28 @@
                         "description": "OAuth 2.0 Client Scope  Scope is a string containing a space-separated list of scope values (as described in Section 3.3 of OAuth 2.0 [RFC6749]) that the client can use when requesting access tokens.",
                         "type": "string"
                     },
                     "sector_identifier_uri": {
                         "description": "OpenID Connect Sector Identifier URI  URL using the https scheme to be used in calculating Pseudonymous Identifiers by the OP. The URL references a file with a single JSON array of redirect_uri values.",
                         "type": "string"
                     },
+                    "skip_consent": {
+                        "description": "SkipConsent skips the consent screen for this client. This field can only be set from the admin API.",
+                        "type": "boolean"
+                    },
+                    "skip_logout_consent": {
+                        "description": "SkipLogoutConsent skips the logout consent screen for this client. This field can only be set from the admin API.",
+                        "type": "boolean"
+                    },
                     "subject_type": {
                         "description": "OpenID Connect Subject Type  The `subject_types_supported` Discovery parameter contains a list of the supported subject_type values for this server. Valid types include `pairwise` and `public`.",
                         "type": "string"
                     },
                     "token_endpoint_auth_method": {
-                        "description": "OAuth 2.0 Token Endpoint Authentication Method  Requested Client Authentication method for the Token Endpoint. The options are:  `client_secret_post`: (default) Send `client_id` and `client_secret` as `application/x-www-form-urlencoded` in the HTTP body. `client_secret_basic`: Send `client_id` and `client_secret` as `application/x-www-form-urlencoded` encoded in the HTTP Authorization header. `private_key_jwt`: Use JSON Web Tokens to authenticate the client. `none`: Used for public clients (native apps, mobile apps) which can not have secrets.",
+                        "description": "OAuth 2.0 Token Endpoint Authentication Method  Requested Client Authentication method for the Token Endpoint. The options are:  `client_secret_basic`: (default) Send `client_id` and `client_secret` as `application/x-www-form-urlencoded` encoded in the HTTP Authorization header. `client_secret_post`: Send `client_id` and `client_secret` as `application/x-www-form-urlencoded` in the HTTP body. `private_key_jwt`: Use JSON Web Tokens to authenticate the client. `none`: Used for public clients (native apps, mobile apps) which can not have secrets.",
                         "type": "string"
                     },
                     "token_endpoint_auth_signing_alg": {
                         "description": "OAuth 2.0 Token Endpoint Signing Algorithm  Requested Client Authentication signing algorithm for the Token Endpoint.",
                         "type": "string"
                     },
                     "tos_uri": {
@@ -347,14 +359,17 @@
                             "type": "string"
                         },
                         "type": "array"
                     }
                 },
                 "type": "object"
             },
+            "OAuth2LoginChallengeParams": {
+                "type": "object"
+            },
             "OAuth2LoginRequest": {
                 "description": "OAuth2LoginRequest struct for OAuth2LoginRequest",
                 "properties": {
                     "challenge": {
                         "description": "ID is the identifier (\\\"login challenge\\\") of the login request. It is used to identify the session.",
                         "type": "string"
                     },
@@ -427,65 +442,159 @@
                             "$ref": "#/components/schemas/identityPatchResponse"
                         },
                         "type": "array"
                     }
                 },
                 "type": "object"
             },
+            "consistencyRequestParameters": {
+                "description": "Control API consistency guarantees",
+                "properties": {
+                    "consistency": {
+                        "description": "Read Consistency Level (preview)\n\nThe read consistency level determines the consistency guarantee for reads:\n\nstrong (slow): The read is guaranteed to return the most recent data committed at the start of the read.\neventual (very fast): The result will return data that is about 4.8 seconds old.\n\nThe default consistency guarantee can be changed in the Ory Network Console or using the Ory CLI with\n`ory patch project --replace '/previews/default_read_consistency_level=\"strong\"'`.\n\nSetting the default consistency level to `eventual` may cause regressions in the future as we add consistency\ncontrols to more APIs. Currently, the following APIs will be affected by this setting:\n\n`GET /admin/identities`\n\nThis feature is in preview and only available in Ory Network.\n ConsistencyLevelUnset  ConsistencyLevelUnset is the unset / default consistency level.\nstrong ConsistencyLevelStrong  ConsistencyLevelStrong is the strong consistency level.\neventual ConsistencyLevelEventual  ConsistencyLevelEventual is the eventual consistency level using follower read timestamps.",
+                        "enum": [
+                            "",
+                            "strong",
+                            "eventual"
+                        ],
+                        "type": "string",
+                        "x-go-enum-desc": " ConsistencyLevelUnset  ConsistencyLevelUnset is the unset / default consistency level.\nstrong ConsistencyLevelStrong  ConsistencyLevelStrong is the strong consistency level.\neventual ConsistencyLevelEventual  ConsistencyLevelEventual is the eventual consistency level using follower read timestamps."
+                    }
+                },
+                "type": "object"
+            },
             "continueWith": {
                 "discriminator": {
                     "mapping": {
                         "set_ory_session_token": "#/components/schemas/continueWithSetOrySessionToken",
+                        "show_recovery_ui": "#/components/schemas/continueWithRecoveryUi",
+                        "show_settings_ui": "#/components/schemas/continueWithSettingsUi",
                         "show_verification_ui": "#/components/schemas/continueWithVerificationUi"
                     },
                     "propertyName": "action"
                 },
                 "oneOf": [
                     {
                         "$ref": "#/components/schemas/continueWithVerificationUi"
                     },
                     {
                         "$ref": "#/components/schemas/continueWithSetOrySessionToken"
+                    },
+                    {
+                        "$ref": "#/components/schemas/continueWithSettingsUi"
+                    },
+                    {
+                        "$ref": "#/components/schemas/continueWithRecoveryUi"
                     }
                 ]
             },
+            "continueWithRecoveryUi": {
+                "description": "Indicates, that the UI flow could be continued by showing a recovery ui",
+                "properties": {
+                    "action": {
+                        "description": "Action will always be `show_recovery_ui`\nshow_recovery_ui ContinueWithActionShowRecoveryUIString",
+                        "enum": [
+                            "show_recovery_ui"
+                        ],
+                        "type": "string",
+                        "x-go-enum-desc": "show_recovery_ui ContinueWithActionShowRecoveryUIString"
+                    },
+                    "flow": {
+                        "$ref": "#/components/schemas/continueWithRecoveryUiFlow"
+                    }
+                },
+                "required": [
+                    "action",
+                    "flow"
+                ],
+                "type": "object"
+            },
+            "continueWithRecoveryUiFlow": {
+                "properties": {
+                    "id": {
+                        "description": "The ID of the recovery flow",
+                        "format": "uuid",
+                        "type": "string"
+                    },
+                    "url": {
+                        "description": "The URL of the recovery flow",
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "id"
+                ],
+                "type": "object"
+            },
             "continueWithSetOrySessionToken": {
                 "description": "Indicates that a session was issued, and the application should use this token for authenticated requests",
                 "properties": {
                     "action": {
-                        "description": "Action will always be `set_ory_session_token`\nset_ory_session_token ContinueWithActionSetOrySessionToken\nshow_verification_ui ContinueWithActionShowVerificationUI",
+                        "description": "Action will always be `set_ory_session_token`\nset_ory_session_token ContinueWithActionSetOrySessionTokenString",
                         "enum": [
-                            "set_ory_session_token",
-                            "show_verification_ui"
+                            "set_ory_session_token"
                         ],
                         "type": "string",
-                        "x-go-enum-desc": "set_ory_session_token ContinueWithActionSetOrySessionToken\nshow_verification_ui ContinueWithActionShowVerificationUI"
+                        "x-go-enum-desc": "set_ory_session_token ContinueWithActionSetOrySessionTokenString"
                     },
                     "ory_session_token": {
                         "description": "Token is the token of the session",
                         "type": "string"
                     }
                 },
                 "required": [
                     "action",
                     "ory_session_token"
                 ],
                 "type": "object"
             },
+            "continueWithSettingsUi": {
+                "description": "Indicates, that the UI flow could be continued by showing a settings ui",
+                "properties": {
+                    "action": {
+                        "description": "Action will always be `show_settings_ui`\nshow_settings_ui ContinueWithActionShowSettingsUIString",
+                        "enum": [
+                            "show_settings_ui"
+                        ],
+                        "type": "string",
+                        "x-go-enum-desc": "show_settings_ui ContinueWithActionShowSettingsUIString"
+                    },
+                    "flow": {
+                        "$ref": "#/components/schemas/continueWithSettingsUiFlow"
+                    }
+                },
+                "required": [
+                    "action",
+                    "flow"
+                ],
+                "type": "object"
+            },
+            "continueWithSettingsUiFlow": {
+                "properties": {
+                    "id": {
+                        "description": "The ID of the settings flow",
+                        "format": "uuid",
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "id"
+                ],
+                "type": "object"
+            },
             "continueWithVerificationUi": {
                 "description": "Indicates, that the UI flow could be continued by showing a verification ui",
                 "properties": {
                     "action": {
-                        "description": "Action will always be `show_verification_ui`\nset_ory_session_token ContinueWithActionSetOrySessionToken\nshow_verification_ui ContinueWithActionShowVerificationUI",
+                        "description": "Action will always be `show_verification_ui`\nshow_verification_ui ContinueWithActionShowVerificationUIString",
                         "enum": [
-                            "set_ory_session_token",
                             "show_verification_ui"
                         ],
                         "type": "string",
-                        "x-go-enum-desc": "set_ory_session_token ContinueWithActionSetOrySessionToken\nshow_verification_ui ContinueWithActionShowVerificationUI"
+                        "x-go-enum-desc": "show_verification_ui ContinueWithActionShowVerificationUIString"
                     },
                     "flow": {
                         "$ref": "#/components/schemas/continueWithVerificationUiFlow"
                     }
                 },
                 "required": [
                     "action",
@@ -554,15 +663,21 @@
                         "type": "array"
                     },
                     "schema_id": {
                         "description": "SchemaID is the ID of the JSON Schema to be used for validating the identity's traits.",
                         "type": "string"
                     },
                     "state": {
-                        "$ref": "#/components/schemas/identityState"
+                        "description": "State is the identity's state.\nactive StateActive\ninactive StateInactive",
+                        "enum": [
+                            "active",
+                            "inactive"
+                        ],
+                        "type": "string",
+                        "x-go-enum-desc": "active StateActive\ninactive StateInactive"
                     },
                     "traits": {
                         "description": "Traits represent an identity's traits. The identity is able to create, modify, and delete traits\nin a self-service manner. The input will always be validated against the JSON Schema defined\nin `schema_url`.",
                         "type": "object"
                     },
                     "verifiable_addresses": {
                         "description": "VerifiableAddresses contains all the addresses that can be verified by the user.\n\nUse this structure to import verified addresses for an identity. Please keep in mind\nthat the address needs to be represented in the Identity Schema or this field will be overwritten\non the next identity update.",
@@ -797,14 +912,17 @@
                     },
                     "metadata_admin": {
                         "$ref": "#/components/schemas/nullJsonRawMessage"
                     },
                     "metadata_public": {
                         "$ref": "#/components/schemas/nullJsonRawMessage"
                     },
+                    "organization_id": {
+                        "$ref": "#/components/schemas/NullUUID"
+                    },
                     "recovery_addresses": {
                         "description": "RecoveryAddresses contains all the addresses that can be used to recover an identity.",
                         "items": {
                             "$ref": "#/components/schemas/recoveryIdentityAddress"
                         },
                         "type": "array",
                         "x-omitempty": true
@@ -814,15 +932,21 @@
                         "type": "string"
                     },
                     "schema_url": {
                         "description": "SchemaURL is the URL of the endpoint where the identity's traits schema can be fetched from.\n\nformat: url",
                         "type": "string"
                     },
                     "state": {
-                        "$ref": "#/components/schemas/identityState"
+                        "description": "State is the identity's state.\n\nThis value has currently no effect.\nactive StateActive\ninactive StateInactive",
+                        "enum": [
+                            "active",
+                            "inactive"
+                        ],
+                        "type": "string",
+                        "x-go-enum-desc": "active StateActive\ninactive StateInactive"
                     },
                     "state_changed_at": {
                         "$ref": "#/components/schemas/nullTime"
                     },
                     "traits": {
                         "$ref": "#/components/schemas/identityTraits"
                     },
@@ -864,29 +988,54 @@
                         "description": "Identifiers represents a list of unique identifiers this credential type matches.",
                         "items": {
                             "type": "string"
                         },
                         "type": "array"
                     },
                     "type": {
-                        "$ref": "#/components/schemas/identityCredentialsType"
+                        "description": "Type discriminates between different types of credentials.\npassword CredentialsTypePassword\noidc CredentialsTypeOIDC\ntotp CredentialsTypeTOTP\nlookup_secret CredentialsTypeLookup\nwebauthn CredentialsTypeWebAuthn\ncode CredentialsTypeCodeAuth\nlink_recovery CredentialsTypeRecoveryLink  CredentialsTypeRecoveryLink is a special credential type linked to the link strategy (recovery flow).  It is not used within the credentials object itself.\ncode_recovery CredentialsTypeRecoveryCode",
+                        "enum": [
+                            "password",
+                            "oidc",
+                            "totp",
+                            "lookup_secret",
+                            "webauthn",
+                            "code",
+                            "link_recovery",
+                            "code_recovery"
+                        ],
+                        "type": "string",
+                        "x-go-enum-desc": "password CredentialsTypePassword\noidc CredentialsTypeOIDC\ntotp CredentialsTypeTOTP\nlookup_secret CredentialsTypeLookup\nwebauthn CredentialsTypeWebAuthn\ncode CredentialsTypeCodeAuth\nlink_recovery CredentialsTypeRecoveryLink  CredentialsTypeRecoveryLink is a special credential type linked to the link strategy (recovery flow).  It is not used within the credentials object itself.\ncode_recovery CredentialsTypeRecoveryCode"
                     },
                     "updated_at": {
                         "description": "UpdatedAt is a helper struct field for gobuffalo.pop.",
                         "format": "date-time",
                         "type": "string"
                     },
                     "version": {
                         "description": "Version refers to the version of the credential. Useful when changing the config schema.",
                         "format": "int64",
                         "type": "integer"
                     }
                 },
                 "type": "object"
             },
+            "identityCredentialsCode": {
+                "description": "CredentialsCode represents a one time login/registration code",
+                "properties": {
+                    "address_type": {
+                        "description": "The type of the address for this code",
+                        "type": "string"
+                    },
+                    "used_at": {
+                        "$ref": "#/components/schemas/NullTime"
+                    }
+                },
+                "type": "object"
+            },
             "identityCredentialsOidc": {
                 "properties": {
                     "providers": {
                         "items": {
                             "$ref": "#/components/schemas/identityCredentialsOidcProvider"
                         },
                         "type": "array"
@@ -902,14 +1051,17 @@
                     },
                     "initial_id_token": {
                         "type": "string"
                     },
                     "initial_refresh_token": {
                         "type": "string"
                     },
+                    "organization": {
+                        "type": "string"
+                    },
                     "provider": {
                         "type": "string"
                     },
                     "subject": {
                         "type": "string"
                     }
                 },
@@ -922,26 +1074,14 @@
                         "description": "HashedPassword is a hash-representation of the password.",
                         "type": "string"
                     }
                 },
                 "title": "CredentialsPassword is contains the configuration for credentials of the type password.",
                 "type": "object"
             },
-            "identityCredentialsType": {
-                "description": "and so on.",
-                "enum": [
-                    "password",
-                    "totp",
-                    "oidc",
-                    "webauthn",
-                    "lookup_secret"
-                ],
-                "title": "CredentialsType  represents several different credential types, like password credentials, passwordless credentials,",
-                "type": "string"
-            },
             "identityPatch": {
                 "description": "Payload for patching an identity",
                 "properties": {
                     "create": {
                         "$ref": "#/components/schemas/createIdentityBody"
                     },
                     "patch_id": {
@@ -997,34 +1137,21 @@
             "identitySchemas": {
                 "description": "List of Identity JSON Schemas",
                 "items": {
                     "$ref": "#/components/schemas/identitySchemaContainer"
                 },
                 "type": "array"
             },
-            "identityState": {
-                "description": "The state can either be `active` or `inactive`.",
-                "enum": [
-                    "active",
-                    "inactive"
-                ],
-                "title": "An Identity's State",
-                "type": "string"
-            },
             "identityTraits": {
                 "description": "Traits represent an identity's traits. The identity is able to create, modify, and delete traits\nin a self-service manner. The input will always be validated against the JSON Schema defined\nin `schema_url`."
             },
             "identityVerifiableAddressStatus": {
                 "description": "VerifiableAddressStatus must not exceed 16 characters as that is the limitation in the SQL Schema",
                 "type": "string"
             },
-            "identityVerifiableAddressType": {
-                "description": "VerifiableAddressType must not exceed 16 characters as that is the limitation in the SQL Schema",
-                "type": "string"
-            },
             "identityWithCredentials": {
                 "description": "Create Identity and Import Credentials",
                 "properties": {
                     "oidc": {
                         "$ref": "#/components/schemas/identityWithCredentialsOidc"
                     },
                     "password": {
@@ -1084,15 +1211,15 @@
                 },
                 "type": "object"
             },
             "identityWithCredentialsPasswordConfig": {
                 "description": "Create Identity and Import Password Credentials Configuration",
                 "properties": {
                     "hashed_password": {
-                        "description": "The hashed password in [PHC format]( https://www.ory.sh/docs/kratos/concepts/credentials/username-email-password#hashed-password-format)",
+                        "description": "The hashed password in [PHC format](https://www.ory.sh/docs/kratos/manage-identities/import-user-accounts-identities#hashed-passwords)",
                         "type": "string"
                     },
                     "password": {
                         "description": "The password in plain text if no hash is available.",
                         "type": "string"
                     }
                 },
@@ -1134,15 +1261,27 @@
                 },
                 "type": "array"
             },
             "loginFlow": {
                 "description": "This object represents a login flow. A login flow is initiated at the \"Initiate Login API / Browser Flow\"\nendpoint by a client.\n\nOnce a login flow is completed successfully, a session cookie or session token will be issued.",
                 "properties": {
                     "active": {
-                        "$ref": "#/components/schemas/identityCredentialsType"
+                        "description": "The active login method\n\nIf set contains the login method used. If the flow is new, it is unset.\npassword CredentialsTypePassword\noidc CredentialsTypeOIDC\ntotp CredentialsTypeTOTP\nlookup_secret CredentialsTypeLookup\nwebauthn CredentialsTypeWebAuthn\ncode CredentialsTypeCodeAuth\nlink_recovery CredentialsTypeRecoveryLink  CredentialsTypeRecoveryLink is a special credential type linked to the link strategy (recovery flow).  It is not used within the credentials object itself.\ncode_recovery CredentialsTypeRecoveryCode",
+                        "enum": [
+                            "password",
+                            "oidc",
+                            "totp",
+                            "lookup_secret",
+                            "webauthn",
+                            "code",
+                            "link_recovery",
+                            "code_recovery"
+                        ],
+                        "type": "string",
+                        "x-go-enum-desc": "password CredentialsTypePassword\noidc CredentialsTypeOIDC\ntotp CredentialsTypeTOTP\nlookup_secret CredentialsTypeLookup\nwebauthn CredentialsTypeWebAuthn\ncode CredentialsTypeCodeAuth\nlink_recovery CredentialsTypeRecoveryLink  CredentialsTypeRecoveryLink is a special credential type linked to the link strategy (recovery flow).  It is not used within the credentials object itself.\ncode_recovery CredentialsTypeRecoveryCode"
                     },
                     "created_at": {
                         "description": "CreatedAt is a helper struct field for gobuffalo.pop.",
                         "format": "date-time",
                         "type": "string"
                     },
                     "expires_at": {
@@ -1163,14 +1302,17 @@
                     "oauth2_login_challenge": {
                         "description": "Ory OAuth 2.0 Login Challenge.\n\nThis value is set using the `login_challenge` query parameter of the registration and login endpoints.\nIf set will cooperate with Ory OAuth2 and OpenID to act as an OAuth2 server / OpenID Provider.",
                         "type": "string"
                     },
                     "oauth2_login_request": {
                         "$ref": "#/components/schemas/OAuth2LoginRequest"
                     },
+                    "organization_id": {
+                        "$ref": "#/components/schemas/NullUUID"
+                    },
                     "refresh": {
                         "description": "Refresh stores whether this login flow should enforce re-authentication.",
                         "type": "boolean"
                     },
                     "request_url": {
                         "description": "RequestURL is the initial URL that was requested from Ory Kratos. It can be used\nto forward information contained in the URL's path or query for example.",
                         "type": "string"
@@ -1182,14 +1324,17 @@
                         "description": "ReturnTo contains the requested return_to URL.",
                         "type": "string"
                     },
                     "session_token_exchange_code": {
                         "description": "SessionTokenExchangeCode holds the secret code that the client can use to retrieve a session token after the login flow has been completed.\nThis is only set if the client has requested a session token exchange code, and if the flow is of type \"api\",\nand only on creating the login flow.",
                         "type": "string"
                     },
+                    "state": {
+                        "description": "State represents the state of this request:\n\nchoose_method: ask the user to choose a method to sign in with\nsent_email: the email has been sent to the user\npassed_challenge: the request was successful and the login challenge was passed."
+                    },
                     "type": {
                         "$ref": "#/components/schemas/selfServiceFlowType"
                     },
                     "ui": {
                         "$ref": "#/components/schemas/uiContainer"
                     },
                     "updated_at": {
@@ -1200,19 +1345,29 @@
                 },
                 "required": [
                     "id",
                     "type",
                     "expires_at",
                     "issued_at",
                     "request_url",
-                    "ui"
+                    "ui",
+                    "state"
                 ],
                 "title": "Login Flow",
                 "type": "object"
             },
+            "loginFlowState": {
+                "description": "The state represents the state of the login flow.\n\nchoose_method: ask the user to choose a method (e.g. login account via email)\nsent_email: the email has been sent to the user\npassed_challenge: the request was successful and the login challenge was passed.",
+                "enum": [
+                    "choose_method",
+                    "sent_email",
+                    "passed_challenge"
+                ],
+                "title": "Login Flow State"
+            },
             "logoutFlow": {
                 "description": "Logout Flow",
                 "properties": {
                     "logout_token": {
                         "description": "LogoutToken can be used to perform logout using AJAX.",
                         "type": "string"
                     },
@@ -1228,14 +1383,17 @@
                 "type": "object"
             },
             "message": {
                 "properties": {
                     "body": {
                         "type": "string"
                     },
+                    "channel": {
+                        "type": "string"
+                    },
                     "created_at": {
                         "description": "CreatedAt is a helper struct field for gobuffalo.pop.",
                         "format": "date-time",
                         "type": "string"
                     },
                     "dispatches": {
                         "description": "Dispatches store information about the attempts of delivering a message\nMay contain an error if any happened, or just the `success` state.",
@@ -1258,29 +1416,30 @@
                     "status": {
                         "$ref": "#/components/schemas/courierMessageStatus"
                     },
                     "subject": {
                         "type": "string"
                     },
                     "template_type": {
-                        "description": "\nrecovery_invalid TypeRecoveryInvalid\nrecovery_valid TypeRecoveryValid\nrecovery_code_invalid TypeRecoveryCodeInvalid\nrecovery_code_valid TypeRecoveryCodeValid\nverification_invalid TypeVerificationInvalid\nverification_valid TypeVerificationValid\nverification_code_invalid TypeVerificationCodeInvalid\nverification_code_valid TypeVerificationCodeValid\notp TypeOTP\nstub TypeTestStub",
+                        "description": "\nrecovery_invalid TypeRecoveryInvalid\nrecovery_valid TypeRecoveryValid\nrecovery_code_invalid TypeRecoveryCodeInvalid\nrecovery_code_valid TypeRecoveryCodeValid\nverification_invalid TypeVerificationInvalid\nverification_valid TypeVerificationValid\nverification_code_invalid TypeVerificationCodeInvalid\nverification_code_valid TypeVerificationCodeValid\nstub TypeTestStub\nlogin_code_valid TypeLoginCodeValid\nregistration_code_valid TypeRegistrationCodeValid",
                         "enum": [
                             "recovery_invalid",
                             "recovery_valid",
                             "recovery_code_invalid",
                             "recovery_code_valid",
                             "verification_invalid",
                             "verification_valid",
                             "verification_code_invalid",
                             "verification_code_valid",
-                            "otp",
-                            "stub"
+                            "stub",
+                            "login_code_valid",
+                            "registration_code_valid"
                         ],
                         "type": "string",
-                        "x-go-enum-desc": "recovery_invalid TypeRecoveryInvalid\nrecovery_valid TypeRecoveryValid\nrecovery_code_invalid TypeRecoveryCodeInvalid\nrecovery_code_valid TypeRecoveryCodeValid\nverification_invalid TypeVerificationInvalid\nverification_valid TypeVerificationValid\nverification_code_invalid TypeVerificationCodeInvalid\nverification_code_valid TypeVerificationCodeValid\notp TypeOTP\nstub TypeTestStub"
+                        "x-go-enum-desc": "recovery_invalid TypeRecoveryInvalid\nrecovery_valid TypeRecoveryValid\nrecovery_code_invalid TypeRecoveryCodeInvalid\nrecovery_code_valid TypeRecoveryCodeValid\nverification_invalid TypeVerificationInvalid\nverification_valid TypeVerificationValid\nverification_code_invalid TypeVerificationCodeInvalid\nverification_code_valid TypeVerificationCodeValid\nstub TypeTestStub\nlogin_code_valid TypeLoginCodeValid\nregistration_code_valid TypeRegistrationCodeValid"
                     },
                     "type": {
                         "$ref": "#/components/schemas/courierMessageType"
                     },
                     "updated_at": {
                         "description": "UpdatedAt is a helper struct field for gobuffalo.pop.",
                         "format": "date-time",
@@ -1376,34 +1535,14 @@
                 "nullable": true
             },
             "nullTime": {
                 "format": "date-time",
                 "title": "NullTime implements sql.NullTime functionality.",
                 "type": "string"
             },
-            "pagination": {
-                "properties": {
-                    "page": {
-                        "default": 1,
-                        "description": "Pagination Page\n\nThis value is currently an integer, but it is not sequential. The value is not the page number, but a\nreference. The next page can be any number and some numbers might return an empty list.\n\nFor example, page 2 might not follow after page 1. And even if page 3 and 5 exist, but page 4 might not exist.",
-                        "format": "int64",
-                        "minimum": 1,
-                        "type": "integer"
-                    },
-                    "per_page": {
-                        "default": 250,
-                        "description": "Items per Page\n\nThis is the number of items per page.",
-                        "format": "int64",
-                        "maximum": 1000,
-                        "minimum": 1,
-                        "type": "integer"
-                    }
-                },
-                "type": "object"
-            },
             "patchIdentitiesBody": {
                 "description": "Patch Identities Body",
                 "properties": {
                     "identities": {
                         "description": "Identities holds the list of patches to apply\n\nrequired",
                         "items": {
                             "$ref": "#/components/schemas/identityPatch"
@@ -1426,15 +1565,15 @@
                 ],
                 "type": "object"
             },
             "recoveryCodeForIdentity": {
                 "description": "Used when an administrator creates a recovery code for an identity.",
                 "properties": {
                     "expires_at": {
-                        "description": "Expires At is the timestamp of when the recovery flow expires\n\nThe timestamp when the recovery link expires.",
+                        "description": "Expires At is the timestamp of when the recovery flow expires\n\nThe timestamp when the recovery code expires.",
                         "format": "date-time",
                         "type": "string"
                     },
                     "recovery_code": {
                         "description": "RecoveryCode is the code that can be used to recover the account",
                         "type": "string"
                     },
@@ -1453,14 +1592,21 @@
             "recoveryFlow": {
                 "description": "This request is used when an identity wants to recover their account.\n\nWe recommend reading the [Account Recovery Documentation](../self-service/flows/password-reset-account-recovery)",
                 "properties": {
                     "active": {
                         "description": "Active, if set, contains the recovery method that is being used. It is initially\nnot set.",
                         "type": "string"
                     },
+                    "continue_with": {
+                        "description": "Contains possible actions that could follow this flow",
+                        "items": {
+                            "$ref": "#/components/schemas/continueWith"
+                        },
+                        "type": "array"
+                    },
                     "expires_at": {
                         "description": "ExpiresAt is the time (UTC) when the request expires. If the user still wishes to update the setting,\na new request has to be initiated.",
                         "format": "date-time",
                         "type": "string"
                     },
                     "id": {
                         "description": "ID represents the request's unique ID. When performing the recovery flow, this\nrepresents the id in the recovery ui's query parameter: http://<selfservice.flows.recovery.ui_url>?request=<id>",
@@ -1477,15 +1623,15 @@
                         "type": "string"
                     },
                     "return_to": {
                         "description": "ReturnTo contains the requested return_to URL.",
                         "type": "string"
                     },
                     "state": {
-                        "$ref": "#/components/schemas/recoveryFlowState"
+                        "description": "State represents the state of this request:\n\nchoose_method: ask the user to choose a method (e.g. recover account via email)\nsent_email: the email has been sent to the user\npassed_challenge: the request was successful and the recovery challenge was passed."
                     },
                     "type": {
                         "$ref": "#/components/schemas/selfServiceFlowType"
                     },
                     "ui": {
                         "$ref": "#/components/schemas/uiContainer"
                     }
@@ -1505,16 +1651,15 @@
             "recoveryFlowState": {
                 "description": "The state represents the state of the recovery flow.\n\nchoose_method: ask the user to choose a method (e.g. recover account via email)\nsent_email: the email has been sent to the user\npassed_challenge: the request was successful and the recovery challenge was passed.",
                 "enum": [
                     "choose_method",
                     "sent_email",
                     "passed_challenge"
                 ],
-                "title": "Recovery Flow State",
-                "type": "string"
+                "title": "Recovery Flow State"
             },
             "recoveryIdentityAddress": {
                 "properties": {
                     "created_at": {
                         "description": "CreatedAt is a helper struct field for gobuffalo.pop.",
                         "format": "date-time",
                         "type": "string"
@@ -1560,15 +1705,27 @@
                 ],
                 "title": "Identity Recovery Link",
                 "type": "object"
             },
             "registrationFlow": {
                 "properties": {
                     "active": {
-                        "$ref": "#/components/schemas/identityCredentialsType"
+                        "description": "Active, if set, contains the registration method that is being used. It is initially\nnot set.\npassword CredentialsTypePassword\noidc CredentialsTypeOIDC\ntotp CredentialsTypeTOTP\nlookup_secret CredentialsTypeLookup\nwebauthn CredentialsTypeWebAuthn\ncode CredentialsTypeCodeAuth\nlink_recovery CredentialsTypeRecoveryLink  CredentialsTypeRecoveryLink is a special credential type linked to the link strategy (recovery flow).  It is not used within the credentials object itself.\ncode_recovery CredentialsTypeRecoveryCode",
+                        "enum": [
+                            "password",
+                            "oidc",
+                            "totp",
+                            "lookup_secret",
+                            "webauthn",
+                            "code",
+                            "link_recovery",
+                            "code_recovery"
+                        ],
+                        "type": "string",
+                        "x-go-enum-desc": "password CredentialsTypePassword\noidc CredentialsTypeOIDC\ntotp CredentialsTypeTOTP\nlookup_secret CredentialsTypeLookup\nwebauthn CredentialsTypeWebAuthn\ncode CredentialsTypeCodeAuth\nlink_recovery CredentialsTypeRecoveryLink  CredentialsTypeRecoveryLink is a special credential type linked to the link strategy (recovery flow).  It is not used within the credentials object itself.\ncode_recovery CredentialsTypeRecoveryCode"
                     },
                     "expires_at": {
                         "description": "ExpiresAt is the time (UTC) when the flow expires. If the user still wishes to log in,\na new flow has to be initiated.",
                         "format": "date-time",
                         "type": "string"
                     },
                     "id": {
@@ -1584,26 +1741,32 @@
                     "oauth2_login_challenge": {
                         "description": "Ory OAuth 2.0 Login Challenge.\n\nThis value is set using the `login_challenge` query parameter of the registration and login endpoints.\nIf set will cooperate with Ory OAuth2 and OpenID to act as an OAuth2 server / OpenID Provider.",
                         "type": "string"
                     },
                     "oauth2_login_request": {
                         "$ref": "#/components/schemas/OAuth2LoginRequest"
                     },
+                    "organization_id": {
+                        "$ref": "#/components/schemas/NullUUID"
+                    },
                     "request_url": {
                         "description": "RequestURL is the initial URL that was requested from Ory Kratos. It can be used\nto forward information contained in the URL's path or query for example.",
                         "type": "string"
                     },
                     "return_to": {
                         "description": "ReturnTo contains the requested return_to URL.",
                         "type": "string"
                     },
                     "session_token_exchange_code": {
                         "description": "SessionTokenExchangeCode holds the secret code that the client can use to retrieve a session token after the flow has been completed.\nThis is only set if the client has requested a session token exchange code, and if the flow is of type \"api\",\nand only on creating the flow.",
                         "type": "string"
                     },
+                    "state": {
+                        "description": "State represents the state of this request:\n\nchoose_method: ask the user to choose a method (e.g. registration with email)\nsent_email: the email has been sent to the user\npassed_challenge: the request was successful and the registration challenge was passed."
+                    },
                     "transient_payload": {
                         "description": "TransientPayload is used to pass data from the registration to a webhook",
                         "type": "object"
                     },
                     "type": {
                         "$ref": "#/components/schemas/selfServiceFlowType"
                     },
@@ -1613,18 +1776,28 @@
                 },
                 "required": [
                     "id",
                     "type",
                     "expires_at",
                     "issued_at",
                     "request_url",
-                    "ui"
+                    "ui",
+                    "state"
                 ],
                 "type": "object"
             },
+            "registrationFlowState": {
+                "description": "choose_method: ask the user to choose a method (e.g. registration with email)\nsent_email: the email has been sent to the user\npassed_challenge: the request was successful and the registration challenge was passed.",
+                "enum": [
+                    "choose_method",
+                    "sent_email",
+                    "passed_challenge"
+                ],
+                "title": "State represents the state of this request:"
+            },
             "selfServiceFlowExpiredError": {
                 "description": "Is sent when a flow is expired",
                 "properties": {
                     "error": {
                         "$ref": "#/components/schemas/genericError"
                     },
                     "expired_at": {
@@ -1686,19 +1859,22 @@
                     "identity": {
                         "$ref": "#/components/schemas/identity"
                     },
                     "issued_at": {
                         "description": "The Session Issuance Timestamp\n\nWhen this session was issued at. Usually equal or close to `authenticated_at`.",
                         "format": "date-time",
                         "type": "string"
+                    },
+                    "tokenized": {
+                        "description": "Tokenized is the tokenized (e.g. JWT) version of the session.\n\nIt is only set when the `tokenize` query parameter was set to a valid tokenize template during calls to `/session/whoami`.",
+                        "type": "string"
                     }
                 },
                 "required": [
-                    "id",
-                    "identity"
+                    "id"
                 ],
                 "type": "object"
             },
             "sessionAuthenticationMethod": {
                 "description": "A singular authenticator used during authentication / login.",
                 "properties": {
                     "aal": {
@@ -1710,23 +1886,28 @@
                         "type": "string"
                     },
                     "method": {
                         "enum": [
                             "link_recovery",
                             "code_recovery",
                             "password",
+                            "code",
                             "totp",
                             "oidc",
                             "webauthn",
                             "lookup_secret",
                             "v0.6_legacy_session"
                         ],
                         "title": "The method used",
                         "type": "string"
                     },
+                    "organization": {
+                        "description": "The Organization id used for authentication",
+                        "type": "string"
+                    },
                     "provider": {
                         "description": "OIDC or SAML provider id used for authentication",
                         "type": "string"
                     }
                 },
                 "title": "AuthenticationMethod identifies an authentication method",
                 "type": "object"
@@ -1802,15 +1983,15 @@
                         "type": "string"
                     },
                     "return_to": {
                         "description": "ReturnTo contains the requested return_to URL.",
                         "type": "string"
                     },
                     "state": {
-                        "$ref": "#/components/schemas/settingsFlowState"
+                        "description": "State represents the state of this flow. It knows two states:\n\nshow_form: No user data has been collected, or it is invalid, and thus the form should be shown.\nsuccess: Indicates that the settings flow has been updated successfully with the provided data.\nDone will stay true when repeatedly checking. If set to true, done will revert back to false only\nwhen a flow with invalid (e.g. \"please use a valid phone number\") data was sent."
                     },
                     "type": {
                         "$ref": "#/components/schemas/selfServiceFlowType"
                     },
                     "ui": {
                         "$ref": "#/components/schemas/uiContainer"
                     }
@@ -1830,16 +2011,15 @@
             },
             "settingsFlowState": {
                 "description": "show_form: No user data has been collected, or it is invalid, and thus the form should be shown.\nsuccess: Indicates that the settings flow has been updated successfully with the provided data.\nDone will stay true when repeatedly checking. If set to true, done will revert back to false only\nwhen a flow with invalid (e.g. \"please use a valid phone number\") data was sent.",
                 "enum": [
                     "show_form",
                     "success"
                 ],
-                "title": "State represents the state of this flow. It knows two states:",
-                "type": "string"
+                "title": "State represents the state of this flow. It knows two states:"
             },
             "successfulCodeExchangeResponse": {
                 "description": "The Response for Registration Flows via API",
                 "properties": {
                     "session": {
                         "$ref": "#/components/schemas/session"
                     },
@@ -2314,15 +2494,21 @@
                         "description": "Store metadata about the identity which the identity itself can see when calling for example the\nsession endpoint. Do not store sensitive information (e.g. credit score) about the identity in this field."
                     },
                     "schema_id": {
                         "description": "SchemaID is the ID of the JSON Schema to be used for validating the identity's traits. If set\nwill update the Identity's SchemaID.",
                         "type": "string"
                     },
                     "state": {
-                        "$ref": "#/components/schemas/identityState"
+                        "description": "State is the identity's state.\nactive StateActive\ninactive StateInactive",
+                        "enum": [
+                            "active",
+                            "inactive"
+                        ],
+                        "type": "string",
+                        "x-go-enum-desc": "active StateActive\ninactive StateInactive"
                     },
                     "traits": {
                         "description": "Traits represent an identity's traits. The identity is able to create, modify, and delete traits\nin a self-service manner. The input will always be validated against the JSON Schema defined\nin `schema_id`.",
                         "type": "object"
                     }
                 },
                 "required": [
@@ -2331,14 +2517,15 @@
                     "state"
                 ],
                 "type": "object"
             },
             "updateLoginFlowBody": {
                 "discriminator": {
                     "mapping": {
+                        "code": "#/components/schemas/updateLoginFlowWithCodeMethod",
                         "lookup_secret": "#/components/schemas/updateLoginFlowWithLookupSecretMethod",
                         "oidc": "#/components/schemas/updateLoginFlowWithOidcMethod",
                         "password": "#/components/schemas/updateLoginFlowWithPasswordMethod",
                         "totp": "#/components/schemas/updateLoginFlowWithTotpMethod",
                         "webauthn": "#/components/schemas/updateLoginFlowWithWebAuthnMethod"
                     },
                     "propertyName": "method"
@@ -2354,17 +2541,50 @@
                         "$ref": "#/components/schemas/updateLoginFlowWithTotpMethod"
                     },
                     {
                         "$ref": "#/components/schemas/updateLoginFlowWithWebAuthnMethod"
                     },
                     {
                         "$ref": "#/components/schemas/updateLoginFlowWithLookupSecretMethod"
+                    },
+                    {
+                        "$ref": "#/components/schemas/updateLoginFlowWithCodeMethod"
                     }
                 ]
             },
+            "updateLoginFlowWithCodeMethod": {
+                "description": "Update Login flow using the code method",
+                "properties": {
+                    "code": {
+                        "description": "Code is the 6 digits code sent to the user",
+                        "type": "string"
+                    },
+                    "csrf_token": {
+                        "description": "CSRFToken is the anti-CSRF token",
+                        "type": "string"
+                    },
+                    "identifier": {
+                        "description": "Identifier is the code identifier\nThe identifier requires that the user has already completed the registration or settings with code flow.",
+                        "type": "string"
+                    },
+                    "method": {
+                        "description": "Method should be set to \"code\" when logging in using the code strategy.",
+                        "type": "string"
+                    },
+                    "resend": {
+                        "description": "Resend is set when the user wants to resend the code",
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "method",
+                    "csrf_token"
+                ],
+                "type": "object"
+            },
             "updateLoginFlowWithLookupSecretMethod": {
                 "description": "Update Login Flow with Lookup Secret Method",
                 "properties": {
                     "csrf_token": {
                         "description": "Sending the anti-csrf token is only required for browser login flows.",
                         "type": "string"
                     },
@@ -2386,14 +2606,22 @@
             "updateLoginFlowWithOidcMethod": {
                 "description": "Update Login Flow with OpenID Connect Method",
                 "properties": {
                     "csrf_token": {
                         "description": "The CSRF Token",
                         "type": "string"
                     },
+                    "id_token": {
+                        "description": "IDToken is an optional id token provided by an OIDC provider\n\nIf submitted, it is verified using the OIDC provider's public key set and the claims are used to populate\nthe OIDC credentials of the identity.\nIf the OIDC provider does not store additional claims (such as name, etc.) in the IDToken itself, you can use\nthe `traits` field to populate the identity's traits. Note, that Apple only includes the users email in the IDToken.\n\nSupported providers are\nApple",
+                        "type": "string"
+                    },
+                    "id_token_nonce": {
+                        "description": "IDTokenNonce is the nonce, used when generating the IDToken.\nIf the provider supports nonce validation, the nonce will be validated against this value and required.",
+                        "type": "string"
+                    },
                     "method": {
                         "description": "Method to use\n\nThis field must be set to `oidc` when using the oidc method.",
                         "type": "string"
                     },
                     "provider": {
                         "description": "The provider to register with",
                         "type": "string"
@@ -2567,14 +2795,15 @@
                 ],
                 "type": "object"
             },
             "updateRegistrationFlowBody": {
                 "description": "Update Registration Request Body",
                 "discriminator": {
                     "mapping": {
+                        "code": "#/components/schemas/updateRegistrationFlowWithCodeMethod",
                         "oidc": "#/components/schemas/updateRegistrationFlowWithOidcMethod",
                         "password": "#/components/schemas/updateRegistrationFlowWithPasswordMethod",
                         "webauthn": "#/components/schemas/updateRegistrationFlowWithWebAuthnMethod"
                     },
                     "propertyName": "method"
                 },
                 "oneOf": [
@@ -2582,24 +2811,69 @@
                         "$ref": "#/components/schemas/updateRegistrationFlowWithPasswordMethod"
                     },
                     {
                         "$ref": "#/components/schemas/updateRegistrationFlowWithOidcMethod"
                     },
                     {
                         "$ref": "#/components/schemas/updateRegistrationFlowWithWebAuthnMethod"
+                    },
+                    {
+                        "$ref": "#/components/schemas/updateRegistrationFlowWithCodeMethod"
                     }
                 ]
             },
+            "updateRegistrationFlowWithCodeMethod": {
+                "description": "Update Registration Flow with Code Method",
+                "properties": {
+                    "code": {
+                        "description": "The OTP Code sent to the user",
+                        "type": "string"
+                    },
+                    "csrf_token": {
+                        "description": "The CSRF Token",
+                        "type": "string"
+                    },
+                    "method": {
+                        "description": "Method to use\n\nThis field must be set to `code` when using the code method.",
+                        "type": "string"
+                    },
+                    "resend": {
+                        "description": "Resend restarts the flow with a new code",
+                        "type": "string"
+                    },
+                    "traits": {
+                        "description": "The identity's traits",
+                        "type": "object"
+                    },
+                    "transient_payload": {
+                        "description": "Transient data to pass along to any webhooks",
+                        "type": "object"
+                    }
+                },
+                "required": [
+                    "traits",
+                    "method"
+                ],
+                "type": "object"
+            },
             "updateRegistrationFlowWithOidcMethod": {
                 "description": "Update Registration Flow with OpenID Connect Method",
                 "properties": {
                     "csrf_token": {
                         "description": "The CSRF Token",
                         "type": "string"
                     },
+                    "id_token": {
+                        "description": "IDToken is an optional id token provided by an OIDC provider\n\nIf submitted, it is verified using the OIDC provider's public key set and the claims are used to populate\nthe OIDC credentials of the identity.\nIf the OIDC provider does not store additional claims (such as name, etc.) in the IDToken itself, you can use\nthe `traits` field to populate the identity's traits. Note, that Apple only includes the users email in the IDToken.\n\nSupported providers are\nApple",
+                        "type": "string"
+                    },
+                    "id_token_nonce": {
+                        "description": "IDTokenNonce is the nonce, used when generating the IDToken.\nIf the provider supports nonce validation, the nonce will be validated against this value and is required.",
+                        "type": "string"
+                    },
                     "method": {
                         "description": "Method to use\n\nThis field must be set to `oidc` when using the oidc method.",
                         "type": "string"
                     },
                     "provider": {
                         "description": "The provider to register with",
                         "type": "string"
@@ -2995,15 +3269,21 @@
                         "example": true,
                         "type": "boolean"
                     },
                     "verified_at": {
                         "$ref": "#/components/schemas/nullTime"
                     },
                     "via": {
-                        "$ref": "#/components/schemas/identityVerifiableAddressType"
+                        "description": "The delivery method",
+                        "enum": [
+                            "email",
+                            "sms"
+                        ],
+                        "example": "email",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "value",
                     "verified",
                     "via",
                     "status"
@@ -3037,15 +3317,15 @@
                         "type": "string"
                     },
                     "return_to": {
                         "description": "ReturnTo contains the requested return_to URL.",
                         "type": "string"
                     },
                     "state": {
-                        "$ref": "#/components/schemas/verificationFlowState"
+                        "description": "State represents the state of this request:\n\nchoose_method: ask the user to choose a method (e.g. verify your email)\nsent_email: the email has been sent to the user\npassed_challenge: the request was successful and the verification challenge was passed."
                     },
                     "type": {
                         "$ref": "#/components/schemas/selfServiceFlowType"
                     },
                     "ui": {
                         "$ref": "#/components/schemas/uiContainer"
                     }
@@ -3062,16 +3342,15 @@
             "verificationFlowState": {
                 "description": "The state represents the state of the verification flow.\n\nchoose_method: ask the user to choose a method (e.g. recover account via email)\nsent_email: the email has been sent to the user\npassed_challenge: the request was successful and the recovery challenge was passed.",
                 "enum": [
                     "choose_method",
                     "sent_email",
                     "passed_challenge"
                 ],
-                "title": "Verification Flow State",
-                "type": "string"
+                "title": "Verification Flow State"
             },
             "version": {
                 "properties": {
                     "version": {
                         "description": "Version is the service's version.",
                         "type": "string"
                     }
@@ -3263,43 +3542,96 @@
         },
         "/admin/identities": {
             "get": {
                 "description": "Lists all [identities](https://www.ory.sh/docs/kratos/concepts/identity-user-model) in the system.",
                 "operationId": "listIdentities",
                 "parameters": [
                     {
-                        "description": "Items per Page\n\nThis is the number of items per page.",
+                        "description": "Deprecated Items per Page\n\nDEPRECATED: Please use `page_token` instead. This parameter will be removed in the future.\n\nThis is the number of items per page.",
                         "in": "query",
                         "name": "per_page",
                         "schema": {
                             "default": 250,
                             "format": "int64",
                             "maximum": 1000,
                             "minimum": 1,
                             "type": "integer"
                         }
                     },
                     {
-                        "description": "Pagination Page\n\nThis value is currently an integer, but it is not sequential. The value is not the page number, but a\nreference. The next page can be any number and some numbers might return an empty list.\n\nFor example, page 2 might not follow after page 1. And even if page 3 and 5 exist, but page 4 might not exist.",
+                        "description": "Deprecated Pagination Page\n\nDEPRECATED: Please use `page_token` instead. This parameter will be removed in the future.\n\nThis value is currently an integer, but it is not sequential. The value is not the page number, but a\nreference. The next page can be any number and some numbers might return an empty list.\n\nFor example, page 2 might not follow after page 1. And even if page 3 and 5 exist, but page 4 might not exist.\nThe first page can be retrieved by omitting this parameter. Following page pointers will be returned in the\n`Link` header.",
                         "in": "query",
                         "name": "page",
                         "schema": {
-                            "default": 1,
                             "format": "int64",
+                            "type": "integer"
+                        }
+                    },
+                    {
+                        "description": "Page Size\n\nThis is the number of items per page to return. For details on pagination please head over to the\n[pagination documentation](https://www.ory.sh/docs/ecosystem/api-design#pagination).",
+                        "in": "query",
+                        "name": "page_size",
+                        "schema": {
+                            "default": 250,
+                            "format": "int64",
+                            "maximum": 500,
                             "minimum": 1,
                             "type": "integer"
                         }
                     },
                     {
-                        "description": "CredentialsIdentifier is the identifier (username, email) of the credentials to look up.",
+                        "description": "Next Page Token\n\nThe next page token. For details on pagination please head over to the\n[pagination documentation](https://www.ory.sh/docs/ecosystem/api-design#pagination).",
+                        "in": "query",
+                        "name": "page_token",
+                        "schema": {
+                            "default": "1",
+                            "minimum": 1,
+                            "type": "string"
+                        }
+                    },
+                    {
+                        "description": "Read Consistency Level (preview)\n\nThe read consistency level determines the consistency guarantee for reads:\n\nstrong (slow): The read is guaranteed to return the most recent data committed at the start of the read.\neventual (very fast): The result will return data that is about 4.8 seconds old.\n\nThe default consistency guarantee can be changed in the Ory Network Console or using the Ory CLI with\n`ory patch project --replace '/previews/default_read_consistency_level=\"strong\"'`.\n\nSetting the default consistency level to `eventual` may cause regressions in the future as we add consistency\ncontrols to more APIs. Currently, the following APIs will be affected by this setting:\n\n`GET /admin/identities`\n\nThis feature is in preview and only available in Ory Network.\n ConsistencyLevelUnset  ConsistencyLevelUnset is the unset / default consistency level.\nstrong ConsistencyLevelStrong  ConsistencyLevelStrong is the strong consistency level.\neventual ConsistencyLevelEventual  ConsistencyLevelEventual is the eventual consistency level using follower read timestamps.",
+                        "in": "query",
+                        "name": "consistency",
+                        "schema": {
+                            "enum": [
+                                "",
+                                "strong",
+                                "eventual"
+                            ],
+                            "type": "string"
+                        },
+                        "x-go-enum-desc": " ConsistencyLevelUnset  ConsistencyLevelUnset is the unset / default consistency level.\nstrong ConsistencyLevelStrong  ConsistencyLevelStrong is the strong consistency level.\neventual ConsistencyLevelEventual  ConsistencyLevelEventual is the eventual consistency level using follower read timestamps."
+                    },
+                    {
+                        "description": "List of ids used to filter identities.\nIf this list is empty, then no filter will be applied.",
+                        "in": "query",
+                        "name": "ids",
+                        "schema": {
+                            "items": {
+                                "type": "string"
+                            },
+                            "type": "array"
+                        }
+                    },
+                    {
+                        "description": "CredentialsIdentifier is the identifier (username, email) of the credentials to look up using exact match.\nOnly one of CredentialsIdentifier and CredentialsIdentifierSimilar can be used.",
                         "in": "query",
                         "name": "credentials_identifier",
                         "schema": {
                             "type": "string"
                         }
+                    },
+                    {
+                        "description": "This is an EXPERIMENTAL parameter that WILL CHANGE. Do NOT rely on consistent, deterministic behavior.\nTHIS PARAMETER WILL BE REMOVED IN AN UPCOMING RELEASE WITHOUT ANY MIGRATION PATH.\n\nCredentialsIdentifierSimilar is the (partial) identifier (username, email) of the credentials to look up using similarity search.\nOnly one of CredentialsIdentifier and CredentialsIdentifierSimilar can be used.",
+                        "in": "query",
+                        "name": "preview_credentials_identifier_similar",
+                        "schema": {
+                            "type": "string"
+                        }
                     }
                 ],
                 "responses": {
                     "200": {
                         "$ref": "#/components/responses/listIdentities"
                     },
                     "default": {
@@ -3521,18 +3853,21 @@
                         "description": "Include Credentials in Response\n\nInclude any credential, for example `password` or `oidc`, in the response. When set to `oidc`, This will return\nthe initial OAuth 2.0 Access Token, OAuth 2.0 Refresh Token and the OpenID Connect ID Token if available.",
                         "in": "query",
                         "name": "include_credential",
                         "schema": {
                             "items": {
                                 "enum": [
                                     "password",
-                                    "totp",
                                     "oidc",
+                                    "totp",
+                                    "lookup_secret",
                                     "webauthn",
-                                    "lookup_secret"
+                                    "code",
+                                    "link_recovery",
+                                    "code_recovery"
                                 ],
                                 "type": "string"
                             },
                             "type": "array"
                         }
                     }
                 ],
@@ -3762,26 +4097,32 @@
                         "name": "id",
                         "required": true,
                         "schema": {
                             "type": "string"
                         }
                     },
                     {
-                        "description": "Type is the credential's Type.\nOne of totp, webauthn, lookup",
+                        "description": "Type is the type of credentials to be deleted.\npassword CredentialsTypePassword\noidc CredentialsTypeOIDC\ntotp CredentialsTypeTOTP\nlookup_secret CredentialsTypeLookup\nwebauthn CredentialsTypeWebAuthn\ncode CredentialsTypeCodeAuth\nlink_recovery CredentialsTypeRecoveryLink  CredentialsTypeRecoveryLink is a special credential type linked to the link strategy (recovery flow).  It is not used within the credentials object itself.\ncode_recovery CredentialsTypeRecoveryCode",
                         "in": "path",
                         "name": "type",
                         "required": true,
                         "schema": {
                             "enum": [
+                                "password",
+                                "oidc",
                                 "totp",
+                                "lookup_secret",
                                 "webauthn",
-                                "lookup"
+                                "code",
+                                "link_recovery",
+                                "code_recovery"
                             ],
                             "type": "string"
-                        }
+                        },
+                        "x-go-enum-desc": "password CredentialsTypePassword\noidc CredentialsTypeOIDC\ntotp CredentialsTypeTOTP\nlookup_secret CredentialsTypeLookup\nwebauthn CredentialsTypeWebAuthn\ncode CredentialsTypeCodeAuth\nlink_recovery CredentialsTypeRecoveryLink  CredentialsTypeRecoveryLink is a special credential type linked to the link strategy (recovery flow).  It is not used within the credentials object itself.\ncode_recovery CredentialsTypeRecoveryCode"
                     }
                 ],
                 "responses": {
                     "204": {
                         "$ref": "#/components/responses/emptyResponse"
                     },
                     "404": {
@@ -3887,37 +4228,57 @@
                 ]
             },
             "get": {
                 "description": "This endpoint returns all sessions that belong to the given Identity.",
                 "operationId": "listIdentitySessions",
                 "parameters": [
                     {
-                        "description": "Items per Page\n\nThis is the number of items per page.",
+                        "description": "Deprecated Items per Page\n\nDEPRECATED: Please use `page_token` instead. This parameter will be removed in the future.\n\nThis is the number of items per page.",
                         "in": "query",
                         "name": "per_page",
                         "schema": {
                             "default": 250,
                             "format": "int64",
                             "maximum": 1000,
                             "minimum": 1,
                             "type": "integer"
                         }
                     },
                     {
-                        "description": "Pagination Page\n\nThis value is currently an integer, but it is not sequential. The value is not the page number, but a\nreference. The next page can be any number and some numbers might return an empty list.\n\nFor example, page 2 might not follow after page 1. And even if page 3 and 5 exist, but page 4 might not exist.",
+                        "description": "Deprecated Pagination Page\n\nDEPRECATED: Please use `page_token` instead. This parameter will be removed in the future.\n\nThis value is currently an integer, but it is not sequential. The value is not the page number, but a\nreference. The next page can be any number and some numbers might return an empty list.\n\nFor example, page 2 might not follow after page 1. And even if page 3 and 5 exist, but page 4 might not exist.\nThe first page can be retrieved by omitting this parameter. Following page pointers will be returned in the\n`Link` header.",
                         "in": "query",
                         "name": "page",
                         "schema": {
-                            "default": 1,
                             "format": "int64",
+                            "type": "integer"
+                        }
+                    },
+                    {
+                        "description": "Page Size\n\nThis is the number of items per page to return. For details on pagination please head over to the\n[pagination documentation](https://www.ory.sh/docs/ecosystem/api-design#pagination).",
+                        "in": "query",
+                        "name": "page_size",
+                        "schema": {
+                            "default": 250,
+                            "format": "int64",
+                            "maximum": 500,
                             "minimum": 1,
                             "type": "integer"
                         }
                     },
                     {
+                        "description": "Next Page Token\n\nThe next page token. For details on pagination please head over to the\n[pagination documentation](https://www.ory.sh/docs/ecosystem/api-design#pagination).",
+                        "in": "query",
+                        "name": "page_token",
+                        "schema": {
+                            "default": "1",
+                            "minimum": 1,
+                            "type": "string"
+                        }
+                    },
+                    {
                         "description": "ID is the identity's ID.",
                         "in": "path",
                         "name": "id",
                         "required": true,
                         "schema": {
                             "type": "string"
                         }
@@ -4044,14 +4405,23 @@
                 ]
             }
         },
         "/admin/recovery/link": {
             "post": {
                 "description": "This endpoint creates a recovery link which should be given to the user in order for them to recover\n(or activate) their account.",
                 "operationId": "createRecoveryLinkForIdentity",
+                "parameters": [
+                    {
+                        "in": "query",
+                        "name": "return_to",
+                        "schema": {
+                            "type": "string"
+                        }
+                    }
+                ],
                 "requestBody": {
                     "content": {
                         "application/json": {
                             "schema": {
                                 "$ref": "#/components/schemas/createRecoveryLinkForIdentityBody"
                             }
                         }
@@ -4502,35 +4872,55 @@
         },
         "/schemas": {
             "get": {
                 "description": "Returns a list of all identity schemas currently in use.",
                 "operationId": "listIdentitySchemas",
                 "parameters": [
                     {
-                        "description": "Items per Page\n\nThis is the number of items per page.",
+                        "description": "Deprecated Items per Page\n\nDEPRECATED: Please use `page_token` instead. This parameter will be removed in the future.\n\nThis is the number of items per page.",
                         "in": "query",
                         "name": "per_page",
                         "schema": {
                             "default": 250,
                             "format": "int64",
                             "maximum": 1000,
                             "minimum": 1,
                             "type": "integer"
                         }
                     },
                     {
-                        "description": "Pagination Page\n\nThis value is currently an integer, but it is not sequential. The value is not the page number, but a\nreference. The next page can be any number and some numbers might return an empty list.\n\nFor example, page 2 might not follow after page 1. And even if page 3 and 5 exist, but page 4 might not exist.",
+                        "description": "Deprecated Pagination Page\n\nDEPRECATED: Please use `page_token` instead. This parameter will be removed in the future.\n\nThis value is currently an integer, but it is not sequential. The value is not the page number, but a\nreference. The next page can be any number and some numbers might return an empty list.\n\nFor example, page 2 might not follow after page 1. And even if page 3 and 5 exist, but page 4 might not exist.\nThe first page can be retrieved by omitting this parameter. Following page pointers will be returned in the\n`Link` header.",
                         "in": "query",
                         "name": "page",
                         "schema": {
-                            "default": 1,
                             "format": "int64",
+                            "type": "integer"
+                        }
+                    },
+                    {
+                        "description": "Page Size\n\nThis is the number of items per page to return. For details on pagination please head over to the\n[pagination documentation](https://www.ory.sh/docs/ecosystem/api-design#pagination).",
+                        "in": "query",
+                        "name": "page_size",
+                        "schema": {
+                            "default": 250,
+                            "format": "int64",
+                            "maximum": 500,
                             "minimum": 1,
                             "type": "integer"
                         }
+                    },
+                    {
+                        "description": "Next Page Token\n\nThe next page token. For details on pagination please head over to the\n[pagination documentation](https://www.ory.sh/docs/ecosystem/api-design#pagination).",
+                        "in": "query",
+                        "name": "page_token",
+                        "schema": {
+                            "default": "1",
+                            "minimum": 1,
+                            "type": "string"
+                        }
                     }
                 ],
                 "responses": {
                     "200": {
                         "$ref": "#/components/responses/identitySchemas"
                     },
                     "default": {
@@ -4664,15 +5054,15 @@
                 "tags": [
                     "frontend"
                 ]
             }
         },
         "/self-service/login": {
             "post": {
-                "description": ":::info\n\nThis endpoint is EXPERIMENTAL and subject to potential breaking changes in the future.\n\n:::\n\nUse this endpoint to complete a login flow. This endpoint\nbehaves differently for API and browser flows.\n\nAPI flows expect `application/json` to be sent in the body and responds with\nHTTP 200 and a application/json body with the session token on success;\nHTTP 410 if the original flow expired with the appropriate error messages set and optionally a `use_flow_id` parameter in the body;\nHTTP 400 on form validation errors.\n\nBrowser flows expect a Content-Type of `application/x-www-form-urlencoded` or `application/json` to be sent in the body and respond with\na HTTP 303 redirect to the post/after login URL or the `return_to` value if it was set and if the login succeeded;\na HTTP 303 redirect to the login UI URL with the flow ID containing the validation errors otherwise.\n\nBrowser flows with an accept header of `application/json` will not redirect but instead respond with\nHTTP 200 and a application/json body with the signed in identity and a `Set-Cookie` header on success;\nHTTP 303 redirect to a fresh login flow if the original flow expired with the appropriate error messages set;\nHTTP 400 on form validation errors.\n\nIf this endpoint is called with `Accept: application/json` in the header, the response contains the flow without a redirect. In the\ncase of an error, the `error.id` of the JSON response body can be one of:\n\n`session_already_available`: The user is already signed in.\n`security_csrf_violation`: Unable to fetch the flow because a CSRF violation occurred.\n`security_identity_mismatch`: The requested `?return_to` address is not allowed to be used. Adjust this in the configuration!\n`browser_location_change_required`: Usually sent when an AJAX request indicates that the browser needs to open a specific URL.\nMost likely used in Social Sign In flows.\n\nMore information can be found at [Ory Kratos User Login](https://www.ory.sh/docs/kratos/self-service/flows/user-login) and [User Registration Documentation](https://www.ory.sh/docs/kratos/self-service/flows/user-registration).",
+                "description": "Use this endpoint to complete a login flow. This endpoint\nbehaves differently for API and browser flows.\n\nAPI flows expect `application/json` to be sent in the body and responds with\nHTTP 200 and a application/json body with the session token on success;\nHTTP 410 if the original flow expired with the appropriate error messages set and optionally a `use_flow_id` parameter in the body;\nHTTP 400 on form validation errors.\n\nBrowser flows expect a Content-Type of `application/x-www-form-urlencoded` or `application/json` to be sent in the body and respond with\na HTTP 303 redirect to the post/after login URL or the `return_to` value if it was set and if the login succeeded;\na HTTP 303 redirect to the login UI URL with the flow ID containing the validation errors otherwise.\n\nBrowser flows with an accept header of `application/json` will not redirect but instead respond with\nHTTP 200 and a application/json body with the signed in identity and a `Set-Cookie` header on success;\nHTTP 303 redirect to a fresh login flow if the original flow expired with the appropriate error messages set;\nHTTP 400 on form validation errors.\n\nIf this endpoint is called with `Accept: application/json` in the header, the response contains the flow without a redirect. In the\ncase of an error, the `error.id` of the JSON response body can be one of:\n\n`session_already_available`: The user is already signed in.\n`security_csrf_violation`: Unable to fetch the flow because a CSRF violation occurred.\n`security_identity_mismatch`: The requested `?return_to` address is not allowed to be used. Adjust this in the configuration!\n`browser_location_change_required`: Usually sent when an AJAX request indicates that the browser needs to open a specific URL.\nMost likely used in Social Sign In flows.\n\nMore information can be found at [Ory Kratos User Login](https://www.ory.sh/docs/kratos/self-service/flows/user-login) and [User Registration Documentation](https://www.ory.sh/docs/kratos/self-service/flows/user-registration).",
                 "operationId": "updateLoginFlow",
                 "parameters": [
                     {
                         "description": "The Login Flow ID\n\nThe value for this parameter comes from `flow` URL Query parameter sent to your\napplication (e.g. `/login?flow=abcde`).",
                         "in": "query",
                         "name": "flow",
                         "required": true,
@@ -4814,14 +5204,22 @@
                     {
                         "description": "The URL to return the browser to after the flow was completed.",
                         "in": "query",
                         "name": "return_to",
                         "schema": {
                             "type": "string"
                         }
+                    },
+                    {
+                        "description": "Via should contain the identity's credential the code should be sent to. Only relevant in aal2 flows.",
+                        "in": "query",
+                        "name": "via",
+                        "schema": {
+                            "type": "string"
+                        }
                     }
                 ],
                 "responses": {
                     "200": {
                         "content": {
                             "application/json": {
                                 "schema": {
@@ -4898,14 +5296,22 @@
                     {
                         "description": "An optional Hydra login challenge. If present, Kratos will cooperate with\nOry Hydra to act as an OAuth2 identity provider.\n\nThe value for this parameter comes from `login_challenge` URL Query parameter sent to your\napplication (e.g. `/login?login_challenge=abcde`).",
                         "in": "query",
                         "name": "login_challenge",
                         "schema": {
                             "type": "string"
                         }
+                    },
+                    {
+                        "description": "An optional organization ID that should be used for logging this user in.\nThis parameter is only effective in the Ory Network.",
+                        "in": "query",
+                        "name": "organization",
+                        "schema": {
+                            "type": "string"
+                        }
                     }
                 ],
                 "responses": {
                     "200": {
                         "content": {
                             "application/json": {
                                 "schema": {
@@ -5194,15 +5600,15 @@
                 "tags": [
                     "frontend"
                 ]
             }
         },
         "/self-service/recovery": {
             "post": {
-                "description": "Use this endpoint to complete a recovery flow. This endpoint\nbehaves differently for API and browser flows and has several states:\n\n`choose_method` expects `flow` (in the URL query) and `email` (in the body) to be sent\nand works with API- and Browser-initiated flows.\nFor API clients and Browser clients with HTTP Header `Accept: application/json` it either returns a HTTP 200 OK when the form is valid and HTTP 400 OK when the form is invalid.\nand a HTTP 303 See Other redirect with a fresh recovery flow if the flow was otherwise invalid (e.g. expired).\nFor Browser clients without HTTP Header `Accept` or with `Accept: text/*` it returns a HTTP 303 See Other redirect to the Recovery UI URL with the Recovery Flow ID appended.\n`sent_email` is the success state after `choose_method` for the `link` method and allows the user to request another recovery email. It\nworks for both API and Browser-initiated flows and returns the same responses as the flow in `choose_method` state.\n`passed_challenge` expects a `token` to be sent in the URL query and given the nature of the flow (\"sending a recovery link\")\ndoes not have any API capabilities. The server responds with a HTTP 303 See Other redirect either to the Settings UI URL\n(if the link was valid) and instructs the user to update their password, or a redirect to the Recover UI URL with\na new Recovery Flow ID which contains an error message that the recovery link was invalid.\n\nMore information can be found at [Ory Kratos Account Recovery Documentation](../self-service/flows/account-recovery).",
+                "description": "Use this endpoint to update a recovery flow. This endpoint\nbehaves differently for API and browser flows and has several states:\n\n`choose_method` expects `flow` (in the URL query) and `email` (in the body) to be sent\nand works with API- and Browser-initiated flows.\nFor API clients and Browser clients with HTTP Header `Accept: application/json` it either returns a HTTP 200 OK when the form is valid and HTTP 400 OK when the form is invalid.\nand a HTTP 303 See Other redirect with a fresh recovery flow if the flow was otherwise invalid (e.g. expired).\nFor Browser clients without HTTP Header `Accept` or with `Accept: text/*` it returns a HTTP 303 See Other redirect to the Recovery UI URL with the Recovery Flow ID appended.\n`sent_email` is the success state after `choose_method` for the `link` method and allows the user to request another recovery email. It\nworks for both API and Browser-initiated flows and returns the same responses as the flow in `choose_method` state.\n`passed_challenge` expects a `token` to be sent in the URL query and given the nature of the flow (\"sending a recovery link\")\ndoes not have any API capabilities. The server responds with a HTTP 303 See Other redirect either to the Settings UI URL\n(if the link was valid) and instructs the user to update their password, or a redirect to the Recover UI URL with\na new Recovery Flow ID which contains an error message that the recovery link was invalid.\n\nMore information can be found at [Ory Kratos Account Recovery Documentation](../self-service/flows/account-recovery).",
                 "operationId": "updateRecoveryFlow",
                 "parameters": [
                     {
                         "description": "The Recovery Flow ID\n\nThe value for this parameter comes from `flow` URL Query parameter sent to your\napplication (e.g. `/recovery?flow=abcde`).",
                         "in": "query",
                         "name": "flow",
                         "required": true,
@@ -5294,23 +5700,23 @@
                                     "$ref": "#/components/schemas/errorGeneric"
                                 }
                             }
                         },
                         "description": "errorGeneric"
                     }
                 },
-                "summary": "Complete Recovery Flow",
+                "summary": "Update Recovery Flow",
                 "tags": [
                     "frontend"
                 ]
             }
         },
         "/self-service/recovery/api": {
             "get": {
-                "description": "This endpoint initiates a recovery flow for API clients such as mobile devices, smart TVs, and so on.\n\nIf a valid provided session cookie or session token is provided, a 400 Bad Request error.\n\nTo fetch an existing recovery flow call `/self-service/recovery/flows?flow=<flow_id>`.\n\nYou MUST NOT use this endpoint in client-side (Single Page Apps, ReactJS, AngularJS) nor server-side (Java Server\nPages, NodeJS, PHP, Golang, ...) browser applications. Using this endpoint in these applications will make\nyou vulnerable to a variety of CSRF attacks.\n\nThis endpoint MUST ONLY be used in scenarios such as native mobile apps (React Native, Objective C, Swift, Java, ...).\n\nMore information can be found at [Ory Kratos Account Recovery Documentation](../self-service/flows/account-recovery).",
+                "description": "This endpoint initiates a recovery flow for API clients such as mobile devices, smart TVs, and so on.\n\nIf a valid provided session cookie or session token is provided, a 400 Bad Request error.\n\nOn an existing recovery flow, use the `getRecoveryFlow` API endpoint.\n\nYou MUST NOT use this endpoint in client-side (Single Page Apps, ReactJS, AngularJS) nor server-side (Java Server\nPages, NodeJS, PHP, Golang, ...) browser applications. Using this endpoint in these applications will make\nyou vulnerable to a variety of CSRF attacks.\n\nThis endpoint MUST ONLY be used in scenarios such as native mobile apps (React Native, Objective C, Swift, Java, ...).\n\nMore information can be found at [Ory Kratos Account Recovery Documentation](../self-service/flows/account-recovery).",
                 "operationId": "createNativeRecoveryFlow",
                 "responses": {
                     "200": {
                         "content": {
                             "application/json": {
                                 "schema": {
                                     "$ref": "#/components/schemas/recoveryFlow"
@@ -5630,15 +6036,15 @@
                 "tags": [
                     "frontend"
                 ]
             }
         },
         "/self-service/registration/browser": {
             "get": {
-                "description": "This endpoint initializes a browser-based user registration flow. This endpoint will set the appropriate\ncookies and anti-CSRF measures required for browser-based flows.\n\n:::info\n\nThis endpoint is EXPERIMENTAL and subject to potential breaking changes in the future.\n\n:::\n\nIf this endpoint is opened as a link in the browser, it will be redirected to\n`selfservice.flows.registration.ui_url` with the flow ID set as the query parameter `?flow=`. If a valid user session\nexists already, the browser will be redirected to `urls.default_redirect_url`.\n\nIf this endpoint is called via an AJAX request, the response contains the flow without a redirect. In the\ncase of an error, the `error.id` of the JSON response body can be one of:\n\n`session_already_available`: The user is already signed in.\n`security_csrf_violation`: Unable to fetch the flow because a CSRF violation occurred.\n`security_identity_mismatch`: The requested `?return_to` address is not allowed to be used. Adjust this in the configuration!\n\nIf this endpoint is called via an AJAX request, the response contains the registration flow without a redirect.\n\nThis endpoint is NOT INTENDED for clients that do not have a browser (Chrome, Firefox, ...) as cookies are needed.\n\nMore information can be found at [Ory Kratos User Login](https://www.ory.sh/docs/kratos/self-service/flows/user-login) and [User Registration Documentation](https://www.ory.sh/docs/kratos/self-service/flows/user-registration).",
+                "description": "This endpoint initializes a browser-based user registration flow. This endpoint will set the appropriate\ncookies and anti-CSRF measures required for browser-based flows.\n\nIf this endpoint is opened as a link in the browser, it will be redirected to\n`selfservice.flows.registration.ui_url` with the flow ID set as the query parameter `?flow=`. If a valid user session\nexists already, the browser will be redirected to `urls.default_redirect_url`.\n\nIf this endpoint is called via an AJAX request, the response contains the flow without a redirect. In the\ncase of an error, the `error.id` of the JSON response body can be one of:\n\n`session_already_available`: The user is already signed in.\n`security_csrf_violation`: Unable to fetch the flow because a CSRF violation occurred.\n`security_identity_mismatch`: The requested `?return_to` address is not allowed to be used. Adjust this in the configuration!\n\nIf this endpoint is called via an AJAX request, the response contains the registration flow without a redirect.\n\nThis endpoint is NOT INTENDED for clients that do not have a browser (Chrome, Firefox, ...) as cookies are needed.\n\nMore information can be found at [Ory Kratos User Login](https://www.ory.sh/docs/kratos/self-service/flows/user-login) and [User Registration Documentation](https://www.ory.sh/docs/kratos/self-service/flows/user-registration).",
                 "operationId": "createBrowserRegistrationFlow",
                 "parameters": [
                     {
                         "description": "The URL to return the browser to after the flow was completed.",
                         "in": "query",
                         "name": "return_to",
                         "schema": {
@@ -5656,14 +6062,21 @@
                     {
                         "description": "The URL to return the browser to after the verification flow was completed.\n\nAfter the registration flow is completed, the user will be sent a verification email.\nUpon completing the verification flow, this URL will be used to override the default\n`selfservice.flows.verification.after.default_redirect_to` value.",
                         "in": "query",
                         "name": "after_verification_return_to",
                         "schema": {
                             "type": "string"
                         }
+                    },
+                    {
+                        "in": "query",
+                        "name": "organization",
+                        "schema": {
+                            "type": "string"
+                        }
                     }
                 ],
                 "responses": {
                     "200": {
                         "content": {
                             "application/json": {
                                 "schema": {
@@ -6467,37 +6880,57 @@
                 ]
             },
             "get": {
                 "description": "This endpoints returns all other active sessions that belong to the logged-in user.\nThe current session can be retrieved by calling the `/sessions/whoami` endpoint.",
                 "operationId": "listMySessions",
                 "parameters": [
                     {
-                        "description": "Items per Page\n\nThis is the number of items per page.",
+                        "description": "Deprecated Items per Page\n\nDEPRECATED: Please use `page_token` instead. This parameter will be removed in the future.\n\nThis is the number of items per page.",
                         "in": "query",
                         "name": "per_page",
                         "schema": {
                             "default": 250,
                             "format": "int64",
                             "maximum": 1000,
                             "minimum": 1,
                             "type": "integer"
                         }
                     },
                     {
-                        "description": "Pagination Page\n\nThis value is currently an integer, but it is not sequential. The value is not the page number, but a\nreference. The next page can be any number and some numbers might return an empty list.\n\nFor example, page 2 might not follow after page 1. And even if page 3 and 5 exist, but page 4 might not exist.",
+                        "description": "Deprecated Pagination Page\n\nDEPRECATED: Please use `page_token` instead. This parameter will be removed in the future.\n\nThis value is currently an integer, but it is not sequential. The value is not the page number, but a\nreference. The next page can be any number and some numbers might return an empty list.\n\nFor example, page 2 might not follow after page 1. And even if page 3 and 5 exist, but page 4 might not exist.\nThe first page can be retrieved by omitting this parameter. Following page pointers will be returned in the\n`Link` header.",
                         "in": "query",
                         "name": "page",
                         "schema": {
-                            "default": 1,
                             "format": "int64",
+                            "type": "integer"
+                        }
+                    },
+                    {
+                        "description": "Page Size\n\nThis is the number of items per page to return. For details on pagination please head over to the\n[pagination documentation](https://www.ory.sh/docs/ecosystem/api-design#pagination).",
+                        "in": "query",
+                        "name": "page_size",
+                        "schema": {
+                            "default": 250,
+                            "format": "int64",
+                            "maximum": 500,
                             "minimum": 1,
                             "type": "integer"
                         }
                     },
                     {
+                        "description": "Next Page Token\n\nThe next page token. For details on pagination please head over to the\n[pagination documentation](https://www.ory.sh/docs/ecosystem/api-design#pagination).",
+                        "in": "query",
+                        "name": "page_token",
+                        "schema": {
+                            "default": "1",
+                            "minimum": 1,
+                            "type": "string"
+                        }
+                    },
+                    {
                         "description": "Set the Session Token when calling from non-browser clients. A session token has a format of `MP2YWEMeM8MxjkGKpH4dqOQ4Q4DlSPaj`.",
                         "in": "header",
                         "name": "X-Session-Token",
                         "schema": {
                             "type": "string"
                         }
                     },
@@ -6630,15 +7063,15 @@
                 "tags": [
                     "frontend"
                 ]
             }
         },
         "/sessions/whoami": {
             "get": {
-                "description": "Uses the HTTP Headers in the GET request to determine (e.g. by using checking the cookies) who is authenticated.\nReturns a session object in the body or 401 if the credentials are invalid or no credentials were sent.\nWhen the request it successful it adds the user ID to the 'X-Kratos-Authenticated-Identity-Id' header\nin the response.\n\nIf you call this endpoint from a server-side application, you must forward the HTTP Cookie Header to this endpoint:\n\n```js\npseudo-code example\nrouter.get('/protected-endpoint', async function (req, res) {\nconst session = await client.toSession(undefined, req.header('cookie'))\n\nconsole.log(session)\n})\n```\n\nWhen calling this endpoint from a non-browser application (e.g. mobile app) you must include the session token:\n\n```js\npseudo-code example\n...\nconst session = await client.toSession(\"the-session-token\")\n\nconsole.log(session)\n```\n\nDepending on your configuration this endpoint might return a 403 status code if the session has a lower Authenticator\nAssurance Level (AAL) than is possible for the identity. This can happen if the identity has password + webauthn\ncredentials (which would result in AAL2) but the session has only AAL1. If this error occurs, ask the user\nto sign in with the second factor or change the configuration.\n\nThis endpoint is useful for:\n\nAJAX calls. Remember to send credentials and set up CORS correctly!\nReverse proxies and API Gateways\nServer-side calls - use the `X-Session-Token` header!\n\nThis endpoint authenticates users by checking:\n\nif the `Cookie` HTTP header was set containing an Ory Kratos Session Cookie;\nif the `Authorization: bearer <ory-session-token>` HTTP header was set with a valid Ory Kratos Session Token;\nif the `X-Session-Token` HTTP header was set with a valid Ory Kratos Session Token.\n\nIf none of these headers are set or the cookie or token are invalid, the endpoint returns a HTTP 401 status code.\n\nAs explained above, this request may fail due to several reasons. The `error.id` can be one of:\n\n`session_inactive`: No active session was found in the request (e.g. no Ory Session Cookie / Ory Session Token).\n`session_aal2_required`: An active session was found but it does not fulfil the Authenticator Assurance Level, implying that the session must (e.g.) authenticate the second factor.",
+                "description": "Uses the HTTP Headers in the GET request to determine (e.g. by using checking the cookies) who is authenticated.\nReturns a session object in the body or 401 if the credentials are invalid or no credentials were sent.\nWhen the request it successful it adds the user ID to the 'X-Kratos-Authenticated-Identity-Id' header\nin the response.\n\nIf you call this endpoint from a server-side application, you must forward the HTTP Cookie Header to this endpoint:\n\n```js\npseudo-code example\nrouter.get('/protected-endpoint', async function (req, res) {\nconst session = await client.toSession(undefined, req.header('cookie'))\n\nconsole.log(session)\n})\n```\n\nWhen calling this endpoint from a non-browser application (e.g. mobile app) you must include the session token:\n\n```js\npseudo-code example\n...\nconst session = await client.toSession(\"the-session-token\")\n\nconsole.log(session)\n```\n\nWhen using a token template, the token is included in the `tokenized` field of the session.\n\n```js\npseudo-code example\n...\nconst session = await client.toSession(\"the-session-token\", { tokenize_as: \"example-jwt-template\" })\n\nconsole.log(session.tokenized) // The JWT\n```\n\nDepending on your configuration this endpoint might return a 403 status code if the session has a lower Authenticator\nAssurance Level (AAL) than is possible for the identity. This can happen if the identity has password + webauthn\ncredentials (which would result in AAL2) but the session has only AAL1. If this error occurs, ask the user\nto sign in with the second factor or change the configuration.\n\nThis endpoint is useful for:\n\nAJAX calls. Remember to send credentials and set up CORS correctly!\nReverse proxies and API Gateways\nServer-side calls - use the `X-Session-Token` header!\n\nThis endpoint authenticates users by checking:\n\nif the `Cookie` HTTP header was set containing an Ory Kratos Session Cookie;\nif the `Authorization: bearer <ory-session-token>` HTTP header was set with a valid Ory Kratos Session Token;\nif the `X-Session-Token` HTTP header was set with a valid Ory Kratos Session Token.\n\nIf none of these headers are set or the cookie or token are invalid, the endpoint returns a HTTP 401 status code.\n\nAs explained above, this request may fail due to several reasons. The `error.id` can be one of:\n\n`session_inactive`: No active session was found in the request (e.g. no Ory Session Cookie / Ory Session Token).\n`session_aal2_required`: An active session was found but it does not fulfil the Authenticator Assurance Level, implying that the session must (e.g.) authenticate the second factor.",
                 "operationId": "toSession",
                 "parameters": [
                     {
                         "description": "Set the Session Token when calling from non-browser clients. A session token has a format of `MP2YWEMeM8MxjkGKpH4dqOQ4Q4DlSPaj`.",
                         "example": "MP2YWEMeM8MxjkGKpH4dqOQ4Q4DlSPaj",
                         "in": "header",
                         "name": "X-Session-Token",
@@ -6650,14 +7083,22 @@
                         "description": "Set the Cookie Header. This is especially useful when calling this endpoint from a server-side application. In that\nscenario you must include the HTTP Cookie Header which originally was included in the request to your server.\nAn example of a session in the HTTP Cookie Header is: `ory_kratos_session=a19iOVAbdzdgl70Rq1QZmrKmcjDtdsviCTZx7m9a9yHIUS8Wa9T7hvqyGTsLHi6Qifn2WUfpAKx9DWp0SJGleIn9vh2YF4A16id93kXFTgIgmwIOvbVAScyrx7yVl6bPZnCx27ec4WQDtaTewC1CpgudeDV2jQQnSaCP6ny3xa8qLH-QUgYqdQuoA_LF1phxgRCUfIrCLQOkolX5nv3ze_f==`.\n\nIt is ok if more than one cookie are included here as all other cookies will be ignored.",
                         "example": "ory_session=a19iOVAbdzdgl70Rq1QZmrKmcjDtdsviCTZx7m9a9yHIUS8Wa9T7hvqyGTsLHi6Qifn2WUfpAKx9DWp0SJGleIn9vh2YF4A16id93kXFTgIgmwIOvbVAScyrx7yVl6bPZnCx27ec4WQDtaTewC1CpgudeDV2jQQnSaCP6ny3xa8qLH-QUgYqdQuoA_LF1phxgRCUfIrCLQOkolX5nv3ze_f==",
                         "in": "header",
                         "name": "Cookie",
                         "schema": {
                             "type": "string"
                         }
+                    },
+                    {
+                        "description": "Returns the session additionally as a token (such as a JWT)\n\nThe value of this parameter has to be a valid, configured Ory Session token template. For more information head over to [the documentation](http://ory.sh/docs/identities/session-to-jwt-cors).",
+                        "in": "query",
+                        "name": "tokenize_as",
+                        "schema": {
+                            "type": "string"
+                        }
                     }
                 ],
                 "responses": {
                     "200": {
                         "content": {
                             "application/json": {
                                 "schema": {
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/package.json` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/package.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8555555555555556%*

 * *Differences: {"'dependencies'": "{delete: ['cheerio', 'highlight.js', 'uuid']}",*

 * * "'devDependencies'": "{'@sveltejs/adapter-node': '^5.0.1', '@sveltejs/kit': '^2.5.6', "*

 * *                      "'@tailwindcss/typography': '^0.5.12', '@typescript-eslint/eslint-plugin': "*

 * *                      "'^7.6.0', '@typescript-eslint/parser': '^7.6.0', 'autoprefixer': "*

 * *                      "'^10.4.19', 'daisyui': '^4.10.1', 'eslint': '^8.57.0', "*

 * *                      "'eslint-config-prettier': '^9.1.0', 'eslint-plugin-svelte': '^2 […]*

```diff
@@ -1,48 +1,46 @@
 {
     "dependencies": {
-        "cheerio": "1.0.0-rc.12",
-        "highlight.js": "^11.9.0",
         "openapi-fetch": "^0.8.2",
-        "set-cookie-parser": "^2.6.0",
-        "uuid": "^9.0.1"
+        "set-cookie-parser": "^2.6.0"
     },
     "devDependencies": {
-        "@sveltejs/adapter-node": "^1.3.1",
-        "@sveltejs/kit": "^1.27.6",
-        "@tailwindcss/typography": "^0.5.10",
+        "@sveltejs/adapter-node": "^5.0.1",
+        "@sveltejs/enhanced-img": "^0.2.0",
+        "@sveltejs/kit": "^2.5.6",
+        "@sveltejs/vite-plugin-svelte": "^3.1.0",
+        "@tailwindcss/typography": "^0.5.12",
         "@types/set-cookie-parser": "^2.4.7",
-        "@types/uuid": "^9.0.7",
-        "@typescript-eslint/eslint-plugin": "^6.13.1",
-        "@typescript-eslint/parser": "^6.13.1",
-        "autoprefixer": "^10.4.16",
-        "daisyui": "^4.4.14",
-        "eslint": "^8.54.0",
-        "eslint-config-prettier": "^9.0.0",
-        "eslint-plugin-svelte": "^2.35.1",
-        "json-schema-to-typescript": "^13.1.1",
-        "openapi-typescript": "^6.7.1",
-        "postcss": "^8.4.31",
+        "@typescript-eslint/eslint-plugin": "^7.6.0",
+        "@typescript-eslint/parser": "^7.6.0",
+        "autoprefixer": "^10.4.19",
+        "daisyui": "^4.10.1",
+        "eslint": "^8.57.0",
+        "eslint-config-prettier": "^9.1.0",
+        "eslint-plugin-svelte": "^2.37.0",
+        "json-schema-to-typescript": "^13.1.2",
+        "openapi-typescript": "^6.7.5",
+        "postcss": "^8.4.38",
         "postcss-load-config": "^4.0.2",
-        "prettier": "^3.1.0",
-        "prettier-plugin-svelte": "^3.1.2",
-        "prettier-plugin-tailwindcss": "^0.5.7",
-        "svelte": "^4.2.8",
-        "svelte-check": "^3.6.2",
-        "tailwindcss": "^3.3.5",
+        "prettier": "^3.2.5",
+        "prettier-plugin-svelte": "^3.2.3",
+        "prettier-plugin-tailwindcss": "^0.5.13",
+        "svelte": "^4.2.14",
+        "svelte-check": "^3.6.9",
+        "tailwindcss": "^3.4.3",
         "tslib": "^2.6.2",
-        "typescript": "^5.3.2",
-        "vite": "^4.5.0"
+        "typescript": "^5.4.5",
+        "vite": "^5.2.8"
     },
     "engines": {
-        "node": ">=18.0.0",
-        "pnpm": "8.10.5"
+        "node": ">=20.0.0",
+        "pnpm": "^8.0.0"
     },
     "name": "lungo",
-    "packageManager": "pnpm@8.10.5",
+    "packageManager": "pnpm@8.15.7",
     "private": true,
     "scripts": {
         "build": "vite build",
         "check": "svelte-kit sync && svelte-check --tsconfig ./tsconfig.json",
         "check:watch": "svelte-kit sync && svelte-check --tsconfig ./tsconfig.json --watch",
         "dev": "vite dev",
         "format": "prettier --write .",
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/pnpm-lock.yaml` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/pnpm-lock.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,106 +1,100 @@
 lockfileVersion: '6.0'
 
 settings:
   autoInstallPeers: true
   excludeLinksFromLockfile: false
 
 dependencies:
-  cheerio:
-    specifier: 1.0.0-rc.12
-    version: 1.0.0-rc.12
-  highlight.js:
-    specifier: ^11.9.0
-    version: 11.9.0
   openapi-fetch:
     specifier: ^0.8.2
     version: 0.8.2
   set-cookie-parser:
     specifier: ^2.6.0
     version: 2.6.0
-  uuid:
-    specifier: ^9.0.1
-    version: 9.0.1
 
 devDependencies:
   '@sveltejs/adapter-node':
-    specifier: ^1.3.1
-    version: 1.3.1(@sveltejs/kit@1.27.6)
+    specifier: ^5.0.1
+    version: 5.0.1(@sveltejs/kit@2.5.6)
+  '@sveltejs/enhanced-img':
+    specifier: ^0.2.0
+    version: 0.2.0(svelte@4.2.14)
   '@sveltejs/kit':
-    specifier: ^1.27.6
-    version: 1.27.6(svelte@4.2.8)(vite@4.5.0)
+    specifier: ^2.5.6
+    version: 2.5.6(@sveltejs/vite-plugin-svelte@3.1.0)(svelte@4.2.14)(vite@5.2.8)
+  '@sveltejs/vite-plugin-svelte':
+    specifier: ^3.1.0
+    version: 3.1.0(svelte@4.2.14)(vite@5.2.8)
   '@tailwindcss/typography':
-    specifier: ^0.5.10
-    version: 0.5.10(tailwindcss@3.3.5)
+    specifier: ^0.5.12
+    version: 0.5.12(tailwindcss@3.4.3)
   '@types/set-cookie-parser':
     specifier: ^2.4.7
     version: 2.4.7
-  '@types/uuid':
-    specifier: ^9.0.7
-    version: 9.0.7
   '@typescript-eslint/eslint-plugin':
-    specifier: ^6.13.1
-    version: 6.13.1(@typescript-eslint/parser@6.13.1)(eslint@8.54.0)(typescript@5.3.2)
+    specifier: ^7.6.0
+    version: 7.6.0(@typescript-eslint/parser@7.6.0)(eslint@8.57.0)(typescript@5.4.5)
   '@typescript-eslint/parser':
-    specifier: ^6.13.1
-    version: 6.13.1(eslint@8.54.0)(typescript@5.3.2)
+    specifier: ^7.6.0
+    version: 7.6.0(eslint@8.57.0)(typescript@5.4.5)
   autoprefixer:
-    specifier: ^10.4.16
-    version: 10.4.16(postcss@8.4.31)
+    specifier: ^10.4.19
+    version: 10.4.19(postcss@8.4.38)
   daisyui:
-    specifier: ^4.4.14
-    version: 4.4.14(postcss@8.4.31)
+    specifier: ^4.10.1
+    version: 4.10.1(postcss@8.4.38)
   eslint:
-    specifier: ^8.54.0
-    version: 8.54.0
+    specifier: ^8.57.0
+    version: 8.57.0
   eslint-config-prettier:
-    specifier: ^9.0.0
-    version: 9.0.0(eslint@8.54.0)
+    specifier: ^9.1.0
+    version: 9.1.0(eslint@8.57.0)
   eslint-plugin-svelte:
-    specifier: ^2.35.1
-    version: 2.35.1(eslint@8.54.0)(svelte@4.2.8)
+    specifier: ^2.37.0
+    version: 2.37.0(eslint@8.57.0)(svelte@4.2.14)
   json-schema-to-typescript:
-    specifier: ^13.1.1
-    version: 13.1.1
+    specifier: ^13.1.2
+    version: 13.1.2
   openapi-typescript:
-    specifier: ^6.7.1
-    version: 6.7.1
+    specifier: ^6.7.5
+    version: 6.7.5
   postcss:
-    specifier: ^8.4.31
-    version: 8.4.31
+    specifier: ^8.4.38
+    version: 8.4.38
   postcss-load-config:
     specifier: ^4.0.2
-    version: 4.0.2(postcss@8.4.31)
+    version: 4.0.2(postcss@8.4.38)
   prettier:
-    specifier: ^3.1.0
-    version: 3.1.0
+    specifier: ^3.2.5
+    version: 3.2.5
   prettier-plugin-svelte:
-    specifier: ^3.1.2
-    version: 3.1.2(prettier@3.1.0)(svelte@4.2.8)
+    specifier: ^3.2.3
+    version: 3.2.3(prettier@3.2.5)(svelte@4.2.14)
   prettier-plugin-tailwindcss:
-    specifier: ^0.5.7
-    version: 0.5.7(prettier-plugin-svelte@3.1.2)(prettier@3.1.0)
+    specifier: ^0.5.13
+    version: 0.5.13(prettier-plugin-svelte@3.2.3)(prettier@3.2.5)
   svelte:
-    specifier: ^4.2.8
-    version: 4.2.8
+    specifier: ^4.2.14
+    version: 4.2.14
   svelte-check:
-    specifier: ^3.6.2
-    version: 3.6.2(postcss-load-config@4.0.2)(postcss@8.4.31)(svelte@4.2.8)
+    specifier: ^3.6.9
+    version: 3.6.9(postcss-load-config@4.0.2)(postcss@8.4.38)(svelte@4.2.14)
   tailwindcss:
-    specifier: ^3.3.5
-    version: 3.3.5
+    specifier: ^3.4.3
+    version: 3.4.3
   tslib:
     specifier: ^2.6.2
     version: 2.6.2
   typescript:
-    specifier: ^5.3.2
-    version: 5.3.2
+    specifier: ^5.4.5
+    version: 5.4.5
   vite:
-    specifier: ^4.5.0
-    version: 4.5.0
+    specifier: ^5.2.8
+    version: 5.2.8
 
 packages:
 
   /@aashutoshrathi/word-wrap@1.2.6:
     resolution: {integrity: sha512-1Yjs2SvM8TflER/OD3cOjhWWOZb58A2t7wpE2S9XfBYTiIl+XFhQG2bjy4Pu1I+EAlCNUzRDYDdFwFYUKvXcIA==}
     engines: {node: '>=0.10.0'}
     dev: true
@@ -124,229 +118,246 @@
     dependencies:
       '@jsdevtools/ono': 7.1.3
       '@types/json-schema': 7.0.15
       call-me-maybe: 1.0.2
       js-yaml: 4.1.0
     dev: true
 
-  /@esbuild/android-arm64@0.18.20:
-    resolution: {integrity: sha512-Nz4rJcchGDtENV0eMKUNa6L12zz2zBDXuhj/Vjh18zGqB44Bi7MBMSXjgunJgjRhCmKOjnPuZp4Mb6OKqtMHLQ==}
+  /@emnapi/runtime@1.1.1:
+    resolution: {integrity: sha512-3bfqkzuR1KLx57nZfjr2NLnFOobvyS0aTszaEGCGqmYMVDRaGvgIZbjGSV/MHSSmLgQ/b9JFHQ5xm5WRZYd+XQ==}
+    requiresBuild: true
+    dependencies:
+      tslib: 2.6.2
+    dev: true
+    optional: true
+
+  /@esbuild/aix-ppc64@0.20.2:
+    resolution: {integrity: sha512-D+EBOJHXdNZcLJRBkhENNG8Wji2kgc9AZ9KiPr1JuZjsNtyHzrsfLRrY0tk2H2aoFu6RANO1y1iPPUCDYWkb5g==}
+    engines: {node: '>=12'}
+    cpu: [ppc64]
+    os: [aix]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@esbuild/android-arm64@0.20.2:
+    resolution: {integrity: sha512-mRzjLacRtl/tWU0SvD8lUEwb61yP9cqQo6noDZP/O8VkwafSYwZ4yWy24kan8jE/IMERpYncRt2dw438LP3Xmg==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [android]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/android-arm@0.18.20:
-    resolution: {integrity: sha512-fyi7TDI/ijKKNZTUJAQqiG5T7YjJXgnzkURqmGj13C6dCqckZBLdl4h7bkhHt/t0WP+zO9/zwroDvANaOqO5Sw==}
+  /@esbuild/android-arm@0.20.2:
+    resolution: {integrity: sha512-t98Ra6pw2VaDhqNWO2Oph2LXbz/EJcnLmKLGBJwEwXX/JAN83Fym1rU8l0JUWK6HkIbWONCSSatf4sf2NBRx/w==}
     engines: {node: '>=12'}
     cpu: [arm]
     os: [android]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/android-x64@0.18.20:
-    resolution: {integrity: sha512-8GDdlePJA8D6zlZYJV/jnrRAi6rOiNaCC/JclcXpB+KIuvfBN4owLtgzY2bsxnx666XjJx2kDPUmnTtR8qKQUg==}
+  /@esbuild/android-x64@0.20.2:
+    resolution: {integrity: sha512-btzExgV+/lMGDDa194CcUQm53ncxzeBrWJcncOBxuC6ndBkKxnHdFJn86mCIgTELsooUmwUm9FkhSp5HYu00Rg==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [android]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/darwin-arm64@0.18.20:
-    resolution: {integrity: sha512-bxRHW5kHU38zS2lPTPOyuyTm+S+eobPUnTNkdJEfAddYgEcll4xkT8DB9d2008DtTbl7uJag2HuE5NZAZgnNEA==}
+  /@esbuild/darwin-arm64@0.20.2:
+    resolution: {integrity: sha512-4J6IRT+10J3aJH3l1yzEg9y3wkTDgDk7TSDFX+wKFiWjqWp/iCfLIYzGyasx9l0SAFPT1HwSCR+0w/h1ES/MjA==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [darwin]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/darwin-x64@0.18.20:
-    resolution: {integrity: sha512-pc5gxlMDxzm513qPGbCbDukOdsGtKhfxD1zJKXjCCcU7ju50O7MeAZ8c4krSJcOIJGFR+qx21yMMVYwiQvyTyQ==}
+  /@esbuild/darwin-x64@0.20.2:
+    resolution: {integrity: sha512-tBcXp9KNphnNH0dfhv8KYkZhjc+H3XBkF5DKtswJblV7KlT9EI2+jeA8DgBjp908WEuYll6pF+UStUCfEpdysA==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [darwin]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/freebsd-arm64@0.18.20:
-    resolution: {integrity: sha512-yqDQHy4QHevpMAaxhhIwYPMv1NECwOvIpGCZkECn8w2WFHXjEwrBn3CeNIYsibZ/iZEUemj++M26W3cNR5h+Tw==}
+  /@esbuild/freebsd-arm64@0.20.2:
+    resolution: {integrity: sha512-d3qI41G4SuLiCGCFGUrKsSeTXyWG6yem1KcGZVS+3FYlYhtNoNgYrWcvkOoaqMhwXSMrZRl69ArHsGJ9mYdbbw==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [freebsd]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/freebsd-x64@0.18.20:
-    resolution: {integrity: sha512-tgWRPPuQsd3RmBZwarGVHZQvtzfEBOreNuxEMKFcd5DaDn2PbBxfwLcj4+aenoh7ctXcbXmOQIn8HI6mCSw5MQ==}
+  /@esbuild/freebsd-x64@0.20.2:
+    resolution: {integrity: sha512-d+DipyvHRuqEeM5zDivKV1KuXn9WeRX6vqSqIDgwIfPQtwMP4jaDsQsDncjTDDsExT4lR/91OLjRo8bmC1e+Cw==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [freebsd]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-arm64@0.18.20:
-    resolution: {integrity: sha512-2YbscF+UL7SQAVIpnWvYwM+3LskyDmPhe31pE7/aoTMFKKzIc9lLbyGUpmmb8a8AixOL61sQ/mFh3jEjHYFvdA==}
+  /@esbuild/linux-arm64@0.20.2:
+    resolution: {integrity: sha512-9pb6rBjGvTFNira2FLIWqDk/uaf42sSyLE8j1rnUpuzsODBq7FvpwHYZxQ/It/8b+QOS1RYfqgGFNLRI+qlq2A==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-arm@0.18.20:
-    resolution: {integrity: sha512-/5bHkMWnq1EgKr1V+Ybz3s1hWXok7mDFUMQ4cG10AfW3wL02PSZi5kFpYKrptDsgb2WAJIvRcDm+qIvXf/apvg==}
+  /@esbuild/linux-arm@0.20.2:
+    resolution: {integrity: sha512-VhLPeR8HTMPccbuWWcEUD1Az68TqaTYyj6nfE4QByZIQEQVWBB8vup8PpR7y1QHL3CpcF6xd5WVBU/+SBEvGTg==}
     engines: {node: '>=12'}
     cpu: [arm]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-ia32@0.18.20:
-    resolution: {integrity: sha512-P4etWwq6IsReT0E1KHU40bOnzMHoH73aXp96Fs8TIT6z9Hu8G6+0SHSw9i2isWrD2nbx2qo5yUqACgdfVGx7TA==}
+  /@esbuild/linux-ia32@0.20.2:
+    resolution: {integrity: sha512-o10utieEkNPFDZFQm9CoP7Tvb33UutoJqg3qKf1PWVeeJhJw0Q347PxMvBgVVFgouYLGIhFYG0UGdBumROyiig==}
     engines: {node: '>=12'}
     cpu: [ia32]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-loong64@0.18.20:
-    resolution: {integrity: sha512-nXW8nqBTrOpDLPgPY9uV+/1DjxoQ7DoB2N8eocyq8I9XuqJ7BiAMDMf9n1xZM9TgW0J8zrquIb/A7s3BJv7rjg==}
+  /@esbuild/linux-loong64@0.20.2:
+    resolution: {integrity: sha512-PR7sp6R/UC4CFVomVINKJ80pMFlfDfMQMYynX7t1tNTeivQ6XdX5r2XovMmha/VjR1YN/HgHWsVcTRIMkymrgQ==}
     engines: {node: '>=12'}
     cpu: [loong64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-mips64el@0.18.20:
-    resolution: {integrity: sha512-d5NeaXZcHp8PzYy5VnXV3VSd2D328Zb+9dEq5HE6bw6+N86JVPExrA6O68OPwobntbNJ0pzCpUFZTo3w0GyetQ==}
+  /@esbuild/linux-mips64el@0.20.2:
+    resolution: {integrity: sha512-4BlTqeutE/KnOiTG5Y6Sb/Hw6hsBOZapOVF6njAESHInhlQAghVVZL1ZpIctBOoTFbQyGW+LsVYZ8lSSB3wkjA==}
     engines: {node: '>=12'}
     cpu: [mips64el]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-ppc64@0.18.20:
-    resolution: {integrity: sha512-WHPyeScRNcmANnLQkq6AfyXRFr5D6N2sKgkFo2FqguP44Nw2eyDlbTdZwd9GYk98DZG9QItIiTlFLHJHjxP3FA==}
+  /@esbuild/linux-ppc64@0.20.2:
+    resolution: {integrity: sha512-rD3KsaDprDcfajSKdn25ooz5J5/fWBylaaXkuotBDGnMnDP1Uv5DLAN/45qfnf3JDYyJv/ytGHQaziHUdyzaAg==}
     engines: {node: '>=12'}
     cpu: [ppc64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-riscv64@0.18.20:
-    resolution: {integrity: sha512-WSxo6h5ecI5XH34KC7w5veNnKkju3zBRLEQNY7mv5mtBmrP/MjNBCAlsM2u5hDBlS3NGcTQpoBvRzqBcRtpq1A==}
+  /@esbuild/linux-riscv64@0.20.2:
+    resolution: {integrity: sha512-snwmBKacKmwTMmhLlz/3aH1Q9T8v45bKYGE3j26TsaOVtjIag4wLfWSiZykXzXuE1kbCE+zJRmwp+ZbIHinnVg==}
     engines: {node: '>=12'}
     cpu: [riscv64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-s390x@0.18.20:
-    resolution: {integrity: sha512-+8231GMs3mAEth6Ja1iK0a1sQ3ohfcpzpRLH8uuc5/KVDFneH6jtAJLFGafpzpMRO6DzJ6AvXKze9LfFMrIHVQ==}
+  /@esbuild/linux-s390x@0.20.2:
+    resolution: {integrity: sha512-wcWISOobRWNm3cezm5HOZcYz1sKoHLd8VL1dl309DiixxVFoFe/o8HnwuIwn6sXre88Nwj+VwZUvJf4AFxkyrQ==}
     engines: {node: '>=12'}
     cpu: [s390x]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-x64@0.18.20:
-    resolution: {integrity: sha512-UYqiqemphJcNsFEskc73jQ7B9jgwjWrSayxawS6UVFZGWrAAtkzjxSqnoclCXxWtfwLdzU+vTpcNYhpn43uP1w==}
+  /@esbuild/linux-x64@0.20.2:
+    resolution: {integrity: sha512-1MdwI6OOTsfQfek8sLwgyjOXAu+wKhLEoaOLTjbijk6E2WONYpH9ZU2mNtR+lZ2B4uwr+usqGuVfFT9tMtGvGw==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/netbsd-x64@0.18.20:
-    resolution: {integrity: sha512-iO1c++VP6xUBUmltHZoMtCUdPlnPGdBom6IrO4gyKPFFVBKioIImVooR5I83nTew5UOYrk3gIJhbZh8X44y06A==}
+  /@esbuild/netbsd-x64@0.20.2:
+    resolution: {integrity: sha512-K8/DhBxcVQkzYc43yJXDSyjlFeHQJBiowJ0uVL6Tor3jGQfSGHNNJcWxNbOI8v5k82prYqzPuwkzHt3J1T1iZQ==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [netbsd]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/openbsd-x64@0.18.20:
-    resolution: {integrity: sha512-e5e4YSsuQfX4cxcygw/UCPIEP6wbIL+se3sxPdCiMbFLBWu0eiZOJ7WoD+ptCLrmjZBK1Wk7I6D/I3NglUGOxg==}
+  /@esbuild/openbsd-x64@0.20.2:
+    resolution: {integrity: sha512-eMpKlV0SThJmmJgiVyN9jTPJ2VBPquf6Kt/nAoo6DgHAoN57K15ZghiHaMvqjCye/uU4X5u3YSMgVBI1h3vKrQ==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [openbsd]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/sunos-x64@0.18.20:
-    resolution: {integrity: sha512-kDbFRFp0YpTQVVrqUd5FTYmWo45zGaXe0X8E1G/LKFC0v8x0vWrhOWSLITcCn63lmZIxfOMXtCfti/RxN/0wnQ==}
+  /@esbuild/sunos-x64@0.20.2:
+    resolution: {integrity: sha512-2UyFtRC6cXLyejf/YEld4Hajo7UHILetzE1vsRcGL3earZEW77JxrFjH4Ez2qaTiEfMgAXxfAZCm1fvM/G/o8w==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [sunos]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/win32-arm64@0.18.20:
-    resolution: {integrity: sha512-ddYFR6ItYgoaq4v4JmQQaAI5s7npztfV4Ag6NrhiaW0RrnOXqBkgwZLofVTlq1daVTQNhtI5oieTvkRPfZrePg==}
+  /@esbuild/win32-arm64@0.20.2:
+    resolution: {integrity: sha512-GRibxoawM9ZCnDxnP3usoUDO9vUkpAxIIZ6GQI+IlVmr5kP3zUq+l17xELTHMWTWzjxa2guPNyrpq1GWmPvcGQ==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/win32-ia32@0.18.20:
-    resolution: {integrity: sha512-Wv7QBi3ID/rROT08SABTS7eV4hX26sVduqDOTe1MvGMjNd3EjOz4b7zeexIR62GTIEKrfJXKL9LFxTYgkyeu7g==}
+  /@esbuild/win32-ia32@0.20.2:
+    resolution: {integrity: sha512-HfLOfn9YWmkSKRQqovpnITazdtquEW8/SoHW7pWpuEeguaZI4QnCRW6b+oZTztdBnZOS2hqJ6im/D5cPzBTTlQ==}
     engines: {node: '>=12'}
     cpu: [ia32]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/win32-x64@0.18.20:
-    resolution: {integrity: sha512-kTdfRcSiDfQca/y9QIkng02avJ+NCaQvrMejlsB3RRv5sE9rRoeBPISaZpKxHELzRxZyLvNts1P27W3wV+8geQ==}
+  /@esbuild/win32-x64@0.20.2:
+    resolution: {integrity: sha512-N49X4lJX27+l9jbLKSqZ6bKNjzQvHaT8IIFUy+YIqmXQdjYCToGWwOItDrfby14c78aDd5NHQl29xingXfCdLQ==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@eslint-community/eslint-utils@4.4.0(eslint@8.54.0):
+  /@eslint-community/eslint-utils@4.4.0(eslint@8.57.0):
     resolution: {integrity: sha512-1/sA4dwrzBAyeUoQ6oxahHKmrZvsnLCg4RfxW3ZFGGmQkSNQPFNLV9CUEFQP1x9EYXHTo5p6xdhZM1Ne9p/AfA==}
     engines: {node: ^12.22.0 || ^14.17.0 || >=16.0.0}
     peerDependencies:
       eslint: ^6.0.0 || ^7.0.0 || >=8.0.0
     dependencies:
-      eslint: 8.54.0
+      eslint: 8.57.0
       eslint-visitor-keys: 3.4.3
     dev: true
 
   /@eslint-community/regexpp@4.10.0:
     resolution: {integrity: sha512-Cu96Sd2By9mCNTx2iyKOmq10v22jUVQv0lQnlGNy16oE9589yE+QADPbrMGCkA51cKZSg3Pu/aTJVTGfL/qjUA==}
     engines: {node: ^12.0.0 || ^14.0.0 || >=16.0.0}
     dev: true
 
-  /@eslint/eslintrc@2.1.3:
-    resolution: {integrity: sha512-yZzuIG+jnVu6hNSzFEN07e8BxF3uAzYtQb6uDkaYZLo6oYZDCq454c5kB8zxnzfCYyP4MIuyBn10L0DqwujTmA==}
+  /@eslint/eslintrc@2.1.4:
+    resolution: {integrity: sha512-269Z39MS6wVJtsoUl10L60WdkhJVdPG24Q4eZTH3nnF6lpvSShEK3wQjDX9JRWAUPvPh7COouPpU9IrqaZFvtQ==}
     engines: {node: ^12.22.0 || ^14.17.0 || >=16.0.0}
     dependencies:
       ajv: 6.12.6
       debug: 4.3.4
       espree: 9.6.1
       globals: 13.23.0
       ignore: 5.2.4
@@ -354,43 +365,231 @@
       js-yaml: 4.1.0
       minimatch: 3.1.2
       strip-json-comments: 3.1.1
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@eslint/js@8.54.0:
-    resolution: {integrity: sha512-ut5V+D+fOoWPgGGNj83GGjnntO39xDy6DWxO0wb7Jp3DcMX0TfIqdzHF85VTQkerdyGmuuMD9AKAo5KiNlf/AQ==}
+  /@eslint/js@8.57.0:
+    resolution: {integrity: sha512-Ys+3g2TaW7gADOJzPt83SJtCDhMjndcDMFVQ/Tj9iA1BfJzFKD9mAUXT3OenpuPHbI6P/myECxRJrofUsDx/5g==}
     engines: {node: ^12.22.0 || ^14.17.0 || >=16.0.0}
     dev: true
 
   /@fastify/busboy@2.1.0:
     resolution: {integrity: sha512-+KpH+QxZU7O4675t3mnkQKcZZg56u+K/Ct2K+N2AZYNVK8kyeo/bI18tI8aPm3tvNNRyTWfj6s5tnGNlcbQRsA==}
     engines: {node: '>=14'}
     dev: true
 
-  /@humanwhocodes/config-array@0.11.13:
-    resolution: {integrity: sha512-JSBDMiDKSzQVngfRjOdFXgFfklaXI4K9nLF49Auh21lmBWRLIK3+xTErTWD4KU54pb6coM6ESE7Awz/FNU3zgQ==}
+  /@humanwhocodes/config-array@0.11.14:
+    resolution: {integrity: sha512-3T8LkOmg45BV5FICb15QQMsyUSWrQ8AygVfC7ZG32zOalnqrilm018ZVCw0eapXux8FtA33q8PSRSstjee3jSg==}
     engines: {node: '>=10.10.0'}
     dependencies:
-      '@humanwhocodes/object-schema': 2.0.1
+      '@humanwhocodes/object-schema': 2.0.2
       debug: 4.3.4
       minimatch: 3.1.2
     transitivePeerDependencies:
       - supports-color
     dev: true
 
   /@humanwhocodes/module-importer@1.0.1:
     resolution: {integrity: sha512-bxveV4V8v5Yb4ncFTT3rPSgZBOpCkjfK0y4oVVVJwIuDVBRMDXrPyXRL988i5ap9m9bnyEEjWfm5WkBmtffLfA==}
     engines: {node: '>=12.22'}
     dev: true
 
-  /@humanwhocodes/object-schema@2.0.1:
-    resolution: {integrity: sha512-dvuCeX5fC9dXgJn9t+X5atfmgQAzUOWqS1254Gh0m6i8wKd10ebXkfNKiRK+1GWi/yTvvLDHpoxLr0xxxeslWw==}
+  /@humanwhocodes/object-schema@2.0.2:
+    resolution: {integrity: sha512-6EwiSjwWYP7pTckG6I5eyFANjPhmPjUX9JRLUSfNPC7FX7zK9gyZAfUEaECL6ALTpGX5AjnBq3C9XmVWPitNpw==}
+    dev: true
+
+  /@img/sharp-darwin-arm64@0.33.3:
+    resolution: {integrity: sha512-FaNiGX1MrOuJ3hxuNzWgsT/mg5OHG/Izh59WW2mk1UwYHUwtfbhk5QNKYZgxf0pLOhx9ctGiGa2OykD71vOnSw==}
+    engines: {glibc: '>=2.26', node: ^18.17.0 || ^20.3.0 || >=21.0.0, npm: '>=9.6.5', pnpm: '>=7.1.0', yarn: '>=3.2.0'}
+    cpu: [arm64]
+    os: [darwin]
+    requiresBuild: true
+    optionalDependencies:
+      '@img/sharp-libvips-darwin-arm64': 1.0.2
+    dev: true
+    optional: true
+
+  /@img/sharp-darwin-x64@0.33.3:
+    resolution: {integrity: sha512-2QeSl7QDK9ru//YBT4sQkoq7L0EAJZA3rtV+v9p8xTKl4U1bUqTIaCnoC7Ctx2kCjQgwFXDasOtPTCT8eCTXvw==}
+    engines: {glibc: '>=2.26', node: ^18.17.0 || ^20.3.0 || >=21.0.0, npm: '>=9.6.5', pnpm: '>=7.1.0', yarn: '>=3.2.0'}
+    cpu: [x64]
+    os: [darwin]
+    requiresBuild: true
+    optionalDependencies:
+      '@img/sharp-libvips-darwin-x64': 1.0.2
+    dev: true
+    optional: true
+
+  /@img/sharp-libvips-darwin-arm64@1.0.2:
+    resolution: {integrity: sha512-tcK/41Rq8IKlSaKRCCAuuY3lDJjQnYIW1UXU1kxcEKrfL8WR7N6+rzNoOxoQRJWTAECuKwgAHnPvqXGN8XfkHA==}
+    engines: {macos: '>=11', npm: '>=9.6.5', pnpm: '>=7.1.0', yarn: '>=3.2.0'}
+    cpu: [arm64]
+    os: [darwin]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@img/sharp-libvips-darwin-x64@1.0.2:
+    resolution: {integrity: sha512-Ofw+7oaWa0HiiMiKWqqaZbaYV3/UGL2wAPeLuJTx+9cXpCRdvQhCLG0IH8YGwM0yGWGLpsF4Su9vM1o6aer+Fw==}
+    engines: {macos: '>=10.13', npm: '>=9.6.5', pnpm: '>=7.1.0', yarn: '>=3.2.0'}
+    cpu: [x64]
+    os: [darwin]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@img/sharp-libvips-linux-arm64@1.0.2:
+    resolution: {integrity: sha512-x7kCt3N00ofFmmkkdshwj3vGPCnmiDh7Gwnd4nUwZln2YjqPxV1NlTyZOvoDWdKQVDL911487HOueBvrpflagw==}
+    engines: {glibc: '>=2.26', npm: '>=9.6.5', pnpm: '>=7.1.0', yarn: '>=3.2.0'}
+    cpu: [arm64]
+    os: [linux]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@img/sharp-libvips-linux-arm@1.0.2:
+    resolution: {integrity: sha512-iLWCvrKgeFoglQxdEwzu1eQV04o8YeYGFXtfWU26Zr2wWT3q3MTzC+QTCO3ZQfWd3doKHT4Pm2kRmLbupT+sZw==}
+    engines: {glibc: '>=2.28', npm: '>=9.6.5', pnpm: '>=7.1.0', yarn: '>=3.2.0'}
+    cpu: [arm]
+    os: [linux]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@img/sharp-libvips-linux-s390x@1.0.2:
+    resolution: {integrity: sha512-cmhQ1J4qVhfmS6szYW7RT+gLJq9dH2i4maq+qyXayUSn9/3iY2ZeWpbAgSpSVbV2E1JUL2Gg7pwnYQ1h8rQIog==}
+    engines: {glibc: '>=2.28', npm: '>=9.6.5', pnpm: '>=7.1.0', yarn: '>=3.2.0'}
+    cpu: [s390x]
+    os: [linux]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@img/sharp-libvips-linux-x64@1.0.2:
+    resolution: {integrity: sha512-E441q4Qdb+7yuyiADVi5J+44x8ctlrqn8XgkDTwr4qPJzWkaHwD489iZ4nGDgcuya4iMN3ULV6NwbhRZJ9Z7SQ==}
+    engines: {glibc: '>=2.26', npm: '>=9.6.5', pnpm: '>=7.1.0', yarn: '>=3.2.0'}
+    cpu: [x64]
+    os: [linux]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@img/sharp-libvips-linuxmusl-arm64@1.0.2:
+    resolution: {integrity: sha512-3CAkndNpYUrlDqkCM5qhksfE+qSIREVpyoeHIU6jd48SJZViAmznoQQLAv4hVXF7xyUB9zf+G++e2v1ABjCbEQ==}
+    engines: {musl: '>=1.2.2', npm: '>=9.6.5', pnpm: '>=7.1.0', yarn: '>=3.2.0'}
+    cpu: [arm64]
+    os: [linux]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@img/sharp-libvips-linuxmusl-x64@1.0.2:
+    resolution: {integrity: sha512-VI94Q6khIHqHWNOh6LLdm9s2Ry4zdjWJwH56WoiJU7NTeDwyApdZZ8c+SADC8OH98KWNQXnE01UdJ9CSfZvwZw==}
+    engines: {musl: '>=1.2.2', npm: '>=9.6.5', pnpm: '>=7.1.0', yarn: '>=3.2.0'}
+    cpu: [x64]
+    os: [linux]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@img/sharp-linux-arm64@0.33.3:
+    resolution: {integrity: sha512-Zf+sF1jHZJKA6Gor9hoYG2ljr4wo9cY4twaxgFDvlG0Xz9V7sinsPp8pFd1XtlhTzYo0IhDbl3rK7P6MzHpnYA==}
+    engines: {glibc: '>=2.26', node: ^18.17.0 || ^20.3.0 || >=21.0.0, npm: '>=9.6.5', pnpm: '>=7.1.0', yarn: '>=3.2.0'}
+    cpu: [arm64]
+    os: [linux]
+    requiresBuild: true
+    optionalDependencies:
+      '@img/sharp-libvips-linux-arm64': 1.0.2
+    dev: true
+    optional: true
+
+  /@img/sharp-linux-arm@0.33.3:
+    resolution: {integrity: sha512-Q7Ee3fFSC9P7vUSqVEF0zccJsZ8GiiCJYGWDdhEjdlOeS9/jdkyJ6sUSPj+bL8VuOYFSbofrW0t/86ceVhx32w==}
+    engines: {glibc: '>=2.28', node: ^18.17.0 || ^20.3.0 || >=21.0.0, npm: '>=9.6.5', pnpm: '>=7.1.0', yarn: '>=3.2.0'}
+    cpu: [arm]
+    os: [linux]
+    requiresBuild: true
+    optionalDependencies:
+      '@img/sharp-libvips-linux-arm': 1.0.2
+    dev: true
+    optional: true
+
+  /@img/sharp-linux-s390x@0.33.3:
+    resolution: {integrity: sha512-vFk441DKRFepjhTEH20oBlFrHcLjPfI8B0pMIxGm3+yilKyYeHEVvrZhYFdqIseSclIqbQ3SnZMwEMWonY5XFA==}
+    engines: {glibc: '>=2.28', node: ^18.17.0 || ^20.3.0 || >=21.0.0, npm: '>=9.6.5', pnpm: '>=7.1.0', yarn: '>=3.2.0'}
+    cpu: [s390x]
+    os: [linux]
+    requiresBuild: true
+    optionalDependencies:
+      '@img/sharp-libvips-linux-s390x': 1.0.2
+    dev: true
+    optional: true
+
+  /@img/sharp-linux-x64@0.33.3:
+    resolution: {integrity: sha512-Q4I++herIJxJi+qmbySd072oDPRkCg/SClLEIDh5IL9h1zjhqjv82H0Seupd+q2m0yOfD+/fJnjSoDFtKiHu2g==}
+    engines: {glibc: '>=2.26', node: ^18.17.0 || ^20.3.0 || >=21.0.0, npm: '>=9.6.5', pnpm: '>=7.1.0', yarn: '>=3.2.0'}
+    cpu: [x64]
+    os: [linux]
+    requiresBuild: true
+    optionalDependencies:
+      '@img/sharp-libvips-linux-x64': 1.0.2
+    dev: true
+    optional: true
+
+  /@img/sharp-linuxmusl-arm64@0.33.3:
+    resolution: {integrity: sha512-qnDccehRDXadhM9PM5hLvcPRYqyFCBN31kq+ErBSZtZlsAc1U4Z85xf/RXv1qolkdu+ibw64fUDaRdktxTNP9A==}
+    engines: {musl: '>=1.2.2', node: ^18.17.0 || ^20.3.0 || >=21.0.0, npm: '>=9.6.5', pnpm: '>=7.1.0', yarn: '>=3.2.0'}
+    cpu: [arm64]
+    os: [linux]
+    requiresBuild: true
+    optionalDependencies:
+      '@img/sharp-libvips-linuxmusl-arm64': 1.0.2
+    dev: true
+    optional: true
+
+  /@img/sharp-linuxmusl-x64@0.33.3:
+    resolution: {integrity: sha512-Jhchim8kHWIU/GZ+9poHMWRcefeaxFIs9EBqf9KtcC14Ojk6qua7ghKiPs0sbeLbLj/2IGBtDcxHyjCdYWkk2w==}
+    engines: {musl: '>=1.2.2', node: ^18.17.0 || ^20.3.0 || >=21.0.0, npm: '>=9.6.5', pnpm: '>=7.1.0', yarn: '>=3.2.0'}
+    cpu: [x64]
+    os: [linux]
+    requiresBuild: true
+    optionalDependencies:
+      '@img/sharp-libvips-linuxmusl-x64': 1.0.2
+    dev: true
+    optional: true
+
+  /@img/sharp-wasm32@0.33.3:
+    resolution: {integrity: sha512-68zivsdJ0koE96stdUfM+gmyaK/NcoSZK5dV5CAjES0FUXS9lchYt8LAB5rTbM7nlWtxaU/2GON0HVN6/ZYJAQ==}
+    engines: {node: ^18.17.0 || ^20.3.0 || >=21.0.0, npm: '>=9.6.5', pnpm: '>=7.1.0', yarn: '>=3.2.0'}
+    cpu: [wasm32]
+    requiresBuild: true
+    dependencies:
+      '@emnapi/runtime': 1.1.1
+    dev: true
+    optional: true
+
+  /@img/sharp-win32-ia32@0.33.3:
+    resolution: {integrity: sha512-CyimAduT2whQD8ER4Ux7exKrtfoaUiVr7HG0zZvO0XTFn2idUWljjxv58GxNTkFb8/J9Ub9AqITGkJD6ZginxQ==}
+    engines: {node: ^18.17.0 || ^20.3.0 || >=21.0.0, npm: '>=9.6.5', pnpm: '>=7.1.0', yarn: '>=3.2.0'}
+    cpu: [ia32]
+    os: [win32]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@img/sharp-win32-x64@0.33.3:
+    resolution: {integrity: sha512-viT4fUIDKnli3IfOephGnolMzhz5VaTvDRkYqtZxOMIoMQ4MrAziO7pT1nVnOt2FAm7qW5aa+CCc13aEY6Le0g==}
+    engines: {node: ^18.17.0 || ^20.3.0 || >=21.0.0, npm: '>=9.6.5', pnpm: '>=7.1.0', yarn: '>=3.2.0'}
+    cpu: [x64]
+    os: [win32]
+    requiresBuild: true
     dev: true
+    optional: true
 
   /@jridgewell/gen-mapping@0.3.3:
     resolution: {integrity: sha512-HLhSWOLRi875zjjMG/r+Nv0oCW8umGb0BgEhyX3dDX3egwZtB8PqLnjz3yedt8R5StBrzcg4aBpnh8UA9D1BoQ==}
     engines: {node: '>=6.0.0'}
     dependencies:
       '@jridgewell/set-array': 1.1.2
       '@jridgewell/sourcemap-codec': 1.4.15
@@ -439,172 +638,406 @@
     resolution: {integrity: sha512-oGB+UxlgWcgQkgwo8GcEGwemoTFt3FIO9ababBmaGwXIoBKZ+GTy0pP185beGg7Llih/NSHSV2XAs1lnznocSg==}
     engines: {node: '>= 8'}
     dependencies:
       '@nodelib/fs.scandir': 2.1.5
       fastq: 1.15.0
     dev: true
 
-  /@polka/url@1.0.0-next.23:
-    resolution: {integrity: sha512-C16M+IYz0rgRhWZdCmK+h58JMv8vijAA61gmz2rspCSwKwzBebpdcsiUmwrtJRdphuY30i6BSLEOP8ppbNLyLg==}
+  /@polka/url@1.0.0-next.24:
+    resolution: {integrity: sha512-2LuNTFBIO0m7kKIQvvPHN6UE63VjpmL9rnEEaOOaiSPbZK+zUOYIzBAWcED+3XYzhYsd/0mD57VdxAEqqV52CQ==}
     dev: true
 
-  /@rollup/plugin-commonjs@25.0.7(rollup@3.29.4):
+  /@rollup/plugin-commonjs@25.0.7(rollup@4.12.0):
     resolution: {integrity: sha512-nEvcR+LRjEjsaSsc4x3XZfCCvZIaSMenZu/OiwOKGN2UhQpAYI7ru7czFvyWbErlpoGjnSX3D5Ch5FcMA3kRWQ==}
     engines: {node: '>=14.0.0'}
     peerDependencies:
       rollup: ^2.68.0||^3.0.0||^4.0.0
     peerDependenciesMeta:
       rollup:
         optional: true
     dependencies:
-      '@rollup/pluginutils': 5.0.5(rollup@3.29.4)
+      '@rollup/pluginutils': 5.1.0(rollup@4.12.0)
       commondir: 1.0.1
       estree-walker: 2.0.2
       glob: 8.1.0
       is-reference: 1.2.1
-      magic-string: 0.30.5
-      rollup: 3.29.4
+      magic-string: 0.30.8
+      rollup: 4.12.0
     dev: true
 
-  /@rollup/plugin-json@6.0.1(rollup@3.29.4):
-    resolution: {integrity: sha512-RgVfl5hWMkxN1h/uZj8FVESvPuBJ/uf6ly6GTj0GONnkfoBN5KC0MSz+PN2OLDgYXMhtG0mWpTrkiOjoxAIevw==}
+  /@rollup/plugin-json@6.1.0(rollup@4.12.0):
+    resolution: {integrity: sha512-EGI2te5ENk1coGeADSIwZ7G2Q8CJS2sF120T7jLw4xFw9n7wIOXHo+kIYRAoVpJAN+kmqZSoO3Fp4JtoNF4ReA==}
     engines: {node: '>=14.0.0'}
     peerDependencies:
       rollup: ^1.20.0||^2.0.0||^3.0.0||^4.0.0
     peerDependenciesMeta:
       rollup:
         optional: true
     dependencies:
-      '@rollup/pluginutils': 5.0.5(rollup@3.29.4)
-      rollup: 3.29.4
+      '@rollup/pluginutils': 5.1.0(rollup@4.12.0)
+      rollup: 4.12.0
     dev: true
 
-  /@rollup/plugin-node-resolve@15.2.3(rollup@3.29.4):
+  /@rollup/plugin-node-resolve@15.2.3(rollup@4.12.0):
     resolution: {integrity: sha512-j/lym8nf5E21LwBT4Df1VD6hRO2L2iwUeUmP7litikRsVp1H6NWx20NEp0Y7su+7XGc476GnXXc4kFeZNGmaSQ==}
     engines: {node: '>=14.0.0'}
     peerDependencies:
       rollup: ^2.78.0||^3.0.0||^4.0.0
     peerDependenciesMeta:
       rollup:
         optional: true
     dependencies:
-      '@rollup/pluginutils': 5.0.5(rollup@3.29.4)
+      '@rollup/pluginutils': 5.1.0(rollup@4.12.0)
       '@types/resolve': 1.20.2
       deepmerge: 4.3.1
       is-builtin-module: 3.2.1
       is-module: 1.0.0
       resolve: 1.22.8
-      rollup: 3.29.4
+      rollup: 4.12.0
     dev: true
 
-  /@rollup/pluginutils@5.0.5(rollup@3.29.4):
-    resolution: {integrity: sha512-6aEYR910NyP73oHiJglti74iRyOwgFU4x3meH/H8OJx6Ry0j6cOVZ5X/wTvub7G7Ao6qaHBEaNsV3GLJkSsF+Q==}
+  /@rollup/pluginutils@5.1.0(rollup@4.12.0):
+    resolution: {integrity: sha512-XTIWOPPcpvyKI6L1NHo0lFlCyznUEyPmPY1mc3KpPVDYulHSTvyeLNVW00QTLIAFNhR3kYnJTQHeGqU4M3n09g==}
     engines: {node: '>=14.0.0'}
     peerDependencies:
       rollup: ^1.20.0||^2.0.0||^3.0.0||^4.0.0
     peerDependenciesMeta:
       rollup:
         optional: true
     dependencies:
       '@types/estree': 1.0.5
       estree-walker: 2.0.2
       picomatch: 2.3.1
-      rollup: 3.29.4
+      rollup: 4.12.0
+    dev: true
+
+  /@rollup/rollup-android-arm-eabi@4.12.0:
+    resolution: {integrity: sha512-+ac02NL/2TCKRrJu2wffk1kZ+RyqxVUlbjSagNgPm94frxtr+XDL12E5Ll1enWskLrtrZ2r8L3wED1orIibV/w==}
+    cpu: [arm]
+    os: [android]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-android-arm-eabi@4.14.0:
+    resolution: {integrity: sha512-jwXtxYbRt1V+CdQSy6Z+uZti7JF5irRKF8hlKfEnF/xJpcNGuuiZMBvuoYM+x9sr9iWGnzrlM0+9hvQ1kgkf1w==}
+    cpu: [arm]
+    os: [android]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-android-arm64@4.12.0:
+    resolution: {integrity: sha512-OBqcX2BMe6nvjQ0Nyp7cC90cnumt8PXmO7Dp3gfAju/6YwG0Tj74z1vKrfRz7qAv23nBcYM8BCbhrsWqO7PzQQ==}
+    cpu: [arm64]
+    os: [android]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-android-arm64@4.14.0:
+    resolution: {integrity: sha512-fI9nduZhCccjzlsA/OuAwtFGWocxA4gqXGTLvOyiF8d+8o0fZUeSztixkYjcGq1fGZY3Tkq4yRvHPFxU+jdZ9Q==}
+    cpu: [arm64]
+    os: [android]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-darwin-arm64@4.12.0:
+    resolution: {integrity: sha512-X64tZd8dRE/QTrBIEs63kaOBG0b5GVEd3ccoLtyf6IdXtHdh8h+I56C2yC3PtC9Ucnv0CpNFJLqKFVgCYe0lOQ==}
+    cpu: [arm64]
+    os: [darwin]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-darwin-arm64@4.14.0:
+    resolution: {integrity: sha512-BcnSPRM76/cD2gQC+rQNGBN6GStBs2pl/FpweW8JYuz5J/IEa0Fr4AtrPv766DB/6b2MZ/AfSIOSGw3nEIP8SA==}
+    cpu: [arm64]
+    os: [darwin]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-darwin-x64@4.12.0:
+    resolution: {integrity: sha512-cc71KUZoVbUJmGP2cOuiZ9HSOP14AzBAThn3OU+9LcA1+IUqswJyR1cAJj3Mg55HbjZP6OLAIscbQsQLrpgTOg==}
+    cpu: [x64]
+    os: [darwin]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-darwin-x64@4.14.0:
+    resolution: {integrity: sha512-LDyFB9GRolGN7XI6955aFeI3wCdCUszFWumWU0deHA8VpR3nWRrjG6GtGjBrQxQKFevnUTHKCfPR4IvrW3kCgQ==}
+    cpu: [x64]
+    os: [darwin]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-linux-arm-gnueabihf@4.12.0:
+    resolution: {integrity: sha512-a6w/Y3hyyO6GlpKL2xJ4IOh/7d+APaqLYdMf86xnczU3nurFTaVN9s9jOXQg97BE4nYm/7Ga51rjec5nfRdrvA==}
+    cpu: [arm]
+    os: [linux]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-linux-arm-gnueabihf@4.14.0:
+    resolution: {integrity: sha512-ygrGVhQP47mRh0AAD0zl6QqCbNsf0eTo+vgwkY6LunBcg0f2Jv365GXlDUECIyoXp1kKwL5WW6rsO429DBY/bA==}
+    cpu: [arm]
+    os: [linux]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-linux-arm64-gnu@4.12.0:
+    resolution: {integrity: sha512-0fZBq27b+D7Ar5CQMofVN8sggOVhEtzFUwOwPppQt0k+VR+7UHMZZY4y+64WJ06XOhBTKXtQB/Sv0NwQMXyNAA==}
+    cpu: [arm64]
+    os: [linux]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-linux-arm64-gnu@4.14.0:
+    resolution: {integrity: sha512-x+uJ6MAYRlHGe9wi4HQjxpaKHPM3d3JjqqCkeC5gpnnI6OWovLdXTpfa8trjxPLnWKyBsSi5kne+146GAxFt4A==}
+    cpu: [arm64]
+    os: [linux]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-linux-arm64-musl@4.12.0:
+    resolution: {integrity: sha512-eTvzUS3hhhlgeAv6bfigekzWZjaEX9xP9HhxB0Dvrdbkk5w/b+1Sxct2ZuDxNJKzsRStSq1EaEkVSEe7A7ipgQ==}
+    cpu: [arm64]
+    os: [linux]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-linux-arm64-musl@4.14.0:
+    resolution: {integrity: sha512-nrRw8ZTQKg6+Lttwqo6a2VxR9tOroa2m91XbdQ2sUUzHoedXlsyvY1fN4xWdqz8PKmf4orDwejxXHjh7YBGUCA==}
+    cpu: [arm64]
+    os: [linux]
+    requiresBuild: true
     dev: true
+    optional: true
+
+  /@rollup/rollup-linux-powerpc64le-gnu@4.14.0:
+    resolution: {integrity: sha512-xV0d5jDb4aFu84XKr+lcUJ9y3qpIWhttO3Qev97z8DKLXR62LC3cXT/bMZXrjLF9X+P5oSmJTzAhqwUbY96PnA==}
+    cpu: [ppc64le]
+    os: [linux]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-linux-riscv64-gnu@4.12.0:
+    resolution: {integrity: sha512-ix+qAB9qmrCRiaO71VFfY8rkiAZJL8zQRXveS27HS+pKdjwUfEhqo2+YF2oI+H/22Xsiski+qqwIBxVewLK7sw==}
+    cpu: [riscv64]
+    os: [linux]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-linux-riscv64-gnu@4.14.0:
+    resolution: {integrity: sha512-SDDhBQwZX6LPRoPYjAZWyL27LbcBo7WdBFWJi5PI9RPCzU8ijzkQn7tt8NXiXRiFMJCVpkuMkBf4OxSxVMizAw==}
+    cpu: [riscv64]
+    os: [linux]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-linux-s390x-gnu@4.14.0:
+    resolution: {integrity: sha512-RxB/qez8zIDshNJDufYlTT0ZTVut5eCpAZ3bdXDU9yTxBzui3KhbGjROK2OYTTor7alM7XBhssgoO3CZ0XD3qA==}
+    cpu: [s390x]
+    os: [linux]
+    requiresBuild: true
+    dev: true
+    optional: true
 
-  /@sveltejs/adapter-node@1.3.1(@sveltejs/kit@1.27.6):
-    resolution: {integrity: sha512-A0VgRQDCDPzdLNoiAbcOxGw4zT1Mc+n1LwT1OmO350R7WxrEqdMUChPPOd1iMfIDWlP4ie6E2d/WQf5es2d4Zw==}
+  /@rollup/rollup-linux-x64-gnu@4.12.0:
+    resolution: {integrity: sha512-TenQhZVOtw/3qKOPa7d+QgkeM6xY0LtwzR8OplmyL5LrgTWIXpTQg2Q2ycBf8jm+SFW2Wt/DTn1gf7nFp3ssVA==}
+    cpu: [x64]
+    os: [linux]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-linux-x64-gnu@4.14.0:
+    resolution: {integrity: sha512-C6y6z2eCNCfhZxT9u+jAM2Fup89ZjiG5pIzZIDycs1IwESviLxwkQcFRGLjnDrP+PT+v5i4YFvlcfAs+LnreXg==}
+    cpu: [x64]
+    os: [linux]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-linux-x64-musl@4.12.0:
+    resolution: {integrity: sha512-LfFdRhNnW0zdMvdCb5FNuWlls2WbbSridJvxOvYWgSBOYZtgBfW9UGNJG//rwMqTX1xQE9BAodvMH9tAusKDUw==}
+    cpu: [x64]
+    os: [linux]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-linux-x64-musl@4.14.0:
+    resolution: {integrity: sha512-i0QwbHYfnOMYsBEyjxcwGu5SMIi9sImDVjDg087hpzXqhBSosxkE7gyIYFHgfFl4mr7RrXksIBZ4DoLoP4FhJg==}
+    cpu: [x64]
+    os: [linux]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-win32-arm64-msvc@4.12.0:
+    resolution: {integrity: sha512-JPDxovheWNp6d7AHCgsUlkuCKvtu3RB55iNEkaQcf0ttsDU/JZF+iQnYcQJSk/7PtT4mjjVG8N1kpwnI9SLYaw==}
+    cpu: [arm64]
+    os: [win32]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-win32-arm64-msvc@4.14.0:
+    resolution: {integrity: sha512-Fq52EYb0riNHLBTAcL0cun+rRwyZ10S9vKzhGKKgeD+XbwunszSY0rVMco5KbOsTlwovP2rTOkiII/fQ4ih/zQ==}
+    cpu: [arm64]
+    os: [win32]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-win32-ia32-msvc@4.12.0:
+    resolution: {integrity: sha512-fjtuvMWRGJn1oZacG8IPnzIV6GF2/XG+h71FKn76OYFqySXInJtseAqdprVTDTyqPxQOG9Exak5/E9Z3+EJ8ZA==}
+    cpu: [ia32]
+    os: [win32]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-win32-ia32-msvc@4.14.0:
+    resolution: {integrity: sha512-e/PBHxPdJ00O9p5Ui43+vixSgVf4NlLsmV6QneGERJ3lnjIua/kim6PRFe3iDueT1rQcgSkYP8ZBBXa/h4iPvw==}
+    cpu: [ia32]
+    os: [win32]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-win32-x64-msvc@4.12.0:
+    resolution: {integrity: sha512-ZYmr5mS2wd4Dew/JjT0Fqi2NPB/ZhZ2VvPp7SmvPZb4Y1CG/LRcS6tcRo2cYU7zLK5A7cdbhWnnWmUjoI4qapg==}
+    cpu: [x64]
+    os: [win32]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-win32-x64-msvc@4.14.0:
+    resolution: {integrity: sha512-aGg7iToJjdklmxlUlJh/PaPNa4PmqHfyRMLunbL3eaMO0gp656+q1zOKkpJ/CVe9CryJv6tAN1HDoR8cNGzkag==}
+    cpu: [x64]
+    os: [win32]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@sveltejs/adapter-node@5.0.1(@sveltejs/kit@2.5.6):
+    resolution: {integrity: sha512-eYdmxdUWMW+dad1JfMsWBPY2vjXz9eE+52A2AQnXPScPJlIxIVk5mmbaEEzrZivLfO2wEcLTZ5vdC03W69x+iA==}
     peerDependencies:
-      '@sveltejs/kit': ^1.0.0
+      '@sveltejs/kit': ^2.4.0
     dependencies:
-      '@rollup/plugin-commonjs': 25.0.7(rollup@3.29.4)
-      '@rollup/plugin-json': 6.0.1(rollup@3.29.4)
-      '@rollup/plugin-node-resolve': 15.2.3(rollup@3.29.4)
-      '@sveltejs/kit': 1.27.6(svelte@4.2.8)(vite@4.5.0)
-      rollup: 3.29.4
+      '@rollup/plugin-commonjs': 25.0.7(rollup@4.12.0)
+      '@rollup/plugin-json': 6.1.0(rollup@4.12.0)
+      '@rollup/plugin-node-resolve': 15.2.3(rollup@4.12.0)
+      '@sveltejs/kit': 2.5.6(@sveltejs/vite-plugin-svelte@3.1.0)(svelte@4.2.14)(vite@5.2.8)
+      rollup: 4.12.0
     dev: true
 
-  /@sveltejs/kit@1.27.6(svelte@4.2.8)(vite@4.5.0):
-    resolution: {integrity: sha512-GsjTkMbKzXdbeRg0tk8S7HNShQ4879ftRr0ZHaZfjbig1xQwG57Bvcm9U9/mpLJtCapLbLWUnygKrgcLISLC8A==}
-    engines: {node: ^16.14 || >=18}
+  /@sveltejs/enhanced-img@0.2.0(svelte@4.2.14):
+    resolution: {integrity: sha512-W6wG0RxQYoL13LmUl8IBHeQatMXSd2ybrjg/WQuE5EoIJq+wUkf1hUDaMp9PHe4ubpnzWK/c0QaE5Ls+zjHimA==}
+    dependencies:
+      magic-string: 0.30.8
+      svelte-parse-markup: 0.1.2(svelte@4.2.14)
+      vite-imagetools: 7.0.1
+    transitivePeerDependencies:
+      - rollup
+      - svelte
+    dev: true
+
+  /@sveltejs/kit@2.5.6(@sveltejs/vite-plugin-svelte@3.1.0)(svelte@4.2.14)(vite@5.2.8):
+    resolution: {integrity: sha512-AYb02Jm5MfNqJHc8zrj7ScQAFAKmTUCkpkfoi8EVaZZDdnjkvI7L2GtnTDhpiXSAZRVitZX4qm59sMS1FgL+lQ==}
+    engines: {node: '>=18.13'}
     hasBin: true
     requiresBuild: true
     peerDependencies:
-      svelte: ^3.54.0 || ^4.0.0-next.0 || ^5.0.0-next.0
-      vite: ^4.0.0
+      '@sveltejs/vite-plugin-svelte': ^3.0.0
+      svelte: ^4.0.0 || ^5.0.0-next.0
+      vite: ^5.0.3
     dependencies:
-      '@sveltejs/vite-plugin-svelte': 2.5.2(svelte@4.2.8)(vite@4.5.0)
-      '@types/cookie': 0.5.4
-      cookie: 0.5.0
+      '@sveltejs/vite-plugin-svelte': 3.1.0(svelte@4.2.14)(vite@5.2.8)
+      '@types/cookie': 0.6.0
+      cookie: 0.6.0
       devalue: 4.3.2
       esm-env: 1.0.0
+      import-meta-resolve: 4.0.0
       kleur: 4.1.5
       magic-string: 0.30.5
-      mrmime: 1.0.1
+      mrmime: 2.0.0
       sade: 1.8.1
       set-cookie-parser: 2.6.0
-      sirv: 2.0.3
-      svelte: 4.2.8
+      sirv: 2.0.4
+      svelte: 4.2.14
       tiny-glob: 0.2.9
-      undici: 5.26.5
-      vite: 4.5.0
-    transitivePeerDependencies:
-      - supports-color
+      vite: 5.2.8
     dev: true
 
-  /@sveltejs/vite-plugin-svelte-inspector@1.0.4(@sveltejs/vite-plugin-svelte@2.5.2)(svelte@4.2.8)(vite@4.5.0):
-    resolution: {integrity: sha512-zjiuZ3yydBtwpF3bj0kQNV0YXe+iKE545QGZVTaylW3eAzFr+pJ/cwK8lZEaRp4JtaJXhD5DyWAV4AxLh6DgaQ==}
-    engines: {node: ^14.18.0 || >= 16}
-    peerDependencies:
-      '@sveltejs/vite-plugin-svelte': ^2.2.0
-      svelte: ^3.54.0 || ^4.0.0
-      vite: ^4.0.0
+  /@sveltejs/vite-plugin-svelte-inspector@2.0.0(@sveltejs/vite-plugin-svelte@3.1.0)(svelte@4.2.14)(vite@5.2.8):
+    resolution: {integrity: sha512-gjr9ZFg1BSlIpfZ4PRewigrvYmHWbDrq2uvvPB1AmTWKuM+dI1JXQSUu2pIrYLb/QncyiIGkFDFKTwJ0XqQZZg==}
+    engines: {node: ^18.0.0 || >=20}
+    peerDependencies:
+      '@sveltejs/vite-plugin-svelte': ^3.0.0
+      svelte: ^4.0.0 || ^5.0.0-next.0
+      vite: ^5.0.0
     dependencies:
-      '@sveltejs/vite-plugin-svelte': 2.5.2(svelte@4.2.8)(vite@4.5.0)
+      '@sveltejs/vite-plugin-svelte': 3.1.0(svelte@4.2.14)(vite@5.2.8)
       debug: 4.3.4
-      svelte: 4.2.8
-      vite: 4.5.0
+      svelte: 4.2.14
+      vite: 5.2.8
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@sveltejs/vite-plugin-svelte@2.5.2(svelte@4.2.8)(vite@4.5.0):
-    resolution: {integrity: sha512-Dfy0Rbl+IctOVfJvWGxrX/3m6vxPLH8o0x+8FA5QEyMUQMo4kGOVIojjryU7YomBAexOTAuYf1RT7809yDziaA==}
-    engines: {node: ^14.18.0 || >= 16}
+  /@sveltejs/vite-plugin-svelte@3.1.0(svelte@4.2.14)(vite@5.2.8):
+    resolution: {integrity: sha512-sY6ncCvg+O3njnzbZexcVtUqOBE3iYmQPJ9y+yXSkOwG576QI/xJrBnQSRXFLGwJNBa0T78JEKg5cIR0WOAuUw==}
+    engines: {node: ^18.0.0 || >=20}
     peerDependencies:
-      svelte: ^3.54.0 || ^4.0.0 || ^5.0.0-next.0
-      vite: ^4.0.0
+      svelte: ^4.0.0 || ^5.0.0-next.0
+      vite: ^5.0.0
     dependencies:
-      '@sveltejs/vite-plugin-svelte-inspector': 1.0.4(@sveltejs/vite-plugin-svelte@2.5.2)(svelte@4.2.8)(vite@4.5.0)
+      '@sveltejs/vite-plugin-svelte-inspector': 2.0.0(@sveltejs/vite-plugin-svelte@3.1.0)(svelte@4.2.14)(vite@5.2.8)
       debug: 4.3.4
       deepmerge: 4.3.1
       kleur: 4.1.5
-      magic-string: 0.30.5
-      svelte: 4.2.8
-      svelte-hmr: 0.15.3(svelte@4.2.8)
-      vite: 4.5.0
-      vitefu: 0.2.5(vite@4.5.0)
+      magic-string: 0.30.9
+      svelte: 4.2.14
+      svelte-hmr: 0.16.0(svelte@4.2.14)
+      vite: 5.2.8
+      vitefu: 0.2.5(vite@5.2.8)
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@tailwindcss/typography@0.5.10(tailwindcss@3.3.5):
-    resolution: {integrity: sha512-Pe8BuPJQJd3FfRnm6H0ulKIGoMEQS+Vq01R6M5aCrFB/ccR/shT+0kXLjouGC1gFLm9hopTFN+DMP0pfwRWzPw==}
+  /@tailwindcss/typography@0.5.12(tailwindcss@3.4.3):
+    resolution: {integrity: sha512-CNwpBpconcP7ppxmuq3qvaCxiRWnbhANpY/ruH4L5qs2GCiVDJXde/pjj2HWPV1+Q4G9+V/etrwUYopdcjAlyg==}
     peerDependencies:
       tailwindcss: '>=3.0.0 || insiders'
     dependencies:
       lodash.castarray: 4.4.0
       lodash.isplainobject: 4.0.6
       lodash.merge: 4.6.2
       postcss-selector-parser: 6.0.10
-      tailwindcss: 3.3.5
+      tailwindcss: 3.4.3
     dev: true
 
-  /@types/cookie@0.5.4:
-    resolution: {integrity: sha512-7z/eR6O859gyWIAjuvBWFzNURmf2oPBmJlfVWkwehU5nzIyjwBsTh7WMmEEV4JFnHuQ3ex4oyTvfKzcyJVDBNA==}
+  /@types/cookie@0.6.0:
+    resolution: {integrity: sha512-4Kh9a6B2bQciAhf7FSuMRRkUWecJgJu9nPnx3yzpsfXX/c50REIqpHY4C82bXP90qrLtXtkDxTZosYO3UpOwlA==}
     dev: true
 
   /@types/estree@1.0.5:
     resolution: {integrity: sha512-/kYRxGDLWzHOB7q+wtSUQlFrtcdUccpfy+X+9iMBpHK8QLLhx2wIPYuS5DYtR9Wa/YlZAbIovy7qVdB1Aq6Lyw==}
     dev: true
 
   /@types/glob@7.2.0:
@@ -632,164 +1065,161 @@
       undici-types: 5.26.5
     dev: true
 
   /@types/prettier@2.7.3:
     resolution: {integrity: sha512-+68kP9yzs4LMp7VNh8gdzMSPZFL44MLGqiHWvttYJe+6qnuVr4Ek9wSBQoveqY/r+LwjCcU29kNVkidwim+kYA==}
     dev: true
 
-  /@types/pug@2.0.9:
-    resolution: {integrity: sha512-Yg4LkgFYvn1faISbDNWmcAC1XoDT8IoMUFspp5mnagKk+UvD2N0IWt5A7GRdMubsNWqgCLmrkf8rXkzNqb4szA==}
+  /@types/pug@2.0.10:
+    resolution: {integrity: sha512-Sk/uYFOBAB7mb74XcpizmH0KOR2Pv3D2Hmrh1Dmy5BmK3MpdSa5kqZcg6EKBdklU0bFXX9gCfzvpnyUehrPIuA==}
     dev: true
 
   /@types/resolve@1.20.2:
     resolution: {integrity: sha512-60BCwRFOZCQhDncwQdxxeOEEkbc5dIMccYLwbxsS4TUNeVECQ/pBJ0j09mrHOl/JJvpRPGwO9SvE4nR2Nb/a4Q==}
     dev: true
 
-  /@types/semver@7.5.6:
-    resolution: {integrity: sha512-dn1l8LaMea/IjDoHNd9J52uBbInB796CDffS6VdIxvqYCPSG0V0DzHp76GpaWnlhg88uYyPbXCDIowa86ybd5A==}
+  /@types/semver@7.5.8:
+    resolution: {integrity: sha512-I8EUhyrgfLrcTkzV3TSsGyl1tSuPrEDzr0yd5m90UgNxQkyDXULk3b6MlQqTCpZpNtWe1K0hzclnZkTcLBe2UQ==}
     dev: true
 
   /@types/set-cookie-parser@2.4.7:
     resolution: {integrity: sha512-+ge/loa0oTozxip6zmhRIk8Z/boU51wl9Q6QdLZcokIGMzY5lFXYy/x7Htj2HTC6/KZP1hUbZ1ekx8DYXICvWg==}
     dependencies:
       '@types/node': 20.9.0
     dev: true
 
-  /@types/uuid@9.0.7:
-    resolution: {integrity: sha512-WUtIVRUZ9i5dYXefDEAI7sh9/O7jGvHg7Df/5O/gtH3Yabe5odI3UWopVR1qbPXQtvOxWu3mM4XxlYeZtMWF4g==}
-    dev: true
-
-  /@typescript-eslint/eslint-plugin@6.13.1(@typescript-eslint/parser@6.13.1)(eslint@8.54.0)(typescript@5.3.2):
-    resolution: {integrity: sha512-5bQDGkXaxD46bPvQt08BUz9YSaO4S0fB1LB5JHQuXTfkGPI3+UUeS387C/e9jRie5GqT8u5kFTrMvAjtX4O5kA==}
-    engines: {node: ^16.0.0 || >=18.0.0}
+  /@typescript-eslint/eslint-plugin@7.6.0(@typescript-eslint/parser@7.6.0)(eslint@8.57.0)(typescript@5.4.5):
+    resolution: {integrity: sha512-gKmTNwZnblUdnTIJu3e9kmeRRzV2j1a/LUO27KNNAnIC5zjy1aSvXSRp4rVNlmAoHlQ7HzX42NbKpcSr4jF80A==}
+    engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
-      '@typescript-eslint/parser': ^6.0.0 || ^6.0.0-alpha
-      eslint: ^7.0.0 || ^8.0.0
+      '@typescript-eslint/parser': ^7.0.0
+      eslint: ^8.56.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
     dependencies:
       '@eslint-community/regexpp': 4.10.0
-      '@typescript-eslint/parser': 6.13.1(eslint@8.54.0)(typescript@5.3.2)
-      '@typescript-eslint/scope-manager': 6.13.1
-      '@typescript-eslint/type-utils': 6.13.1(eslint@8.54.0)(typescript@5.3.2)
-      '@typescript-eslint/utils': 6.13.1(eslint@8.54.0)(typescript@5.3.2)
-      '@typescript-eslint/visitor-keys': 6.13.1
+      '@typescript-eslint/parser': 7.6.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/scope-manager': 7.6.0
+      '@typescript-eslint/type-utils': 7.6.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/utils': 7.6.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/visitor-keys': 7.6.0
       debug: 4.3.4
-      eslint: 8.54.0
+      eslint: 8.57.0
       graphemer: 1.4.0
-      ignore: 5.2.4
+      ignore: 5.3.1
       natural-compare: 1.4.0
-      semver: 7.5.4
-      ts-api-utils: 1.0.3(typescript@5.3.2)
-      typescript: 5.3.2
+      semver: 7.6.0
+      ts-api-utils: 1.3.0(typescript@5.4.5)
+      typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@typescript-eslint/parser@6.13.1(eslint@8.54.0)(typescript@5.3.2):
-    resolution: {integrity: sha512-fs2XOhWCzRhqMmQf0eicLa/CWSaYss2feXsy7xBD/pLyWke/jCIVc2s1ikEAtSW7ina1HNhv7kONoEfVNEcdDQ==}
-    engines: {node: ^16.0.0 || >=18.0.0}
+  /@typescript-eslint/parser@7.6.0(eslint@8.57.0)(typescript@5.4.5):
+    resolution: {integrity: sha512-usPMPHcwX3ZoPWnBnhhorc14NJw9J4HpSXQX4urF2TPKG0au0XhJoZyX62fmvdHONUkmyUe74Hzm1//XA+BoYg==}
+    engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
-      eslint: ^7.0.0 || ^8.0.0
+      eslint: ^8.56.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
     dependencies:
-      '@typescript-eslint/scope-manager': 6.13.1
-      '@typescript-eslint/types': 6.13.1
-      '@typescript-eslint/typescript-estree': 6.13.1(typescript@5.3.2)
-      '@typescript-eslint/visitor-keys': 6.13.1
+      '@typescript-eslint/scope-manager': 7.6.0
+      '@typescript-eslint/types': 7.6.0
+      '@typescript-eslint/typescript-estree': 7.6.0(typescript@5.4.5)
+      '@typescript-eslint/visitor-keys': 7.6.0
       debug: 4.3.4
-      eslint: 8.54.0
-      typescript: 5.3.2
+      eslint: 8.57.0
+      typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@typescript-eslint/scope-manager@6.13.1:
-    resolution: {integrity: sha512-BW0kJ7ceiKi56GbT2KKzZzN+nDxzQK2DS6x0PiSMPjciPgd/JRQGMibyaN2cPt2cAvuoH0oNvn2fwonHI+4QUQ==}
-    engines: {node: ^16.0.0 || >=18.0.0}
+  /@typescript-eslint/scope-manager@7.6.0:
+    resolution: {integrity: sha512-ngttyfExA5PsHSx0rdFgnADMYQi+Zkeiv4/ZxGYUWd0nLs63Ha0ksmp8VMxAIC0wtCFxMos7Lt3PszJssG/E6w==}
+    engines: {node: ^18.18.0 || >=20.0.0}
     dependencies:
-      '@typescript-eslint/types': 6.13.1
-      '@typescript-eslint/visitor-keys': 6.13.1
+      '@typescript-eslint/types': 7.6.0
+      '@typescript-eslint/visitor-keys': 7.6.0
     dev: true
 
-  /@typescript-eslint/type-utils@6.13.1(eslint@8.54.0)(typescript@5.3.2):
-    resolution: {integrity: sha512-A2qPlgpxx2v//3meMqQyB1qqTg1h1dJvzca7TugM3Yc2USDY+fsRBiojAEo92HO7f5hW5mjAUF6qobOPzlBCBQ==}
-    engines: {node: ^16.0.0 || >=18.0.0}
+  /@typescript-eslint/type-utils@7.6.0(eslint@8.57.0)(typescript@5.4.5):
+    resolution: {integrity: sha512-NxAfqAPNLG6LTmy7uZgpK8KcuiS2NZD/HlThPXQRGwz6u7MDBWRVliEEl1Gj6U7++kVJTpehkhZzCJLMK66Scw==}
+    engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
-      eslint: ^7.0.0 || ^8.0.0
+      eslint: ^8.56.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
     dependencies:
-      '@typescript-eslint/typescript-estree': 6.13.1(typescript@5.3.2)
-      '@typescript-eslint/utils': 6.13.1(eslint@8.54.0)(typescript@5.3.2)
+      '@typescript-eslint/typescript-estree': 7.6.0(typescript@5.4.5)
+      '@typescript-eslint/utils': 7.6.0(eslint@8.57.0)(typescript@5.4.5)
       debug: 4.3.4
-      eslint: 8.54.0
-      ts-api-utils: 1.0.3(typescript@5.3.2)
-      typescript: 5.3.2
+      eslint: 8.57.0
+      ts-api-utils: 1.3.0(typescript@5.4.5)
+      typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@typescript-eslint/types@6.13.1:
-    resolution: {integrity: sha512-gjeEskSmiEKKFIbnhDXUyiqVma1gRCQNbVZ1C8q7Zjcxh3WZMbzWVfGE9rHfWd1msQtPS0BVD9Jz9jded44eKg==}
-    engines: {node: ^16.0.0 || >=18.0.0}
+  /@typescript-eslint/types@7.6.0:
+    resolution: {integrity: sha512-h02rYQn8J+MureCvHVVzhl69/GAfQGPQZmOMjG1KfCl7o3HtMSlPaPUAPu6lLctXI5ySRGIYk94clD/AUMCUgQ==}
+    engines: {node: ^18.18.0 || >=20.0.0}
     dev: true
 
-  /@typescript-eslint/typescript-estree@6.13.1(typescript@5.3.2):
-    resolution: {integrity: sha512-sBLQsvOC0Q7LGcUHO5qpG1HxRgePbT6wwqOiGLpR8uOJvPJbfs0mW3jPA3ujsDvfiVwVlWUDESNXv44KtINkUQ==}
-    engines: {node: ^16.0.0 || >=18.0.0}
+  /@typescript-eslint/typescript-estree@7.6.0(typescript@5.4.5):
+    resolution: {integrity: sha512-+7Y/GP9VuYibecrCQWSKgl3GvUM5cILRttpWtnAu8GNL9j11e4tbuGZmZjJ8ejnKYyBRb2ddGQ3rEFCq3QjMJw==}
+    engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
     dependencies:
-      '@typescript-eslint/types': 6.13.1
-      '@typescript-eslint/visitor-keys': 6.13.1
+      '@typescript-eslint/types': 7.6.0
+      '@typescript-eslint/visitor-keys': 7.6.0
       debug: 4.3.4
       globby: 11.1.0
       is-glob: 4.0.3
-      semver: 7.5.4
-      ts-api-utils: 1.0.3(typescript@5.3.2)
-      typescript: 5.3.2
+      minimatch: 9.0.4
+      semver: 7.6.0
+      ts-api-utils: 1.3.0(typescript@5.4.5)
+      typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@typescript-eslint/utils@6.13.1(eslint@8.54.0)(typescript@5.3.2):
-    resolution: {integrity: sha512-ouPn/zVoan92JgAegesTXDB/oUp6BP1v8WpfYcqh649ejNc9Qv+B4FF2Ff626kO1xg0wWwwG48lAJ4JuesgdOw==}
-    engines: {node: ^16.0.0 || >=18.0.0}
+  /@typescript-eslint/utils@7.6.0(eslint@8.57.0)(typescript@5.4.5):
+    resolution: {integrity: sha512-x54gaSsRRI+Nwz59TXpCsr6harB98qjXYzsRxGqvA5Ue3kQH+FxS7FYU81g/omn22ML2pZJkisy6Q+ElK8pBCA==}
+    engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
-      eslint: ^7.0.0 || ^8.0.0
+      eslint: ^8.56.0
     dependencies:
-      '@eslint-community/eslint-utils': 4.4.0(eslint@8.54.0)
+      '@eslint-community/eslint-utils': 4.4.0(eslint@8.57.0)
       '@types/json-schema': 7.0.15
-      '@types/semver': 7.5.6
-      '@typescript-eslint/scope-manager': 6.13.1
-      '@typescript-eslint/types': 6.13.1
-      '@typescript-eslint/typescript-estree': 6.13.1(typescript@5.3.2)
-      eslint: 8.54.0
-      semver: 7.5.4
+      '@types/semver': 7.5.8
+      '@typescript-eslint/scope-manager': 7.6.0
+      '@typescript-eslint/types': 7.6.0
+      '@typescript-eslint/typescript-estree': 7.6.0(typescript@5.4.5)
+      eslint: 8.57.0
+      semver: 7.6.0
     transitivePeerDependencies:
       - supports-color
       - typescript
     dev: true
 
-  /@typescript-eslint/visitor-keys@6.13.1:
-    resolution: {integrity: sha512-NDhQUy2tg6XGNBGDRm1XybOHSia8mcXmlbKWoQP+nm1BIIMxa55shyJfZkHpEBN62KNPLrocSM2PdPcaLgDKMQ==}
-    engines: {node: ^16.0.0 || >=18.0.0}
+  /@typescript-eslint/visitor-keys@7.6.0:
+    resolution: {integrity: sha512-4eLB7t+LlNUmXzfOu1VAIAdkjbu5xNSerURS9X/S5TUKWFRpXRQZbmtPqgKmYx8bj3J0irtQXSiWAOY82v+cgw==}
+    engines: {node: ^18.18.0 || >=20.0.0}
     dependencies:
-      '@typescript-eslint/types': 6.13.1
+      '@typescript-eslint/types': 7.6.0
       eslint-visitor-keys: 3.4.3
     dev: true
 
   /@ungap/structured-clone@1.2.0:
     resolution: {integrity: sha512-zuVdFrMJiuCDQUMCzQaD6KL28MjnqqN8XnAqiEq9PNm/hCPTSGfrXCOfwj1ow4LFb/tNymJPwsNbVePc1xFqrQ==}
     dev: true
 
@@ -860,49 +1290,45 @@
     dev: true
 
   /array-union@2.1.0:
     resolution: {integrity: sha512-HGyxoOTYUyCM6stUe6EJgnd4EoewAI7zMdfqO+kGjnlZmBDz/cR5pf8r/cR4Wq60sL/p0IkcjUEEPwS3GFrIyw==}
     engines: {node: '>=8'}
     dev: true
 
-  /autoprefixer@10.4.16(postcss@8.4.31):
-    resolution: {integrity: sha512-7vd3UC6xKp0HLfua5IjZlcXvGAGy7cBAXTg2lyQ/8WpNhd6SiZ8Be+xm3FyBSYJx5GKcpRCzBh7RH4/0dnY+uQ==}
+  /autoprefixer@10.4.19(postcss@8.4.38):
+    resolution: {integrity: sha512-BaENR2+zBZ8xXhM4pUaKUxlVdxZ0EZhjvbopwnXmxRUfqDmwSpC2lAi/QXvx7NRdPCo1WKEcEF6mV64si1z4Ew==}
     engines: {node: ^10 || ^12 || >=14}
     hasBin: true
     peerDependencies:
       postcss: ^8.1.0
     dependencies:
-      browserslist: 4.22.1
-      caniuse-lite: 1.0.30001562
+      browserslist: 4.23.0
+      caniuse-lite: 1.0.30001605
       fraction.js: 4.3.7
       normalize-range: 0.1.2
       picocolors: 1.0.0
-      postcss: 8.4.31
+      postcss: 8.4.38
       postcss-value-parser: 4.2.0
     dev: true
 
-  /axobject-query@3.2.1:
-    resolution: {integrity: sha512-jsyHu61e6N4Vbz/v18DHwWYKK0bSWLqn47eeDSKPB7m8tqMHF9YJ+mhIk2lVteyZrY8tnSj/jHOv4YiTCuCJgg==}
+  /axobject-query@4.0.0:
+    resolution: {integrity: sha512-+60uv1hiVFhHZeO+Lz0RYzsVHy5Wr1ayX0mwda9KPDVLNJgZ1T9Ny7VmFbLDzxsH0D87I86vgj3gFrjTJUYznw==}
     dependencies:
       dequal: 2.0.3
     dev: true
 
   /balanced-match@1.0.2:
     resolution: {integrity: sha512-3oSeUO0TMV67hN1AmbXsK4yaqU7tjiHlbxRDZOpH0KW9+CeX4bRAaX0Anxt0tx2MrpRpWwQaPwIlISEJhYU5Pw==}
     dev: true
 
   /binary-extensions@2.2.0:
     resolution: {integrity: sha512-jDctJ/IVQbZoJykoeHbhXpOlNBqGNcwXJKJog42E5HDPUwQTSdjCHdihjj0DlnheQ7blbT6dHOafNAiS8ooQKA==}
     engines: {node: '>=8'}
     dev: true
 
-  /boolbase@1.0.0:
-    resolution: {integrity: sha512-JZOSA7Mo9sNGB8+UjSgzdLtokWAky1zbztM3WRLCbZ70/3cTANmQmOdR7y2g+J0e2WXywy1yS468tY+IruqEww==}
-    dev: false
-
   /brace-expansion@1.1.11:
     resolution: {integrity: sha512-iCuPHDFgrHX7H2vEI/5xpz07zSHB00TpugqhmYtVmMO6518mCuRMoOYFldEBl0g187ufozdaHgWKcYFb61qGiA==}
     dependencies:
       balanced-match: 1.0.2
       concat-map: 0.0.1
     dev: true
 
@@ -915,23 +1341,23 @@
   /braces@3.0.2:
     resolution: {integrity: sha512-b8um+L1RzM3WDSzvhm6gIz1yfTbBt6YTlcEKAvsmqCZZFw46z626lVj9j1yEPW33H5H+lBQpZMP1k8l+78Ha0A==}
     engines: {node: '>=8'}
     dependencies:
       fill-range: 7.0.1
     dev: true
 
-  /browserslist@4.22.1:
-    resolution: {integrity: sha512-FEVc202+2iuClEhZhrWy6ZiAcRLvNMyYcxZ8raemul1DYVOVdFsbqckWLdsixQZCpJlwe77Z3UTalE7jsjnKfQ==}
+  /browserslist@4.23.0:
+    resolution: {integrity: sha512-QW8HiM1shhT2GuzkvklfjcKDiWFXHOeFCIA/huJPwHsslwcydgk7X+z2zXpEijP98UCY7HbubZt5J2Zgvf0CaQ==}
     engines: {node: ^6 || ^7 || ^8 || ^9 || ^10 || ^11 || ^12 || >=13.7}
     hasBin: true
     dependencies:
-      caniuse-lite: 1.0.30001562
-      electron-to-chromium: 1.4.585
-      node-releases: 2.0.13
-      update-browserslist-db: 1.0.13(browserslist@4.22.1)
+      caniuse-lite: 1.0.30001605
+      electron-to-chromium: 1.4.677
+      node-releases: 2.0.14
+      update-browserslist-db: 1.0.13(browserslist@4.23.0)
     dev: true
 
   /buffer-crc32@0.2.13:
     resolution: {integrity: sha512-VO9Ht/+p3SN7SKWqcrgEzjGbRSJYTx+Q1pTQC0wrWqHx0vpJraQ6GtHx8tvcg1rlK1byhU5gccxgOgj7B0TDkQ==}
     dev: true
 
   /builtin-modules@3.3.0:
@@ -949,50 +1375,26 @@
     dev: true
 
   /camelcase-css@2.0.1:
     resolution: {integrity: sha512-QOSvevhslijgYwRx6Rv7zKdMF8lbRmx+uQGx2+vDc+KI/eBnsy9kit5aj23AgGu3pa4t9AgwbnXWqS+iOY+2aA==}
     engines: {node: '>= 6'}
     dev: true
 
-  /caniuse-lite@1.0.30001562:
-    resolution: {integrity: sha512-kfte3Hym//51EdX4239i+Rmp20EsLIYGdPkERegTgU19hQWCRhsRFGKHTliUlsry53tv17K7n077Kqa0WJU4ng==}
+  /caniuse-lite@1.0.30001605:
+    resolution: {integrity: sha512-nXwGlFWo34uliI9z3n6Qc0wZaf7zaZWA1CPZ169La5mV3I/gem7bst0vr5XQH5TJXZIMfDeZyOrZnSlVzKxxHQ==}
     dev: true
 
   /chalk@4.1.2:
     resolution: {integrity: sha512-oKnbhFyRIXpUuez8iBMmyEa4nbj4IOQyuhc/wy9kY7/WVPcwIO9VA668Pu8RkO7+0G76SLROeyw9CpQ061i4mA==}
     engines: {node: '>=10'}
     dependencies:
       ansi-styles: 4.3.0
       supports-color: 7.2.0
     dev: true
 
-  /cheerio-select@2.1.0:
-    resolution: {integrity: sha512-9v9kG0LvzrlcungtnJtpGNxY+fzECQKhK4EGJX2vByejiMX84MFNQw4UxPJl3bFbTMw+Dfs37XaIkCwTZfLh4g==}
-    dependencies:
-      boolbase: 1.0.0
-      css-select: 5.1.0
-      css-what: 6.1.0
-      domelementtype: 2.3.0
-      domhandler: 5.0.3
-      domutils: 3.1.0
-    dev: false
-
-  /cheerio@1.0.0-rc.12:
-    resolution: {integrity: sha512-VqR8m68vM46BNnuZ5NtnGBKIE/DfN0cRIzg9n40EIq9NOv90ayxLBXA8fXC5gquFRGJSTRqBq25Jt2ECLR431Q==}
-    engines: {node: '>= 6'}
-    dependencies:
-      cheerio-select: 2.1.0
-      dom-serializer: 2.0.0
-      domhandler: 5.0.3
-      domutils: 3.1.0
-      htmlparser2: 8.0.2
-      parse5: 7.1.2
-      parse5-htmlparser2-tree-adapter: 7.0.0
-    dev: false
-
   /chokidar@3.5.3:
     resolution: {integrity: sha512-Dr3sfKRP6oTcjf2JmUmFJfeVMvXBdegxB0iVQ5eb2V10uFJUCAS8OByZdVAyVb8xXNz3GjjTgj9kLWsZTqE6kw==}
     engines: {node: '>= 8.10.0'}
     dependencies:
       anymatch: 3.1.3
       braces: 3.0.2
       glob-parent: 5.1.2
@@ -1032,51 +1434,56 @@
       color-name: 1.1.4
     dev: true
 
   /color-name@1.1.4:
     resolution: {integrity: sha512-dOy+3AuW3a2wNbZHIuMZpTcgjGuLU/uBL/ubcZF9OXbDo8ff4O8yVp5Bf0efS8uEoYo5q4Fx7dY9OgQGXgAsQA==}
     dev: true
 
+  /color-string@1.9.1:
+    resolution: {integrity: sha512-shrVawQFojnZv6xM40anx4CkoDP+fZsw/ZerEMsW/pyzsRbElpsL/DBVW7q3ExxwusdNXI3lXpuhEZkzs8p5Eg==}
+    dependencies:
+      color-name: 1.1.4
+      simple-swizzle: 0.2.2
+    dev: true
+
+  /color@4.2.3:
+    resolution: {integrity: sha512-1rXeuUUiGGrykh+CeBdu5Ie7OJwinCgQY0bc7GCRxy5xVHy+moaqkpL/jqQq0MtQOeYcrqEz4abc5f0KtU7W4A==}
+    engines: {node: '>=12.5.0'}
+    dependencies:
+      color-convert: 2.0.1
+      color-string: 1.9.1
+    dev: true
+
   /commander@4.1.1:
     resolution: {integrity: sha512-NOKm8xhkzAjzFx8B2v5OAHT+u5pRQc2UCa2Vq9jYL/31o2wi9mxBA7LIFs3sV5VSC49z6pEhfbMULvShKj26WA==}
     engines: {node: '>= 6'}
     dev: true
 
   /commondir@1.0.1:
     resolution: {integrity: sha512-W9pAhw0ja1Edb5GVdIF1mjZw/ASI0AlShXM83UUGe2DVr5TdAPEA1OA8m/g8zWp9x6On7gqufY+FatDbC3MDQg==}
     dev: true
 
   /concat-map@0.0.1:
     resolution: {integrity: sha512-/Srv4dswyQNBfohGpz9o6Yb3Gz3SrUDqBH5rTuhGR7ahtlbYKnVxw2bCFMRljaA7EXHaXZ8wsHdodFvbkhKmqg==}
     dev: true
 
-  /cookie@0.5.0:
-    resolution: {integrity: sha512-YZ3GUyn/o8gfKJlnlX7g7xq4gyO6OSuhGPKaaGssGB2qgDUS0gPgtTvoyZLTt9Ab6dC4hfc9dV5arkvc/OCmrw==}
+  /cookie@0.6.0:
+    resolution: {integrity: sha512-U71cyTamuh1CRNCfpGY6to28lxvNwPG4Guz/EVjgf3Jmzv0vlDp1atT9eS5dDjMYHucpHbWns6Lwf3BKz6svdw==}
     engines: {node: '>= 0.6'}
     dev: true
 
   /cross-spawn@7.0.3:
     resolution: {integrity: sha512-iRDPJKUPVEND7dHPO8rkbOnPpyDygcDFtWjpeWNCgy8WP2rXcxXL8TskReQl6OrB2G7+UJrags1q15Fudc7G6w==}
     engines: {node: '>= 8'}
     dependencies:
       path-key: 3.1.1
       shebang-command: 2.0.0
       which: 2.0.2
     dev: true
 
-  /css-select@5.1.0:
-    resolution: {integrity: sha512-nwoRF1rvRRnnCqqY7updORDsuqKzqYJ28+oSMaJMMgOauh3fvwHqMS7EZpIPqK8GL+g9mKxF1vP/ZjSeNjEVHg==}
-    dependencies:
-      boolbase: 1.0.0
-      css-what: 6.1.0
-      domhandler: 5.0.3
-      domutils: 3.1.0
-      nth-check: 2.1.1
-    dev: false
-
   /css-selector-tokenizer@0.8.0:
     resolution: {integrity: sha512-Jd6Ig3/pe62/qe5SBPTN8h8LeUg/pT4lLgtavPf7updwwHpvFzxvOQBHYj2LZDMjUnBzgvIUSjRcf6oT5HzHFg==}
     dependencies:
       cssesc: 3.0.0
       fastparse: 1.1.2
     dev: true
 
@@ -1084,19 +1491,14 @@
     resolution: {integrity: sha512-6Fv1DV/TYw//QF5IzQdqsNDjx/wc8TrMBZsqjL9eW01tWb7R7k/mq+/VXfJCl7SoD5emsJop9cOByJZfs8hYIw==}
     engines: {node: ^10 || ^12.20.0 || ^14.13.0 || >=15.0.0}
     dependencies:
       mdn-data: 2.0.30
       source-map-js: 1.0.2
     dev: true
 
-  /css-what@6.1.0:
-    resolution: {integrity: sha512-HTUrgRJ7r4dsZKU6GjmpfRK1O76h97Z8MfS1G0FozR+oF2kG6Vfe8JE6zwrkbxigziPHinCJ+gCPjA9EaBDtRw==}
-    engines: {node: '>= 6'}
-    dev: false
-
   /cssesc@3.0.0:
     resolution: {integrity: sha512-/Tb/JcjK111nNScGob5MNtsntNM1aCNUDipB/TkwZFhyDrrE47SOx/18wF2bbjgc3ZzCSKW1T5nt5EbFoAz/Vg==}
     engines: {node: '>=4'}
     hasBin: true
     dev: true
 
   /culori@3.2.0:
@@ -1107,22 +1509,22 @@
   /d@1.0.1:
     resolution: {integrity: sha512-m62ShEObQ39CfralilEQRjH6oAMtNCV1xJyEx5LpRYUVN+EviphDgUc/F3hnYbADmkiNs67Y+3ylmlG7Lnu+FA==}
     dependencies:
       es5-ext: 0.10.62
       type: 1.2.0
     dev: true
 
-  /daisyui@4.4.14(postcss@8.4.31):
-    resolution: {integrity: sha512-1g37QzzDFM0QLQe+qRBswkGKyaGijk84t01UMg1ytkFhQxru3zeMh5nWcpC9KnqzKgnITkpSebpGqq4gP8zRrg==}
+  /daisyui@4.10.1(postcss@8.4.38):
+    resolution: {integrity: sha512-Ds0Z0Fv+Xf6ZEqV4Q5JIOeKfg83xxnww0Lzid0V94vPtlQ0yYmucEa33zSctsX2VEgBALtmk5zVEqd59pnUbuQ==}
     engines: {node: '>=16.9.0'}
     dependencies:
       css-selector-tokenizer: 0.8.0
       culori: 3.2.0
       picocolors: 1.0.0
-      postcss-js: 4.0.1(postcss@8.4.31)
+      postcss-js: 4.0.1(postcss@8.4.38)
     transitivePeerDependencies:
       - postcss
     dev: true
 
   /debug@4.3.4:
     resolution: {integrity: sha512-PRWFHuSU3eDtQJPvnNY7Jcket1j0t5OuOsFzPPzsekD52Zl8qUfFIPEiswXqIvHWGVHOgX+7G/vCNNhehwxfkQ==}
     engines: {node: '>=6.0'}
@@ -1150,14 +1552,19 @@
     dev: true
 
   /detect-indent@6.1.0:
     resolution: {integrity: sha512-reYkTUJAZb9gUuZ2RvVCNhVHdg62RHnJ7WJl8ftMi4diZ6NWlciOzQN88pUhSELEwflJht4oQDv0F0BMlwaYtA==}
     engines: {node: '>=8'}
     dev: true
 
+  /detect-libc@2.0.3:
+    resolution: {integrity: sha512-bwy0MGW55bG41VqxxypOsdSdGqLwXPI/focwgTYCFMbdUiBAxLg9CFzG08sz2aqzknwiX7Hkl0bQENjg8iLByw==}
+    engines: {node: '>=8'}
+    dev: true
+
   /devalue@4.3.2:
     resolution: {integrity: sha512-KqFl6pOgOW+Y6wJgu80rHpo2/3H07vr8ntR9rkkFIRETewbf5GaYYcakYfiKz89K+sLsuPkQIZaXDMjUObZwWg==}
     dev: true
 
   /didyoumean@1.2.2:
     resolution: {integrity: sha512-gxtyfqMg7GKyhQmb056K7M3xszy/myH8w+B4RT+QXBQsvAOdc3XymqDDPHx1BgPgsdAA5SIifona89YtRATDzw==}
     dev: true
@@ -1176,50 +1583,18 @@
   /doctrine@3.0.0:
     resolution: {integrity: sha512-yS+Q5i3hBf7GBkd4KG8a7eBNNWNGLTaEwwYWUijIYM7zrlYDM0BFXHjjPWlWZ1Rg7UaddZeIDmi9jF3HmqiQ2w==}
     engines: {node: '>=6.0.0'}
     dependencies:
       esutils: 2.0.3
     dev: true
 
-  /dom-serializer@2.0.0:
-    resolution: {integrity: sha512-wIkAryiqt/nV5EQKqQpo3SToSOV9J0DnbJqwK7Wv/Trc92zIAYZ4FlMu+JPFW1DfGFt81ZTCGgDEabffXeLyJg==}
-    dependencies:
-      domelementtype: 2.3.0
-      domhandler: 5.0.3
-      entities: 4.5.0
-    dev: false
-
-  /domelementtype@2.3.0:
-    resolution: {integrity: sha512-OLETBj6w0OsagBwdXnPdN0cnMfF9opN69co+7ZrbfPGrdpPVNBUj02spi6B1N7wChLQiPn4CSH/zJvXw56gmHw==}
-    dev: false
-
-  /domhandler@5.0.3:
-    resolution: {integrity: sha512-cgwlv/1iFQiFnU96XXgROh8xTeetsnJiDsTc7TYCLFd9+/WNkIqPTxiM/8pSd8VIrhXGTf1Ny1q1hquVqDJB5w==}
-    engines: {node: '>= 4'}
-    dependencies:
-      domelementtype: 2.3.0
-    dev: false
-
-  /domutils@3.1.0:
-    resolution: {integrity: sha512-H78uMmQtI2AhgDJjWeQmHwJJ2bLPD3GMmO7Zja/ZZh84wkm+4ut+IUnUdRa8uCGX88DiVx1j6FRe1XfxEgjEZA==}
-    dependencies:
-      dom-serializer: 2.0.0
-      domelementtype: 2.3.0
-      domhandler: 5.0.3
-    dev: false
-
-  /electron-to-chromium@1.4.585:
-    resolution: {integrity: sha512-B4yBlX0azdA3rVMxpYwLQfDpdwOgcnLCkpvSOd68iFmeedo+WYjaBJS3/W58LVD8CB2nf+o7C4K9xz1l09RkWg==}
+  /electron-to-chromium@1.4.677:
+    resolution: {integrity: sha512-erDa3CaDzwJOpyvfKhOiJjBVNnMM0qxHq47RheVVwsSQrgBA9ZSGV9kdaOfZDPXcHzhG7lBxhj6A7KvfLJBd6Q==}
     dev: true
 
-  /entities@4.5.0:
-    resolution: {integrity: sha512-V0hjH4dGPh9Ao5p0MoRY6BVqtwCjhz6vI5LT8AJ55H+4g9/4vbHx1I54fS0XuclLhDHArPQCiMjDxjaL8fPxhw==}
-    engines: {node: '>=0.12'}
-    dev: false
-
   /es5-ext@0.10.62:
     resolution: {integrity: sha512-BHLqn0klhEpnOKSrzn/Xsz2UIW8j+cGmo9JLzr8BiUapV8hPL9+FliFqjwr9ngW7jWdnxv6eO+/LqyhJVqgrjA==}
     engines: {node: '>=0.10'}
     requiresBuild: true
     dependencies:
       es6-iterator: 2.0.3
       es6-symbol: 3.1.3
@@ -1250,96 +1625,98 @@
     dependencies:
       d: 1.0.1
       es5-ext: 0.10.62
       es6-iterator: 2.0.3
       es6-symbol: 3.1.3
     dev: true
 
-  /esbuild@0.18.20:
-    resolution: {integrity: sha512-ceqxoedUrcayh7Y7ZX6NdbbDzGROiyVBgC4PriJThBKSVPWnnFHZAkfI1lJT8QFkOwH4qOS2SJkS4wvpGl8BpA==}
+  /esbuild@0.20.2:
+    resolution: {integrity: sha512-WdOOppmUNU+IbZ0PaDiTst80zjnrOkyJNHoKupIcVyU8Lvla3Ugx94VzkQ32Ijqd7UhHJy75gNWDMUekcrSJ6g==}
     engines: {node: '>=12'}
     hasBin: true
     requiresBuild: true
     optionalDependencies:
-      '@esbuild/android-arm': 0.18.20
-      '@esbuild/android-arm64': 0.18.20
-      '@esbuild/android-x64': 0.18.20
-      '@esbuild/darwin-arm64': 0.18.20
-      '@esbuild/darwin-x64': 0.18.20
-      '@esbuild/freebsd-arm64': 0.18.20
-      '@esbuild/freebsd-x64': 0.18.20
-      '@esbuild/linux-arm': 0.18.20
-      '@esbuild/linux-arm64': 0.18.20
-      '@esbuild/linux-ia32': 0.18.20
-      '@esbuild/linux-loong64': 0.18.20
-      '@esbuild/linux-mips64el': 0.18.20
-      '@esbuild/linux-ppc64': 0.18.20
-      '@esbuild/linux-riscv64': 0.18.20
-      '@esbuild/linux-s390x': 0.18.20
-      '@esbuild/linux-x64': 0.18.20
-      '@esbuild/netbsd-x64': 0.18.20
-      '@esbuild/openbsd-x64': 0.18.20
-      '@esbuild/sunos-x64': 0.18.20
-      '@esbuild/win32-arm64': 0.18.20
-      '@esbuild/win32-ia32': 0.18.20
-      '@esbuild/win32-x64': 0.18.20
+      '@esbuild/aix-ppc64': 0.20.2
+      '@esbuild/android-arm': 0.20.2
+      '@esbuild/android-arm64': 0.20.2
+      '@esbuild/android-x64': 0.20.2
+      '@esbuild/darwin-arm64': 0.20.2
+      '@esbuild/darwin-x64': 0.20.2
+      '@esbuild/freebsd-arm64': 0.20.2
+      '@esbuild/freebsd-x64': 0.20.2
+      '@esbuild/linux-arm': 0.20.2
+      '@esbuild/linux-arm64': 0.20.2
+      '@esbuild/linux-ia32': 0.20.2
+      '@esbuild/linux-loong64': 0.20.2
+      '@esbuild/linux-mips64el': 0.20.2
+      '@esbuild/linux-ppc64': 0.20.2
+      '@esbuild/linux-riscv64': 0.20.2
+      '@esbuild/linux-s390x': 0.20.2
+      '@esbuild/linux-x64': 0.20.2
+      '@esbuild/netbsd-x64': 0.20.2
+      '@esbuild/openbsd-x64': 0.20.2
+      '@esbuild/sunos-x64': 0.20.2
+      '@esbuild/win32-arm64': 0.20.2
+      '@esbuild/win32-ia32': 0.20.2
+      '@esbuild/win32-x64': 0.20.2
     dev: true
 
-  /escalade@3.1.1:
-    resolution: {integrity: sha512-k0er2gUkLf8O0zKJiAhmkTnJlTvINGv7ygDNPbeIsX/TJjGJZHuh9B2UxbsaEkmlEo9MfhrSzmhIlhRlI2GXnw==}
+  /escalade@3.1.2:
+    resolution: {integrity: sha512-ErCHMCae19vR8vQGe50xIsVomy19rg6gFu3+r3jkEO46suLMWBksvVyoGgQV+jOfl84ZSOSlmv6Gxa89PmTGmA==}
     engines: {node: '>=6'}
     dev: true
 
   /escape-string-regexp@4.0.0:
     resolution: {integrity: sha512-TtpcNJ3XAzx3Gq8sWRzJaVajRs0uVxA2YAkdb1jm2YkPz4G6egUFAyA3n5vtEIZefPk5Wa4UXbKuS5fKkJWdgA==}
     engines: {node: '>=10'}
     dev: true
 
-  /eslint-compat-utils@0.1.2(eslint@8.54.0):
-    resolution: {integrity: sha512-Jia4JDldWnFNIru1Ehx1H5s9/yxiRHY/TimCuUc0jNexew3cF1gI6CYZil1ociakfWO3rRqFjl1mskBblB3RYg==}
+  /eslint-compat-utils@0.5.0(eslint@8.57.0):
+    resolution: {integrity: sha512-dc6Y8tzEcSYZMHa+CMPLi/hyo1FzNeonbhJL7Ol0ccuKQkwopJcJBA9YL/xmMTLU1eKigXo9vj9nALElWYSowg==}
     engines: {node: '>=12'}
     peerDependencies:
       eslint: '>=6.0.0'
     dependencies:
-      eslint: 8.54.0
+      eslint: 8.57.0
+      semver: 7.6.0
     dev: true
 
-  /eslint-config-prettier@9.0.0(eslint@8.54.0):
-    resolution: {integrity: sha512-IcJsTkJae2S35pRsRAwoCE+925rJJStOdkKnLVgtE+tEpqU0EVVM7OqrwxqgptKdX29NUwC82I5pXsGFIgSevw==}
+  /eslint-config-prettier@9.1.0(eslint@8.57.0):
+    resolution: {integrity: sha512-NSWl5BFQWEPi1j4TjVNItzYV7dZXZ+wP6I6ZhrBGpChQhZRUaElihE9uRRkcbRnNb76UMKDF3r+WTmNcGPKsqw==}
     hasBin: true
     peerDependencies:
       eslint: '>=7.0.0'
     dependencies:
-      eslint: 8.54.0
+      eslint: 8.57.0
     dev: true
 
-  /eslint-plugin-svelte@2.35.1(eslint@8.54.0)(svelte@4.2.8):
-    resolution: {integrity: sha512-IF8TpLnROSGy98Z3NrsKXWDSCbNY2ReHDcrYTuXZMbfX7VmESISR78TWgO9zdg4Dht1X8coub5jKwHzP0ExRug==}
+  /eslint-plugin-svelte@2.37.0(eslint@8.57.0)(svelte@4.2.14):
+    resolution: {integrity: sha512-H/2Gz7agYHEMEEzRuLYuCmAIdjuBnbhFG9hOK0yCdSBvvJGJMkjo+lR6j67OIvLOavgp4L7zA5LnDKi8WqdPhQ==}
     engines: {node: ^14.17.0 || >=16.0.0}
     peerDependencies:
-      eslint: ^7.0.0 || ^8.0.0-0
-      svelte: ^3.37.0 || ^4.0.0
+      eslint: ^7.0.0 || ^8.0.0-0 || ^9.0.0-0
+      svelte: ^3.37.0 || ^4.0.0 || ^5.0.0-next.95
     peerDependenciesMeta:
       svelte:
         optional: true
     dependencies:
-      '@eslint-community/eslint-utils': 4.4.0(eslint@8.54.0)
+      '@eslint-community/eslint-utils': 4.4.0(eslint@8.57.0)
       '@jridgewell/sourcemap-codec': 1.4.15
       debug: 4.3.4
-      eslint: 8.54.0
-      eslint-compat-utils: 0.1.2(eslint@8.54.0)
+      eslint: 8.57.0
+      eslint-compat-utils: 0.5.0(eslint@8.57.0)
       esutils: 2.0.3
-      known-css-properties: 0.29.0
-      postcss: 8.4.31
-      postcss-load-config: 3.1.4(postcss@8.4.31)
-      postcss-safe-parser: 6.0.0(postcss@8.4.31)
-      postcss-selector-parser: 6.0.13
-      semver: 7.5.4
-      svelte: 4.2.8
-      svelte-eslint-parser: 0.33.1(svelte@4.2.8)
+      known-css-properties: 0.30.0
+      postcss: 8.4.38
+      postcss-load-config: 3.1.4(postcss@8.4.38)
+      postcss-safe-parser: 6.0.0(postcss@8.4.38)
+      postcss-selector-parser: 6.0.16
+      semver: 7.6.0
+      svelte: 4.2.14
+      svelte-eslint-parser: 0.34.1(svelte@4.2.14)
     transitivePeerDependencies:
       - supports-color
       - ts-node
     dev: true
 
   /eslint-scope@7.2.2:
     resolution: {integrity: sha512-dOt21O7lTMhDM+X9mB4GX+DZrZtCUJPL/wlcTqxyrx5IvO0IYtILdtrQGQp+8n5S0gwSVmOf9NQrjMOgfQZlIg==}
@@ -1350,24 +1727,24 @@
     dev: true
 
   /eslint-visitor-keys@3.4.3:
     resolution: {integrity: sha512-wpc+LXeiyiisxPlEkUzU6svyS1frIO3Mgxj1fdy7Pm8Ygzguax2N3Fa/D/ag1WqbOprdI+uY6wMUl8/a2G+iag==}
     engines: {node: ^12.22.0 || ^14.17.0 || >=16.0.0}
     dev: true
 
-  /eslint@8.54.0:
-    resolution: {integrity: sha512-NY0DfAkM8BIZDVl6PgSa1ttZbx3xHgJzSNJKYcQglem6CppHyMhRIQkBVSSMaSRnLhig3jsDbEzOjwCVt4AmmA==}
+  /eslint@8.57.0:
+    resolution: {integrity: sha512-dZ6+mexnaTIbSBZWgou51U6OmzIhYM2VcNdtiTtI7qPNZm35Akpr0f6vtw3w1Kmn5PYo+tZVfh13WrhpS6oLqQ==}
     engines: {node: ^12.22.0 || ^14.17.0 || >=16.0.0}
     hasBin: true
     dependencies:
-      '@eslint-community/eslint-utils': 4.4.0(eslint@8.54.0)
+      '@eslint-community/eslint-utils': 4.4.0(eslint@8.57.0)
       '@eslint-community/regexpp': 4.10.0
-      '@eslint/eslintrc': 2.1.3
-      '@eslint/js': 8.54.0
-      '@humanwhocodes/config-array': 0.11.13
+      '@eslint/eslintrc': 2.1.4
+      '@eslint/js': 8.57.0
+      '@humanwhocodes/config-array': 0.11.14
       '@humanwhocodes/module-importer': 1.0.1
       '@nodelib/fs.walk': 1.2.8
       '@ungap/structured-clone': 1.2.0
       ajv: 6.12.6
       chalk: 4.1.2
       cross-spawn: 7.0.3
       debug: 4.3.4
@@ -1625,15 +2002,15 @@
   /globby@11.1.0:
     resolution: {integrity: sha512-jhIXaOzy1sb8IyocaruWSn1TjmnBVs8Ayhcy83rmxNJ8q2uWKCAj3CnJY+KpGSXCueAPc0i05kVvVKtP1t9S3g==}
     engines: {node: '>=10'}
     dependencies:
       array-union: 2.1.0
       dir-glob: 3.0.1
       fast-glob: 3.3.2
-      ignore: 5.3.0
+      ignore: 5.3.1
       merge2: 1.4.1
       slash: 3.0.0
     dev: true
 
   /globrex@0.1.2:
     resolution: {integrity: sha512-uHJgbwAMwNFf5mLst7IWLNg14x1CkeqglJb/K3doi4dw6q2IvAAmM/Y81kevy83wP+Sst+nutFTYOGg3d1lsxg==}
     dev: true
@@ -1654,46 +2031,43 @@
   /hasown@2.0.0:
     resolution: {integrity: sha512-vUptKVTpIJhcczKBbgnS+RtcuYMB8+oNzPK2/Hp3hanz8JmpATdmmgLgSaadVREkDm+e2giHwY3ZRkyjSIDDFA==}
     engines: {node: '>= 0.4'}
     dependencies:
       function-bind: 1.1.2
     dev: true
 
-  /highlight.js@11.9.0:
-    resolution: {integrity: sha512-fJ7cW7fQGCYAkgv4CPfwFHrfd/cLS4Hau96JuJ+ZTOWhjnhoeN1ub1tFmALm/+lW5z4WCAuAV9bm05AP0mS6Gw==}
-    engines: {node: '>=12.0.0'}
-    dev: false
-
-  /htmlparser2@8.0.2:
-    resolution: {integrity: sha512-GYdjWKDkbRLkZ5geuHs5NY1puJ+PXwP7+fHPRz06Eirsb9ugf6d8kkXav6ADhcODhFFPMIXyxkxSuMf3D6NCFA==}
-    dependencies:
-      domelementtype: 2.3.0
-      domhandler: 5.0.3
-      domutils: 3.1.0
-      entities: 4.5.0
-    dev: false
-
   /ignore@5.2.4:
     resolution: {integrity: sha512-MAb38BcSbH0eHNBxn7ql2NH/kX33OkB3lZ1BNdh7ENeRChHTYsTvWrMubiIAMNS2llXEEgZ1MUOBtXChP3kaFQ==}
     engines: {node: '>= 4'}
     dev: true
 
-  /ignore@5.3.0:
-    resolution: {integrity: sha512-g7dmpshy+gD7mh88OC9NwSGTKoc3kyLAZQRU1mt53Aw/vnvfXnbC+F/7F7QoYVKbV+KNvJx8wArewKy1vXMtlg==}
+  /ignore@5.3.1:
+    resolution: {integrity: sha512-5Fytz/IraMjqpwfd34ke28PTVMjZjJG2MPn5t7OE4eUCUNf8BAa7b5WUS9/Qvr6mwOQS7Mk6vdsMno5he+T8Xw==}
     engines: {node: '>= 4'}
     dev: true
 
+  /imagetools-core@7.0.0:
+    resolution: {integrity: sha512-6fYbD7u4VIOt6fqKrOlbF77JXgUVyUmEJIPlfYVTuR/S2Ig9cX3gukGiLEU0aSetcfE7CYnhLTPtTEu4mLwhCw==}
+    engines: {node: '>=18.0.0'}
+    dependencies:
+      sharp: 0.33.3
+    dev: true
+
   /import-fresh@3.3.0:
     resolution: {integrity: sha512-veYYhQa+D1QBKznvhUHxb8faxlrwUnxseDAbAp457E0wLNio2bOSKnjYDhMj+YiAq61xrMGhQk9iXVk5FzgQMw==}
     engines: {node: '>=6'}
     dependencies:
       parent-module: 1.0.1
       resolve-from: 4.0.0
     dev: true
 
+  /import-meta-resolve@4.0.0:
+    resolution: {integrity: sha512-okYUR7ZQPH+efeuMJGlq4f8ubUgO50kByRPyt/Cy1Io4PSRsPjxME+YlVaCOx+NIToW7hCsZNFJyTPFFKepRSA==}
+    dev: true
+
   /imurmurhash@0.1.4:
     resolution: {integrity: sha512-JmXMZ6wuvDmLiHEml9ykzqO6lwFbof0GG4IkcGaENdCRDDmMVnny7s5HsIgHCbaq0w2MyPhDqkhTUgS2LU2PHA==}
     engines: {node: '>=0.8.19'}
     dev: true
 
   /inflight@1.0.6:
     resolution: {integrity: sha512-k92I/b08q4wvFscXCLvqfsHCrjrF7yiXsQuIVvVE7N82W3+aqpzuUdBbfhWcy/FZR3/4IgflMgKLOsvPDrGCJA==}
@@ -1702,14 +2076,18 @@
       wrappy: 1.0.2
     dev: true
 
   /inherits@2.0.4:
     resolution: {integrity: sha512-k/vGaX4/Yla3WzyMCvTQOXYeIHvqOKtnqBduzTHpzpQZzAskKMhZ2K+EnBiSM9zGSoIFeMpXKxa4dYeZIQqewQ==}
     dev: true
 
+  /is-arrayish@0.3.2:
+    resolution: {integrity: sha512-eVRqCvVlZbuw3GrM63ovNSNAeA1K16kaR/LRY/92w0zxQ5/1YzwblUX652i4Xs9RwAGjW9d9y6X88t8OaAJfWQ==}
+    dev: true
+
   /is-binary-path@2.1.0:
     resolution: {integrity: sha512-ZMERYes6pDydyuGidse7OsHxtbI7WVeUEozgR/g7rd0xUimYNlvZRE/K2MgZTjWy725IfelLeVcEM97mmtRGXw==}
     engines: {node: '>=8'}
     dependencies:
       binary-extensions: 2.2.0
     dev: true
 
@@ -1784,16 +2162,16 @@
       argparse: 2.0.1
     dev: true
 
   /json-buffer@3.0.1:
     resolution: {integrity: sha512-4bV5BfR2mqfQTJm+V5tPPdf+ZpuhiIvTuAB5g8kcrXOZpTT/QwwVRWBywX1ozr6lEuPdbHxwaJlm9G6mI2sfSQ==}
     dev: true
 
-  /json-schema-to-typescript@13.1.1:
-    resolution: {integrity: sha512-F3CYhtA7F3yPbb8vF7sFchk/2dnr1/yTKf8RcvoNpjnh67ZS/ZMH1ElLt5KHAtf2/bymiejLQQszszPWEeTdSw==}
+  /json-schema-to-typescript@13.1.2:
+    resolution: {integrity: sha512-17G+mjx4nunvOpkPvcz7fdwUwYCEwyH8vR3Ym3rFiQ8uzAL3go+c1306Kk7iGRk8HuXBXqy+JJJmpYl0cvOllw==}
     engines: {node: '>=12.0.0'}
     hasBin: true
     dependencies:
       '@bcherny/json-schema-ref-parser': 10.0.5-fork
       '@types/json-schema': 7.0.15
       '@types/lodash': 4.14.201
       '@types/prettier': 2.7.3
@@ -1824,16 +2202,16 @@
     dev: true
 
   /kleur@4.1.5:
     resolution: {integrity: sha512-o+NO+8WrRiQEE4/7nwRJhN1HWpVmJm511pBHUxPLtp0BUISzlBplORYSmTclCnJvQq2tKu/sgl3xVpkc7ZWuQQ==}
     engines: {node: '>=6'}
     dev: true
 
-  /known-css-properties@0.29.0:
-    resolution: {integrity: sha512-Ne7wqW7/9Cz54PDt4I3tcV+hAyat8ypyOGzYRJQfdxnnjeWsTxt1cy8pjvvKeI5kfXuyvULyeeAvwvvtAX3ayQ==}
+  /known-css-properties@0.30.0:
+    resolution: {integrity: sha512-VSWXYUnsPu9+WYKkfmJyLKtIvaRJi1kXUqVmBACORXZQxT5oZDsoZ2vQP+bQFDnWtpI/4eq3MLoRMjI2fnLzTQ==}
     dev: true
 
   /levn@0.4.1:
     resolution: {integrity: sha512-+bT2uH4E5LGE7h/n3evcS/sQlJXCpIp6ym8OWJ5eV6+67Dsql/LaaT7qJBAt2rzfoa/5QBGBhxDix1dMt2kQKQ==}
     engines: {node: '>= 0.8.0'}
     dependencies:
       prelude-ls: 1.2.1
@@ -1890,23 +2268,30 @@
 
   /lru-queue@0.1.0:
     resolution: {integrity: sha512-BpdYkt9EvGl8OfWHDQPISVpcl5xZthb+XPsbELj5AQXxIC8IriDZIQYjBJPEm5rS420sjZ0TLEzRcq5KdBhYrQ==}
     dependencies:
       es5-ext: 0.10.62
     dev: true
 
-  /magic-string@0.27.0:
-    resolution: {integrity: sha512-8UnnX2PeRAPZuN12svgR9j7M1uWMovg/CEnIwIG0LFkXSJJe4PdfUGiTGl8V9bsBHFUtfVINcSyYxd7q+kx9fA==}
+  /magic-string@0.30.5:
+    resolution: {integrity: sha512-7xlpfBaQaP/T6Vh8MO/EqXSW5En6INHEvEXQiuff7Gku0PWjU3uf6w/j9o7O+SpB5fOAkrI5HeoNgwjEO0pFsA==}
     engines: {node: '>=12'}
     dependencies:
       '@jridgewell/sourcemap-codec': 1.4.15
     dev: true
 
-  /magic-string@0.30.5:
-    resolution: {integrity: sha512-7xlpfBaQaP/T6Vh8MO/EqXSW5En6INHEvEXQiuff7Gku0PWjU3uf6w/j9o7O+SpB5fOAkrI5HeoNgwjEO0pFsA==}
+  /magic-string@0.30.8:
+    resolution: {integrity: sha512-ISQTe55T2ao7XtlAStud6qwYPZjE4GK1S/BeVPus4jrq6JuOnQ00YKQC581RWhR122W7msZV263KzVeLoqidyQ==}
+    engines: {node: '>=12'}
+    dependencies:
+      '@jridgewell/sourcemap-codec': 1.4.15
+    dev: true
+
+  /magic-string@0.30.9:
+    resolution: {integrity: sha512-S1+hd+dIrC8EZqKyT9DstTH/0Z+f76kmmvZnkfQVmOpDEF9iVgdYif3Q/pIWHmCoo59bQVGW0kVL3e2nl+9+Sw==}
     engines: {node: '>=12'}
     dependencies:
       '@jridgewell/sourcemap-codec': 1.4.15
     dev: true
 
   /mdn-data@2.0.30:
     resolution: {integrity: sha512-GaqWWShW4kv/G9IEucWScBx9G1/vsFZZJUO+tD26M8J8z3Kw5RDQjaoZe03YAClgeS/SWPOcb4nkFBTEi5DUEA==}
@@ -1952,14 +2337,21 @@
   /minimatch@5.1.6:
     resolution: {integrity: sha512-lKwV/1brpG6mBUFHtb7NUmtABCb2WZZmm2wNiOA5hAb8VdCS4B3dtMWyvcoViccwAW/COERjXLt0zP1zXUN26g==}
     engines: {node: '>=10'}
     dependencies:
       brace-expansion: 2.0.1
     dev: true
 
+  /minimatch@9.0.4:
+    resolution: {integrity: sha512-KqWh+VchfxcMNRAJjj2tnsSJdNbHsVgnkBhTNrW7AjVo6OvLtxw8zfT9oLw1JSohlFzJ8jCoTgaoXvJ+kHt6fw==}
+    engines: {node: '>=16 || 14 >=14.17'}
+    dependencies:
+      brace-expansion: 2.0.1
+    dev: true
+
   /minimist@1.2.8:
     resolution: {integrity: sha512-2yyAR8qBkN3YuheJanUpWC5U3bb5osDywNB8RzDVlDwDHbocAJveqqj1u8+SVD7jkWT4yvsHCpWqqWqAxb0zCA==}
     dev: true
 
   /mkdirp@0.5.6:
     resolution: {integrity: sha512-FP+p8RB8OWpF3YZBCrP5gtADmtXApB5AMLn+vdyA+PyxCjrCs00mjyUozssO33cwDeT3wNGdLxJ5M//YqtHAJw==}
     hasBin: true
@@ -1974,16 +2366,16 @@
     dev: true
 
   /mri@1.2.0:
     resolution: {integrity: sha512-tzzskb3bG8LvYGFF/mDTpq3jpI6Q9wc3LEmBaghu+DdCssd1FakN7Bc0hVNmEyGq1bq3RgfkCb3cmQLpNPOroA==}
     engines: {node: '>=4'}
     dev: true
 
-  /mrmime@1.0.1:
-    resolution: {integrity: sha512-hzzEagAgDyoU1Q6yg5uI+AorQgdvMCur3FcKf7NhMKWsaYg+RnbTyHRa/9IlLF9rf455MOCtcqqrQQ83pPP7Uw==}
+  /mrmime@2.0.0:
+    resolution: {integrity: sha512-eu38+hdgojoyq63s+yTpN4XMBdt5l8HhMhc4VKLO9KM5caLIBvUm4thi7fFaxyTmCKeNnXZ5pAlBwCUnhA09uw==}
     engines: {node: '>=10'}
     dev: true
 
   /ms@2.1.2:
     resolution: {integrity: sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==}
     dev: true
 
@@ -2005,34 +2397,28 @@
     resolution: {integrity: sha512-OWND8ei3VtNC9h7V60qff3SVobHr996CTwgxubgyQYEpg290h9J0buyECNNJexkFm5sOajh5G116RYA1c8ZMSw==}
     dev: true
 
   /next-tick@1.1.0:
     resolution: {integrity: sha512-CXdUiJembsNjuToQvxayPZF9Vqht7hewsvy2sOWafLvi2awflj9mOC6bHIg50orX8IJvWKY9wYQ/zB2kogPslQ==}
     dev: true
 
-  /node-releases@2.0.13:
-    resolution: {integrity: sha512-uYr7J37ae/ORWdZeQ1xxMJe3NtdmqMC/JZK+geofDrkLUApKRHPd18/TxtBOJ4A0/+uUIliorNrfYV6s1b02eQ==}
+  /node-releases@2.0.14:
+    resolution: {integrity: sha512-y10wOWt8yZpqXmOgRo77WaHEmhYQYGNA6y421PKsKYWEK8aW+cqAphborZDhqfyKrbZEN92CN1X2KbafY2s7Yw==}
     dev: true
 
   /normalize-path@3.0.0:
     resolution: {integrity: sha512-6eZs5Ls3WtCisHWp9S2GUy8dqkpGi4BVSz3GaqiE6ezub0512ESztXUwUB6C6IKbQkY2Pnb/mD4WYojCRwcwLA==}
     engines: {node: '>=0.10.0'}
     dev: true
 
   /normalize-range@0.1.2:
     resolution: {integrity: sha512-bdok/XvKII3nUpklnV6P2hxtMNrCboOjAcyBuQnWEhO665FwrSNRxU+AqpsyvO6LgGYPspN+lu5CLtw4jPRKNA==}
     engines: {node: '>=0.10.0'}
     dev: true
 
-  /nth-check@2.1.1:
-    resolution: {integrity: sha512-lqjrjmaOoAnWfMmBPL+XNnynZh2+swxiX3WUE0s4yEHI6m+AwrK2UZOimIRl3X/4QctVqS8AiZjFqyOGrMXb/w==}
-    dependencies:
-      boolbase: 1.0.0
-    dev: false
-
   /object-assign@4.1.1:
     resolution: {integrity: sha512-rJgTQnkUnH1sFw8yT6VSU3zD3sWmu6sZhIseY8VX+GRu3P6F7Fu+JNDoXfklElbLJSnc3FUQHVe4cU5hj+BcUg==}
     engines: {node: '>=0.10.0'}
     dev: true
 
   /object-hash@3.0.0:
     resolution: {integrity: sha512-RSn9F68PjH9HqtltsSnqYC1XXoWe9Bju5+213R98cNGttag9q9yAOTzdbsqvIa7aNm5WffBZFpWYr2aWrklWAw==}
@@ -2051,23 +2437,23 @@
       openapi-typescript-helpers: 0.0.5
     dev: false
 
   /openapi-typescript-helpers@0.0.5:
     resolution: {integrity: sha512-MRffg93t0hgGZbYTxg60hkRIK2sRuEOHEtCUgMuLgbCC33TMQ68AmxskzUlauzZYD47+ENeGV/ElI7qnWqrAxA==}
     dev: false
 
-  /openapi-typescript@6.7.1:
-    resolution: {integrity: sha512-Q3Ltt0KUm2smcPrsaR8qKmSwQ1KM4yGDJVoQdpYa0yvKPeN8huDx5utMT7DvwvJastHHzUxajjivK3WN2+fobg==}
+  /openapi-typescript@6.7.5:
+    resolution: {integrity: sha512-ZD6dgSZi0u1QCP55g8/2yS5hNJfIpgqsSGHLxxdOjvY7eIrXzj271FJEQw33VwsZ6RCtO/NOuhxa7GBWmEudyA==}
     hasBin: true
     dependencies:
       ansi-colors: 4.1.3
       fast-glob: 3.3.2
       js-yaml: 4.1.0
       supports-color: 9.4.0
-      undici: 5.27.2
+      undici: 5.28.3
       yargs-parser: 21.1.1
     dev: true
 
   /optionator@0.9.3:
     resolution: {integrity: sha512-JjCoypp+jKn1ttEFExxhetCKeJt9zhAgAve5FXHixTvFDW/5aEktX9bufBKLRRMdU7bNtpLfcGu94B3cdEJgjg==}
     engines: {node: '>= 0.8.0'}
     dependencies:
@@ -2096,27 +2482,14 @@
   /parent-module@1.0.1:
     resolution: {integrity: sha512-GQ2EWRpQV8/o+Aw8YqtfZZPfNRWZYkbidE9k5rpl/hC3vtHHBfGm2Ifi6qWV+coDGkrUKZAxE3Lot5kcsRlh+g==}
     engines: {node: '>=6'}
     dependencies:
       callsites: 3.1.0
     dev: true
 
-  /parse5-htmlparser2-tree-adapter@7.0.0:
-    resolution: {integrity: sha512-B77tOZrqqfUfnVcOrUvfdLbz4pu4RopLD/4vmu3HUPswwTA8OH0EMW9BlWR2B0RCoiZRAHEUu7IxeP1Pd1UU+g==}
-    dependencies:
-      domhandler: 5.0.3
-      parse5: 7.1.2
-    dev: false
-
-  /parse5@7.1.2:
-    resolution: {integrity: sha512-Czj1WaSVpaoj0wbhMzLmWD69anp2WH7FXMB9n1Sy8/ZFF9jolSQVMu1Ij5WIyGmcBmhk7EOndpO4mIpihVqAXw==}
-    dependencies:
-      entities: 4.5.0
-    dev: false
-
   /path-exists@4.0.0:
     resolution: {integrity: sha512-ak9Qy5Q7jYb2Wwcey5Fpvg2KoAc/ZIhLSLOSBmRmygPsGwkVVt0fZa0qrtMz+m6tJTAHfZQ8FnmB4MG4LWy7/w==}
     engines: {node: '>=8'}
     dev: true
 
   /path-is-absolute@1.0.1:
     resolution: {integrity: sha512-AVbw3UJ2e9bq64vSaS9Am0fje1Pa8pbGqTTsmXfaIiMpnr5DlDhfJOuLj9Sf95ZPVDAUerDfEk88MPmPe7UCQg==}
@@ -2160,96 +2533,96 @@
     dev: true
 
   /pirates@4.0.6:
     resolution: {integrity: sha512-saLsH7WeYYPiD25LDuLRRY/i+6HaPYr6G1OUlN39otzkSTxKnubR9RTxS3/Kk50s1g2JTgFwWQDQyplC5/SHZg==}
     engines: {node: '>= 6'}
     dev: true
 
-  /postcss-import@15.1.0(postcss@8.4.31):
+  /postcss-import@15.1.0(postcss@8.4.38):
     resolution: {integrity: sha512-hpr+J05B2FVYUAXHeK1YyI267J/dDDhMU6B6civm8hSY1jYJnBXxzKDKDswzJmtLHryrjhnDjqqp/49t8FALew==}
     engines: {node: '>=14.0.0'}
     peerDependencies:
       postcss: ^8.0.0
     dependencies:
-      postcss: 8.4.31
+      postcss: 8.4.38
       postcss-value-parser: 4.2.0
       read-cache: 1.0.0
       resolve: 1.22.8
     dev: true
 
-  /postcss-js@4.0.1(postcss@8.4.31):
+  /postcss-js@4.0.1(postcss@8.4.38):
     resolution: {integrity: sha512-dDLF8pEO191hJMtlHFPRa8xsizHaM82MLfNkUHdUtVEV3tgTp5oj+8qbEqYM57SLfc74KSbw//4SeJma2LRVIw==}
     engines: {node: ^12 || ^14 || >= 16}
     peerDependencies:
       postcss: ^8.4.21
     dependencies:
       camelcase-css: 2.0.1
-      postcss: 8.4.31
+      postcss: 8.4.38
     dev: true
 
-  /postcss-load-config@3.1.4(postcss@8.4.31):
+  /postcss-load-config@3.1.4(postcss@8.4.38):
     resolution: {integrity: sha512-6DiM4E7v4coTE4uzA8U//WhtPwyhiim3eyjEMFCnUpzbrkK9wJHgKDT2mR+HbtSrd/NubVaYTOpSpjUl8NQeRg==}
     engines: {node: '>= 10'}
     peerDependencies:
       postcss: '>=8.0.9'
       ts-node: '>=9.0.0'
     peerDependenciesMeta:
       postcss:
         optional: true
       ts-node:
         optional: true
     dependencies:
       lilconfig: 2.1.0
-      postcss: 8.4.31
+      postcss: 8.4.38
       yaml: 1.10.2
     dev: true
 
-  /postcss-load-config@4.0.2(postcss@8.4.31):
+  /postcss-load-config@4.0.2(postcss@8.4.38):
     resolution: {integrity: sha512-bSVhyJGL00wMVoPUzAVAnbEoWyqRxkjv64tUl427SKnPrENtq6hJwUojroMz2VB+Q1edmi4IfrAPpami5VVgMQ==}
     engines: {node: '>= 14'}
     peerDependencies:
       postcss: '>=8.0.9'
       ts-node: '>=9.0.0'
     peerDependenciesMeta:
       postcss:
         optional: true
       ts-node:
         optional: true
     dependencies:
       lilconfig: 3.0.0
-      postcss: 8.4.31
+      postcss: 8.4.38
       yaml: 2.3.4
     dev: true
 
-  /postcss-nested@6.0.1(postcss@8.4.31):
+  /postcss-nested@6.0.1(postcss@8.4.38):
     resolution: {integrity: sha512-mEp4xPMi5bSWiMbsgoPfcP74lsWLHkQbZc3sY+jWYd65CUwXrUaTp0fmNpa01ZcETKlIgUdFN/MpS2xZtqL9dQ==}
     engines: {node: '>=12.0'}
     peerDependencies:
       postcss: ^8.2.14
     dependencies:
-      postcss: 8.4.31
+      postcss: 8.4.38
       postcss-selector-parser: 6.0.13
     dev: true
 
-  /postcss-safe-parser@6.0.0(postcss@8.4.31):
+  /postcss-safe-parser@6.0.0(postcss@8.4.38):
     resolution: {integrity: sha512-FARHN8pwH+WiS2OPCxJI8FuRJpTVnn6ZNFiqAM2aeW2LwTHWWmWgIyKC6cUo0L8aeKiF/14MNvnpls6R2PBeMQ==}
     engines: {node: '>=12.0'}
     peerDependencies:
       postcss: ^8.3.3
     dependencies:
-      postcss: 8.4.31
+      postcss: 8.4.38
     dev: true
 
-  /postcss-scss@4.0.9(postcss@8.4.31):
+  /postcss-scss@4.0.9(postcss@8.4.38):
     resolution: {integrity: sha512-AjKOeiwAitL/MXxQW2DliT28EKukvvbEWx3LBmJIRN8KfBGZbRTxNYW0kSqi1COiTZ57nZ9NW06S6ux//N1c9A==}
     engines: {node: '>=12.0'}
     peerDependencies:
       postcss: ^8.4.29
     dependencies:
-      postcss: 8.4.31
+      postcss: 8.4.38
     dev: true
 
   /postcss-selector-parser@6.0.10:
     resolution: {integrity: sha512-IQ7TZdoaqbT+LCpShg46jnZVlhWD2w6iQYAcYXfHARZ7X1t/UGhhceQDs5X0cGqKvYlHNOuv7Oa1xmb0oQuA3w==}
     engines: {node: '>=4'}
     dependencies:
       cssesc: 3.0.0
@@ -2260,106 +2633,114 @@
     resolution: {integrity: sha512-EaV1Gl4mUEV4ddhDnv/xtj7sxwrwxdetHdWUGnT4VJQf+4d05v6lHYZr8N573k5Z0BViss7BDhfWtKS3+sfAqQ==}
     engines: {node: '>=4'}
     dependencies:
       cssesc: 3.0.0
       util-deprecate: 1.0.2
     dev: true
 
+  /postcss-selector-parser@6.0.16:
+    resolution: {integrity: sha512-A0RVJrX+IUkVZbW3ClroRWurercFhieevHB38sr2+l9eUClMqome3LmEmnhlNy+5Mr2EYN6B2Kaw9wYdd+VHiw==}
+    engines: {node: '>=4'}
+    dependencies:
+      cssesc: 3.0.0
+      util-deprecate: 1.0.2
+    dev: true
+
   /postcss-value-parser@4.2.0:
     resolution: {integrity: sha512-1NNCs6uurfkVbeXG4S8JFT9t19m45ICnif8zWLd5oPSZ50QnwMfK+H3jv408d4jw/7Bttv5axS5IiHoLaVNHeQ==}
     dev: true
 
-  /postcss@8.4.31:
-    resolution: {integrity: sha512-PS08Iboia9mts/2ygV3eLpY5ghnUcfLV/EXTOW1E2qYxJKGGBUtNjN76FYHnMs36RmARn41bC0AZmn+rR0OVpQ==}
+  /postcss@8.4.38:
+    resolution: {integrity: sha512-Wglpdk03BSfXkHoQa3b/oulrotAkwrlLDRSOb9D0bN86FdRyE9lppSp33aHNPgBa0JKCoB+drFLZkQoRRYae5A==}
     engines: {node: ^10 || ^12 || >=14}
     dependencies:
       nanoid: 3.3.7
       picocolors: 1.0.0
-      source-map-js: 1.0.2
+      source-map-js: 1.2.0
     dev: true
 
   /prelude-ls@1.2.1:
     resolution: {integrity: sha512-vkcDPrRZo1QZLbn5RLGPpg/WmIQ65qoWWhcGKf/b5eplkkarX0m9z8ppCat4mlOqUsWpyNuYgO3VRyrYHSzX5g==}
     engines: {node: '>= 0.8.0'}
     dev: true
 
-  /prettier-plugin-svelte@3.1.2(prettier@3.1.0)(svelte@4.2.8):
-    resolution: {integrity: sha512-7xfMZtwgAWHMT0iZc8jN4o65zgbAQ3+O32V6W7pXrqNvKnHnkoyQCGCbKeUyXKZLbYE0YhFRnamfxfkEGxm8qA==}
+  /prettier-plugin-svelte@3.2.3(prettier@3.2.5)(svelte@4.2.14):
+    resolution: {integrity: sha512-wJq8RunyFlWco6U0WJV5wNCM7zpBFakS76UBSbmzMGpncpK98NZABaE+s7n8/APDCEVNHXC5Mpq+MLebQtsRlg==}
     peerDependencies:
       prettier: ^3.0.0
       svelte: ^3.2.0 || ^4.0.0-next.0 || ^5.0.0-next.0
     dependencies:
-      prettier: 3.1.0
-      svelte: 4.2.8
+      prettier: 3.2.5
+      svelte: 4.2.14
     dev: true
 
-  /prettier-plugin-tailwindcss@0.5.7(prettier-plugin-svelte@3.1.2)(prettier@3.1.0):
-    resolution: {integrity: sha512-4v6uESAgwCni6YF6DwJlRaDjg9Z+al5zM4JfngcazMy4WEf/XkPS5TEQjbD+DZ5iNuG6RrKQLa/HuX2SYzC3kQ==}
+  /prettier-plugin-tailwindcss@0.5.13(prettier-plugin-svelte@3.2.3)(prettier@3.2.5):
+    resolution: {integrity: sha512-2tPWHCFNC+WRjAC4SIWQNSOdcL1NNkydXim8w7TDqlZi+/ulZYz2OouAI6qMtkggnPt7lGamboj6LcTMwcCvoQ==}
     engines: {node: '>=14.21.3'}
     peerDependencies:
       '@ianvs/prettier-plugin-sort-imports': '*'
       '@prettier/plugin-pug': '*'
       '@shopify/prettier-plugin-liquid': '*'
-      '@shufo/prettier-plugin-blade': '*'
       '@trivago/prettier-plugin-sort-imports': '*'
+      '@zackad/prettier-plugin-twig-melody': '*'
       prettier: ^3.0
       prettier-plugin-astro: '*'
       prettier-plugin-css-order: '*'
       prettier-plugin-import-sort: '*'
       prettier-plugin-jsdoc: '*'
       prettier-plugin-marko: '*'
       prettier-plugin-organize-attributes: '*'
       prettier-plugin-organize-imports: '*'
+      prettier-plugin-sort-imports: '*'
       prettier-plugin-style-order: '*'
       prettier-plugin-svelte: '*'
-      prettier-plugin-twig-melody: '*'
     peerDependenciesMeta:
       '@ianvs/prettier-plugin-sort-imports':
         optional: true
       '@prettier/plugin-pug':
         optional: true
       '@shopify/prettier-plugin-liquid':
         optional: true
-      '@shufo/prettier-plugin-blade':
-        optional: true
       '@trivago/prettier-plugin-sort-imports':
         optional: true
+      '@zackad/prettier-plugin-twig-melody':
+        optional: true
       prettier-plugin-astro:
         optional: true
       prettier-plugin-css-order:
         optional: true
       prettier-plugin-import-sort:
         optional: true
       prettier-plugin-jsdoc:
         optional: true
       prettier-plugin-marko:
         optional: true
       prettier-plugin-organize-attributes:
         optional: true
       prettier-plugin-organize-imports:
         optional: true
+      prettier-plugin-sort-imports:
+        optional: true
       prettier-plugin-style-order:
         optional: true
       prettier-plugin-svelte:
         optional: true
-      prettier-plugin-twig-melody:
-        optional: true
     dependencies:
-      prettier: 3.1.0
-      prettier-plugin-svelte: 3.1.2(prettier@3.1.0)(svelte@4.2.8)
+      prettier: 3.2.5
+      prettier-plugin-svelte: 3.2.3(prettier@3.2.5)(svelte@4.2.14)
     dev: true
 
   /prettier@2.8.8:
     resolution: {integrity: sha512-tdN8qQGvNjw4CHbY+XXk0JgCXn9QiF21a55rBe5LJAU+kDyC4WQn4+awm2Xfk2lQMk5fKup9XgzTZtGkjBdP9Q==}
     engines: {node: '>=10.13.0'}
     hasBin: true
     dev: true
 
-  /prettier@3.1.0:
-    resolution: {integrity: sha512-TQLvXjq5IAibjh8EpBIkNKxO749UEWABoiIZehEPiY4GNpVdhaFKqSTu+QrlU6D2dPAfubRmtJTi4K4YkQ5eXw==}
+  /prettier@3.2.5:
+    resolution: {integrity: sha512-3/GWa9aOC0YeD7LUfvOG2NiDyhOWRvt1k+rcKhOuYnMY24iiCphgneUfJDyFXd6rZCAnuLBv6UeAULtrhT/F4A==}
     engines: {node: '>=14'}
     hasBin: true
     dev: true
 
   /punycode@2.3.1:
     resolution: {integrity: sha512-vYt7UD1U9Wg6138shLtLOvdAu+8DsC/ilFtEVHcH+wydcSpNE20AfSOduf6MkRFahL5FY7X1oU7nKVZFtfq8Fg==}
     engines: {node: '>=6'}
@@ -2411,19 +2792,59 @@
   /rimraf@3.0.2:
     resolution: {integrity: sha512-JZkJMZkAGFFPP2YqXZXPbMlMBgsxzE8ILs4lMIX/2o0L9UBw9O/Y3o6wFw/i9YLapcUJWwqbi3kdxIPdC62TIA==}
     hasBin: true
     dependencies:
       glob: 7.2.3
     dev: true
 
-  /rollup@3.29.4:
-    resolution: {integrity: sha512-oWzmBZwvYrU0iJHtDmhsm662rC15FRXmcjCk1xD771dFDx5jJ02ufAQQTn0etB2emNk4J9EZg/yWKpsn9BWGRw==}
-    engines: {node: '>=14.18.0', npm: '>=8.0.0'}
+  /rollup@4.12.0:
+    resolution: {integrity: sha512-wz66wn4t1OHIJw3+XU7mJJQV/2NAfw5OAk6G6Hoo3zcvz/XOfQ52Vgi+AN4Uxoxi0KBBwk2g8zPrTDA4btSB/Q==}
+    engines: {node: '>=18.0.0', npm: '>=8.0.0'}
     hasBin: true
+    dependencies:
+      '@types/estree': 1.0.5
+    optionalDependencies:
+      '@rollup/rollup-android-arm-eabi': 4.12.0
+      '@rollup/rollup-android-arm64': 4.12.0
+      '@rollup/rollup-darwin-arm64': 4.12.0
+      '@rollup/rollup-darwin-x64': 4.12.0
+      '@rollup/rollup-linux-arm-gnueabihf': 4.12.0
+      '@rollup/rollup-linux-arm64-gnu': 4.12.0
+      '@rollup/rollup-linux-arm64-musl': 4.12.0
+      '@rollup/rollup-linux-riscv64-gnu': 4.12.0
+      '@rollup/rollup-linux-x64-gnu': 4.12.0
+      '@rollup/rollup-linux-x64-musl': 4.12.0
+      '@rollup/rollup-win32-arm64-msvc': 4.12.0
+      '@rollup/rollup-win32-ia32-msvc': 4.12.0
+      '@rollup/rollup-win32-x64-msvc': 4.12.0
+      fsevents: 2.3.3
+    dev: true
+
+  /rollup@4.14.0:
+    resolution: {integrity: sha512-Qe7w62TyawbDzB4yt32R0+AbIo6m1/sqO7UPzFS8Z/ksL5mrfhA0v4CavfdmFav3D+ub4QeAgsGEe84DoWe/nQ==}
+    engines: {node: '>=18.0.0', npm: '>=8.0.0'}
+    hasBin: true
+    dependencies:
+      '@types/estree': 1.0.5
     optionalDependencies:
+      '@rollup/rollup-android-arm-eabi': 4.14.0
+      '@rollup/rollup-android-arm64': 4.14.0
+      '@rollup/rollup-darwin-arm64': 4.14.0
+      '@rollup/rollup-darwin-x64': 4.14.0
+      '@rollup/rollup-linux-arm-gnueabihf': 4.14.0
+      '@rollup/rollup-linux-arm64-gnu': 4.14.0
+      '@rollup/rollup-linux-arm64-musl': 4.14.0
+      '@rollup/rollup-linux-powerpc64le-gnu': 4.14.0
+      '@rollup/rollup-linux-riscv64-gnu': 4.14.0
+      '@rollup/rollup-linux-s390x-gnu': 4.14.0
+      '@rollup/rollup-linux-x64-gnu': 4.14.0
+      '@rollup/rollup-linux-x64-musl': 4.14.0
+      '@rollup/rollup-win32-arm64-msvc': 4.14.0
+      '@rollup/rollup-win32-ia32-msvc': 4.14.0
+      '@rollup/rollup-win32-x64-msvc': 4.14.0
       fsevents: 2.3.3
     dev: true
 
   /run-parallel@1.2.0:
     resolution: {integrity: sha512-5l4VyZR86LZ/lDxZTR6jqL8AFE2S0IFLMP26AbjsLVADxHdhB/c0GUsH+y39UfCi3dzz8OlQuPmnaJOMoDHQBA==}
     dependencies:
       queue-microtask: 1.2.3
@@ -2441,43 +2862,79 @@
     dependencies:
       es6-promise: 3.3.1
       graceful-fs: 4.2.11
       mkdirp: 0.5.6
       rimraf: 2.7.1
     dev: true
 
-  /semver@7.5.4:
-    resolution: {integrity: sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==}
+  /semver@7.6.0:
+    resolution: {integrity: sha512-EnwXhrlwXMk9gKu5/flx5sv/an57AkRplG3hTK68W7FRDN+k+OWBj65M7719OkA82XLBxrcX0KSHj+X5COhOVg==}
     engines: {node: '>=10'}
     hasBin: true
     dependencies:
       lru-cache: 6.0.0
     dev: true
 
   /set-cookie-parser@2.6.0:
     resolution: {integrity: sha512-RVnVQxTXuerk653XfuliOxBP81Sf0+qfQE73LIYKcyMYHG94AuH0kgrQpRDuTZnSmjpysHmzxJXKNfa6PjFhyQ==}
 
+  /sharp@0.33.3:
+    resolution: {integrity: sha512-vHUeXJU1UvlO/BNwTpT0x/r53WkLUVxrmb5JTgW92fdFCFk0ispLMAeu/jPO2vjkXM1fYUi3K7/qcLF47pwM1A==}
+    engines: {libvips: '>=8.15.2', node: ^18.17.0 || ^20.3.0 || >=21.0.0}
+    requiresBuild: true
+    dependencies:
+      color: 4.2.3
+      detect-libc: 2.0.3
+      semver: 7.6.0
+    optionalDependencies:
+      '@img/sharp-darwin-arm64': 0.33.3
+      '@img/sharp-darwin-x64': 0.33.3
+      '@img/sharp-libvips-darwin-arm64': 1.0.2
+      '@img/sharp-libvips-darwin-x64': 1.0.2
+      '@img/sharp-libvips-linux-arm': 1.0.2
+      '@img/sharp-libvips-linux-arm64': 1.0.2
+      '@img/sharp-libvips-linux-s390x': 1.0.2
+      '@img/sharp-libvips-linux-x64': 1.0.2
+      '@img/sharp-libvips-linuxmusl-arm64': 1.0.2
+      '@img/sharp-libvips-linuxmusl-x64': 1.0.2
+      '@img/sharp-linux-arm': 0.33.3
+      '@img/sharp-linux-arm64': 0.33.3
+      '@img/sharp-linux-s390x': 0.33.3
+      '@img/sharp-linux-x64': 0.33.3
+      '@img/sharp-linuxmusl-arm64': 0.33.3
+      '@img/sharp-linuxmusl-x64': 0.33.3
+      '@img/sharp-wasm32': 0.33.3
+      '@img/sharp-win32-ia32': 0.33.3
+      '@img/sharp-win32-x64': 0.33.3
+    dev: true
+
   /shebang-command@2.0.0:
     resolution: {integrity: sha512-kHxr2zZpYtdmrN1qDjrrX/Z1rR1kG8Dx+gkpK1G4eXmvXswmcE1hTWBWYUzlraYw1/yZp6YuDY77YtvbN0dmDA==}
     engines: {node: '>=8'}
     dependencies:
       shebang-regex: 3.0.0
     dev: true
 
   /shebang-regex@3.0.0:
     resolution: {integrity: sha512-7++dFhtcx3353uBaq8DDR4NuxBetBzC7ZQOhmTQInHEd6bSrXdiEyzCvG07Z44UYdLShWUyXt5M/yhz8ekcb1A==}
     engines: {node: '>=8'}
     dev: true
 
-  /sirv@2.0.3:
-    resolution: {integrity: sha512-O9jm9BsID1P+0HOi81VpXPoDxYP374pkOLzACAoyUQ/3OUVndNpsz6wMnY2z+yOxzbllCKZrM+9QrWsv4THnyA==}
+  /simple-swizzle@0.2.2:
+    resolution: {integrity: sha512-JA//kQgZtbuY83m+xT+tXJkmJncGMTFT+C+g2h2R9uxkYIrE2yy9sgmcLhCnw57/WSD+Eh3J97FPEDFnbXnDUg==}
+    dependencies:
+      is-arrayish: 0.3.2
+    dev: true
+
+  /sirv@2.0.4:
+    resolution: {integrity: sha512-94Bdh3cC2PKrbgSOUqTiGPWVZeSiXfKOVZNJniWoqrWrRkB1CJzBU3NEbiTsPcYy1lDsANA/THzS+9WBiy5nfQ==}
     engines: {node: '>= 10'}
     dependencies:
-      '@polka/url': 1.0.0-next.23
-      mrmime: 1.0.1
+      '@polka/url': 1.0.0-next.24
+      mrmime: 2.0.0
       totalist: 3.0.1
     dev: true
 
   /slash@3.0.0:
     resolution: {integrity: sha512-g9Q1haeby36OSStwb4ntCGGGaKsaVSjQ68fBxoQcutl5fS1vuY18H3wSt3jFyFtrkx+Kz0V1G85A4MyAdDMi2Q==}
     engines: {node: '>=8'}
     dev: true
@@ -2493,14 +2950,19 @@
     dev: true
 
   /source-map-js@1.0.2:
     resolution: {integrity: sha512-R0XvVJ9WusLiqTCEiGCmICCMplcCkIwwR11mOSD9CR5u+IXYdiseeEuXCVAjS54zqwkLcPNnmU4OeJ6tUrWhDw==}
     engines: {node: '>=0.10.0'}
     dev: true
 
+  /source-map-js@1.2.0:
+    resolution: {integrity: sha512-itJW8lvSA0TXEphiRoawsCksnlf8SyvmFzIhltqAHluXd88pkCd+cXJVHTDwdCr0IzwptSm035IHQktUu1QUMg==}
+    engines: {node: '>=0.10.0'}
+    dev: true
+
   /strip-ansi@6.0.1:
     resolution: {integrity: sha512-Y38VPSHcqkFrCpFnQ9vuSXmquuv5oXOKpGeT6aGrr3o3Gc9AlVa6JBfUSOCnbxGGZF+/0ooI7KrPuUSztUdU5A==}
     engines: {node: '>=8'}
     dependencies:
       ansi-regex: 5.0.1
     dev: true
 
@@ -2543,77 +3005,85 @@
     dev: true
 
   /supports-preserve-symlinks-flag@1.0.0:
     resolution: {integrity: sha512-ot0WnXS9fgdkgIcePe6RHNk1WA8+muPa6cSjeR3V8K27q9BB1rTE3R1p7Hv0z1ZyAc8s6Vvv8DIyWf681MAt0w==}
     engines: {node: '>= 0.4'}
     dev: true
 
-  /svelte-check@3.6.2(postcss-load-config@4.0.2)(postcss@8.4.31)(svelte@4.2.8):
-    resolution: {integrity: sha512-E6iFh4aUCGJLRz6QZXH3gcN/VFfkzwtruWSRmlKrLWQTiO6VzLsivR6q02WYLGNAGecV3EocqZuCDrC2uttZ0g==}
+  /svelte-check@3.6.9(postcss-load-config@4.0.2)(postcss@8.4.38)(svelte@4.2.14):
+    resolution: {integrity: sha512-hDQrk3L0osX07djQyMiXocKysTLfusqi8AriNcCiQxhQR49/LonYolcUGMtZ0fbUR8HTR198Prrgf52WWU9wEg==}
     hasBin: true
     peerDependencies:
       svelte: ^3.55.0 || ^4.0.0-next.0 || ^4.0.0 || ^5.0.0-next.0
     dependencies:
       '@jridgewell/trace-mapping': 0.3.20
       chokidar: 3.5.3
       fast-glob: 3.3.2
       import-fresh: 3.3.0
       picocolors: 1.0.0
       sade: 1.8.1
-      svelte: 4.2.8
-      svelte-preprocess: 5.1.0(postcss-load-config@4.0.2)(postcss@8.4.31)(svelte@4.2.8)(typescript@5.3.2)
-      typescript: 5.3.2
+      svelte: 4.2.14
+      svelte-preprocess: 5.1.3(postcss-load-config@4.0.2)(postcss@8.4.38)(svelte@4.2.14)(typescript@5.4.5)
+      typescript: 5.4.5
     transitivePeerDependencies:
       - '@babel/core'
       - coffeescript
       - less
       - postcss
       - postcss-load-config
       - pug
       - sass
       - stylus
       - sugarss
     dev: true
 
-  /svelte-eslint-parser@0.33.1(svelte@4.2.8):
-    resolution: {integrity: sha512-vo7xPGTlKBGdLH8T5L64FipvTrqv3OQRx9d2z5X05KKZDlF4rQk8KViZO4flKERY+5BiVdOh7zZ7JGJWo5P0uA==}
+  /svelte-eslint-parser@0.34.1(svelte@4.2.14):
+    resolution: {integrity: sha512-9+uLA1pqI9AZioKVGJzYYmlOZWxfoCXSbAM9iaNm7H01XlYlzRTtJfZgl9o3StQGN41PfGJIbkKkfk3e/pHFfA==}
     engines: {node: ^12.22.0 || ^14.17.0 || >=16.0.0}
     peerDependencies:
-      svelte: ^3.37.0 || ^4.0.0
+      svelte: ^3.37.0 || ^4.0.0 || ^5.0.0-next.94
     peerDependenciesMeta:
       svelte:
         optional: true
     dependencies:
       eslint-scope: 7.2.2
       eslint-visitor-keys: 3.4.3
       espree: 9.6.1
-      postcss: 8.4.31
-      postcss-scss: 4.0.9(postcss@8.4.31)
-      svelte: 4.2.8
+      postcss: 8.4.38
+      postcss-scss: 4.0.9(postcss@8.4.38)
+      svelte: 4.2.14
     dev: true
 
-  /svelte-hmr@0.15.3(svelte@4.2.8):
-    resolution: {integrity: sha512-41snaPswvSf8TJUhlkoJBekRrABDXDMdpNpT2tfHIv4JuhgvHqLMhEPGtaQn0BmbNSTkuz2Ed20DF2eHw0SmBQ==}
+  /svelte-hmr@0.16.0(svelte@4.2.14):
+    resolution: {integrity: sha512-Gyc7cOS3VJzLlfj7wKS0ZnzDVdv3Pn2IuVeJPk9m2skfhcu5bq3wtIZyQGggr7/Iim5rH5cncyQft/kRLupcnA==}
     engines: {node: ^12.20 || ^14.13.1 || >= 16}
     peerDependencies:
       svelte: ^3.19.0 || ^4.0.0
     dependencies:
-      svelte: 4.2.8
+      svelte: 4.2.14
     dev: true
 
-  /svelte-preprocess@5.1.0(postcss-load-config@4.0.2)(postcss@8.4.31)(svelte@4.2.8)(typescript@5.3.2):
-    resolution: {integrity: sha512-EkErPiDzHAc0k2MF5m6vBNmRUh338h2myhinUw/xaqsLs7/ZvsgREiLGj03VrSzbY/TB5ZXgBOsKraFee5yceA==}
-    engines: {node: '>= 14.10.0'}
+  /svelte-parse-markup@0.1.2(svelte@4.2.14):
+    resolution: {integrity: sha512-DycY7DJr7VqofiJ63ut1/NEG92HrWWL56VWITn/cJCu+LlZhMoBkBXT4opUitPEEwbq1nMQbv4vTKUfbOqIW1g==}
+    peerDependencies:
+      svelte: ^3.0.0 || ^4.0.0
+    dependencies:
+      svelte: 4.2.14
+    dev: true
+
+  /svelte-preprocess@5.1.3(postcss-load-config@4.0.2)(postcss@8.4.38)(svelte@4.2.14)(typescript@5.4.5):
+    resolution: {integrity: sha512-xxAkmxGHT+J/GourS5mVJeOXZzne1FR5ljeOUAMXUkfEhkLEllRreXpbl3dIYJlcJRfL1LO1uIAPpBpBfiqGPw==}
+    engines: {node: '>= 16.0.0', pnpm: ^8.0.0}
     requiresBuild: true
     peerDependencies:
       '@babel/core': ^7.10.2
       coffeescript: ^2.5.1
       less: ^3.11.3 || ^4.0.0
       postcss: ^7 || ^8
-      postcss-load-config: ^2.1.0 || ^3.0.0 || ^4.0.0
+      postcss-load-config: ^2.1.0 || ^3.0.0 || ^4.0.0 || ^5.0.0
       pug: ^3.0.0
       sass: ^1.26.8
       stylus: ^0.55.0
       sugarss: ^2.0.0 || ^3.0.0 || ^4.0.0
       svelte: ^3.23.0 || ^4.0.0-next.0 || ^4.0.0 || ^5.0.0-next.0
       typescript: '>=3.9.5 || ^4.0.0 || ^5.0.0'
     peerDependenciesMeta:
@@ -2634,46 +3104,47 @@
       stylus:
         optional: true
       sugarss:
         optional: true
       typescript:
         optional: true
     dependencies:
-      '@types/pug': 2.0.9
+      '@types/pug': 2.0.10
       detect-indent: 6.1.0
-      magic-string: 0.27.0
-      postcss: 8.4.31
-      postcss-load-config: 4.0.2(postcss@8.4.31)
+      magic-string: 0.30.8
+      postcss: 8.4.38
+      postcss-load-config: 4.0.2(postcss@8.4.38)
       sorcery: 0.11.0
       strip-indent: 3.0.0
-      svelte: 4.2.8
-      typescript: 5.3.2
+      svelte: 4.2.14
+      typescript: 5.4.5
     dev: true
 
-  /svelte@4.2.8:
-    resolution: {integrity: sha512-hU6dh1MPl8gh6klQZwK/n73GiAHiR95IkFsesLPbMeEZi36ydaXL/ZAb4g9sayT0MXzpxyZjR28yderJHxcmYA==}
+  /svelte@4.2.14:
+    resolution: {integrity: sha512-ry3+YlWqZpHxLy45MW4MZIxNdvB+Wl7p2nnstWKbOAewaJyNJuOtivSbRChcfIej6wFBjWqyKmf/NgK1uW2JAA==}
     engines: {node: '>=16'}
     dependencies:
       '@ampproject/remapping': 2.2.1
       '@jridgewell/sourcemap-codec': 1.4.15
       '@jridgewell/trace-mapping': 0.3.20
+      '@types/estree': 1.0.5
       acorn: 8.11.2
       aria-query: 5.3.0
-      axobject-query: 3.2.1
+      axobject-query: 4.0.0
       code-red: 1.0.4
       css-tree: 2.3.1
       estree-walker: 3.0.3
       is-reference: 3.0.2
       locate-character: 3.0.0
       magic-string: 0.30.5
       periscopic: 3.1.0
     dev: true
 
-  /tailwindcss@3.3.5:
-    resolution: {integrity: sha512-5SEZU4J7pxZgSkv7FP1zY8i2TIAOooNZ1e/OGtxIEv6GltpoiXUqWvLy89+a10qYTB1N5Ifkuw9lqQkN9sscvA==}
+  /tailwindcss@3.4.3:
+    resolution: {integrity: sha512-U7sxQk/n397Bmx4JHbJx/iSOOv5G+II3f1kpLpY2QeUv5DcPdcTsYLlusZfq1NthHS1c1cZoyFmmkex1rzke0A==}
     engines: {node: '>=14.0.0'}
     hasBin: true
     dependencies:
       '@alloc/quick-lru': 5.2.0
       arg: 5.0.2
       chokidar: 3.5.3
       didyoumean: 1.2.2
@@ -2683,19 +3154,19 @@
       is-glob: 4.0.3
       jiti: 1.21.0
       lilconfig: 2.1.0
       micromatch: 4.0.5
       normalize-path: 3.0.0
       object-hash: 3.0.0
       picocolors: 1.0.0
-      postcss: 8.4.31
-      postcss-import: 15.1.0(postcss@8.4.31)
-      postcss-js: 4.0.1(postcss@8.4.31)
-      postcss-load-config: 4.0.2(postcss@8.4.31)
-      postcss-nested: 6.0.1(postcss@8.4.31)
+      postcss: 8.4.38
+      postcss-import: 15.1.0(postcss@8.4.38)
+      postcss-js: 4.0.1(postcss@8.4.38)
+      postcss-load-config: 4.0.2(postcss@8.4.38)
+      postcss-nested: 6.0.1(postcss@8.4.38)
       postcss-selector-parser: 6.0.13
       resolve: 1.22.8
       sucrase: 3.34.0
     transitivePeerDependencies:
       - ts-node
     dev: true
 
@@ -2738,21 +3209,21 @@
     dev: true
 
   /totalist@3.0.1:
     resolution: {integrity: sha512-sf4i37nQ2LBx4m3wB74y+ubopq6W/dIzXg0FDGjsYnZHVa1Da8FH853wlL2gtUhg+xJXjfk3kUZS3BRoQeoQBQ==}
     engines: {node: '>=6'}
     dev: true
 
-  /ts-api-utils@1.0.3(typescript@5.3.2):
-    resolution: {integrity: sha512-wNMeqtMz5NtwpT/UZGY5alT+VoKdSsOOP/kqHFcUW1P/VRhH2wJ48+DN2WwUliNbQ976ETwDL0Ifd2VVvgonvg==}
-    engines: {node: '>=16.13.0'}
+  /ts-api-utils@1.3.0(typescript@5.4.5):
+    resolution: {integrity: sha512-UQMIo7pb8WRomKR1/+MFVLTroIvDVtMX3K6OUir8ynLyzB8Jeriont2bTAtmNPa1ekAgN7YPDyf6V+ygrdU+eQ==}
+    engines: {node: '>=16'}
     peerDependencies:
       typescript: '>=4.2.0'
     dependencies:
-      typescript: 5.3.2
+      typescript: 5.4.5
     dev: true
 
   /ts-interface-checker@0.1.13:
     resolution: {integrity: sha512-Y/arvbn+rrz3JCKl9C4kVNfTfSm2/mEp5FSz5EsZSANGPSlQrpRI5M4PKF+mJnE52jOO90PnPSc3Ur3bTQw0gA==}
     dev: true
 
   /tslib@2.6.2:
@@ -2775,70 +3246,68 @@
     resolution: {integrity: sha512-+5nt5AAniqsCnu2cEQQdpzCAh33kVx8n0VoFidKpB1dVVLAN/F+bgVOqOJqOnEnrhp222clB5p3vUlD+1QAnfg==}
     dev: true
 
   /type@2.7.2:
     resolution: {integrity: sha512-dzlvlNlt6AXU7EBSfpAscydQ7gXB+pPGsPnfJnZpiNJBDj7IaJzQlBZYGdEi4R9HmPdBv2XmWJ6YUtoTa7lmCw==}
     dev: true
 
-  /typescript@5.3.2:
-    resolution: {integrity: sha512-6l+RyNy7oAHDfxC4FzSJcz9vnjTKxrLpDG5M2Vu4SHRVNg6xzqZp6LYSR9zjqQTu8DU/f5xwxUdADOkbrIX2gQ==}
+  /typescript@5.4.5:
+    resolution: {integrity: sha512-vcI4UpRgg81oIRUFwR0WSIHKt11nJ7SAVlYNIu+QpqeyXP+gpQJy/Z4+F0aGxSE4MqwjyXvW/TzgkLAx2AGHwQ==}
     engines: {node: '>=14.17'}
     hasBin: true
     dev: true
 
   /undici-types@5.26.5:
     resolution: {integrity: sha512-JlCMO+ehdEIKqlFxk6IfVoAUVmgz7cU7zD/h9XZ0qzeosSHmUJVOzSQvvYSYWXkFXC+IfLKSIffhv0sVZup6pA==}
     dev: true
 
-  /undici@5.26.5:
-    resolution: {integrity: sha512-cSb4bPFd5qgR7qr2jYAi0hlX9n5YKK2ONKkLFkxl+v/9BvC0sOpZjBHDBSXc5lWAf5ty9oZdRXytBIHzgUcerw==}
+  /undici@5.28.3:
+    resolution: {integrity: sha512-3ItfzbrhDlINjaP0duwnNsKpDQk3acHI3gVJ1z4fmwMK31k5G9OVIAMLSIaP6w4FaGkaAkN6zaQO9LUvZ1t7VA==}
     engines: {node: '>=14.0'}
     dependencies:
       '@fastify/busboy': 2.1.0
     dev: true
 
-  /undici@5.27.2:
-    resolution: {integrity: sha512-iS857PdOEy/y3wlM3yRp+6SNQQ6xU0mmZcwRSriqk+et/cwWAtwmIGf6WkoDN2EK/AMdCO/dfXzIwi+rFMrjjQ==}
-    engines: {node: '>=14.0'}
-    dependencies:
-      '@fastify/busboy': 2.1.0
-    dev: true
-
-  /update-browserslist-db@1.0.13(browserslist@4.22.1):
+  /update-browserslist-db@1.0.13(browserslist@4.23.0):
     resolution: {integrity: sha512-xebP81SNcPuNpPP3uzeW1NYXxI3rxyJzF3pD6sH4jE7o/IX+WtSpwnVU+qIsDPyk0d3hmFQ7mjqc6AtV604hbg==}
     hasBin: true
     peerDependencies:
       browserslist: '>= 4.21.0'
     dependencies:
-      browserslist: 4.22.1
-      escalade: 3.1.1
+      browserslist: 4.23.0
+      escalade: 3.1.2
       picocolors: 1.0.0
     dev: true
 
   /uri-js@4.4.1:
     resolution: {integrity: sha512-7rKUyy33Q1yc98pQ1DAmLtwX109F7TIfWlW1Ydo8Wl1ii1SeHieeh0HHfPeL2fMXK6z0s8ecKs9frCuLJvndBg==}
     dependencies:
       punycode: 2.3.1
     dev: true
 
   /util-deprecate@1.0.2:
     resolution: {integrity: sha512-EPD5q1uXyFxJpCrLnCc1nHnq3gOa6DZBocAIiI2TaSCA7VCJ1UJDMagCzIkXNsUYfD1daK//LTEQ8xiIbrHtcw==}
     dev: true
 
-  /uuid@9.0.1:
-    resolution: {integrity: sha512-b+1eJOlsR9K8HJpow9Ok3fiWOWSIcIzXodvv0rQjVoOVNpWMpxf1wZNpt4y9h10odCNrqnYp1OBzRktckBe3sA==}
-    hasBin: true
-    dev: false
+  /vite-imagetools@7.0.1:
+    resolution: {integrity: sha512-23jnLhkTH0HR9Vd9LxMYnajOLeo0RJNEAHhtlsQP6kfPuOBoTzt54rWbEWB9jmhEXAOflLQpM+FrmilVPAoyGA==}
+    engines: {node: '>=18.0.0'}
+    dependencies:
+      '@rollup/pluginutils': 5.1.0(rollup@4.12.0)
+      imagetools-core: 7.0.0
+    transitivePeerDependencies:
+      - rollup
+    dev: true
 
-  /vite@4.5.0:
-    resolution: {integrity: sha512-ulr8rNLA6rkyFAlVWw2q5YJ91v098AFQ2R0PRFwPzREXOUJQPtFUG0t+/ZikhaOCDqFoDhN6/v8Sq0o4araFAw==}
-    engines: {node: ^14.18.0 || >=16.0.0}
+  /vite@5.2.8:
+    resolution: {integrity: sha512-OyZR+c1CE8yeHw5V5t59aXsUPPVTHMDjEZz8MgguLL/Q7NblxhZUlTu9xSPqlsUO/y+X7dlU05jdhvyycD55DA==}
+    engines: {node: ^18.0.0 || >=20.0.0}
     hasBin: true
     peerDependencies:
-      '@types/node': '>= 14'
+      '@types/node': ^18.0.0 || >=20.0.0
       less: '*'
       lightningcss: ^1.21.0
       sass: '*'
       stylus: '*'
       sugarss: '*'
       terser: ^5.4.0
     peerDependenciesMeta:
@@ -2853,30 +3322,30 @@
       stylus:
         optional: true
       sugarss:
         optional: true
       terser:
         optional: true
     dependencies:
-      esbuild: 0.18.20
-      postcss: 8.4.31
-      rollup: 3.29.4
+      esbuild: 0.20.2
+      postcss: 8.4.38
+      rollup: 4.14.0
     optionalDependencies:
       fsevents: 2.3.3
     dev: true
 
-  /vitefu@0.2.5(vite@4.5.0):
+  /vitefu@0.2.5(vite@5.2.8):
     resolution: {integrity: sha512-SgHtMLoqaeeGnd2evZ849ZbACbnwQCIwRH57t18FxcXoZop0uQu0uzlIhJBlF/eWVzuce0sHeqPcDo+evVcg8Q==}
     peerDependencies:
       vite: ^3.0.0 || ^4.0.0 || ^5.0.0
     peerDependenciesMeta:
       vite:
         optional: true
     dependencies:
-      vite: 4.5.0
+      vite: 5.2.8
     dev: true
 
   /which@2.0.2:
     resolution: {integrity: sha512-BLI3Tl1TW3Pvl70l3yq3Y64i+awpwXqsGBYWkkqMtnbXgrMD+yj7rhW0kuEDxzJaYXGjEW5ogapKNMEKNMjibA==}
     engines: {node: '>= 8'}
     hasBin: true
     dependencies:
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/actions.ts` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/actions.ts`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,20 @@
 export function safeClick(node: HTMLButtonElement, { callback }: SCParams): ActionReturn<SCParams> {
     const handleClick = async (e: Event) => {
         if (node.disabled) {
             return
         }
 
         node.disabled = true
-        await callback(e)
-        node.disabled = false
+
+        try {
+            await callback(e)
+        } finally {
+            node.disabled = false
+        }
     }
 
     node.addEventListener("click", handleClick)
 
     return {
         destroy() {
             node.removeEventListener("click", handleClick)
@@ -88,7 +92,32 @@
     return {
         destroy() {
             node.removeEventListener("scroll", handleScroll)
             unsubscribe()
         },
     }
 }
+
+export function skeleton(node: HTMLIFrameElement | HTMLImageElement): ActionReturn {
+    if (node instanceof HTMLIFrameElement) {
+        if (node.contentDocument === null || node.contentDocument.readyState === "complete") {
+            return {}
+        }
+    } else {
+        if (node.complete) {
+            return {}
+        }
+    }
+
+    const handler = () => {
+        node.classList.remove("skeleton")
+    }
+
+    node.classList.add("skeleton")
+    node.addEventListener("load", handler)
+
+    return {
+        destroy() {
+            node.removeEventListener("load", handler)
+        },
+    }
+}
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/components/FormBuilder.svelte` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/FormBuilder.svelte`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 <script lang="ts">
     import type { ActionResult } from "@sveltejs/kit"
     import { applyAction, enhance } from "$app/forms"
     import { page } from "$app/stores"
     import { PasswordInput } from "$lib/components"
     import type { KratosComponents } from "$lib/types"
 
+    export let primaryGroup: KratosComponents["schemas"]["uiNode"]["group"] | undefined = undefined
     export let validationFreeButtons = [] as string[]
 
     const clipMessage = (msg: string) => {
         return msg.slice(0, msg.indexOf(".") + 1 || msg.length)
     }
     const getGroupActionTitle = (group: KratosComponents["schemas"]["uiNode"]["group"]) => {
         return (
-            nodes.find((node) => node.group === group && node.type === "input" && node.attributes.type === "submit")
-                ?.meta.label?.text ?? ""
+            nodes
+                .find((node) => node.group === group && node.type === "input" && node.attributes.type === "submit")
+                ?.meta.label?.text.split(" with")[0] ?? ""
         )
     }
     const getNodeId = (node: KratosComponents["schemas"]["uiNode"]) => {
         if (node.type === "input") {
             return node.meta.label?.id ?? node.attributes.name + node.attributes.value
         } else {
             return node.attributes.id
@@ -39,15 +41,17 @@
 
     let disabled = false
     let flow: string
     let actionNodes: KratosComponents["schemas"]["uiNodeInput"][]
     let messages: KratosComponents["schemas"]["uiTexts"]
     let nodes: KratosComponents["schemas"]["uiNodes"] = $page.data.nodes
     let currentGroup: KratosComponents["schemas"]["uiNode"]["group"] =
-        nodes.find((node) => node.group !== "default")?.group ?? "default"
+        primaryGroup && nodes.some((node) => node.group === primaryGroup)
+            ? primaryGroup
+            : nodes.find((node) => node.group !== "default")?.group ?? "default"
     let otherGroups: KratosComponents["schemas"]["uiNode"]["group"][]
 
     $: actionNodes = nodes.filter(
         (node) =>
             (node.group === "default" || node.group === currentGroup) &&
             node.type === "input" &&
             node.attributes.type === "submit"
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/components/LoadingIndicator.svelte` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/LoadingIndicator.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/components/NavRail.svelte` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/NavRail.svelte`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 <script lang="ts">
     import { page } from "$app/stores"
     import { scrollShadow, scrollSync } from "$lib/actions"
     import { SwappableIcon } from "$lib/components"
-    import { truncateTitle, useStore } from "$lib/utils"
+    import { truncate, useAppIcon, useStore } from "$lib/utils"
 
     const { currentApp, darkTheme, syncedScrollTops } = useStore()
 </script>
 
 <nav
     class="scrollbar-none w-16 overflow-y-auto py-10"
     use:scrollShadow
     use:scrollSync={{ id: "nav", stores: syncedScrollTops }}
 >
     <ul class="menu items-center gap-1 px-0 py-2">
-        {#each $page.data.apps as { name, href, icon } (name)}
+        {#each $page.data.apps as { name, descriptiveName, href } (name)}
             {@const active = $currentApp?.name === name}
+            {@const { icon, altIcon } = useAppIcon(name)}
             <li class="mt-3 h-8 w-14 transition" class:-translate-y-3={active}>
                 <a class="rounded-full py-1" class:!active={active} {href}>
                     <SwappableIcon
                         class={active && $darkTheme === false ? "fill-neutral-content" : ""}
-                        {active}
                         {icon}
+                        {altIcon}
+                        altIconActive={active}
                     />
                 </a>
             </li>
             <li
                 class="pointer-events-none -mt-7 mb-4 py-1 transition"
                 class:translate-y-4={active}
                 class:opacity-0={!active}
             >
                 <span class="p-0 text-xs font-semibold">
-                    {truncateTitle(name, 8)}
+                    {truncate(descriptiveName, 8)}
                 </span>
             </li>
         {/each}
     </ul>
 </nav>
```

#### html2text {}

```diff
@@ -1,7 +1,9 @@
 } >
-    * {#each $page.data.apps as { name, href, icon } (name)} {@const active =
-      $currentApp?.name === name}
+    * {#each $page.data.apps as { name, descriptiveName, href } (name)} {@const
+      active = $currentApp?.name === name} {@const { icon, altIcon } =
+      useAppIcon(name)}
     * href}>
-    * & $darkTheme === false ? "fill-neutral-content" : ""} {active} {icon} />
-{truncateTitle(name, 8)}
+    * & $darkTheme === false ? "fill-neutral-content" : ""} {icon} {altIcon}
+      altIconActive={active} />
+{truncate(descriptiveName, 8)}
 {/each}
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/components/PasswordInput.svelte` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/PasswordInput.svelte`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <script lang="ts">
     import { SwappableIcon } from "$lib/components"
-    import { EIcon } from "$lib/types"
+    import { VisibilityOffIcon, VisibilityOnIcon } from "$lib/icons"
 
     export let name = ""
     export let value = ""
     export let disabled = false
     export let required = false
     export let autocomplete = "off"
     export let placeholder = ""
@@ -24,10 +24,10 @@
         {value}
         {disabled}
         {required}
         {autocomplete}
         {placeholder}
     />
     <button class="absolute right-3 top-3 h-6 w-6" type="button" on:click={handleClick}>
-        <SwappableIcon active={visible} icon={EIcon.Visibility} />
+        <SwappableIcon icon={VisibilityOnIcon} altIcon={VisibilityOffIcon} altIconActive={visible} />
     </button>
 </span>
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/components/PatchedInlineFrame.svelte` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/PatchedIFrame.svelte`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <script lang="ts">
-    import { onMount } from "svelte"
     import parser from "set-cookie-parser"
+    import { onMount } from "svelte"
     import { goto } from "$app/navigation"
     import { page } from "$app/stores"
     import { getUrlParts, isSameHost, useStore } from "$lib/utils"
 
-    const { currentApp, currentInlineFrame } = useStore()
+    const { currentApp, currentIFrame } = useStore()
 
     const getOriginalUrl = (url: string | URL) => {
         if (typeof url === "string") {
             const { path, query, hash } = getUrlParts(url)
             const params = new URLSearchParams(query)
             params.delete("iframe", "1")
 
@@ -42,14 +42,15 @@
     }
 
     const handleLoad = (e: Event) => {
         const iframe = e.target as HTMLIFrameElement
         const open = iframe.contentWindow!.open.bind(iframe.contentWindow!)
         const pushState = iframe.contentWindow!.history.pushState.bind(iframe.contentWindow!.history)
         const replaceState = iframe.contentWindow!.history.replaceState.bind(iframe.contentWindow!.history)
+        // @ts-expect-error type definition is inaccurate
         const cookie = Object.getOwnPropertyDescriptor(iframe.contentWindow!.Document.prototype, "cookie")!
         const getCookie = cookie.get!.bind(iframe.contentDocument)
         const setCookie = cookie.set!.bind(iframe.contentDocument)
 
         // In case the History API is called before the iframe is loaded
         if (!iframe.contentWindow!.location.search.includes("iframe=1")) {
             replaceState(null, "", getModifiedUrl(iframe.contentWindow!.location.href))
@@ -148,28 +149,28 @@
             },
         })
     }
 
     let iFrame: HTMLIFrameElement | undefined
 
     onMount(() => {
-        $currentInlineFrame = iFrame
+        $currentIFrame = iFrame
         iFrame!.addEventListener("load", handleLoad)
         iFrame!.src = getModifiedUrl($page.url)
 
         const unsubscribe = currentApp.subscribe((value) => {
             if (value) {
                 if (!iFrame!.src.match(`^(?:https?://[^/]+)?${value.href}`)) {
                     iFrame!.src = value.href + "?iframe=1"
                 }
             }
         })
 
         return () => {
             unsubscribe()
             iFrame!.removeEventListener("load", handleLoad)
-            $currentInlineFrame = undefined
+            $currentIFrame = undefined
         }
     })
 </script>
 
 <iframe title={$currentApp?.name ?? ""} class="h-full w-full" bind:this={iFrame} />
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/components/index.ts` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/index.ts`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 export { default as AppShell } from "./AppShell.svelte"
-export { default as Avatar } from "./Avatar.svelte"
-export { default as CodeBlock } from "./CodeBlock.svelte"
 export { default as FormBuilder } from "./FormBuilder.svelte"
 export { default as HeroFrame } from "./HeroFrame.svelte"
 export { default as LoadingIndicator } from "./LoadingIndicator.svelte"
 export { default as NavRail } from "./NavRail.svelte"
 export { default as PasswordInput } from "./PasswordInput.svelte"
-export { default as PatchedInlineFrame } from "./PatchedInlineFrame.svelte"
+export { default as PatchedIFrame } from "./PatchedIFrame.svelte"
 export { default as SwappableIcon } from "./SwappableIcon.svelte"
 export { default as ThemeSelector } from "./ThemeSelector.svelte"
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/Account.svelte` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Account.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/Close.svelte` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Close.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/DarkMode.svelte` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/DarkMode.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/FolderOutline.svelte` & `lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/web/lib/icons/FolderOutline.svelte`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!--suppress JSUnusedGlobalSymbols -->
 <script lang="ts">
     import type { ComponentProps } from "svelte"
-    import BaseIcon from "./BaseIcon.svelte"
+    import BaseIcon from "$lib/icons/BaseIcon.svelte"
 
     // eslint-disable-next-line @typescript-eslint/no-unused-vars
     type $$Props = ComponentProps<BaseIcon>
 </script>
 
 <BaseIcon {...$$restProps}>
     <path
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/Fullscreen.svelte` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Fullscreen.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/Jupyter.svelte` & `lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/web/lib/icons/Jupyter.svelte`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!--suppress JSUnusedGlobalSymbols -->
 <script lang="ts">
     import type { ComponentProps } from "svelte"
-    import BaseIcon from "./BaseIcon.svelte"
+    import BaseIcon from "$lib/icons/BaseIcon.svelte"
 
     // eslint-disable-next-line @typescript-eslint/no-unused-vars
     type $$Props = ComponentProps<BaseIcon>
 </script>
 
 <BaseIcon {...$$restProps}>
     <path
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/LightMode.svelte` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/LightMode.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/Logout.svelte` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Logout.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/Menu.svelte` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Menu.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/NetworkLock.svelte` & `lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/lib/icons/NetworkLock.svelte`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!--suppress JSUnusedGlobalSymbols -->
 <script lang="ts">
     import type { ComponentProps } from "svelte"
-    import BaseIcon from "./BaseIcon.svelte"
+    import BaseIcon from "$lib/icons/BaseIcon.svelte"
 
     // eslint-disable-next-line @typescript-eslint/no-unused-vars
     type $$Props = ComponentProps<BaseIcon>
 </script>
 
 <BaseIcon {...$$restProps}>
     <path
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/NoteOutline.svelte` & `lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/web/lib/icons/NoteOutline.svelte`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!--suppress JSUnusedGlobalSymbols -->
 <script lang="ts">
     import type { ComponentProps } from "svelte"
-    import BaseIcon from "./BaseIcon.svelte"
+    import BaseIcon from "$lib/icons/BaseIcon.svelte"
 
     // eslint-disable-next-line @typescript-eslint/no-unused-vars
     type $$Props = ComponentProps<BaseIcon>
 </script>
 
 <BaseIcon {...$$restProps}>
     <path
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/ProxyOutline.svelte` & `lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/lib/icons/ProxyOutline.svelte`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!--suppress JSUnusedGlobalSymbols -->
 <script lang="ts">
     import type { ComponentProps } from "svelte"
-    import BaseIcon from "./BaseIcon.svelte"
+    import BaseIcon from "$lib/icons/BaseIcon.svelte"
 
     // eslint-disable-next-line @typescript-eslint/no-unused-vars
     type $$Props = ComponentProps<BaseIcon>
 </script>
 
 <BaseIcon {...$$restProps}>
     <path
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/ProxySolid.svelte` & `lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/lib/icons/ProxySolid.svelte`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!--suppress JSUnusedGlobalSymbols -->
 <script lang="ts">
     import type { ComponentProps } from "svelte"
-    import BaseIcon from "./BaseIcon.svelte"
+    import BaseIcon from "$lib/icons/BaseIcon.svelte"
 
     // eslint-disable-next-line @typescript-eslint/no-unused-vars
     type $$Props = ComponentProps<BaseIcon>
 </script>
 
 <BaseIcon {...$$restProps}>
     <path
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/RStudioOutline.svelte` & `lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/web/lib/icons/RStudioOutline.svelte`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!--suppress JSUnusedGlobalSymbols -->
 <script lang="ts">
     import type { ComponentProps } from "svelte"
-    import BaseIcon from "./BaseIcon.svelte"
+    import BaseIcon from "$lib/icons/BaseIcon.svelte"
 
     // eslint-disable-next-line @typescript-eslint/no-unused-vars
     type $$Props = ComponentProps<BaseIcon>
 </script>
 
 <BaseIcon {...$$restProps}>
     <path
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/RStudioSolid.svelte` & `lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/web/lib/icons/RStudioSolid.svelte`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!--suppress JSUnusedGlobalSymbols -->
 <script lang="ts">
     import type { ComponentProps } from "svelte"
-    import BaseIcon from "./BaseIcon.svelte"
+    import BaseIcon from "$lib/icons/BaseIcon.svelte"
 
     // eslint-disable-next-line @typescript-eslint/no-unused-vars
     type $$Props = ComponentProps<BaseIcon>
 </script>
 
 <BaseIcon {...$$restProps}>
     <path
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/Reset.svelte` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Reset.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/Settings.svelte` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Settings.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/VisibilityOff.svelte` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/VisibilityOff.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/icons/VisibilityOn.svelte` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/VisibilityOn.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/stores.ts` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/stores.ts`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import { derived, type Readable, writable, type Writable } from "svelte/store"
 import type { Page } from "@sveltejs/kit"
-import { type App, ETheme } from "$lib/types"
+import { page } from "$app/stores"
+import { type AppInfo, ETheme } from "$lib/types"
 
 export function allowScroll(): Writable<boolean> {
     return writable(true)
 }
 
-export function currentApp(page: Readable<Page>): Readable<App | undefined> {
-    return derived(page, ($page: Page) => $page.data.apps?.find((app: App) => $page.url.pathname.startsWith(app.href)))
+export function currentApp(page: Readable<Page>): Readable<AppInfo | undefined> {
+    return derived(page, ($page: Page) =>
+        $page.data.apps?.find((app: AppInfo) => $page.url.pathname.startsWith(app.href))
+    )
 }
 
-export function currentInlineFrame(): Writable<HTMLIFrameElement | undefined> {
+export function currentContainer(): Writable<HTMLDivElement | undefined> {
+    return writable(undefined)
+}
+
+export function currentIFrame(): Writable<HTMLIFrameElement | undefined> {
     return writable(undefined)
 }
 
 export function currentTheme(): Writable<ETheme> {
     return writable(ETheme.Auto)
 }
 
@@ -31,14 +38,36 @@
                 return true
             default:
                 return false
         }
     })
 }
 
-export function loginForm(): Writable<object | undefined> {
-    return writable(undefined)
+export function isSafari(): Writable<boolean> {
+    return writable(false)
 }
 
 export function syncedScrollTop(): Writable<number> {
     return writable(0)
 }
+
+export class Store {
+    allowScroll: Writable<boolean>
+    currentApp: Readable<AppInfo | undefined>
+    currentContainer: Writable<HTMLDivElement | undefined>
+    currentIFrame: Writable<HTMLIFrameElement | undefined>
+    currentTheme: Writable<ETheme>
+    darkTheme: Readable<boolean | undefined>
+    isSafari: Writable<boolean>
+    syncedScrollTops: { [key: string]: Writable<number> }
+
+    constructor() {
+        this.allowScroll = allowScroll()
+        this.currentApp = currentApp(page)
+        this.currentContainer = currentContainer()
+        this.currentIFrame = currentIFrame()
+        this.currentTheme = currentTheme()
+        this.darkTheme = darkTheme(this.currentTheme)
+        this.isSafari = isSafari()
+        this.syncedScrollTops = {}
+    }
+}
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/types/keto.d.ts` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/types/keto.d.ts`

 * *Files 19% similar despite different names*

```diff
@@ -1,878 +1,891 @@
 /**
  * This file was auto-generated by openapi-typescript.
  * Do not make direct changes to the file.
  */
 
-
 export interface paths {
-  "/admin/relation-tuples": {
+    "/admin/relation-tuples": {
+        /**
+         * Create a Relationship
+         * @description Use this endpoint to create a relationship.
+         */
+        put: operations["createRelationship"]
+        /**
+         * Delete Relationships
+         * @description Use this endpoint to delete relationships
+         */
+        delete: operations["deleteRelationships"]
+        /**
+         * Patch Multiple Relationships
+         * @description Use this endpoint to patch one or more relationships.
+         */
+        patch: operations["patchRelationships"]
+    }
+    "/health/alive": {
+        /**
+         * Check HTTP Server Status
+         * @description This endpoint returns a HTTP 200 status code when Ory Keto is accepting incoming
+         * HTTP requests. This status does currently not include checks whether the database connection is working.
+         *
+         * If the service supports TLS Edge Termination, this endpoint does not require the
+         * `X-Forwarded-Proto` header to be set.
+         *
+         * Be aware that if you are running multiple nodes of this service, the health status will never
+         * refer to the cluster state, only to a single instance.
+         */
+        get: operations["isAlive"]
+    }
+    "/health/ready": {
+        /**
+         * Check HTTP Server and Database Status
+         * @description This endpoint returns a HTTP 200 status code when Ory Keto is up running and the environment dependencies (e.g.
+         * the database) are responsive as well.
+         *
+         * If the service supports TLS Edge Termination, this endpoint does not require the
+         * `X-Forwarded-Proto` header to be set.
+         *
+         * Be aware that if you are running multiple nodes of Ory Keto, the health status will never
+         * refer to the cluster state, only to a single instance.
+         */
+        get: operations["isReady"]
+    }
+    "/namespaces": {
+        /**
+         * Query namespaces
+         * @description Get all namespaces
+         */
+        get: operations["listRelationshipNamespaces"]
+    }
+    "/opl/syntax/check": {
+        /**
+         * Check the syntax of an OPL file
+         * @description The OPL file is expected in the body of the request.
+         */
+        post: operations["checkOplSyntax"]
+    }
+    "/relation-tuples": {
+        /**
+         * Query relationships
+         * @description Get all relationships that match the query. Only the namespace field is required.
+         */
+        get: operations["getRelationships"]
+    }
+    "/relation-tuples/check": {
+        /**
+         * Check a permission
+         * @description To learn how relationship tuples and the check works, head over to [the documentation](https://www.ory.sh/docs/keto/concepts/api-overview).
+         */
+        get: operations["checkPermissionOrError"]
+        /**
+         * Check a permission
+         * @description To learn how relationship tuples and the check works, head over to [the documentation](https://www.ory.sh/docs/keto/concepts/api-overview).
+         */
+        post: operations["postCheckPermissionOrError"]
+    }
+    "/relation-tuples/check/openapi": {
+        /**
+         * Check a permission
+         * @description To learn how relationship tuples and the check works, head over to [the documentation](https://www.ory.sh/docs/keto/concepts/api-overview).
+         */
+        get: operations["checkPermission"]
+        /**
+         * Check a permission
+         * @description To learn how relationship tuples and the check works, head over to [the documentation](https://www.ory.sh/docs/keto/concepts/api-overview).
+         */
+        post: operations["postCheckPermission"]
+    }
+    "/relation-tuples/expand": {
+        /**
+         * Expand a Relationship into permissions.
+         * @description Use this endpoint to expand a relationship tuple into permissions.
+         */
+        get: operations["expandPermissions"]
+    }
+    "/version": {
+        /**
+         * Return Running Software Version.
+         * @description This endpoint returns the version of Ory Keto.
+         *
+         * If the service supports TLS Edge Termination, this endpoint does not require the
+         * `X-Forwarded-Proto` header to be set.
+         *
+         * Be aware that if you are running multiple nodes of this service, the version will never
+         * refer to the cluster state, only to a single instance.
+         */
+        get: operations["getVersion"]
+    }
+}
+
+export type webhooks = Record<string, never>
+
+export interface components {
+    schemas: {
+        DefaultError: unknown
+        ParseError: {
+            end?: components["schemas"]["SourcePosition"]
+            message?: string
+            start?: components["schemas"]["SourcePosition"]
+        }
+        SourcePosition: {
+            /** Format: int64 */
+            Line?: number
+            /** Format: int64 */
+            column?: number
+        }
+        /** Format: uuid4 */
+        UUID: string
+        /** @description Ory Permission Language Document */
+        checkOplSyntaxBody: string
+        /** CheckOPLSyntaxResponse represents the response for an OPL syntax check request. */
+        checkOplSyntaxResult: {
+            /** @description The list of syntax errors */
+            errors?: components["schemas"]["ParseError"][]
+        }
+        /**
+         * Check Permission Result
+         * @description The content of the allowed field is mirrored in the HTTP status code.
+         */
+        checkPermissionResult: {
+            /** @description whether the relation tuple is allowed */
+            allowed: boolean
+        }
+        /** @description Create Relationship Request Body */
+        createRelationshipBody: {
+            /** @description Namespace to query */
+            namespace?: string
+            /** @description Object to query */
+            object?: string
+            /** @description Relation to query */
+            relation?: string
+            /**
+             * @description SubjectID to query
+             *
+             * Either SubjectSet or SubjectID can be provided.
+             */
+            subject_id?: string
+            subject_set?: components["schemas"]["subjectSet"]
+        }
+        /**
+         * JSON API Error Response
+         * @description The standard Ory JSON API error format.
+         */
+        errorGeneric: {
+            error: components["schemas"]["genericError"]
+        }
+        expandedPermissionTree: {
+            /** @description The children of the node, possibly none. */
+            children?: components["schemas"]["expandedPermissionTree"][]
+            tuple?: components["schemas"]["relationship"]
+            /**
+             * @description The type of the node.
+             * union TreeNodeUnion
+             * exclusion TreeNodeExclusion
+             * intersection TreeNodeIntersection
+             * leaf TreeNodeLeaf
+             * tuple_to_subject_set TreeNodeTupleToSubjectSet
+             * computed_subject_set TreeNodeComputedSubjectSet
+             * not TreeNodeNot
+             * unspecified TreeNodeUnspecified
+             * @enum {string}
+             */
+            type:
+                | "union"
+                | "exclusion"
+                | "intersection"
+                | "leaf"
+                | "tuple_to_subject_set"
+                | "computed_subject_set"
+                | "not"
+                | "unspecified"
+        }
+        genericError: {
+            /**
+             * Format: int64
+             * @description The status code
+             * @example 404
+             */
+            code?: number
+            /**
+             * @description Debug information
+             *
+             * This field is often not exposed to protect against leaking
+             * sensitive information.
+             * @example SQL field "foo" is not a bool.
+             */
+            debug?: string
+            /** @description Further error details */
+            details?: {
+                [key: string]: unknown
+            }
+            /**
+             * @description The error ID
+             *
+             * Useful when trying to identify various errors in application logic.
+             */
+            id?: string
+            /**
+             * @description Error message
+             *
+             * The error's message.
+             * @example The resource could not be found
+             */
+            message: string
+            /**
+             * @description A human-readable reason for the error
+             * @example User with ID 1234 does not exist.
+             */
+            reason?: string
+            /**
+             * @description The request ID
+             *
+             * The request ID is often exposed internally in order to trace
+             * errors across service architectures. This is often a UUID.
+             * @example d7ef54b1-ec15-46e6-bccb-524b82c035e6
+             */
+            request?: string
+            /**
+             * @description The status description
+             * @example Not Found
+             */
+            status?: string
+        }
+        healthNotReadyStatus: {
+            /** @description Errors contains a list of errors that caused the not ready status. */
+            errors?: {
+                [key: string]: string
+            }
+        }
+        healthStatus: {
+            /** @description Status always contains "ok". */
+            status?: string
+        }
+        namespace: {
+            /** @description Name of the namespace. */
+            name?: string
+        }
+        /** @description Check Permission using Post Request Body */
+        postCheckPermissionBody: {
+            /** @description Namespace to query */
+            namespace?: string
+            /** @description Object to query */
+            object?: string
+            /** @description Relation to query */
+            relation?: string
+            /**
+             * @description SubjectID to query
+             *
+             * Either SubjectSet or SubjectID can be provided.
+             */
+            subject_id?: string
+            subject_set?: components["schemas"]["subjectSet"]
+        }
+        /** @description Post Check Permission Or Error Body */
+        postCheckPermissionOrErrorBody: {
+            /** @description Namespace to query */
+            namespace?: string
+            /** @description Object to query */
+            object?: string
+            /** @description Relation to query */
+            relation?: string
+            /**
+             * @description SubjectID to query
+             *
+             * Either SubjectSet or SubjectID can be provided.
+             */
+            subject_id?: string
+            subject_set?: components["schemas"]["subjectSet"]
+        }
+        /** @description Relation Query */
+        relationQuery: {
+            /** @description Namespace to query */
+            namespace?: string
+            /** @description Object to query */
+            object?: string
+            /** @description Relation to query */
+            relation?: string
+            /**
+             * @description SubjectID to query
+             *
+             * Either SubjectSet or SubjectID can be provided.
+             */
+            subject_id?: string
+            subject_set?: components["schemas"]["subjectSet"]
+        }
+        /** @description Relationship */
+        relationship: {
+            /** @description Namespace of the Relation Tuple */
+            namespace: string
+            /** @description Object of the Relation Tuple */
+            object: string
+            /** @description Relation of the Relation Tuple */
+            relation: string
+            /**
+             * @description SubjectID of the Relation Tuple
+             *
+             * Either SubjectSet or SubjectID can be provided.
+             */
+            subject_id?: string
+            subject_set?: components["schemas"]["subjectSet"]
+        }
+        /** @description Relationship Namespace List */
+        relationshipNamespaces: {
+            namespaces?: components["schemas"]["namespace"][]
+        }
+        /** @description Payload for patching a relationship */
+        relationshipPatch: {
+            /** @enum {string} */
+            action?: "insert" | "delete"
+            relation_tuple?: components["schemas"]["relationship"]
+        }
+        /** @description Paginated Relationship List */
+        relationships: {
+            /**
+             * @description The opaque token to provide in a subsequent request
+             * to get the next page. It is the empty string iff this is
+             * the last page.
+             */
+            next_page_token?: string
+            relation_tuples?: components["schemas"]["relationship"][]
+        }
+        subjectSet: {
+            /** @description Namespace of the Subject Set */
+            namespace: string
+            /** @description Object of the Subject Set */
+            object: string
+            /** @description Relation of the Subject Set */
+            relation: string
+        }
+        unexpectedError: string
+        version: {
+            /** @description Version is the service's version. */
+            version?: string
+        }
+    }
+    responses: {
+        /** @description Empty responses are sent when, for example, resources are deleted. The HTTP status code for empty responses is typically 204. */
+        emptyResponse: {
+            content: never
+        }
+    }
+    parameters: never
+    requestBodies: never
+    headers: never
+    pathItems: never
+}
+
+export type $defs = Record<string, never>
+
+export type external = Record<string, never>
+
+export interface operations {
     /**
      * Create a Relationship
      * @description Use this endpoint to create a relationship.
      */
-    put: operations["createRelationship"];
+    createRelationship: {
+        requestBody?: {
+            content: {
+                "application/json": components["schemas"]["createRelationshipBody"]
+            }
+        }
+        responses: {
+            /** @description relationship */
+            201: {
+                content: {
+                    "application/json": components["schemas"]["relationship"]
+                }
+            }
+            /** @description errorGeneric */
+            400: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+            /** @description errorGeneric */
+            default: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+        }
+    }
     /**
      * Delete Relationships
      * @description Use this endpoint to delete relationships
      */
-    delete: operations["deleteRelationships"];
+    deleteRelationships: {
+        parameters: {
+            query?: {
+                /** @description Namespace of the Relationship */
+                namespace?: string
+                /** @description Object of the Relationship */
+                object?: string
+                /** @description Relation of the Relationship */
+                relation?: string
+                /** @description SubjectID of the Relationship */
+                subject_id?: string
+                /** @description Namespace of the Subject Set */
+                "subject_set.namespace"?: string
+                /** @description Object of the Subject Set */
+                "subject_set.object"?: string
+                /** @description Relation of the Subject Set */
+                "subject_set.relation"?: string
+            }
+        }
+        responses: {
+            204: components["responses"]["emptyResponse"]
+            /** @description errorGeneric */
+            400: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+            /** @description errorGeneric */
+            default: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+        }
+    }
     /**
      * Patch Multiple Relationships
      * @description Use this endpoint to patch one or more relationships.
      */
-    patch: operations["patchRelationships"];
-  };
-  "/health/alive": {
+    patchRelationships: {
+        requestBody?: {
+            content: {
+                "application/json": components["schemas"]["relationshipPatch"][]
+            }
+        }
+        responses: {
+            204: components["responses"]["emptyResponse"]
+            /** @description errorGeneric */
+            400: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+            /** @description errorGeneric */
+            404: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+            /** @description errorGeneric */
+            default: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+        }
+    }
     /**
      * Check HTTP Server Status
      * @description This endpoint returns a HTTP 200 status code when Ory Keto is accepting incoming
      * HTTP requests. This status does currently not include checks whether the database connection is working.
      *
      * If the service supports TLS Edge Termination, this endpoint does not require the
      * `X-Forwarded-Proto` header to be set.
      *
      * Be aware that if you are running multiple nodes of this service, the health status will never
      * refer to the cluster state, only to a single instance.
      */
-    get: operations["isAlive"];
-  };
-  "/health/ready": {
+    isAlive: {
+        responses: {
+            /** @description Ory Keto is ready to accept connections. */
+            200: {
+                content: {
+                    "application/json": {
+                        /** @description Always "ok". */
+                        status: string
+                    }
+                }
+            }
+            /** @description Unexpected error */
+            default: {
+                content: {
+                    "text/plain": string
+                }
+            }
+        }
+    }
     /**
      * Check HTTP Server and Database Status
      * @description This endpoint returns a HTTP 200 status code when Ory Keto is up running and the environment dependencies (e.g.
      * the database) are responsive as well.
      *
      * If the service supports TLS Edge Termination, this endpoint does not require the
      * `X-Forwarded-Proto` header to be set.
      *
      * Be aware that if you are running multiple nodes of Ory Keto, the health status will never
      * refer to the cluster state, only to a single instance.
      */
-    get: operations["isReady"];
-  };
-  "/namespaces": {
+    isReady: {
+        responses: {
+            /** @description Ory Keto is ready to accept requests. */
+            200: {
+                content: {
+                    "application/json": {
+                        /** @description Always "ok". */
+                        status: string
+                    }
+                }
+            }
+            /** @description Ory Kratos is not yet ready to accept requests. */
+            503: {
+                content: {
+                    "application/json": {
+                        /** @description Errors contains a list of errors that caused the not ready status. */
+                        errors: {
+                            [key: string]: string
+                        }
+                    }
+                }
+            }
+            /** @description Unexpected error */
+            default: {
+                content: {
+                    "text/plain": string
+                }
+            }
+        }
+    }
     /**
      * Query namespaces
      * @description Get all namespaces
      */
-    get: operations["listRelationshipNamespaces"];
-  };
-  "/opl/syntax/check": {
+    listRelationshipNamespaces: {
+        responses: {
+            /** @description relationshipNamespaces */
+            200: {
+                content: {
+                    "application/json": components["schemas"]["relationshipNamespaces"]
+                }
+            }
+            /** @description errorGeneric */
+            default: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+        }
+    }
     /**
      * Check the syntax of an OPL file
      * @description The OPL file is expected in the body of the request.
      */
-    post: operations["checkOplSyntax"];
-  };
-  "/relation-tuples": {
+    checkOplSyntax: {
+        requestBody?: {
+            content: {
+                "text/plain": components["schemas"]["checkOplSyntaxBody"]
+            }
+        }
+        responses: {
+            /** @description checkOplSyntaxResult */
+            200: {
+                content: {
+                    "application/json": components["schemas"]["checkOplSyntaxResult"]
+                }
+            }
+            /** @description errorGeneric */
+            400: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+            /** @description errorGeneric */
+            default: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+        }
+    }
     /**
      * Query relationships
      * @description Get all relationships that match the query. Only the namespace field is required.
      */
-    get: operations["getRelationships"];
-  };
-  "/relation-tuples/check": {
+    getRelationships: {
+        parameters: {
+            query?: {
+                page_token?: string
+                page_size?: number
+                /** @description Namespace of the Relationship */
+                namespace?: string
+                /** @description Object of the Relationship */
+                object?: string
+                /** @description Relation of the Relationship */
+                relation?: string
+                /** @description SubjectID of the Relationship */
+                subject_id?: string
+                /** @description Namespace of the Subject Set */
+                "subject_set.namespace"?: string
+                /** @description Object of the Subject Set */
+                "subject_set.object"?: string
+                /** @description Relation of the Subject Set */
+                "subject_set.relation"?: string
+            }
+        }
+        responses: {
+            /** @description relationships */
+            200: {
+                content: {
+                    "application/json": components["schemas"]["relationships"]
+                }
+            }
+            /** @description errorGeneric */
+            404: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+            /** @description errorGeneric */
+            default: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+        }
+    }
     /**
      * Check a permission
      * @description To learn how relationship tuples and the check works, head over to [the documentation](https://www.ory.sh/docs/keto/concepts/api-overview).
      */
-    get: operations["checkPermissionOrError"];
+    checkPermissionOrError: {
+        parameters: {
+            query?: {
+                /** @description Namespace of the Relationship */
+                namespace?: string
+                /** @description Object of the Relationship */
+                object?: string
+                /** @description Relation of the Relationship */
+                relation?: string
+                /** @description SubjectID of the Relationship */
+                subject_id?: string
+                /** @description Namespace of the Subject Set */
+                "subject_set.namespace"?: string
+                /** @description Object of the Subject Set */
+                "subject_set.object"?: string
+                /** @description Relation of the Subject Set */
+                "subject_set.relation"?: string
+                "max-depth"?: number
+            }
+        }
+        responses: {
+            /** @description checkPermissionResult */
+            200: {
+                content: {
+                    "application/json": components["schemas"]["checkPermissionResult"]
+                }
+            }
+            /** @description errorGeneric */
+            400: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+            /** @description checkPermissionResult */
+            403: {
+                content: {
+                    "application/json": components["schemas"]["checkPermissionResult"]
+                }
+            }
+            /** @description errorGeneric */
+            default: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+        }
+    }
     /**
      * Check a permission
      * @description To learn how relationship tuples and the check works, head over to [the documentation](https://www.ory.sh/docs/keto/concepts/api-overview).
      */
-    post: operations["postCheckPermissionOrError"];
-  };
-  "/relation-tuples/check/openapi": {
+    postCheckPermissionOrError: {
+        parameters: {
+            query?: {
+                "max-depth"?: number
+            }
+        }
+        requestBody?: {
+            content: {
+                "application/json": components["schemas"]["postCheckPermissionOrErrorBody"]
+            }
+        }
+        responses: {
+            /** @description checkPermissionResult */
+            200: {
+                content: {
+                    "application/json": components["schemas"]["checkPermissionResult"]
+                }
+            }
+            /** @description errorGeneric */
+            400: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+            /** @description checkPermissionResult */
+            403: {
+                content: {
+                    "application/json": components["schemas"]["checkPermissionResult"]
+                }
+            }
+            /** @description errorGeneric */
+            default: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+        }
+    }
     /**
      * Check a permission
      * @description To learn how relationship tuples and the check works, head over to [the documentation](https://www.ory.sh/docs/keto/concepts/api-overview).
      */
-    get: operations["checkPermission"];
+    checkPermission: {
+        parameters: {
+            query?: {
+                /** @description Namespace of the Relationship */
+                namespace?: string
+                /** @description Object of the Relationship */
+                object?: string
+                /** @description Relation of the Relationship */
+                relation?: string
+                /** @description SubjectID of the Relationship */
+                subject_id?: string
+                /** @description Namespace of the Subject Set */
+                "subject_set.namespace"?: string
+                /** @description Object of the Subject Set */
+                "subject_set.object"?: string
+                /** @description Relation of the Subject Set */
+                "subject_set.relation"?: string
+                "max-depth"?: number
+            }
+        }
+        responses: {
+            /** @description checkPermissionResult */
+            200: {
+                content: {
+                    "application/json": components["schemas"]["checkPermissionResult"]
+                }
+            }
+            /** @description errorGeneric */
+            400: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+            /** @description errorGeneric */
+            default: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+        }
+    }
     /**
      * Check a permission
      * @description To learn how relationship tuples and the check works, head over to [the documentation](https://www.ory.sh/docs/keto/concepts/api-overview).
      */
-    post: operations["postCheckPermission"];
-  };
-  "/relation-tuples/expand": {
+    postCheckPermission: {
+        parameters: {
+            query?: {
+                "max-depth"?: number
+            }
+        }
+        requestBody?: {
+            content: {
+                "application/json": components["schemas"]["postCheckPermissionBody"]
+            }
+        }
+        responses: {
+            /** @description checkPermissionResult */
+            200: {
+                content: {
+                    "application/json": components["schemas"]["checkPermissionResult"]
+                }
+            }
+            /** @description errorGeneric */
+            400: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+            /** @description errorGeneric */
+            default: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+        }
+    }
     /**
      * Expand a Relationship into permissions.
      * @description Use this endpoint to expand a relationship tuple into permissions.
      */
-    get: operations["expandPermissions"];
-  };
-  "/version": {
+    expandPermissions: {
+        parameters: {
+            query: {
+                /** @description Namespace of the Subject Set */
+                namespace: string
+                /** @description Object of the Subject Set */
+                object: string
+                /** @description Relation of the Subject Set */
+                relation: string
+                "max-depth"?: number
+            }
+        }
+        responses: {
+            /** @description expandedPermissionTree */
+            200: {
+                content: {
+                    "application/json": components["schemas"]["expandedPermissionTree"]
+                }
+            }
+            /** @description errorGeneric */
+            400: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+            /** @description errorGeneric */
+            404: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+            /** @description errorGeneric */
+            default: {
+                content: {
+                    "application/json": components["schemas"]["errorGeneric"]
+                }
+            }
+        }
+    }
     /**
      * Return Running Software Version.
      * @description This endpoint returns the version of Ory Keto.
      *
      * If the service supports TLS Edge Termination, this endpoint does not require the
      * `X-Forwarded-Proto` header to be set.
      *
      * Be aware that if you are running multiple nodes of this service, the version will never
      * refer to the cluster state, only to a single instance.
      */
-    get: operations["getVersion"];
-  };
-}
-
-export type webhooks = Record<string, never>;
-
-export interface components {
-  schemas: {
-    ParseError: {
-      end?: components["schemas"]["SourcePosition"];
-      message?: string;
-      start?: components["schemas"]["SourcePosition"];
-    };
-    SourcePosition: {
-      /** Format: int64 */
-      Line?: number;
-      /** Format: int64 */
-      column?: number;
-    };
-    /** Format: uuid4 */
-    UUID: string;
-    /** @description Ory Permission Language Document */
-    checkOplSyntaxBody: string;
-    /** CheckOPLSyntaxResponse represents the response for an OPL syntax check request. */
-    checkOplSyntaxResult: {
-      /** @description The list of syntax errors */
-      errors?: components["schemas"]["ParseError"][];
-    };
-    /**
-     * Check Permission Result
-     * @description The content of the allowed field is mirrored in the HTTP status code.
-     */
-    checkPermissionResult: {
-      /** @description whether the relation tuple is allowed */
-      allowed: boolean;
-    };
-    /** @description Create Relationship Request Body */
-    createRelationshipBody: {
-      /** @description Namespace to query */
-      namespace?: string;
-      /** @description Object to query */
-      object?: string;
-      /** @description Relation to query */
-      relation?: string;
-      /**
-       * @description SubjectID to query
-       *
-       * Either SubjectSet or SubjectID can be provided.
-       */
-      subject_id?: string;
-      subject_set?: components["schemas"]["subjectSet"];
-    };
-    /**
-     * JSON API Error Response
-     * @description The standard Ory JSON API error format.
-     */
-    errorGeneric: {
-      error: components["schemas"]["genericError"];
-    };
-    expandedPermissionTree: {
-      /** @description The children of the node, possibly none. */
-      children?: components["schemas"]["expandedPermissionTree"][];
-      tuple?: components["schemas"]["relationship"];
-      /**
-       * @description The type of the node.
-       * union TreeNodeUnion
-       * exclusion TreeNodeExclusion
-       * intersection TreeNodeIntersection
-       * leaf TreeNodeLeaf
-       * tuple_to_subject_set TreeNodeTupleToSubjectSet
-       * computed_subject_set TreeNodeComputedSubjectSet
-       * not TreeNodeNot
-       * unspecified TreeNodeUnspecified
-       * @enum {string}
-       */
-      type: "union" | "exclusion" | "intersection" | "leaf" | "tuple_to_subject_set" | "computed_subject_set" | "not" | "unspecified";
-    };
-    genericError: {
-      /**
-       * Format: int64
-       * @description The status code
-       * @example 404
-       */
-      code?: number;
-      /**
-       * @description Debug information
-       *
-       * This field is often not exposed to protect against leaking
-       * sensitive information.
-       * @example SQL field "foo" is not a bool.
-       */
-      debug?: string;
-      /** @description Further error details */
-      details?: {
-        [key: string]: unknown;
-      };
-      /**
-       * @description The error ID
-       *
-       * Useful when trying to identify various errors in application logic.
-       */
-      id?: string;
-      /**
-       * @description Error message
-       *
-       * The error's message.
-       * @example The resource could not be found
-       */
-      message: string;
-      /**
-       * @description A human-readable reason for the error
-       * @example User with ID 1234 does not exist.
-       */
-      reason?: string;
-      /**
-       * @description The request ID
-       *
-       * The request ID is often exposed internally in order to trace
-       * errors across service architectures. This is often a UUID.
-       * @example d7ef54b1-ec15-46e6-bccb-524b82c035e6
-       */
-      request?: string;
-      /**
-       * @description The status description
-       * @example Not Found
-       */
-      status?: string;
-    };
-    healthNotReadyStatus: {
-      /** @description Errors contains a list of errors that caused the not ready status. */
-      errors?: {
-        [key: string]: string;
-      };
-    };
-    healthStatus: {
-      /** @description Status always contains "ok". */
-      status?: string;
-    };
-    namespace: {
-      /** @description Name of the namespace. */
-      name?: string;
-    };
-    /** @description Check Permission using Post Request Body */
-    postCheckPermissionBody: {
-      /** @description Namespace to query */
-      namespace?: string;
-      /** @description Object to query */
-      object?: string;
-      /** @description Relation to query */
-      relation?: string;
-      /**
-       * @description SubjectID to query
-       *
-       * Either SubjectSet or SubjectID can be provided.
-       */
-      subject_id?: string;
-      subject_set?: components["schemas"]["subjectSet"];
-    };
-    /** @description Post Check Permission Or Error Body */
-    postCheckPermissionOrErrorBody: {
-      /** @description Namespace to query */
-      namespace?: string;
-      /** @description Object to query */
-      object?: string;
-      /** @description Relation to query */
-      relation?: string;
-      /**
-       * @description SubjectID to query
-       *
-       * Either SubjectSet or SubjectID can be provided.
-       */
-      subject_id?: string;
-      subject_set?: components["schemas"]["subjectSet"];
-    };
-    /** @description Relation Query */
-    relationQuery: {
-      /** @description Namespace to query */
-      namespace?: string;
-      /** @description Object to query */
-      object?: string;
-      /** @description Relation to query */
-      relation?: string;
-      /**
-       * @description SubjectID to query
-       *
-       * Either SubjectSet or SubjectID can be provided.
-       */
-      subject_id?: string;
-      subject_set?: components["schemas"]["subjectSet"];
-    };
-    /** @description Relationship */
-    relationship: {
-      /** @description Namespace of the Relation Tuple */
-      namespace: string;
-      /** @description Object of the Relation Tuple */
-      object: string;
-      /** @description Relation of the Relation Tuple */
-      relation: string;
-      /**
-       * @description SubjectID of the Relation Tuple
-       *
-       * Either SubjectSet or SubjectID can be provided.
-       */
-      subject_id?: string;
-      subject_set?: components["schemas"]["subjectSet"];
-    };
-    /** @description Relationship Namespace List */
-    relationshipNamespaces: {
-      namespaces?: components["schemas"]["namespace"][];
-    };
-    /** @description Payload for patching a relationship */
-    relationshipPatch: {
-      /** @enum {string} */
-      action?: "insert" | "delete";
-      relation_tuple?: components["schemas"]["relationship"];
-    };
-    /** @description Paginated Relationship List */
-    relationships: {
-      /**
-       * @description The opaque token to provide in a subsequent request
-       * to get the next page. It is the empty string iff this is
-       * the last page.
-       */
-      next_page_token?: string;
-      relation_tuples?: components["schemas"]["relationship"][];
-    };
-    subjectSet: {
-      /** @description Namespace of the Subject Set */
-      namespace: string;
-      /** @description Object of the Subject Set */
-      object: string;
-      /** @description Relation of the Subject Set */
-      relation: string;
-    };
-    version: {
-      /** @description Version is the service's version. */
-      version?: string;
-    };
-  };
-  responses: {
-    /** @description Empty responses are sent when, for example, resources are deleted. The HTTP status code for empty responses is typically 204. */
-    emptyResponse: {
-      content: never;
-    };
-  };
-  parameters: never;
-  requestBodies: never;
-  headers: never;
-  pathItems: never;
-}
-
-export type $defs = Record<string, never>;
-
-export type external = Record<string, never>;
-
-export interface operations {
-
-  /**
-   * Create a Relationship
-   * @description Use this endpoint to create a relationship.
-   */
-  createRelationship: {
-    requestBody?: {
-      content: {
-        "application/json": components["schemas"]["createRelationshipBody"];
-      };
-    };
-    responses: {
-      /** @description relationship */
-      201: {
-        content: {
-          "application/json": components["schemas"]["relationship"];
-        };
-      };
-      /** @description errorGeneric */
-      400: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-      /** @description errorGeneric */
-      default: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-    };
-  };
-  /**
-   * Delete Relationships
-   * @description Use this endpoint to delete relationships
-   */
-  deleteRelationships: {
-    parameters: {
-      query?: {
-        /** @description Namespace of the Relationship */
-        namespace?: string;
-        /** @description Object of the Relationship */
-        object?: string;
-        /** @description Relation of the Relationship */
-        relation?: string;
-        /** @description SubjectID of the Relationship */
-        subject_id?: string;
-        /** @description Namespace of the Subject Set */
-        "subject_set.namespace"?: string;
-        /** @description Object of the Subject Set */
-        "subject_set.object"?: string;
-        /** @description Relation of the Subject Set */
-        "subject_set.relation"?: string;
-      };
-    };
-    responses: {
-      204: components["responses"]["emptyResponse"];
-      /** @description errorGeneric */
-      400: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-      /** @description errorGeneric */
-      default: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-    };
-  };
-  /**
-   * Patch Multiple Relationships
-   * @description Use this endpoint to patch one or more relationships.
-   */
-  patchRelationships: {
-    requestBody?: {
-      content: {
-        "application/json": components["schemas"]["relationshipPatch"][];
-      };
-    };
-    responses: {
-      204: components["responses"]["emptyResponse"];
-      /** @description errorGeneric */
-      400: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-      /** @description errorGeneric */
-      404: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-      /** @description errorGeneric */
-      default: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-    };
-  };
-  /**
-   * Check HTTP Server Status
-   * @description This endpoint returns a HTTP 200 status code when Ory Keto is accepting incoming
-   * HTTP requests. This status does currently not include checks whether the database connection is working.
-   *
-   * If the service supports TLS Edge Termination, this endpoint does not require the
-   * `X-Forwarded-Proto` header to be set.
-   *
-   * Be aware that if you are running multiple nodes of this service, the health status will never
-   * refer to the cluster state, only to a single instance.
-   */
-  isAlive: {
-    responses: {
-      /** @description Ory Keto is ready to accept connections. */
-      200: {
-        content: {
-          "application/json": {
-            /** @description Always "ok". */
-            status: string;
-          };
-        };
-      };
-      /** @description genericError */
-      500: {
-        content: {
-          "application/json": components["schemas"]["genericError"];
-        };
-      };
-    };
-  };
-  /**
-   * Check HTTP Server and Database Status
-   * @description This endpoint returns a HTTP 200 status code when Ory Keto is up running and the environment dependencies (e.g.
-   * the database) are responsive as well.
-   *
-   * If the service supports TLS Edge Termination, this endpoint does not require the
-   * `X-Forwarded-Proto` header to be set.
-   *
-   * Be aware that if you are running multiple nodes of Ory Keto, the health status will never
-   * refer to the cluster state, only to a single instance.
-   */
-  isReady: {
-    responses: {
-      /** @description Ory Keto is ready to accept requests. */
-      200: {
-        content: {
-          "application/json": {
-            /** @description Always "ok". */
-            status: string;
-          };
-        };
-      };
-      /** @description Ory Kratos is not yet ready to accept requests. */
-      503: {
-        content: {
-          "application/json": {
-            /** @description Errors contains a list of errors that caused the not ready status. */
-            errors: {
-              [key: string]: string;
-            };
-          };
-        };
-      };
-    };
-  };
-  /**
-   * Query namespaces
-   * @description Get all namespaces
-   */
-  listRelationshipNamespaces: {
-    responses: {
-      /** @description relationshipNamespaces */
-      200: {
-        content: {
-          "application/json": components["schemas"]["relationshipNamespaces"];
-        };
-      };
-      /** @description errorGeneric */
-      default: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-    };
-  };
-  /**
-   * Check the syntax of an OPL file
-   * @description The OPL file is expected in the body of the request.
-   */
-  checkOplSyntax: {
-    requestBody?: {
-      content: {
-        "text/plain": components["schemas"]["checkOplSyntaxBody"];
-      };
-    };
-    responses: {
-      /** @description checkOplSyntaxResult */
-      200: {
-        content: {
-          "application/json": components["schemas"]["checkOplSyntaxResult"];
-        };
-      };
-      /** @description errorGeneric */
-      400: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-      /** @description errorGeneric */
-      default: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-    };
-  };
-  /**
-   * Query relationships
-   * @description Get all relationships that match the query. Only the namespace field is required.
-   */
-  getRelationships: {
-    parameters: {
-      query?: {
-        page_token?: string;
-        page_size?: number;
-        /** @description Namespace of the Relationship */
-        namespace?: string;
-        /** @description Object of the Relationship */
-        object?: string;
-        /** @description Relation of the Relationship */
-        relation?: string;
-        /** @description SubjectID of the Relationship */
-        subject_id?: string;
-        /** @description Namespace of the Subject Set */
-        "subject_set.namespace"?: string;
-        /** @description Object of the Subject Set */
-        "subject_set.object"?: string;
-        /** @description Relation of the Subject Set */
-        "subject_set.relation"?: string;
-      };
-    };
-    responses: {
-      /** @description relationships */
-      200: {
-        content: {
-          "application/json": components["schemas"]["relationships"];
-        };
-      };
-      /** @description errorGeneric */
-      404: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-      /** @description errorGeneric */
-      default: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-    };
-  };
-  /**
-   * Check a permission
-   * @description To learn how relationship tuples and the check works, head over to [the documentation](https://www.ory.sh/docs/keto/concepts/api-overview).
-   */
-  checkPermissionOrError: {
-    parameters: {
-      query?: {
-        /** @description Namespace of the Relationship */
-        namespace?: string;
-        /** @description Object of the Relationship */
-        object?: string;
-        /** @description Relation of the Relationship */
-        relation?: string;
-        /** @description SubjectID of the Relationship */
-        subject_id?: string;
-        /** @description Namespace of the Subject Set */
-        "subject_set.namespace"?: string;
-        /** @description Object of the Subject Set */
-        "subject_set.object"?: string;
-        /** @description Relation of the Subject Set */
-        "subject_set.relation"?: string;
-        "max-depth"?: number;
-      };
-    };
-    responses: {
-      /** @description checkPermissionResult */
-      200: {
-        content: {
-          "application/json": components["schemas"]["checkPermissionResult"];
-        };
-      };
-      /** @description errorGeneric */
-      400: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-      /** @description checkPermissionResult */
-      403: {
-        content: {
-          "application/json": components["schemas"]["checkPermissionResult"];
-        };
-      };
-      /** @description errorGeneric */
-      default: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-    };
-  };
-  /**
-   * Check a permission
-   * @description To learn how relationship tuples and the check works, head over to [the documentation](https://www.ory.sh/docs/keto/concepts/api-overview).
-   */
-  postCheckPermissionOrError: {
-    parameters: {
-      query?: {
-        /** @description nolint:deadcode,unused */
-        "max-depth"?: number;
-      };
-    };
-    requestBody?: {
-      content: {
-        "application/json": components["schemas"]["postCheckPermissionOrErrorBody"];
-      };
-    };
-    responses: {
-      /** @description checkPermissionResult */
-      200: {
-        content: {
-          "application/json": components["schemas"]["checkPermissionResult"];
-        };
-      };
-      /** @description errorGeneric */
-      400: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-      /** @description checkPermissionResult */
-      403: {
-        content: {
-          "application/json": components["schemas"]["checkPermissionResult"];
-        };
-      };
-      /** @description errorGeneric */
-      default: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-    };
-  };
-  /**
-   * Check a permission
-   * @description To learn how relationship tuples and the check works, head over to [the documentation](https://www.ory.sh/docs/keto/concepts/api-overview).
-   */
-  checkPermission: {
-    parameters: {
-      query?: {
-        /** @description Namespace of the Relationship */
-        namespace?: string;
-        /** @description Object of the Relationship */
-        object?: string;
-        /** @description Relation of the Relationship */
-        relation?: string;
-        /** @description SubjectID of the Relationship */
-        subject_id?: string;
-        /** @description Namespace of the Subject Set */
-        "subject_set.namespace"?: string;
-        /** @description Object of the Subject Set */
-        "subject_set.object"?: string;
-        /** @description Relation of the Subject Set */
-        "subject_set.relation"?: string;
-        "max-depth"?: number;
-      };
-    };
-    responses: {
-      /** @description checkPermissionResult */
-      200: {
-        content: {
-          "application/json": components["schemas"]["checkPermissionResult"];
-        };
-      };
-      /** @description errorGeneric */
-      400: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-      /** @description errorGeneric */
-      default: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-    };
-  };
-  /**
-   * Check a permission
-   * @description To learn how relationship tuples and the check works, head over to [the documentation](https://www.ory.sh/docs/keto/concepts/api-overview).
-   */
-  postCheckPermission: {
-    parameters: {
-      query?: {
-        "max-depth"?: number;
-      };
-    };
-    requestBody?: {
-      content: {
-        "application/json": components["schemas"]["postCheckPermissionBody"];
-      };
-    };
-    responses: {
-      /** @description checkPermissionResult */
-      200: {
-        content: {
-          "application/json": components["schemas"]["checkPermissionResult"];
-        };
-      };
-      /** @description errorGeneric */
-      400: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-      /** @description errorGeneric */
-      default: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-    };
-  };
-  /**
-   * Expand a Relationship into permissions.
-   * @description Use this endpoint to expand a relationship tuple into permissions.
-   */
-  expandPermissions: {
-    parameters: {
-      query: {
-        /** @description Namespace of the Subject Set */
-        namespace: string;
-        /** @description Object of the Subject Set */
-        object: string;
-        /** @description Relation of the Subject Set */
-        relation: string;
-        "max-depth"?: number;
-      };
-    };
-    responses: {
-      /** @description expandedPermissionTree */
-      200: {
-        content: {
-          "application/json": components["schemas"]["expandedPermissionTree"];
-        };
-      };
-      /** @description errorGeneric */
-      400: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-      /** @description errorGeneric */
-      404: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-      /** @description errorGeneric */
-      default: {
-        content: {
-          "application/json": components["schemas"]["errorGeneric"];
-        };
-      };
-    };
-  };
-  /**
-   * Return Running Software Version.
-   * @description This endpoint returns the version of Ory Keto.
-   *
-   * If the service supports TLS Edge Termination, this endpoint does not require the
-   * `X-Forwarded-Proto` header to be set.
-   *
-   * Be aware that if you are running multiple nodes of this service, the version will never
-   * refer to the cluster state, only to a single instance.
-   */
-  getVersion: {
-    responses: {
-      /** @description Returns the Ory Keto version. */
-      200: {
-        content: {
-          "application/json": {
-            /** @description The version of Ory Keto. */
-            version: string;
-          };
-        };
-      };
-    };
-  };
+    getVersion: {
+        responses: {
+            /** @description Returns the Ory Keto version. */
+            200: {
+                content: {
+                    "application/json": {
+                        /** @description The version of Ory Keto. */
+                        version: string
+                    }
+                }
+            }
+        }
+    }
 }
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/lib/types/kratos.d.ts` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/types/kratos.d.ts`

 * *Files 2% similar despite different names*

```diff
@@ -204,21 +204,15 @@
          * More information can be found at [Ory Kratos User User Facing Error Documentation](https://www.ory.sh/docs/kratos/self-service/flows/user-facing-errors).
          */
         get: operations["getFlowError"]
     }
     "/self-service/login": {
         /**
          * Submit a Login Flow
-         * @description :::info
-         *
-         * This endpoint is EXPERIMENTAL and subject to potential breaking changes in the future.
-         *
-         * :::
-         *
-         * Use this endpoint to complete a login flow. This endpoint
+         * @description Use this endpoint to complete a login flow. This endpoint
          * behaves differently for API and browser flows.
          *
          * API flows expect `application/json` to be sent in the body and responds with
          * HTTP 200 and a application/json body with the session token on success;
          * HTTP 410 if the original flow expired with the appropriate error messages set and optionally a `use_flow_id` parameter in the body;
          * HTTP 400 on form validation errors.
          *
@@ -375,16 +369,16 @@
          *
          * When calling this endpoint from a backend, please ensure to properly forward the HTTP cookies.
          */
         get: operations["createBrowserLogoutFlow"]
     }
     "/self-service/recovery": {
         /**
-         * Complete Recovery Flow
-         * @description Use this endpoint to complete a recovery flow. This endpoint
+         * Update Recovery Flow
+         * @description Use this endpoint to update a recovery flow. This endpoint
          * behaves differently for API and browser flows and has several states:
          *
          * `choose_method` expects `flow` (in the URL query) and `email` (in the body) to be sent
          * and works with API- and Browser-initiated flows.
          * For API clients and Browser clients with HTTP Header `Accept: application/json` it either returns a HTTP 200 OK when the form is valid and HTTP 400 OK when the form is invalid.
          * and a HTTP 303 See Other redirect with a fresh recovery flow if the flow was otherwise invalid (e.g. expired).
          * For Browser clients without HTTP Header `Accept` or with `Accept: text/*` it returns a HTTP 303 See Other redirect to the Recovery UI URL with the Recovery Flow ID appended.
@@ -402,15 +396,15 @@
     "/self-service/recovery/api": {
         /**
          * Create Recovery Flow for Native Apps
          * @description This endpoint initiates a recovery flow for API clients such as mobile devices, smart TVs, and so on.
          *
          * If a valid provided session cookie or session token is provided, a 400 Bad Request error.
          *
-         * To fetch an existing recovery flow call `/self-service/recovery/flows?flow=<flow_id>`.
+         * On an existing recovery flow, use the `getRecoveryFlow` API endpoint.
          *
          * You MUST NOT use this endpoint in client-side (Single Page Apps, ReactJS, AngularJS) nor server-side (Java Server
          * Pages, NodeJS, PHP, Golang, ...) browser applications. Using this endpoint in these applications will make
          * you vulnerable to a variety of CSRF attacks.
          *
          * This endpoint MUST ONLY be used in scenarios such as native mobile apps (React Native, Objective C, Swift, Java, ...).
          *
@@ -519,20 +513,14 @@
     }
     "/self-service/registration/browser": {
         /**
          * Create Registration Flow for Browsers
          * @description This endpoint initializes a browser-based user registration flow. This endpoint will set the appropriate
          * cookies and anti-CSRF measures required for browser-based flows.
          *
-         * :::info
-         *
-         * This endpoint is EXPERIMENTAL and subject to potential breaking changes in the future.
-         *
-         * :::
-         *
          * If this endpoint is opened as a link in the browser, it will be redirected to
          * `selfservice.flows.registration.ui_url` with the flow ID set as the query parameter `?flow=`. If a valid user session
          * exists already, the browser will be redirected to `urls.default_redirect_url`.
          *
          * If this endpoint is called via an AJAX request, the response contains the flow without a redirect. In the
          * case of an error, the `error.id` of the JSON response body can be one of:
          *
@@ -831,14 +819,24 @@
          * pseudo-code example
          * ...
          * const session = await client.toSession("the-session-token")
          *
          * console.log(session)
          * ```
          *
+         * When using a token template, the token is included in the `tokenized` field of the session.
+         *
+         * ```js
+         * pseudo-code example
+         * ...
+         * const session = await client.toSession("the-session-token", { tokenize_as: "example-jwt-template" })
+         *
+         * console.log(session.tokenized) // The JWT
+         * ```
+         *
          * Depending on your configuration this endpoint might return a 403 status code if the session has a lower Authenticator
          * Assurance Level (AAL) than is possible for the identity. This can happen if the identity has password + webauthn
          * credentials (which would result in AAL2) but the session has only AAL1. If this error occurs, ask the user
          * to sign in with the second factor or change the configuration.
          *
          * This endpoint is useful for:
          *
@@ -905,29 +903,31 @@
         NullString: string | null
         /** Format: date-time */
         NullTime: string | null
         /** Format: uuid4 */
         NullUUID: string | null
         /** OAuth2Client OAuth 2.0 Clients are used to perform OAuth 2.0 and OpenID Connect flows. Usually, OAuth 2.0 clients are generated for applications which want to consume your OAuth 2.0 or OpenID Connect capabilities. */
         OAuth2Client: {
+            /** @description OAuth 2.0 Access Token Strategy  AccessTokenStrategy is the strategy used to generate access tokens. Valid options are `jwt` and `opaque`. `jwt` is a bad idea, see https://www.ory.sh/docs/hydra/advanced#json-web-tokens Setting the stragegy here overrides the global setting in `strategies.access_token`. */
+            access_token_strategy?: string
             allowed_cors_origins?: string[]
             audience?: string[]
             /** @description Specify a time duration in milliseconds, seconds, minutes, hours. */
             authorization_code_grant_access_token_lifespan?: string
             /** @description Specify a time duration in milliseconds, seconds, minutes, hours. */
             authorization_code_grant_id_token_lifespan?: string
             /** @description Specify a time duration in milliseconds, seconds, minutes, hours. */
             authorization_code_grant_refresh_token_lifespan?: string
             /** @description OpenID Connect Back-Channel Logout Session Required  Boolean value specifying whether the RP requires that a sid (session ID) Claim be included in the Logout Token to identify the RP session with the OP when the backchannel_logout_uri is used. If omitted, the default value is false. */
             backchannel_logout_session_required?: boolean
             /** @description OpenID Connect Back-Channel Logout URI  RP URL that will cause the RP to log itself out when sent a Logout Token by the OP. */
             backchannel_logout_uri?: string
             /** @description Specify a time duration in milliseconds, seconds, minutes, hours. */
             client_credentials_grant_access_token_lifespan?: string
-            /** @description OAuth 2.0 Client ID  The ID is autogenerated and immutable. */
+            /** @description OAuth 2.0 Client ID  The ID is immutable. If no ID is provided, a UUID4 will be generated. */
             client_id?: string
             /** @description OAuth 2.0 Client Name  The human-readable name of the client to be presented to the end-user during authorization. */
             client_name?: string
             /** @description OAuth 2.0 Client Secret  The secret will be included in the create request as cleartext, and then never again. The secret is kept in hashed format and is not recoverable once lost. */
             client_secret?: string
             /**
              * Format: int64
@@ -980,17 +980,21 @@
             request_object_signing_alg?: string
             request_uris?: string[]
             response_types?: string[]
             /** @description OAuth 2.0 Client Scope  Scope is a string containing a space-separated list of scope values (as described in Section 3.3 of OAuth 2.0 [RFC6749]) that the client can use when requesting access tokens. */
             scope?: string
             /** @description OpenID Connect Sector Identifier URI  URL using the https scheme to be used in calculating Pseudonymous Identifiers by the OP. The URL references a file with a single JSON array of redirect_uri values. */
             sector_identifier_uri?: string
+            /** @description SkipConsent skips the consent screen for this client. This field can only be set from the admin API. */
+            skip_consent?: boolean
+            /** @description SkipLogoutConsent skips the logout consent screen for this client. This field can only be set from the admin API. */
+            skip_logout_consent?: boolean
             /** @description OpenID Connect Subject Type  The `subject_types_supported` Discovery parameter contains a list of the supported subject_type values for this server. Valid types include `pairwise` and `public`. */
             subject_type?: string
-            /** @description OAuth 2.0 Token Endpoint Authentication Method  Requested Client Authentication method for the Token Endpoint. The options are:  `client_secret_post`: (default) Send `client_id` and `client_secret` as `application/x-www-form-urlencoded` in the HTTP body. `client_secret_basic`: Send `client_id` and `client_secret` as `application/x-www-form-urlencoded` encoded in the HTTP Authorization header. `private_key_jwt`: Use JSON Web Tokens to authenticate the client. `none`: Used for public clients (native apps, mobile apps) which can not have secrets. */
+            /** @description OAuth 2.0 Token Endpoint Authentication Method  Requested Client Authentication method for the Token Endpoint. The options are:  `client_secret_basic`: (default) Send `client_id` and `client_secret` as `application/x-www-form-urlencoded` encoded in the HTTP Authorization header. `client_secret_post`: Send `client_id` and `client_secret` as `application/x-www-form-urlencoded` in the HTTP body. `private_key_jwt`: Use JSON Web Tokens to authenticate the client. `none`: Used for public clients (native apps, mobile apps) which can not have secrets. */
             token_endpoint_auth_method?: string
             /** @description OAuth 2.0 Token Endpoint Signing Algorithm  Requested Client Authentication signing algorithm for the Token Endpoint. */
             token_endpoint_auth_signing_alg?: string
             /** @description OAuth 2.0 Client Terms of Service URI  A URL string pointing to a human-readable terms of service document for the client that describes a contractual relationship between the end-user and the client that the end-user accepts when authorizing the client. */
             tos_uri?: string
             /**
              * Format: date-time
@@ -1011,14 +1015,15 @@
                 [key: string]: unknown
             }
             /** @description LoginHint hints about the login identifier the End-User might use to log in (if necessary). This hint can be used by an RP if it first asks the End-User for their e-mail address (or other identifier) and then wants to pass that value as a hint to the discovered authorization service. This value MAY also be a phone number in the format specified for the phone_number Claim. The use of this parameter is optional. */
             login_hint?: string
             /** @description UILocales is the End-User'id preferred languages and scripts for the user interface, represented as a space-separated list of BCP47 [RFC5646] language tag values, ordered by preference. For instance, the value \"fr-CA fr en\" represents a preference for French as spoken in Canada, then French (without a region designation), followed by English (without a region designation). An error SHOULD NOT result if some or all of the requested locales are not supported by the OpenID Provider. */
             ui_locales?: string[]
         }
+        OAuth2LoginChallengeParams: Record<string, never>
         /** @description OAuth2LoginRequest struct for OAuth2LoginRequest */
         OAuth2LoginRequest: {
             /** @description ID is the identifier (\"login challenge\") of the login request. It is used to identify the session. */
             challenge?: string
             client?: components["schemas"]["OAuth2Client"]
             oidc_context?: components["schemas"]["OAuth2ConsentRequestOpenIDConnectContext"]
             /** @description RequestURL is the original OAuth 2.0 Authorization URL requested by the OAuth 2.0 client. It is the URL which initiates the OAuth 2.0 Authorization Code or OAuth 2.0 Implicit flow. This URL is typically not needed, but might come in handy if you want to deal with additional request parameters. */
@@ -1051,38 +1056,100 @@
          */
         authenticatorAssuranceLevel: "aal0" | "aal1" | "aal2" | "aal3"
         /** @description Patch identities response */
         batchPatchIdentitiesResponse: {
             /** @description The patch responses for the individual identities. */
             identities?: components["schemas"]["identityPatchResponse"][]
         }
+        /** @description Control API consistency guarantees */
+        consistencyRequestParameters: {
+            /**
+             * @description Read Consistency Level (preview)
+             *
+             * The read consistency level determines the consistency guarantee for reads:
+             *
+             * strong (slow): The read is guaranteed to return the most recent data committed at the start of the read.
+             * eventual (very fast): The result will return data that is about 4.8 seconds old.
+             *
+             * The default consistency guarantee can be changed in the Ory Network Console or using the Ory CLI with
+             * `ory patch project --replace '/previews/default_read_consistency_level="strong"'`.
+             *
+             * Setting the default consistency level to `eventual` may cause regressions in the future as we add consistency
+             * controls to more APIs. Currently, the following APIs will be affected by this setting:
+             *
+             * `GET /admin/identities`
+             *
+             * This feature is in preview and only available in Ory Network.
+             *  ConsistencyLevelUnset  ConsistencyLevelUnset is the unset / default consistency level.
+             * strong ConsistencyLevelStrong  ConsistencyLevelStrong is the strong consistency level.
+             * eventual ConsistencyLevelEventual  ConsistencyLevelEventual is the eventual consistency level using follower read timestamps.
+             * @enum {string}
+             */
+            consistency?: "" | "strong" | "eventual"
+        }
         continueWith:
             | components["schemas"]["continueWithVerificationUi"]
             | components["schemas"]["continueWithSetOrySessionToken"]
+            | components["schemas"]["continueWithSettingsUi"]
+            | components["schemas"]["continueWithRecoveryUi"]
+        /** @description Indicates, that the UI flow could be continued by showing a recovery ui */
+        continueWithRecoveryUi: {
+            /**
+             * @description Action will always be `show_recovery_ui`
+             * show_recovery_ui ContinueWithActionShowRecoveryUIString
+             * @enum {string}
+             */
+            action: "show_recovery_ui"
+            flow: components["schemas"]["continueWithRecoveryUiFlow"]
+        }
+        continueWithRecoveryUiFlow: {
+            /**
+             * Format: uuid
+             * @description The ID of the recovery flow
+             */
+            id: string
+            /** @description The URL of the recovery flow */
+            url?: string
+        }
         /** @description Indicates that a session was issued, and the application should use this token for authenticated requests */
         continueWithSetOrySessionToken: {
             /**
              * @description Action will always be `set_ory_session_token`
-             * set_ory_session_token ContinueWithActionSetOrySessionToken
-             * show_verification_ui ContinueWithActionShowVerificationUI
+             * set_ory_session_token ContinueWithActionSetOrySessionTokenString
              * @enum {string}
              */
-            action: "set_ory_session_token" | "show_verification_ui"
+            action: "set_ory_session_token"
             /** @description Token is the token of the session */
             ory_session_token: string
         }
+        /** @description Indicates, that the UI flow could be continued by showing a settings ui */
+        continueWithSettingsUi: {
+            /**
+             * @description Action will always be `show_settings_ui`
+             * show_settings_ui ContinueWithActionShowSettingsUIString
+             * @enum {string}
+             */
+            action: "show_settings_ui"
+            flow: components["schemas"]["continueWithSettingsUiFlow"]
+        }
+        continueWithSettingsUiFlow: {
+            /**
+             * Format: uuid
+             * @description The ID of the settings flow
+             */
+            id: string
+        }
         /** @description Indicates, that the UI flow could be continued by showing a verification ui */
         continueWithVerificationUi: {
             /**
              * @description Action will always be `show_verification_ui`
-             * set_ory_session_token ContinueWithActionSetOrySessionToken
-             * show_verification_ui ContinueWithActionShowVerificationUI
+             * show_verification_ui ContinueWithActionShowVerificationUIString
              * @enum {string}
              */
-            action: "set_ory_session_token" | "show_verification_ui"
+            action: "show_verification_ui"
             flow: components["schemas"]["continueWithVerificationUiFlow"]
         }
         continueWithVerificationUiFlow: {
             /**
              * Format: uuid
              * @description The ID of the verification flow
              */
@@ -1119,15 +1186,21 @@
              * Use this structure to import recovery addresses for an identity. Please keep in mind
              * that the address needs to be represented in the Identity Schema or this field will be overwritten
              * on the next identity update.
              */
             recovery_addresses?: components["schemas"]["recoveryIdentityAddress"][]
             /** @description SchemaID is the ID of the JSON Schema to be used for validating the identity's traits. */
             schema_id: string
-            state?: components["schemas"]["identityState"]
+            /**
+             * @description State is the identity's state.
+             * active StateActive
+             * inactive StateInactive
+             * @enum {string}
+             */
+            state?: "active" | "inactive"
             /**
              * @description Traits represent an identity's traits. The identity is able to create, modify, and delete traits
              * in a self-service manner. The input will always be validated against the JSON Schema defined
              * in `schema_url`.
              */
             traits: Record<string, never>
             /**
@@ -1306,25 +1379,34 @@
              *
              * The Identity ID can not be changed and can not be chosen. This ensures future
              * compatibility and optimization for distributed stores such as CockroachDB.
              */
             id: string
             metadata_admin?: components["schemas"]["nullJsonRawMessage"]
             metadata_public?: components["schemas"]["nullJsonRawMessage"]
+            organization_id?: components["schemas"]["NullUUID"]
             /** @description RecoveryAddresses contains all the addresses that can be used to recover an identity. */
             recovery_addresses?: components["schemas"]["recoveryIdentityAddress"][]
             /** @description SchemaID is the ID of the JSON Schema to be used for validating the identity's traits. */
             schema_id: string
             /**
              * @description SchemaURL is the URL of the endpoint where the identity's traits schema can be fetched from.
              *
              * format: url
              */
             schema_url: string
-            state?: components["schemas"]["identityState"]
+            /**
+             * @description State is the identity's state.
+             *
+             * This value has currently no effect.
+             * active StateActive
+             * inactive StateInactive
+             * @enum {string}
+             */
+            state?: "active" | "inactive"
             state_changed_at?: components["schemas"]["nullTime"]
             traits: components["schemas"]["identityTraits"]
             /**
              * Format: date-time
              * @description UpdatedAt is a helper struct field for gobuffalo.pop.
              */
             updated_at?: string
@@ -1337,49 +1419,70 @@
             /**
              * Format: date-time
              * @description CreatedAt is a helper struct field for gobuffalo.pop.
              */
             created_at?: string
             /** @description Identifiers represents a list of unique identifiers this credential type matches. */
             identifiers?: string[]
-            type?: components["schemas"]["identityCredentialsType"]
+            /**
+             * @description Type discriminates between different types of credentials.
+             * password CredentialsTypePassword
+             * oidc CredentialsTypeOIDC
+             * totp CredentialsTypeTOTP
+             * lookup_secret CredentialsTypeLookup
+             * webauthn CredentialsTypeWebAuthn
+             * code CredentialsTypeCodeAuth
+             * link_recovery CredentialsTypeRecoveryLink  CredentialsTypeRecoveryLink is a special credential type linked to the link strategy (recovery flow).  It is not used within the credentials object itself.
+             * code_recovery CredentialsTypeRecoveryCode
+             * @enum {string}
+             */
+            type?:
+                | "password"
+                | "oidc"
+                | "totp"
+                | "lookup_secret"
+                | "webauthn"
+                | "code"
+                | "link_recovery"
+                | "code_recovery"
             /**
              * Format: date-time
              * @description UpdatedAt is a helper struct field for gobuffalo.pop.
              */
             updated_at?: string
             /**
              * Format: int64
              * @description Version refers to the version of the credential. Useful when changing the config schema.
              */
             version?: number
         }
+        /** @description CredentialsCode represents a one time login/registration code */
+        identityCredentialsCode: {
+            /** @description The type of the address for this code */
+            address_type?: string
+            used_at?: components["schemas"]["NullTime"]
+        }
         /** CredentialsOIDC is contains the configuration for credentials of the type oidc. */
         identityCredentialsOidc: {
             providers?: components["schemas"]["identityCredentialsOidcProvider"][]
         }
         /** CredentialsOIDCProvider is contains a specific OpenID COnnect credential for a particular connection (e.g. Google). */
         identityCredentialsOidcProvider: {
             initial_access_token?: string
             initial_id_token?: string
             initial_refresh_token?: string
+            organization?: string
             provider?: string
             subject?: string
         }
         /** CredentialsPassword is contains the configuration for credentials of the type password. */
         identityCredentialsPassword: {
             /** @description HashedPassword is a hash-representation of the password. */
             hashed_password?: string
         }
-        /**
-         * CredentialsType  represents several different credential types, like password credentials, passwordless credentials,
-         * @description and so on.
-         * @enum {string}
-         */
-        identityCredentialsType: "password" | "totp" | "oidc" | "webauthn" | "lookup_secret"
         /** @description Payload for patching an identity */
         identityPatch: {
             create?: components["schemas"]["createIdentityBody"]
             /**
              * Format: uuid
              * @description The ID of this patch.
              *
@@ -1416,29 +1519,21 @@
             id?: string
             /** @description The actual Identity JSON Schema */
             schema?: Record<string, never>
         }
         /** @description List of Identity JSON Schemas */
         identitySchemas: components["schemas"]["identitySchemaContainer"][]
         /**
-         * An Identity's State
-         * @description The state can either be `active` or `inactive`.
-         * @enum {string}
-         */
-        identityState: "active" | "inactive"
-        /**
          * @description Traits represent an identity's traits. The identity is able to create, modify, and delete traits
          * in a self-service manner. The input will always be validated against the JSON Schema defined
          * in `schema_url`.
          */
         identityTraits: unknown
         /** @description VerifiableAddressStatus must not exceed 16 characters as that is the limitation in the SQL Schema */
         identityVerifiableAddressStatus: string
-        /** @description VerifiableAddressType must not exceed 16 characters as that is the limitation in the SQL Schema */
-        identityVerifiableAddressType: string
         /** @description Create Identity and Import Credentials */
         identityWithCredentials: {
             oidc?: components["schemas"]["identityWithCredentialsOidc"]
             password?: components["schemas"]["identityWithCredentialsPassword"]
         }
         /** @description Create Identity and Import Social Sign In Credentials */
         identityWithCredentialsOidc: {
@@ -1458,15 +1553,15 @@
         }
         /** @description Create Identity and Import Password Credentials */
         identityWithCredentialsPassword: {
             config?: components["schemas"]["identityWithCredentialsPasswordConfig"]
         }
         /** @description Create Identity and Import Password Credentials Configuration */
         identityWithCredentialsPasswordConfig: {
-            /** @description The hashed password in [PHC format]( https://www.ory.sh/docs/kratos/concepts/credentials/username-email-password#hashed-password-format) */
+            /** @description The hashed password in [PHC format](https://www.ory.sh/docs/kratos/manage-identities/import-user-accounts-identities#hashed-passwords) */
             hashed_password?: string
             /** @description The password in plain text if no hash is available. */
             password?: string
         }
         /** @description A JSONPatch document as defined by RFC 6902 */
         jsonPatch: {
             /**
@@ -1502,15 +1597,37 @@
          * Login Flow
          * @description This object represents a login flow. A login flow is initiated at the "Initiate Login API / Browser Flow"
          * endpoint by a client.
          *
          * Once a login flow is completed successfully, a session cookie or session token will be issued.
          */
         loginFlow: {
-            active?: components["schemas"]["identityCredentialsType"]
+            /**
+             * @description The active login method
+             *
+             * If set contains the login method used. If the flow is new, it is unset.
+             * password CredentialsTypePassword
+             * oidc CredentialsTypeOIDC
+             * totp CredentialsTypeTOTP
+             * lookup_secret CredentialsTypeLookup
+             * webauthn CredentialsTypeWebAuthn
+             * code CredentialsTypeCodeAuth
+             * link_recovery CredentialsTypeRecoveryLink  CredentialsTypeRecoveryLink is a special credential type linked to the link strategy (recovery flow).  It is not used within the credentials object itself.
+             * code_recovery CredentialsTypeRecoveryCode
+             * @enum {string}
+             */
+            active?:
+                | "password"
+                | "oidc"
+                | "totp"
+                | "lookup_secret"
+                | "webauthn"
+                | "code"
+                | "link_recovery"
+                | "code_recovery"
             /**
              * Format: date-time
              * @description CreatedAt is a helper struct field for gobuffalo.pop.
              */
             created_at?: string
             /**
              * Format: date-time
@@ -1533,14 +1650,15 @@
              * @description Ory OAuth 2.0 Login Challenge.
              *
              * This value is set using the `login_challenge` query parameter of the registration and login endpoints.
              * If set will cooperate with Ory OAuth2 and OpenID to act as an OAuth2 server / OpenID Provider.
              */
             oauth2_login_challenge?: string
             oauth2_login_request?: components["schemas"]["OAuth2LoginRequest"]
+            organization_id?: components["schemas"]["NullUUID"]
             /** @description Refresh stores whether this login flow should enforce re-authentication. */
             refresh?: boolean
             /**
              * @description RequestURL is the initial URL that was requested from Ory Kratos. It can be used
              * to forward information contained in the URL's path or query for example.
              */
             request_url: string
@@ -1549,35 +1667,54 @@
             return_to?: string
             /**
              * @description SessionTokenExchangeCode holds the secret code that the client can use to retrieve a session token after the login flow has been completed.
              * This is only set if the client has requested a session token exchange code, and if the flow is of type "api",
              * and only on creating the login flow.
              */
             session_token_exchange_code?: string
+            /**
+             * @description State represents the state of this request:
+             *
+             * choose_method: ask the user to choose a method to sign in with
+             * sent_email: the email has been sent to the user
+             * passed_challenge: the request was successful and the login challenge was passed.
+             */
+            state: unknown
             type: components["schemas"]["selfServiceFlowType"]
             ui: components["schemas"]["uiContainer"]
             /**
              * Format: date-time
              * @description UpdatedAt is a helper struct field for gobuffalo.pop.
              */
             updated_at?: string
         }
+        /**
+         * Login Flow State
+         * @description The state represents the state of the login flow.
+         *
+         * choose_method: ask the user to choose a method (e.g. login account via email)
+         * sent_email: the email has been sent to the user
+         * passed_challenge: the request was successful and the login challenge was passed.
+         * @enum {unknown}
+         */
+        loginFlowState: "choose_method" | "sent_email" | "passed_challenge"
         /** @description Logout Flow */
         logoutFlow: {
             /** @description LogoutToken can be used to perform logout using AJAX. */
             logout_token: string
             /**
              * @description LogoutURL can be opened in a browser to sign the user out.
              *
              * format: uri
              */
             logout_url: string
         }
         message: {
             body: string
+            channel?: string
             /**
              * Format: date-time
              * @description CreatedAt is a helper struct field for gobuffalo.pop.
              */
             created_at: string
             /**
              * @description Dispatches store information about the attempts of delivering a message
@@ -1597,29 +1734,31 @@
              * recovery_valid TypeRecoveryValid
              * recovery_code_invalid TypeRecoveryCodeInvalid
              * recovery_code_valid TypeRecoveryCodeValid
              * verification_invalid TypeVerificationInvalid
              * verification_valid TypeVerificationValid
              * verification_code_invalid TypeVerificationCodeInvalid
              * verification_code_valid TypeVerificationCodeValid
-             * otp TypeOTP
              * stub TypeTestStub
+             * login_code_valid TypeLoginCodeValid
+             * registration_code_valid TypeRegistrationCodeValid
              * @enum {string}
              */
             template_type:
                 | "recovery_invalid"
                 | "recovery_valid"
                 | "recovery_code_invalid"
                 | "recovery_code_valid"
                 | "verification_invalid"
                 | "verification_valid"
                 | "verification_code_invalid"
                 | "verification_code_valid"
-                | "otp"
                 | "stub"
+                | "login_code_valid"
+                | "registration_code_valid"
             type: components["schemas"]["courierMessageType"]
             /**
              * Format: date-time
              * @description UpdatedAt is a helper struct field for gobuffalo.pop.
              */
             updated_at: string
         }
@@ -1663,41 +1802,20 @@
             error?: components["schemas"]["genericError"]
             /** @description Points to where to redirect the user to next. */
             redirect_browser_to: string
         }
         nullDuration: string | null
         nullInt64: number | null
         /** @description NullJSONRawMessage represents a json.RawMessage that works well with JSON, SQL, and Swagger and is NULLable- */
-        nullJsonRawMessage: Record<string, unknown> | null
+        nullJsonRawMessage: unknown
         /**
          * NullTime implements sql.NullTime functionality.
          * Format: date-time
          */
         nullTime: string
-        pagination: {
-            /**
-             * Format: int64
-             * @description Pagination Page
-             *
-             * This value is currently an integer, but it is not sequential. The value is not the page number, but a
-             * reference. The next page can be any number and some numbers might return an empty list.
-             *
-             * For example, page 2 might not follow after page 1. And even if page 3 and 5 exist, but page 4 might not exist.
-             * @default 1
-             */
-            page?: number
-            /**
-             * Format: int64
-             * @description Items per Page
-             *
-             * This is the number of items per page.
-             * @default 250
-             */
-            per_page?: number
-        }
         /** @description Patch Identities Body */
         patchIdentitiesBody: {
             /**
              * @description Identities holds the list of patches to apply
              *
              * required
              */
@@ -1717,15 +1835,15 @@
          * @description Used when an administrator creates a recovery code for an identity.
          */
         recoveryCodeForIdentity: {
             /**
              * Format: date-time
              * @description Expires At is the timestamp of when the recovery flow expires
              *
-             * The timestamp when the recovery link expires.
+             * The timestamp when the recovery code expires.
              */
             expires_at?: string
             /** @description RecoveryCode is the code that can be used to recover the account */
             recovery_code: string
             /**
              * @description RecoveryLink with flow
              *
@@ -1741,14 +1859,16 @@
          */
         recoveryFlow: {
             /**
              * @description Active, if set, contains the recovery method that is being used. It is initially
              * not set.
              */
             active?: string
+            /** @description Contains possible actions that could follow this flow */
+            continue_with?: components["schemas"]["continueWith"][]
             /**
              * Format: date-time
              * @description ExpiresAt is the time (UTC) when the request expires. If the user still wishes to update the setting,
              * a new request has to be initiated.
              */
             expires_at: string
             /**
@@ -1765,26 +1885,33 @@
             /**
              * @description RequestURL is the initial URL that was requested from Ory Kratos. It can be used
              * to forward information contained in the URL's path or query for example.
              */
             request_url: string
             /** @description ReturnTo contains the requested return_to URL. */
             return_to?: string
-            state: components["schemas"]["recoveryFlowState"]
+            /**
+             * @description State represents the state of this request:
+             *
+             * choose_method: ask the user to choose a method (e.g. recover account via email)
+             * sent_email: the email has been sent to the user
+             * passed_challenge: the request was successful and the recovery challenge was passed.
+             */
+            state: unknown
             type: components["schemas"]["selfServiceFlowType"]
             ui: components["schemas"]["uiContainer"]
         }
         /**
          * Recovery Flow State
          * @description The state represents the state of the recovery flow.
          *
          * choose_method: ask the user to choose a method (e.g. recover account via email)
          * sent_email: the email has been sent to the user
          * passed_challenge: the request was successful and the recovery challenge was passed.
-         * @enum {string}
+         * @enum {unknown}
          */
         recoveryFlowState: "choose_method" | "sent_email" | "passed_challenge"
         recoveryIdentityAddress: {
             /**
              * Format: date-time
              * @description CreatedAt is a helper struct field for gobuffalo.pop.
              */
@@ -1815,15 +1942,36 @@
              * @description Recovery Link
              *
              * This link can be used to recover the account.
              */
             recovery_link: string
         }
         registrationFlow: {
-            active?: components["schemas"]["identityCredentialsType"]
+            /**
+             * @description Active, if set, contains the registration method that is being used. It is initially
+             * not set.
+             * password CredentialsTypePassword
+             * oidc CredentialsTypeOIDC
+             * totp CredentialsTypeTOTP
+             * lookup_secret CredentialsTypeLookup
+             * webauthn CredentialsTypeWebAuthn
+             * code CredentialsTypeCodeAuth
+             * link_recovery CredentialsTypeRecoveryLink  CredentialsTypeRecoveryLink is a special credential type linked to the link strategy (recovery flow).  It is not used within the credentials object itself.
+             * code_recovery CredentialsTypeRecoveryCode
+             * @enum {string}
+             */
+            active?:
+                | "password"
+                | "oidc"
+                | "totp"
+                | "lookup_secret"
+                | "webauthn"
+                | "code"
+                | "link_recovery"
+                | "code_recovery"
             /**
              * Format: date-time
              * @description ExpiresAt is the time (UTC) when the flow expires. If the user still wishes to log in,
              * a new flow has to be initiated.
              */
             expires_at: string
             /**
@@ -1841,32 +1989,49 @@
              * @description Ory OAuth 2.0 Login Challenge.
              *
              * This value is set using the `login_challenge` query parameter of the registration and login endpoints.
              * If set will cooperate with Ory OAuth2 and OpenID to act as an OAuth2 server / OpenID Provider.
              */
             oauth2_login_challenge?: string
             oauth2_login_request?: components["schemas"]["OAuth2LoginRequest"]
+            organization_id?: components["schemas"]["NullUUID"]
             /**
              * @description RequestURL is the initial URL that was requested from Ory Kratos. It can be used
              * to forward information contained in the URL's path or query for example.
              */
             request_url: string
             /** @description ReturnTo contains the requested return_to URL. */
             return_to?: string
             /**
              * @description SessionTokenExchangeCode holds the secret code that the client can use to retrieve a session token after the flow has been completed.
              * This is only set if the client has requested a session token exchange code, and if the flow is of type "api",
              * and only on creating the flow.
              */
             session_token_exchange_code?: string
+            /**
+             * @description State represents the state of this request:
+             *
+             * choose_method: ask the user to choose a method (e.g. registration with email)
+             * sent_email: the email has been sent to the user
+             * passed_challenge: the request was successful and the registration challenge was passed.
+             */
+            state: unknown
             /** @description TransientPayload is used to pass data from the registration to a webhook */
             transient_payload?: Record<string, never>
             type: components["schemas"]["selfServiceFlowType"]
             ui: components["schemas"]["uiContainer"]
         }
+        /**
+         * State represents the state of this request:
+         * @description choose_method: ask the user to choose a method (e.g. registration with email)
+         * sent_email: the email has been sent to the user
+         * passed_challenge: the request was successful and the registration challenge was passed.
+         * @enum {unknown}
+         */
+        registrationFlowState: "choose_method" | "sent_email" | "passed_challenge"
         /** @description Is sent when a flow is expired */
         selfServiceFlowExpiredError: {
             error?: components["schemas"]["genericError"]
             /**
              * Format: date-time
              * @description When the flow has expired
              */
@@ -1907,22 +2072,28 @@
              */
             expires_at?: string
             /**
              * Format: uuid
              * @description Session ID
              */
             id: string
-            identity: components["schemas"]["identity"]
+            identity?: components["schemas"]["identity"]
             /**
              * Format: date-time
              * @description The Session Issuance Timestamp
              *
              * When this session was issued at. Usually equal or close to `authenticated_at`.
              */
             issued_at?: string
+            /**
+             * @description Tokenized is the tokenized (e.g. JWT) version of the session.
+             *
+             * It is only set when the `tokenize` query parameter was set to a valid tokenize template during calls to `/session/whoami`.
+             */
+            tokenized?: string
         }
         /**
          * AuthenticationMethod identifies an authentication method
          * @description A singular authenticator used during authentication / login.
          */
         sessionAuthenticationMethod: {
             aal?: components["schemas"]["authenticatorAssuranceLevel"]
@@ -1935,19 +2106,22 @@
              * The method used
              * @enum {string}
              */
             method?:
                 | "link_recovery"
                 | "code_recovery"
                 | "password"
+                | "code"
                 | "totp"
                 | "oidc"
                 | "webauthn"
                 | "lookup_secret"
                 | "v0.6_legacy_session"
+            /** @description The Organization id used for authentication */
+            organization?: string
             /** @description OIDC or SAML provider id used for authentication */
             provider?: string
         }
         /**
          * List of (Used) AuthenticationMethods
          * @description A list of authenticators which were used to authenticate the session.
          */
@@ -2007,25 +2181,33 @@
             /**
              * @description RequestURL is the initial URL that was requested from Ory Kratos. It can be used
              * to forward information contained in the URL's path or query for example.
              */
             request_url: string
             /** @description ReturnTo contains the requested return_to URL. */
             return_to?: string
-            state: components["schemas"]["settingsFlowState"]
+            /**
+             * @description State represents the state of this flow. It knows two states:
+             *
+             * show_form: No user data has been collected, or it is invalid, and thus the form should be shown.
+             * success: Indicates that the settings flow has been updated successfully with the provided data.
+             * Done will stay true when repeatedly checking. If set to true, done will revert back to false only
+             * when a flow with invalid (e.g. "please use a valid phone number") data was sent.
+             */
+            state: unknown
             type: components["schemas"]["selfServiceFlowType"]
             ui: components["schemas"]["uiContainer"]
         }
         /**
          * State represents the state of this flow. It knows two states:
          * @description show_form: No user data has been collected, or it is invalid, and thus the form should be shown.
          * success: Indicates that the settings flow has been updated successfully with the provided data.
          * Done will stay true when repeatedly checking. If set to true, done will revert back to false only
          * when a flow with invalid (e.g. "please use a valid phone number") data was sent.
-         * @enum {string}
+         * @enum {unknown}
          */
         settingsFlowState: "show_form" | "success"
         /** @description The Response for Registration Flows via API */
         successfulCodeExchangeResponse: {
             session: components["schemas"]["session"]
             /**
              * @description The Session Token
@@ -2132,14 +2314,15 @@
             | components["schemas"]["uiNodeText"]
             | components["schemas"]["uiNodeInput"]
             | components["schemas"]["uiNodeImage"]
             | components["schemas"]["uiNodeAnchor"]
             | components["schemas"]["uiNodeScript"]
         /** Anchor represents an anchor node. */
         uiNodeAnchor: {
+            attributes: components["schemas"]["uiNodeAnchorAttributes"]
             /**
              * @description Group specifies which group (e.g. password authenticator) this node belongs to.
              * default DefaultGroup
              * password PasswordGroup
              * oidc OpenIDConnectGroup
              * profile ProfileGroup
              * link LinkGroup
@@ -2148,15 +2331,14 @@
              * lookup_secret LookupGroup
              * webauthn WebAuthnGroup
              * @enum {string}
              */
             group: "default" | "password" | "oidc" | "profile" | "link" | "code" | "totp" | "lookup_secret" | "webauthn"
             messages: components["schemas"]["uiTexts"]
             meta: components["schemas"]["uiNodeMeta"]
-            attributes: components["schemas"]["uiNodeAnchorAttributes"]
             type: "a"
         }
         /** AnchorAttributes represents the attributes of an anchor node. */
         uiNodeAnchorAttributes: {
             /**
              * @description The link's href (destination) URL.
              *
@@ -2170,14 +2352,15 @@
              * is primarily used to allow compatibility with OpenAPI 3.0.  In this struct it technically always is "a".
              */
             node_type: string
             title: components["schemas"]["uiText"]
         }
         /** Image represents an image node. */
         uiNodeImage: {
+            attributes: components["schemas"]["uiNodeImageAttributes"]
             /**
              * @description Group specifies which group (e.g. password authenticator) this node belongs to.
              * default DefaultGroup
              * password PasswordGroup
              * oidc OpenIDConnectGroup
              * profile ProfileGroup
              * link LinkGroup
@@ -2186,15 +2369,14 @@
              * lookup_secret LookupGroup
              * webauthn WebAuthnGroup
              * @enum {string}
              */
             group: "default" | "password" | "oidc" | "profile" | "link" | "code" | "totp" | "lookup_secret" | "webauthn"
             messages: components["schemas"]["uiTexts"]
             meta: components["schemas"]["uiNodeMeta"]
-            attributes: components["schemas"]["uiNodeImageAttributes"]
             type: "img"
         }
         /** ImageAttributes represents the attributes of an image node. */
         uiNodeImageAttributes: {
             /**
              * Format: int64
              * @description Height of the image
@@ -2217,14 +2399,15 @@
              * Format: int64
              * @description Width of the image
              */
             width: number
         }
         /** Input represents an input node. */
         uiNodeInput: {
+            attributes: components["schemas"]["uiNodeInputAttributes"]
             /**
              * @description Group specifies which group (e.g. password authenticator) this node belongs to.
              * default DefaultGroup
              * password PasswordGroup
              * oidc OpenIDConnectGroup
              * profile ProfileGroup
              * link LinkGroup
@@ -2233,15 +2416,14 @@
              * lookup_secret LookupGroup
              * webauthn WebAuthnGroup
              * @enum {string}
              */
             group: "default" | "password" | "oidc" | "profile" | "link" | "code" | "totp" | "lookup_secret" | "webauthn"
             messages: components["schemas"]["uiTexts"]
             meta: components["schemas"]["uiNodeMeta"]
-            attributes: components["schemas"]["uiNodeInputAttributes"]
             type: "input"
         }
         /** @description InputAttributes represents the attributes of an input node */
         uiNodeInputAttributes: {
             /**
              * @description The autocomplete attribute for the input.
              * email InputAttributeAutocompleteEmail
@@ -2310,14 +2492,15 @@
          * be used to render UIs.
          */
         uiNodeMeta: {
             label?: components["schemas"]["uiText"]
         }
         /** Script represents a script node. */
         uiNodeScript: {
+            attributes: components["schemas"]["uiNodeScriptAttributes"]
             /**
              * @description Group specifies which group (e.g. password authenticator) this node belongs to.
              * default DefaultGroup
              * password PasswordGroup
              * oidc OpenIDConnectGroup
              * profile ProfileGroup
              * link LinkGroup
@@ -2326,15 +2509,14 @@
              * lookup_secret LookupGroup
              * webauthn WebAuthnGroup
              * @enum {string}
              */
             group: "default" | "password" | "oidc" | "profile" | "link" | "code" | "totp" | "lookup_secret" | "webauthn"
             messages: components["schemas"]["uiTexts"]
             meta: components["schemas"]["uiNodeMeta"]
-            attributes: components["schemas"]["uiNodeScriptAttributes"]
             type: "script"
         }
         /** ScriptAttributes represent script nodes which load javascript. */
         uiNodeScriptAttributes: {
             /** @description The script async type */
             async: boolean
             /** @description The script cross origin policy */
@@ -2361,14 +2543,15 @@
             /** @description The script source */
             src: string
             /** @description The script MIME type */
             type: string
         }
         /** Text represents a text node. */
         uiNodeText: {
+            attributes: components["schemas"]["uiNodeTextAttributes"]
             /**
              * @description Group specifies which group (e.g. password authenticator) this node belongs to.
              * default DefaultGroup
              * password PasswordGroup
              * oidc OpenIDConnectGroup
              * profile ProfileGroup
              * link LinkGroup
@@ -2377,15 +2560,14 @@
              * lookup_secret LookupGroup
              * webauthn WebAuthnGroup
              * @enum {string}
              */
             group: "default" | "password" | "oidc" | "profile" | "link" | "code" | "totp" | "lookup_secret" | "webauthn"
             messages: components["schemas"]["uiTexts"]
             meta: components["schemas"]["uiNodeMeta"]
-            attributes: components["schemas"]["uiNodeTextAttributes"]
             type: "text"
         }
         /** TextAttributes represents the attributes of a text node. */
         uiNodeTextAttributes: {
             /** @description A unique identifier */
             id: string
             /**
@@ -2424,42 +2606,82 @@
              */
             metadata_public?: unknown
             /**
              * @description SchemaID is the ID of the JSON Schema to be used for validating the identity's traits. If set
              * will update the Identity's SchemaID.
              */
             schema_id: string
-            state: components["schemas"]["identityState"]
+            /**
+             * @description State is the identity's state.
+             * active StateActive
+             * inactive StateInactive
+             * @enum {string}
+             */
+            state: "active" | "inactive"
             /**
              * @description Traits represent an identity's traits. The identity is able to create, modify, and delete traits
              * in a self-service manner. The input will always be validated against the JSON Schema defined
              * in `schema_id`.
              */
             traits: Record<string, never>
         }
         updateLoginFlowBody:
             | components["schemas"]["updateLoginFlowWithPasswordMethod"]
             | components["schemas"]["updateLoginFlowWithOidcMethod"]
             | components["schemas"]["updateLoginFlowWithTotpMethod"]
             | components["schemas"]["updateLoginFlowWithWebAuthnMethod"]
             | components["schemas"]["updateLoginFlowWithLookupSecretMethod"]
+            | components["schemas"]["updateLoginFlowWithCodeMethod"]
+        /** @description Update Login flow using the code method */
+        updateLoginFlowWithCodeMethod: {
+            /** @description Code is the 6 digits code sent to the user */
+            code?: string
+            /** @description CSRFToken is the anti-CSRF token */
+            csrf_token: string
+            /**
+             * @description Identifier is the code identifier
+             * The identifier requires that the user has already completed the registration or settings with code flow.
+             */
+            identifier?: string
+            /** @description Method should be set to "code" when logging in using the code strategy. */
+            method: string
+            /** @description Resend is set when the user wants to resend the code */
+            resend?: string
+        }
         /** @description Update Login Flow with Lookup Secret Method */
         updateLoginFlowWithLookupSecretMethod: {
             /** @description Sending the anti-csrf token is only required for browser login flows. */
             csrf_token?: string
             /** @description The lookup secret. */
             lookup_secret: string
             /** @description Method should be set to "lookup_secret" when logging in using the lookup_secret strategy. */
             method: string
         }
         /** @description Update Login Flow with OpenID Connect Method */
         updateLoginFlowWithOidcMethod: {
             /** @description The CSRF Token */
             csrf_token?: string
             /**
+             * @description IDToken is an optional id token provided by an OIDC provider
+             *
+             * If submitted, it is verified using the OIDC provider's public key set and the claims are used to populate
+             * the OIDC credentials of the identity.
+             * If the OIDC provider does not store additional claims (such as name, etc.) in the IDToken itself, you can use
+             * the `traits` field to populate the identity's traits. Note, that Apple only includes the users email in the IDToken.
+             *
+             * Supported providers are
+             * Apple
+             */
+            id_token?: string
+            /**
+             * @description IDTokenNonce is the nonce, used when generating the IDToken.
+             * If the provider supports nonce validation, the nonce will be validated against this value and required.
+             */
+            id_token_nonce?: string
+            /**
              * @description Method to use
              *
              * This field must be set to `oidc` when using the oidc method.
              */
             method: string
             /** @description The provider to register with */
             provider: string
@@ -2578,19 +2800,56 @@
             method: "link" | "code"
         }
         /** @description Update Registration Request Body */
         updateRegistrationFlowBody:
             | components["schemas"]["updateRegistrationFlowWithPasswordMethod"]
             | components["schemas"]["updateRegistrationFlowWithOidcMethod"]
             | components["schemas"]["updateRegistrationFlowWithWebAuthnMethod"]
+            | components["schemas"]["updateRegistrationFlowWithCodeMethod"]
+        /** @description Update Registration Flow with Code Method */
+        updateRegistrationFlowWithCodeMethod: {
+            /** @description The OTP Code sent to the user */
+            code?: string
+            /** @description The CSRF Token */
+            csrf_token?: string
+            /**
+             * @description Method to use
+             *
+             * This field must be set to `code` when using the code method.
+             */
+            method: string
+            /** @description Resend restarts the flow with a new code */
+            resend?: string
+            /** @description The identity's traits */
+            traits: Record<string, never>
+            /** @description Transient data to pass along to any webhooks */
+            transient_payload?: Record<string, never>
+        }
         /** @description Update Registration Flow with OpenID Connect Method */
         updateRegistrationFlowWithOidcMethod: {
             /** @description The CSRF Token */
             csrf_token?: string
             /**
+             * @description IDToken is an optional id token provided by an OIDC provider
+             *
+             * If submitted, it is verified using the OIDC provider's public key set and the claims are used to populate
+             * the OIDC credentials of the identity.
+             * If the OIDC provider does not store additional claims (such as name, etc.) in the IDToken itself, you can use
+             * the `traits` field to populate the identity's traits. Note, that Apple only includes the users email in the IDToken.
+             *
+             * Supported providers are
+             * Apple
+             */
+            id_token?: string
+            /**
+             * @description IDTokenNonce is the nonce, used when generating the IDToken.
+             * If the provider supports nonce validation, the nonce will be validated against this value and is required.
+             */
+            id_token_nonce?: string
+            /**
              * @description Method to use
              *
              * This field must be set to `oidc` when using the oidc method.
              */
             method: string
             /** @description The provider to register with */
             provider: string
@@ -2901,15 +3160,20 @@
             value: string
             /**
              * @description Indicates if the address has already been verified
              * @example true
              */
             verified: boolean
             verified_at?: components["schemas"]["nullTime"]
-            via: components["schemas"]["identityVerifiableAddressType"]
+            /**
+             * @description The delivery method
+             * @example email
+             * @enum {string}
+             */
+            via: "email" | "sms"
         }
         /**
          * A Verification Flow
          * @description Used to verify an out-of-band communication
          * channel such as an email address or a phone number.
          *
          * For more information head over to: https://www.ory.sh/docs/kratos/self-service/flows/verify-email-account-activation
@@ -2943,26 +3207,33 @@
             /**
              * @description RequestURL is the initial URL that was requested from Ory Kratos. It can be used
              * to forward information contained in the URL's path or query for example.
              */
             request_url?: string
             /** @description ReturnTo contains the requested return_to URL. */
             return_to?: string
-            state: components["schemas"]["verificationFlowState"]
+            /**
+             * @description State represents the state of this request:
+             *
+             * choose_method: ask the user to choose a method (e.g. verify your email)
+             * sent_email: the email has been sent to the user
+             * passed_challenge: the request was successful and the verification challenge was passed.
+             */
+            state: unknown
             type: components["schemas"]["selfServiceFlowType"]
             ui: components["schemas"]["uiContainer"]
         }
         /**
          * Verification Flow State
          * @description The state represents the state of the verification flow.
          *
          * choose_method: ask the user to choose a method (e.g. recover account via email)
          * sent_email: the email has been sent to the user
          * passed_challenge: the request was successful and the recovery challenge was passed.
-         * @enum {string}
+         * @enum {unknown}
          */
         verificationFlowState: "choose_method" | "sent_email" | "passed_challenge"
         version: {
             /** @description Version is the service's version. */
             version?: string
         }
         webAuthnJavaScript: string
@@ -3131,30 +3402,88 @@
      * List Identities
      * @description Lists all [identities](https://www.ory.sh/docs/kratos/concepts/identity-user-model) in the system.
      */
     listIdentities: {
         parameters: {
             query?: {
                 /**
-                 * @description Items per Page
+                 * @description Deprecated Items per Page
+                 *
+                 * DEPRECATED: Please use `page_token` instead. This parameter will be removed in the future.
                  *
                  * This is the number of items per page.
                  */
                 per_page?: number
                 /**
-                 * @description Pagination Page
+                 * @description Deprecated Pagination Page
+                 *
+                 * DEPRECATED: Please use `page_token` instead. This parameter will be removed in the future.
                  *
                  * This value is currently an integer, but it is not sequential. The value is not the page number, but a
                  * reference. The next page can be any number and some numbers might return an empty list.
                  *
                  * For example, page 2 might not follow after page 1. And even if page 3 and 5 exist, but page 4 might not exist.
+                 * The first page can be retrieved by omitting this parameter. Following page pointers will be returned in the
+                 * `Link` header.
                  */
                 page?: number
-                /** @description CredentialsIdentifier is the identifier (username, email) of the credentials to look up. */
+                /**
+                 * @description Page Size
+                 *
+                 * This is the number of items per page to return. For details on pagination please head over to the
+                 * [pagination documentation](https://www.ory.sh/docs/ecosystem/api-design#pagination).
+                 */
+                page_size?: number
+                /**
+                 * @description Next Page Token
+                 *
+                 * The next page token. For details on pagination please head over to the
+                 * [pagination documentation](https://www.ory.sh/docs/ecosystem/api-design#pagination).
+                 */
+                page_token?: string
+                /**
+                 * @description Read Consistency Level (preview)
+                 *
+                 * The read consistency level determines the consistency guarantee for reads:
+                 *
+                 * strong (slow): The read is guaranteed to return the most recent data committed at the start of the read.
+                 * eventual (very fast): The result will return data that is about 4.8 seconds old.
+                 *
+                 * The default consistency guarantee can be changed in the Ory Network Console or using the Ory CLI with
+                 * `ory patch project --replace '/previews/default_read_consistency_level="strong"'`.
+                 *
+                 * Setting the default consistency level to `eventual` may cause regressions in the future as we add consistency
+                 * controls to more APIs. Currently, the following APIs will be affected by this setting:
+                 *
+                 * `GET /admin/identities`
+                 *
+                 * This feature is in preview and only available in Ory Network.
+                 *  ConsistencyLevelUnset  ConsistencyLevelUnset is the unset / default consistency level.
+                 * strong ConsistencyLevelStrong  ConsistencyLevelStrong is the strong consistency level.
+                 * eventual ConsistencyLevelEventual  ConsistencyLevelEventual is the eventual consistency level using follower read timestamps.
+                 */
+                consistency?: "" | "strong" | "eventual"
+                /**
+                 * @description List of ids used to filter identities.
+                 * If this list is empty, then no filter will be applied.
+                 */
+                ids?: string[]
+                /**
+                 * @description CredentialsIdentifier is the identifier (username, email) of the credentials to look up using exact match.
+                 * Only one of CredentialsIdentifier and CredentialsIdentifierSimilar can be used.
+                 */
                 credentials_identifier?: string
+                /**
+                 * @description This is an EXPERIMENTAL parameter that WILL CHANGE. Do NOT rely on consistent, deterministic behavior.
+                 * THIS PARAMETER WILL BE REMOVED IN AN UPCOMING RELEASE WITHOUT ANY MIGRATION PATH.
+                 *
+                 * CredentialsIdentifierSimilar is the (partial) identifier (username, email) of the credentials to look up using similarity search.
+                 * Only one of CredentialsIdentifier and CredentialsIdentifierSimilar can be used.
+                 */
+                preview_credentials_identifier_similar?: string
             }
         }
         responses: {
             200: components["responses"]["listIdentities"]
             /** @description errorGeneric */
             default: {
                 content: {
@@ -3253,15 +3582,24 @@
             query?: {
                 /**
                  * @description Include Credentials in Response
                  *
                  * Include any credential, for example `password` or `oidc`, in the response. When set to `oidc`, This will return
                  * the initial OAuth 2.0 Access Token, OAuth 2.0 Refresh Token and the OpenID Connect ID Token if available.
                  */
-                include_credential?: ("password" | "totp" | "oidc" | "webauthn" | "lookup_secret")[]
+                include_credential?: (
+                    | "password"
+                    | "oidc"
+                    | "totp"
+                    | "lookup_secret"
+                    | "webauthn"
+                    | "code"
+                    | "link_recovery"
+                    | "code_recovery"
+                )[]
             }
             path: {
                 /** @description ID must be set to the ID of identity you want to get */
                 id: string
             }
         }
         responses: {
@@ -3421,18 +3759,33 @@
      */
     deleteIdentityCredentials: {
         parameters: {
             path: {
                 /** @description ID is the identity's ID. */
                 id: string
                 /**
-                 * @description Type is the credential's Type.
-                 * One of totp, webauthn, lookup
-                 */
-                type: "totp" | "webauthn" | "lookup"
+                 * @description Type is the type of credentials to be deleted.
+                 * password CredentialsTypePassword
+                 * oidc CredentialsTypeOIDC
+                 * totp CredentialsTypeTOTP
+                 * lookup_secret CredentialsTypeLookup
+                 * webauthn CredentialsTypeWebAuthn
+                 * code CredentialsTypeCodeAuth
+                 * link_recovery CredentialsTypeRecoveryLink  CredentialsTypeRecoveryLink is a special credential type linked to the link strategy (recovery flow).  It is not used within the credentials object itself.
+                 * code_recovery CredentialsTypeRecoveryCode
+                 */
+                type:
+                    | "password"
+                    | "oidc"
+                    | "totp"
+                    | "lookup_secret"
+                    | "webauthn"
+                    | "code"
+                    | "link_recovery"
+                    | "code_recovery"
             }
         }
         responses: {
             204: components["responses"]["emptyResponse"]
             /** @description errorGeneric */
             404: {
                 content: {
@@ -3451,28 +3804,48 @@
      * List an Identity's Sessions
      * @description This endpoint returns all sessions that belong to the given Identity.
      */
     listIdentitySessions: {
         parameters: {
             query?: {
                 /**
-                 * @description Items per Page
+                 * @description Deprecated Items per Page
+                 *
+                 * DEPRECATED: Please use `page_token` instead. This parameter will be removed in the future.
                  *
                  * This is the number of items per page.
                  */
                 per_page?: number
                 /**
-                 * @description Pagination Page
+                 * @description Deprecated Pagination Page
+                 *
+                 * DEPRECATED: Please use `page_token` instead. This parameter will be removed in the future.
                  *
                  * This value is currently an integer, but it is not sequential. The value is not the page number, but a
                  * reference. The next page can be any number and some numbers might return an empty list.
                  *
                  * For example, page 2 might not follow after page 1. And even if page 3 and 5 exist, but page 4 might not exist.
+                 * The first page can be retrieved by omitting this parameter. Following page pointers will be returned in the
+                 * `Link` header.
                  */
                 page?: number
+                /**
+                 * @description Page Size
+                 *
+                 * This is the number of items per page to return. For details on pagination please head over to the
+                 * [pagination documentation](https://www.ory.sh/docs/ecosystem/api-design#pagination).
+                 */
+                page_size?: number
+                /**
+                 * @description Next Page Token
+                 *
+                 * The next page token. For details on pagination please head over to the
+                 * [pagination documentation](https://www.ory.sh/docs/ecosystem/api-design#pagination).
+                 */
+                page_token?: string
                 /** @description Active is a boolean flag that filters out sessions based on the state. If no value is provided, all sessions are returned. */
                 active?: boolean
             }
             path: {
                 /** @description ID is the identity's ID. */
                 id: string
             }
@@ -3578,14 +3951,19 @@
     }
     /**
      * Create a Recovery Link
      * @description This endpoint creates a recovery link which should be given to the user in order for them to recover
      * (or activate) their account.
      */
     createRecoveryLinkForIdentity: {
+        parameters: {
+            query?: {
+                return_to?: string
+            }
+        }
         requestBody?: {
             content: {
                 "application/json": components["schemas"]["createRecoveryLinkForIdentityBody"]
             }
         }
         responses: {
             /** @description recoveryLinkForIdentity */
@@ -3851,28 +4229,48 @@
      * Get all Identity Schemas
      * @description Returns a list of all identity schemas currently in use.
      */
     listIdentitySchemas: {
         parameters: {
             query?: {
                 /**
-                 * @description Items per Page
+                 * @description Deprecated Items per Page
+                 *
+                 * DEPRECATED: Please use `page_token` instead. This parameter will be removed in the future.
                  *
                  * This is the number of items per page.
                  */
                 per_page?: number
                 /**
-                 * @description Pagination Page
+                 * @description Deprecated Pagination Page
+                 *
+                 * DEPRECATED: Please use `page_token` instead. This parameter will be removed in the future.
                  *
                  * This value is currently an integer, but it is not sequential. The value is not the page number, but a
                  * reference. The next page can be any number and some numbers might return an empty list.
                  *
                  * For example, page 2 might not follow after page 1. And even if page 3 and 5 exist, but page 4 might not exist.
+                 * The first page can be retrieved by omitting this parameter. Following page pointers will be returned in the
+                 * `Link` header.
                  */
                 page?: number
+                /**
+                 * @description Page Size
+                 *
+                 * This is the number of items per page to return. For details on pagination please head over to the
+                 * [pagination documentation](https://www.ory.sh/docs/ecosystem/api-design#pagination).
+                 */
+                page_size?: number
+                /**
+                 * @description Next Page Token
+                 *
+                 * The next page token. For details on pagination please head over to the
+                 * [pagination documentation](https://www.ory.sh/docs/ecosystem/api-design#pagination).
+                 */
+                page_token?: string
             }
         }
         responses: {
             200: components["responses"]["identitySchemas"]
             /** @description errorGeneric */
             default: {
                 content: {
@@ -3955,21 +4353,15 @@
                     "application/json": components["schemas"]["errorGeneric"]
                 }
             }
         }
     }
     /**
      * Submit a Login Flow
-     * @description :::info
-     *
-     * This endpoint is EXPERIMENTAL and subject to potential breaking changes in the future.
-     *
-     * :::
-     *
-     * Use this endpoint to complete a login flow. This endpoint
+     * @description Use this endpoint to complete a login flow. This endpoint
      * behaves differently for API and browser flows.
      *
      * API flows expect `application/json` to be sent in the body and responds with
      * HTTP 200 and a application/json body with the session token on success;
      * HTTP 410 if the original flow expired with the appropriate error messages set and optionally a `use_flow_id` parameter in the body;
      * HTTP 400 on form validation errors.
      *
@@ -4102,14 +4494,16 @@
                 /**
                  * @description EnableSessionTokenExchangeCode requests the login flow to include a code that can be used to retrieve the session token
                  * after the login flow has been completed.
                  */
                 return_session_token_exchange_code?: boolean
                 /** @description The URL to return the browser to after the flow was completed. */
                 return_to?: string
+                /** @description Via should contain the identity's credential the code should be sent to. Only relevant in aal2 flows. */
+                via?: string
             }
             header?: {
                 /** @description The Session Token of the Identity performing the settings flow. */
                 "X-Session-Token"?: string
             }
         }
         responses: {
@@ -4185,14 +4579,19 @@
                  * @description An optional Hydra login challenge. If present, Kratos will cooperate with
                  * Ory Hydra to act as an OAuth2 identity provider.
                  *
                  * The value for this parameter comes from `login_challenge` URL Query parameter sent to your
                  * application (e.g. `/login?login_challenge=abcde`).
                  */
                 login_challenge?: string
+                /**
+                 * @description An optional organization ID that should be used for logging this user in.
+                 * This parameter is only effective in the Ory Network.
+                 */
+                organization?: string
             }
             header?: {
                 /**
                  * @description HTTP Cookies
                  *
                  * When using the SDK in a browser app, on the server side you must include the HTTP Cookie Header
                  * sent by the client to your server here. This ensures that CSRF and session cookies are respected.
@@ -4443,16 +4842,16 @@
                 content: {
                     "application/json": components["schemas"]["errorGeneric"]
                 }
             }
         }
     }
     /**
-     * Complete Recovery Flow
-     * @description Use this endpoint to complete a recovery flow. This endpoint
+     * Update Recovery Flow
+     * @description Use this endpoint to update a recovery flow. This endpoint
      * behaves differently for API and browser flows and has several states:
      *
      * `choose_method` expects `flow` (in the URL query) and `email` (in the body) to be sent
      * and works with API- and Browser-initiated flows.
      * For API clients and Browser clients with HTTP Header `Accept: application/json` it either returns a HTTP 200 OK when the form is valid and HTTP 400 OK when the form is invalid.
      * and a HTTP 303 See Other redirect with a fresh recovery flow if the flow was otherwise invalid (e.g. expired).
      * For Browser clients without HTTP Header `Accept` or with `Accept: text/*` it returns a HTTP 303 See Other redirect to the Recovery UI URL with the Recovery Flow ID appended.
@@ -4537,15 +4936,15 @@
     }
     /**
      * Create Recovery Flow for Native Apps
      * @description This endpoint initiates a recovery flow for API clients such as mobile devices, smart TVs, and so on.
      *
      * If a valid provided session cookie or session token is provided, a 400 Bad Request error.
      *
-     * To fetch an existing recovery flow call `/self-service/recovery/flows?flow=<flow_id>`.
+     * On an existing recovery flow, use the `getRecoveryFlow` API endpoint.
      *
      * You MUST NOT use this endpoint in client-side (Single Page Apps, ReactJS, AngularJS) nor server-side (Java Server
      * Pages, NodeJS, PHP, Golang, ...) browser applications. Using this endpoint in these applications will make
      * you vulnerable to a variety of CSRF attacks.
      *
      * This endpoint MUST ONLY be used in scenarios such as native mobile apps (React Native, Objective C, Swift, Java, ...).
      *
@@ -4832,20 +5231,14 @@
         }
     }
     /**
      * Create Registration Flow for Browsers
      * @description This endpoint initializes a browser-based user registration flow. This endpoint will set the appropriate
      * cookies and anti-CSRF measures required for browser-based flows.
      *
-     * :::info
-     *
-     * This endpoint is EXPERIMENTAL and subject to potential breaking changes in the future.
-     *
-     * :::
-     *
      * If this endpoint is opened as a link in the browser, it will be redirected to
      * `selfservice.flows.registration.ui_url` with the flow ID set as the query parameter `?flow=`. If a valid user session
      * exists already, the browser will be redirected to `urls.default_redirect_url`.
      *
      * If this endpoint is called via an AJAX request, the response contains the flow without a redirect. In the
      * case of an error, the `error.id` of the JSON response body can be one of:
      *
@@ -4879,14 +5272,15 @@
                  * @description The URL to return the browser to after the verification flow was completed.
                  *
                  * After the registration flow is completed, the user will be sent a verification email.
                  * Upon completing the verification flow, this URL will be used to override the default
                  * `selfservice.flows.verification.after.default_redirect_to` value.
                  */
                 after_verification_return_to?: string
+                organization?: string
             }
         }
         responses: {
             /** @description registrationFlow */
             200: {
                 content: {
                     "application/json": components["schemas"]["registrationFlow"]
@@ -5550,28 +5944,48 @@
      * @description This endpoints returns all other active sessions that belong to the logged-in user.
      * The current session can be retrieved by calling the `/sessions/whoami` endpoint.
      */
     listMySessions: {
         parameters: {
             query?: {
                 /**
-                 * @description Items per Page
+                 * @description Deprecated Items per Page
+                 *
+                 * DEPRECATED: Please use `page_token` instead. This parameter will be removed in the future.
                  *
                  * This is the number of items per page.
                  */
                 per_page?: number
                 /**
-                 * @description Pagination Page
+                 * @description Deprecated Pagination Page
+                 *
+                 * DEPRECATED: Please use `page_token` instead. This parameter will be removed in the future.
                  *
                  * This value is currently an integer, but it is not sequential. The value is not the page number, but a
                  * reference. The next page can be any number and some numbers might return an empty list.
                  *
                  * For example, page 2 might not follow after page 1. And even if page 3 and 5 exist, but page 4 might not exist.
+                 * The first page can be retrieved by omitting this parameter. Following page pointers will be returned in the
+                 * `Link` header.
                  */
                 page?: number
+                /**
+                 * @description Page Size
+                 *
+                 * This is the number of items per page to return. For details on pagination please head over to the
+                 * [pagination documentation](https://www.ory.sh/docs/ecosystem/api-design#pagination).
+                 */
+                page_size?: number
+                /**
+                 * @description Next Page Token
+                 *
+                 * The next page token. For details on pagination please head over to the
+                 * [pagination documentation](https://www.ory.sh/docs/ecosystem/api-design#pagination).
+                 */
+                page_token?: string
             }
             header?: {
                 /** @description Set the Session Token when calling from non-browser clients. A session token has a format of `MP2YWEMeM8MxjkGKpH4dqOQ4Q4DlSPaj`. */
                 "X-Session-Token"?: string
                 /**
                  * @description Set the Cookie Header. This is especially useful when calling this endpoint from a server-side application. In that
                  * scenario you must include the HTTP Cookie Header which originally was included in the request to your server.
@@ -5718,14 +6132,24 @@
      * pseudo-code example
      * ...
      * const session = await client.toSession("the-session-token")
      *
      * console.log(session)
      * ```
      *
+     * When using a token template, the token is included in the `tokenized` field of the session.
+     *
+     * ```js
+     * pseudo-code example
+     * ...
+     * const session = await client.toSession("the-session-token", { tokenize_as: "example-jwt-template" })
+     *
+     * console.log(session.tokenized) // The JWT
+     * ```
+     *
      * Depending on your configuration this endpoint might return a 403 status code if the session has a lower Authenticator
      * Assurance Level (AAL) than is possible for the identity. This can happen if the identity has password + webauthn
      * credentials (which would result in AAL2) but the session has only AAL1. If this error occurs, ask the user
      * to sign in with the second factor or change the configuration.
      *
      * This endpoint is useful for:
      *
@@ -5744,14 +6168,22 @@
      * As explained above, this request may fail due to several reasons. The `error.id` can be one of:
      *
      * `session_inactive`: No active session was found in the request (e.g. no Ory Session Cookie / Ory Session Token).
      * `session_aal2_required`: An active session was found but it does not fulfil the Authenticator Assurance Level, implying that the session must (e.g.) authenticate the second factor.
      */
     toSession: {
         parameters: {
+            query?: {
+                /**
+                 * @description Returns the session additionally as a token (such as a JWT)
+                 *
+                 * The value of this parameter has to be a valid, configured Ory Session token template. For more information head over to [the documentation](http://ory.sh/docs/identities/session-to-jwt-cors).
+                 */
+                tokenize_as?: string
+            }
             header?: {
                 /**
                  * @description Set the Session Token when calling from non-browser clients. A session token has a format of `MP2YWEMeM8MxjkGKpH4dqOQ4Q4DlSPaj`.
                  * @example MP2YWEMeM8MxjkGKpH4dqOQ4Q4DlSPaj
                  */
                 "X-Session-Token"?: string
                 /**
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(account)/account/+page.server.ts` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/account/+page.server.ts`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import { type Cookies, fail, redirect } from "@sveltejs/kit"
-import { createKratosClient } from "$lib/server/api"
+import { fail, redirect } from "@sveltejs/kit"
+import { createKratosClient } from "$lib/server/utils"
 import type { KratosComponents } from "$lib/types"
-import { getFlow, getRandomId } from "$lib/utils"
+import { getFlowId, getRandomId } from "$lib/utils"
 
 export const actions = {
-    default: async ({ cookies, request }: { cookies: Cookies; request: Request }) => {
+    default: async ({ cookies, fetch, request }) => {
         const data = await request.formData()
 
         const client = createKratosClient(cookies, fetch)
         const response = await client.POST("/self-service/settings", {
             params: { query: { flow: data.get("flow") as string } },
             body: {
                 csrf_token: data.get("csrf_token") as string,
@@ -16,15 +16,15 @@
                 password: data.get("password") as string,
             },
         })
 
         switch (response.response.status) {
             case 200:
                 return {
-                    flow: getFlow(response.data!.ui.action),
+                    flow: getFlowId(response.data!.ui.action),
                     messages: response.data!.ui.messages,
                     nodes: response.data!.ui.nodes,
                 }
             case 303:
                 return fail(400, {
                     messages: [
                         {
@@ -32,15 +32,15 @@
                             text: "Session expired. Please refresh the page and try again.",
                             type: "error",
                         },
                     ],
                 })
             case 400:
                 return fail(400, {
-                    flow: getFlow((response.error as KratosComponents["schemas"]["settingsFlow"]).ui.action),
+                    flow: getFlowId((response.error as KratosComponents["schemas"]["settingsFlow"]).ui.action),
                     messages: (response.error as KratosComponents["schemas"]["settingsFlow"]).ui.messages,
                     nodes: (response.error as KratosComponents["schemas"]["settingsFlow"]).ui.nodes,
                 })
             default:
                 return fail(400, {
                     messages: [
                         {
@@ -50,32 +50,32 @@
                         },
                     ],
                 })
         }
     },
 }
 
-export async function load({ cookies, fetch }: { cookies: Cookies; fetch: typeof global.fetch }) {
+export async function load({ cookies, fetch }) {
     const client = createKratosClient(cookies, fetch)
     const response = await client.GET("/self-service/settings/browser", { params: {} })
 
     switch (response.response.status) {
         case 200:
             return {
-                flow: getFlow(response.data!.ui.action),
+                flow: getFlowId(response.data!.ui.action),
                 messages: response.data!.ui.messages,
                 nodes: response.data!.ui.nodes,
             }
         default:
             // Invalid session or insufficient session privileges
-            throw redirect(302, "/login")
+            redirect(302, "/login")
     }
 
     // return {
-    //     flow: getFlow("https://playground.com/self-service/login?flow=33f6079a-ef14-4084-af13-34a91e53cd6c"),
+    //     flow: getFlowId("https://playground.com/self-service/login?flow=33f6079a-ef14-4084-af13-34a91e53cd6c"),
     //     messages: [],
     //     nodes: [
     //         {
     //             type: "input",
     //             group: "default",
     //             attributes: {
     //                 name: "csrf_token",
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(account)/login/+page.server.ts` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/login/+page.server.ts`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,48 @@
-import { type Cookies, fail, redirect } from "@sveltejs/kit"
-import { createKratosClient } from "$lib/server/api"
+import { fail, redirect } from "@sveltejs/kit"
+import { createKratosClient } from "$lib/server/utils"
 import type { KratosComponents } from "$lib/types"
-import { getFlow, getRandomId } from "$lib/utils"
+import { getFlowId, getRandomId } from "$lib/utils"
 
 export const actions = {
-    default: async ({ cookies, request }: { cookies: Cookies; request: Request }) => {
+    default: async ({ cookies, fetch, request }) => {
         const data = await request.formData()
 
         const client = createKratosClient(cookies, fetch)
         const response = await client.POST("/self-service/login", {
             params: { query: { flow: data.get("flow") as string } },
             body: {
                 csrf_token: data.get("csrf_token") as string,
                 method: data.get("method") as string,
                 identifier: data.get("identifier") as string,
-                password: data.get("password") as string,
+                ...(data.get("resend")
+                    ? { resend: data.get("resend") as string }
+                    : data.get("password")
+                      ? { password: data.get("password") as string }
+                      : { code: data.get("code") as string }),
             },
         })
 
         switch (response.response.status) {
             case 200:
-                throw redirect(302, "/")
+                redirect(302, "/")
+            // eslint-disable-next-line no-fallthrough
             case 303:
                 return fail(400, {
                     messages: [
                         {
                             id: getRandomId(),
                             text: "Session expired. Please refresh the page and try again.",
                             type: "error",
                         },
                     ],
                 })
             case 400:
                 return fail(400, {
-                    flow: getFlow((response.error as KratosComponents["schemas"]["loginFlow"]).ui.action),
+                    flow: getFlowId((response.error as KratosComponents["schemas"]["loginFlow"]).ui.action),
                     messages: (response.error as KratosComponents["schemas"]["loginFlow"]).ui.messages,
                     nodes: (response.error as KratosComponents["schemas"]["loginFlow"]).ui.nodes,
                 })
             default:
                 return fail(400, {
                     messages: [
                         {
@@ -47,32 +52,32 @@
                         },
                     ],
                 })
         }
     },
 }
 
-export async function load({ cookies, fetch }: { cookies: Cookies; fetch: typeof global.fetch }) {
+export async function load({ cookies, fetch }) {
     const client = createKratosClient(cookies, fetch)
     const response = await client.GET("/self-service/login/browser", { params: {} })
 
     switch (response.response.status) {
         case 200:
             return {
-                flow: getFlow(response.data!.ui.action),
+                flow: getFlowId(response.data!.ui.action),
                 messages: response.data!.ui.messages,
                 nodes: response.data!.ui.nodes,
             }
         default:
             // Already logged in
-            throw redirect(302, "/")
+            redirect(302, "/")
     }
 
     // return {
-    //     flow: getFlow("https://playground.com/self-service/login?flow=33f6079a-ef14-4084-af13-34a91e53cd6c"),
+    //     flow: getFlowId("https://playground.com/self-service/login?flow=33f6079a-ef14-4084-af13-34a91e53cd6c"),
     //     messages: [
     //         // {
     //         //     id: 4000001,
     //         //     text: "Wrong credentials.",
     //         //     type: "error",
     //         // },
     //     ],
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(account)/login/+page.svelte` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/login/+page.svelte`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 <script lang="ts">
     import { FormBuilder, HeroFrame } from "$lib/components"
     import { SITE_TITLE } from "$lib/constants"
     import { AccountIcon } from "$lib/icons"
 </script>
 
 <HeroFrame wrapped>
-    <span class="text-center text-4xl">Welcome to {SITE_TITLE}</span>
+    <span class="text-balance text-center text-4xl">Welcome to {SITE_TITLE}</span>
     <span class="mb-6 h-12 w-12">
         <AccountIcon />
     </span>
-    <FormBuilder>
+    <FormBuilder primaryGroup="password" validationFreeButtons={["resend"]}>
         <span class="inline-flex">
             <a class="link text-sm" href="/recover">Forgot password?</a>
         </span>
     </FormBuilder>
 </HeroFrame>
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(account)/recover/+page.server.ts` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/recover/+page.server.ts`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import { type Cookies, fail, redirect } from "@sveltejs/kit"
-import { createKratosClient } from "$lib/server/api"
+import { fail, redirect } from "@sveltejs/kit"
+import { createKratosClient } from "$lib/server/utils"
 import type { KratosComponents } from "$lib/types"
-import { getFlow, getRandomId } from "$lib/utils"
+import { getFlowId, getRandomId } from "$lib/utils"
 
 export const actions = {
-    default: async ({ cookies, request }: { cookies: Cookies; request: Request }) => {
+    default: async ({ cookies, fetch, request }) => {
         const data = await request.formData()
 
         const client = createKratosClient(cookies, fetch)
         const response = await client.POST("/self-service/recovery", {
             params: { query: { flow: data.get("flow") as string } },
             body: {
                 csrf_token: data.get("csrf_token") as string,
@@ -16,19 +16,19 @@
                 ...(data.get("email") ? { email: data.get("email") as string } : { code: data.get("code") as string }),
             },
         })
 
         switch (response.response.status) {
             case 200:
                 if (!data.get("email")) {
-                    throw redirect(302, "/account")
+                    redirect(302, "/account")
                 }
 
                 return {
-                    flow: getFlow(response.data!.ui.action),
+                    flow: getFlowId(response.data!.ui.action),
                     messages: response.data!.ui.messages,
                     nodes: response.data!.ui.nodes,
                 }
             case 303:
                 return fail(400, {
                     messages: [
                         {
@@ -36,21 +36,21 @@
                             text: "Session expired. Please refresh the page and try again.",
                             type: "error",
                         },
                     ],
                 })
             case 400:
                 return fail(400, {
-                    flow: getFlow((response.error as KratosComponents["schemas"]["recoveryFlow"]).ui.action),
+                    flow: getFlowId((response.error as KratosComponents["schemas"]["recoveryFlow"]).ui.action),
                     messages: (response.error as KratosComponents["schemas"]["recoveryFlow"]).ui.messages,
                     nodes: (response.error as KratosComponents["schemas"]["recoveryFlow"]).ui.nodes,
                 })
             case 422:
                 if (!data.get("email")) {
-                    throw redirect(302, "/account")
+                    redirect(302, "/account")
                 }
 
                 break
             default:
                 return fail(400, {
                     messages: [
                         {
@@ -60,32 +60,32 @@
                         },
                     ],
                 })
         }
     },
 }
 
-export async function load({ cookies, fetch }: { cookies: Cookies; fetch: typeof global.fetch }) {
+export async function load({ cookies, fetch }) {
     const client = createKratosClient(cookies, fetch)
     const response = await client.GET("/self-service/recovery/browser", { params: {} })
 
     switch (response.response.status) {
         case 200:
             return {
-                flow: getFlow(response.data!.ui.action),
+                flow: getFlowId(response.data!.ui.action),
                 messages: response.data!.ui.messages,
                 nodes: response.data!.ui.nodes,
             }
         default:
             // Already logged in
-            throw redirect(302, "/account")
+            redirect(302, "/account")
     }
 
     // return {
-    //     flow: getFlow("https://playground.com/self-service/login?flow=33f6079a-ef14-4084-af13-34a91e53cd6c"),
+    //     flow: getFlowId("https://playground.com/self-service/login?flow=33f6079a-ef14-4084-af13-34a91e53cd6c"),
     //     messages: [
     //         // {
     //         //     id: 4000001,
     //         //     text: "Wrong credentials.",
     //         //     type: "error",
     //         // },
     //     ],
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(apps)/+page.svelte` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(apps)/+page.svelte`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 <script lang="ts">
+    import { skeleton } from "$lib/actions"
+    import CoverImage from "$lib/assets/cover.jpg?enhanced"
     import { HeroFrame } from "$lib/components"
     import { SITE_SUBTITLE, SITE_TITLE } from "$lib/constants"
     import { getRandomElement } from "$lib/utils"
 
     export let data
 
     const subtitle = getRandomElement(JSON.parse(SITE_SUBTITLE) as string[])
 </script>
 
 <HeroFrame>
     <div class="hero h-full">
         <div class="hero-content flex-col gap-16 lg:flex-row-reverse lg:gap-32">
-            <img src="/cover.jpg" alt="cover" class="max-h-48 w-80 rounded-box object-cover shadow-2xl lg:max-h-none" />
+            <enhanced:img
+                class="max-h-48 w-80 rounded-box object-cover shadow-2xl lg:max-h-none"
+                src={CoverImage}
+                alt="cover"
+                use:skeleton
+            />
             <div>
                 {#if data.userInfo}
                     <h1 class="text-4xl font-bold">Welcome back, {data.userInfo.name.first}</h1>
                     <p class="pt-4 text-lg">{subtitle}</p>
                 {:else}
                     <h1 class="text-4xl font-bold">Welcome to {SITE_TITLE}</h1>
                     <p class="pb-10 pt-4 text-lg lg:pb-20">{subtitle}</p>
```

#### html2text {}

```diff
@@ -1,8 +1,7 @@
-[cover]
 {#if data.userInfo}
 ************ WWeellccoommee bbaacckk,, {{ddaattaa..uusseerrIInnffoo..nnaammee..ffiirrsstt}} ************
 {subtitle}
 {:else}
 ************ WWeellccoommee ttoo {{SSIITTEE__TTIITTLLEE}} ************
 {subtitle}
 _S_i_g_n_ _i_n {/if}
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(apps)/app/jupyterhub/+layout.server.ts` & `lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/web/routes/+layout.server.ts`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,12 @@
 import { load as loadHtmlString } from "cheerio"
-import type { Cookies } from "@sveltejs/kit"
-import { wrapFetch } from "$lib/server/api"
-import { JUPYTERHUB_BASE_URL, JUPYTERHUB_PASSWORD } from "$lib/server/constants"
-import type { User } from "$lib/types"
-
-export async function load({
-    cookies,
-    fetch,
-    parent,
-}: {
-    cookies: Cookies
-    fetch: typeof global.fetch
-    parent: () => Promise<{ userInfo: User["traits"] | undefined }>
-}) {
+import { JUPYTERHUB_BASE_URL, JUPYTERHUB_PASSWORD } from "$lib/plugins/jupyterhub/server/constants.server"
+import { wrapFetch } from "$lib/utils"
+
+export async function load({ cookies, fetch, parent }) {
     const wrappedFetch = wrapFetch({
         fetch,
         baseUrl: JUPYTERHUB_BASE_URL,
         cookies,
         cookiePath: "/app/jupyterhub",
         credentials: "include",
         ensureOk: true,
@@ -38,11 +28,11 @@
     await wrappedFetch("/app/jupyterhub/hub/login", {
         method: "POST",
         redirect: "manual",
         headers: { "Content-Type": "application/x-www-form-urlencoded" },
         body: new URLSearchParams({
             _xsrf: csrf,
             username,
-            password: JUPYTERHUB_PASSWORD!,
+            password: JUPYTERHUB_PASSWORD,
         }),
     })
 }
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/(apps)/app/rstudio/+layout.server.ts` & `lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/web/routes/+layout.server.ts`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,12 @@
 import { load as loadHtmlString } from "cheerio"
-import type { Cookies } from "@sveltejs/kit"
-import { wrapFetch } from "$lib/server/api"
-import { RSTUDIO_BASE_URL, RSTUDIO_PASSWORD } from "$lib/server/constants"
-import type { User } from "$lib/types"
+import { RSTUDIO_BASE_URL, RSTUDIO_PASSWORD } from "$lib/plugins/rstudio/server/constants.server"
+import { wrapFetch } from "$lib/utils"
 
-export async function load({
-    cookies,
-    fetch,
-    parent,
-}: {
-    cookies: Cookies
-    fetch: typeof global.fetch
-    parent: () => Promise<{ userInfo: User["traits"] | undefined }>
-}) {
+export async function load({ cookies, fetch, parent }) {
     const wrappedFetch = wrapFetch({
         fetch,
         baseUrl: RSTUDIO_BASE_URL,
         cookies,
         cookiePath: "/app/rstudio",
         credentials: "include",
         ensureOk: true,
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/+error.svelte` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/+error.svelte`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <script lang="ts">
     import { page } from "$app/stores"
     import { HeroFrame } from "$lib/components"
 </script>
 
 <HeroFrame>
     <div class="hero h-full">
-        <div class="hero-content text-center">
-            <div class="max-w-xl">
+        <div class="hero-content text-balance text-center">
+            <div class="flex max-w-lg flex-col md:max-w-xl">
                 {#if $page.status === 429}
                     <h1 class="my-6 text-4xl font-bold">Hey, you're going too fast!</h1>
                     <a class="link text-lg" href="/">Let's take a break.</a>
                 {:else if String($page.status).startsWith("4")}
                     <h1 class="my-6 text-4xl font-bold">Seems like you're lost...</h1>
                     <a class="link text-lg" href="/">Let's not stuck here forever.</a>
                 {:else}
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/+layout.server.ts` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/+layout.server.ts`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,37 @@
-import type { Cookies } from "@sveltejs/kit"
-import { createKetoClient, createKratosClient } from "$lib/server/api"
-import { EApp } from "$lib/server/types"
-import { createApp } from "$lib/server/utils"
-import type { App, User } from "$lib/types"
+import { createKetoClient, createKratosClient, getAllApps } from "$lib/server/utils"
+import type { AppInfo, User } from "$lib/types"
 
-async function getAllowedApps(fetch: typeof global.fetch, username?: string): Promise<App[]> {
+async function getAllowedApps(fetch: typeof global.fetch, username?: string): Promise<AppInfo[]> {
     const client = createKetoClient(fetch)
-    const allowedApps = []
     const apps = []
 
-    for (const app of Object.values(EApp)) {
+    for (const app of getAllApps()) {
         const response = await client.GET("/relation-tuples/check", {
             params: {
                 query: {
                     namespace: "app",
-                    object: app,
+                    object: app.name,
                     relation: "access",
                     subject_id: username ?? "anonymous",
                 },
             },
         })
 
         switch (response.response.status) {
             case 200:
-                allowedApps.push(app)
+                apps.push(app)
                 break
         }
     }
 
-    if (allowedApps.includes(EApp.FileBrowser)) {
-        apps.push(createApp(EApp.FileBrowser))
-    }
-    if (allowedApps.includes(EApp.PrivateBin)) {
-        apps.push(createApp(EApp.PrivateBin))
-    }
-    if (allowedApps.includes(EApp.JupyterHub)) {
-        apps.push(createApp(EApp.JupyterHub))
-    }
-    if (allowedApps.includes(EApp.RStudio)) {
-        apps.push(createApp(EApp.RStudio))
-    }
-    if (allowedApps.includes(EApp.XRay)) {
-        apps.push(createApp(EApp.XRay))
-    }
-
     return apps
 }
 
-export async function load({ cookies, fetch, url }: { cookies: Cookies; fetch: typeof global.fetch; url: URL }) {
+export async function load({ cookies, fetch, url }) {
     const title = url.pathname.split("/").pop() || "home"
 
     const client = createKratosClient(cookies, fetch)
     const response = await client.GET("/sessions/whoami", { params: {} })
 
     switch (response.response.status) {
         case 200:
@@ -81,15 +61,15 @@
                 logoutToken: undefined,
                 title,
                 userInfo: undefined,
             }
     }
 
     // return {
-    //     apps: [createApp(EApp.PrivateBin), createApp(EApp.XRay)],
+    //     apps: [],
     //     logoutToken: "test123",
     //     title,
     //     userInfo: {
     //         username: "test",
     //         email: "testuser12345@gmail.com",
     //         name: {
     //             first: "Test",
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/src/routes/+layout.svelte` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/+layout.svelte`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 <script lang="ts">
     import "../app.pcss"
     import { onMount } from "svelte"
     import { page } from "$app/stores"
     import { AppShell, LoadingIndicator } from "$lib/components"
     import { ETheme } from "$lib/types"
-    import { createStore, createTitle } from "$lib/utils"
+    import { createStore, usePageTitle } from "$lib/utils"
 
-    const { allowScroll, currentTheme } = createStore()
+    const { allowScroll, currentTheme, isSafari } = createStore()
 
     onMount(() => {
         const theme = localStorage.getItem("theme")
         $currentTheme = theme && Object.values(ETheme).includes(theme as ETheme) ? (theme as ETheme) : ETheme.Auto
+
+        // @ts-expect-error exists for Safari on macOS
+        $isSafari = window.safari !== undefined
     })
 </script>
 
 <div>
     <LoadingIndicator />
     <AppShell>
         <slot />
     </AppShell>
 </div>
 
 <svelte:head>
-    <title>{createTitle($page.data.title)}</title>
+    <title>{usePageTitle($page.data.title)}</title>
     {#if !$allowScroll}
         <style>
             body {
                 overflow: hidden;
             }
         </style>
     {/if}
```

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/static/cover.jpg` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/assets/cover.jpg`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/static/favicon.png` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/static/favicon.png`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/tailwind.config.cjs` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/tailwind.config.cjs`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/src/lungo_cli/resources/web/tsconfig.json` & `lungo_cli-0.3.0/src/lungo_cli/resources/web/tsconfig.json`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.2.3/PKG-INFO` & `lungo_cli-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: lungo-cli
-Version: 0.2.3
+Version: 0.3.0
 Summary: A user-friendly home lab setup designed for small-to-mid-scale on-premises hosting.
 Home-page: https://github.com/raymond-u/lungo
 Keywords: homelab,self-host
 Author: raymond-u
 Author-email: 36328498+raymond-u@users.noreply.github.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: cryptography (>=42.0.2,<43.0.0)
-Requires-Dist: importlib-resources (>=6.0.1,<7.0.0)
+Requires-Dist: aenum (>=3.1.15,<4.0.0)
+Requires-Dist: cryptography (>=42.0.5,<43.0.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
+Requires-Dist: packaging (>=24.0,<25.0)
 Requires-Dist: platformdirs (>=4.2.0,<5.0.0)
-Requires-Dist: pydantic-yaml (>=1.2.1,<2.0.0)
-Requires-Dist: pydantic[email] (>=2.6.1,<3.0.0)
+Requires-Dist: pydantic-yaml (>=1.3.0,<2.0.0)
+Requires-Dist: pydantic[email] (>=2.6.4,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Requires-Dist: typer (>=0.12.3,<0.13.0)
 Project-URL: Documentation, https://raymond-u.github.io/lungo/
 Project-URL: Repository, https://github.com/raymond-u/lungo
 Description-Content-Type: text/markdown
 
 <br>
 
 <h1 align="center">
@@ -49,15 +49,15 @@
 
 <br>
 
 ## Features
 
 - **Complete configurability** - manage everything declaratively through YAML files
 - **Seamless interoperability** - access all applications via a single sign-on portal
-- **Batteries included** - benefit from a diverse range of applications
+- **Batteries included** - extend functionality with both built-in and custom plugins
 - **Containerized solution** - designed to operate in a rootless Docker environment
 - **Security by default** - use HTTPS and secure server settings across the system
 
 ## Installation
 
 The recommended way to install Lungo is via [pipx](https://pypa.github.io/pipx/):
```

#### html2text {}

```diff
@@ -1,42 +1,42 @@
-Metadata-Version: 2.1 Name: lungo-cli Version: 0.2.3 Summary: A user-friendly
+Metadata-Version: 2.1 Name: lungo-cli Version: 0.3.0 Summary: A user-friendly
 home lab setup designed for small-to-mid-scale on-premises hosting. Home-page:
 https://github.com/raymond-u/lungo Keywords: homelab,self-host Author: raymond-
 u Author-email: 36328498+raymond-u@users.noreply.github.com Requires-Python:
->=3.11,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Requires-Dist: cryptography (>=42.0.2,<43.0.0) Requires-Dist:
-importlib-resources (>=6.0.1,<7.0.0) Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
-Requires-Dist: platformdirs (>=4.2.0,<5.0.0) Requires-Dist: pydantic-yaml
-(>=1.2.1,<2.0.0) Requires-Dist: pydantic[email] (>=2.6.1,<3.0.0) Requires-Dist:
-requests (>=2.31.0,<3.0.0) Requires-Dist: typer[all] (>=0.9.0,<0.10.0) Project-
-URL: Documentation, https://raymond-u.github.io/lungo/ Project-URL: Repository,
+>=3.12,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.12 Requires-Dist: aenum (>=3.1.15,<4.0.0)
+Requires-Dist: cryptography (>=42.0.5,<43.0.0) Requires-Dist: jinja2
+(>=3.1.3,<4.0.0) Requires-Dist: packaging (>=24.0,<25.0) Requires-Dist:
+platformdirs (>=4.2.0,<5.0.0) Requires-Dist: pydantic-yaml (>=1.3.0,<2.0.0)
+Requires-Dist: pydantic[email] (>=2.6.4,<3.0.0) Requires-Dist: requests
+(>=2.31.0,<3.0.0) Requires-Dist: typer (>=0.12.3,<0.13.0) Project-URL:
+Documentation, https://raymond-u.github.io/lungo/ Project-URL: Repository,
 https://github.com/raymond-u/lungo Description-Content-Type: text/markdown
                                 ************ _[[_LL_uu_nn_gg_oo_]]
                                      LLuunnggoo
                                      ************
   A user-friendly home lab setup designed for small-to-mid-scale on-premises
                                    hosting.
                          _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_:_ _M_I_T_]
 
 ## Features - **Complete configurability** - manage everything declaratively
 through YAML files - **Seamless interoperability** - access all applications
-via a single sign-on portal - **Batteries included** - benefit from a diverse
-range of applications - **Containerized solution** - designed to operate in a
-rootless Docker environment - **Security by default** - use HTTPS and secure
-server settings across the system ## Installation The recommended way to
-install Lungo is via [pipx](https://pypa.github.io/pipx/): ```bash pipx install
-lungo-cli ``` Note that Lungo is built upon [Docker Compose](https://
-github.com/docker/compose). Before proceeding, please ensure that Docker is
-installed on your machine. Alternatively, you can use [Podman Compose](https://
-github.com/containers/podman-compose) with [Podman](https://podman.io/). You
-can also [use Docker Compose with Podman](https://fedoramagazine.org/use-
-docker-compose-with-podman-to-orchestrate-containers-on-fedora/). For
-instructions on setting up these tools, please refer to their respective
-documentation. ## Quickstart Copy the example configuration files to the
-platform-specific configuration directory. For example, on Linux, you can use
-the following command: ```bash mkdir -p ~/.config/lungo cp examples/
+via a single sign-on portal - **Batteries included** - extend functionality
+with both built-in and custom plugins - **Containerized solution** - designed
+to operate in a rootless Docker environment - **Security by default** - use
+HTTPS and secure server settings across the system ## Installation The
+recommended way to install Lungo is via [pipx](https://pypa.github.io/pipx/):
+```bash pipx install lungo-cli ``` Note that Lungo is built upon [Docker
+Compose](https://github.com/docker/compose). Before proceeding, please ensure
+that Docker is installed on your machine. Alternatively, you can use [Podman
+Compose](https://github.com/containers/podman-compose) with [Podman](https://
+podman.io/). You can also [use Docker Compose with Podman](https://
+fedoramagazine.org/use-docker-compose-with-podman-to-orchestrate-containers-on-
+fedora/). For instructions on setting up these tools, please refer to their
+respective documentation. ## Quickstart Copy the example configuration files to
+the platform-specific configuration directory. For example, on Linux, you can
+use the following command: ```bash mkdir -p ~/.config/lungo cp examples/
 * ~/.config/lungo ``` Edit the configuration files according to your
 preferences. Then, launch the Lungo service by running the following command:
 ```bash lungo up ``` ## Documentation For more information, please refer to the
 [documentation](https://raymond-u.github.io/lungo/). ## License This project is
 licensed under the MIT License. See [LICENSE](LICENSE) for details.
```


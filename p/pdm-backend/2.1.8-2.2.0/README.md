# Comparing `tmp/pdm_backend-2.1.8.tar.gz` & `tmp/pdm_backend-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_backend-2.1.8.tar", last modified: Wed Dec 27 07:00:14 2023, max compression
+gzip compressed data, was "pdm_backend-2.2.0.tar", last modified: Sun Apr 14 07:54:48 2024, max compression
```

## Comparing `pdm_backend-2.1.8.tar` & `pdm_backend-2.2.0.tar`

### file list

```diff
@@ -1,181 +1,185 @@
--rw-r--r--   0        0        0     1067 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/LICENSE
--rw-r--r--   0        0        0     1711 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/README.md
--rw-r--r--   0        0        0     2273 2023-12-27 07:00:14.563159 pdm_backend-2.1.8/pyproject.toml
--rw-r--r--   0        0        0     3282 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/__init__.py
--rw-r--r--   0        0        0        0 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/__init__.py
--rw-r--r--   0        0        0      197 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/LICENSE
--rw-r--r--   0        0        0    10174 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/LICENSE.BSD
--rw-r--r--   0        0        0      661 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     3265 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/_elffile.py
--rw-r--r--   0        0        0     8813 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     2524 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     9606 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     5115 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/_tokenizer.py
--rw-r--r--   0        0        0     7928 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/markers.py
--rw-r--r--   0        0        0        0 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/py.typed
--rw-r--r--   0        0        0     3264 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    38937 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    16469 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4355 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    16315 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/version.py
--rw-r--r--   0        0        0     1113 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/pyproject_metadata/LICENSE
--rw-r--r--   0        0        0    19827 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/pyproject_metadata/__init__.py
--rw-r--r--   0        0        0        0 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/pyproject_metadata/py.typed
--rw-r--r--   0        0        0     1072 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/tomli/LICENSE
--rw-r--r--   0        0        0      396 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2023-12-27 07:00:03.135141 pdm_backend-2.1.8/src/pdm/backend/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/_vendor/tomli/_types.py
--rw-r--r--   0        0        0       26 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/_vendor/tomli/py.typed
--rw-r--r--   0        0        0     1072 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/_vendor/tomli_w/LICENSE
--rw-r--r--   0        0        0      177 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/_vendor/tomli_w/__init__.py
--rw-r--r--   0        0        0     6132 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/_vendor/tomli_w/_writer.py
--rw-r--r--   0        0        0       26 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/_vendor/tomli_w/py.typed
--rw-r--r--   0        0        0       70 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/_vendor/vendor.txt
--rw-r--r--   0        0        0    12629 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/base.py
--rw-r--r--   0        0        0     9872 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/config.py
--rw-r--r--   0        0        0     3974 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/editable.py
--rw-r--r--   0        0        0      452 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/exceptions.py
--rw-r--r--   0        0        0      108 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/hooks/__init__.py
--rw-r--r--   0        0        0     4593 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/hooks/base.py
--rw-r--r--   0        0        0     6458 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/hooks/setuptools.py
--rw-r--r--   0        0        0     5235 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/hooks/version/__init__.py
--rw-r--r--   0        0        0    10129 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/hooks/version/scm.py
--rw-r--r--   0        0        0      759 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/intree.py
--rw-r--r--   0        0        0    14958 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/macosx_platform.py
--rw-r--r--   0        0        0        0 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/py.typed
--rw-r--r--   0        0        0     3050 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/sdist.py
--rw-r--r--   0        0        0     1381 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/structures.py
--rw-r--r--   0        0        0     7665 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/utils.py
--rw-r--r--   0        0        0    11818 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/src/pdm/backend/wheel.py
--rw-r--r--   0        0        0       72 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/__init__.py
--rw-r--r--   0        0        0      929 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/conftest.py
--rw-r--r--   0        0        0      856 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/hooks/hook_class.py
--rw-r--r--   0        0        0      599 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/hooks/hook_module.py
--rw-r--r--   0        0        0      599 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/hooks/local_hook.py
--rw-r--r--   0        0        0       12 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-cextension-in-src/LICENSE
--rw-r--r--   0        0        0      138 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-cextension-in-src/pdm.lock
--rw-r--r--   0        0        0      234 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-cextension-in-src/pdm_build.py
--rw-r--r--   0        0        0      558 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml
--rw-r--r--   0        0        0       22 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-cextension-in-src/src/my_package/__init__.py
--rw-r--r--   0        0        0      478 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-cextension-in-src/src/my_package/hellomodule.c
--rw-r--r--   0        0        0       12 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-cextension/LICENSE
--rw-r--r--   0        0        0       22 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-cextension/my_package/__init__.py
--rw-r--r--   0        0        0      478 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-cextension/my_package/hellomodule.c
--rw-r--r--   0        0        0      138 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-cextension/pdm.lock
--rw-r--r--   0        0        0      230 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-cextension/pdm_build.py
--rw-r--r--   0        0        0      554 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-cextension/pyproject.toml
--rw-r--r--   0        0        0       12 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-combined-extras/LICENSE
--rw-r--r--   0        0        0       26 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-combined-extras/demo.py
--rw-r--r--   0        0        0      379 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-combined-extras/pyproject.toml
--rw-r--r--   0        0        0       12 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-explicit-package-dir/LICENSE
--rw-r--r--   0        0        0       24 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-explicit-package-dir/README.md
--rw-r--r--   0        0        0       16 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-explicit-package-dir/data_out.json
--rw-r--r--   0        0        0       22 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/data.json
--rw-r--r--   0        0        0      433 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-explicit-package-dir/pyproject.toml
--rw-r--r--   0        0        0       21 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-explicit-package-dir/single_module.py
--rw-r--r--   0        0        0       12 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-module/LICENSE
--rw-r--r--   0        0        0       24 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-module/README.md
--rw-r--r--   0        0        0       14 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-module/bar_module.py
--rw-r--r--   0        0        0       60 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-module/foo_module.py
--rw-r--r--   0        0        0      402 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-module/pyproject.toml
--rw-r--r--   0        0        0       24 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-no-license/README.md
--rw-r--r--   0        0        0      406 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-no-license/pyproject.toml
--rw-r--r--   0        0        0       36 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-no-license/src/foo_module.py
--rw-r--r--   0        0        0        0 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-no-version/README.md
-lrwxr-xr-x   0        0        0        0 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-no-version/anothername.toml -> pyproject.toml
--rw-r--r--   0        0        0      330 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-no-version/pyproject.toml
--rw-r--r--   0        0        0       12 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include-error/LICENSE
--rw-r--r--   0        0        0       24 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include-error/README.md
--rw-r--r--   0        0        0       16 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include-error/data_out.json
--rw-r--r--   0        0        0       22 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include-error/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include-error/my_package/data.json
--rw-r--r--   0        0        0     7700 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include-error/pdm.lock
--rw-r--r--   0        0        0      555 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include-error/pyproject.toml
--rw-r--r--   0        0        0     4259 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include-error/requirements.txt
--rw-r--r--   0        0        0      604 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt
--rw-r--r--   0        0        0       21 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include-error/single_module.py
--rw-r--r--   0        0        0       12 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include/LICENSE
--rw-r--r--   0        0        0       24 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include/README.md
--rw-r--r--   0        0        0       16 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include/data_out.json
--rw-r--r--   0        0        0       22 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include/my_package/data.json
--rw-r--r--   0        0        0     7700 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include/pdm.lock
--rw-r--r--   0        0        0      642 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include/pyproject.toml
--rw-r--r--   0        0        0     4259 2023-12-27 07:00:03.139141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include/requirements.txt
--rw-r--r--   0        0        0      604 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include/requirements_simple.txt
--rwxr-xr-x   0        0        0       32 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include/scripts/data/my_script.sh
--rw-r--r--   0        0        0       21 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include/single_module.py
--rw-r--r--   0        0        0       12 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-with-deep-path/LICENSE
--rw-r--r--   0        0        0       24 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-with-deep-path/README.md
--rw-r--r--   0        0        0       22 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-with-deep-path/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_a.json
--rw-r--r--   0        0        0       16 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_inner/data_b.json
--rw-r--r--   0        0        0      574 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml
--rw-r--r--   0        0        0       12 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-with-tests/LICENSE
--rw-r--r--   0        0        0       24 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-with-tests/README.md
--rw-r--r--   0        0        0       22 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-with-tests/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-with-tests/my_package/data.json
--rw-r--r--   0        0        0     7700 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-with-tests/pdm.lock
--rw-r--r--   0        0        0      513 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-with-tests/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package-with-tests/tests/__init__.py
--rw-r--r--   0        0        0       12 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package/LICENSE
--rw-r--r--   0        0        0       24 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package/README.md
--rw-r--r--   0        0        0       16 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package/data_out.json
--rw-r--r--   0        0        0       22 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package/my_package/data.json
--rwxr-xr-x   0        0        0        0 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package/my_package/executable
--rw-r--r--   0        0        0     2461 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package/pdm.lock
--rw-r--r--   0        0        0      598 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package/pyproject.toml
--rw-r--r--   0        0        0     4259 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package/requirements.txt
--rw-r--r--   0        0        0      604 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package/requirements_simple.txt
--rw-r--r--   0        0        0       21 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-package/single_module.py
--rw-r--r--   0        0        0       12 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-pep420-package/LICENSE
--rw-r--r--   0        0        0       24 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-pep420-package/README.md
--rw-r--r--   0        0        0       22 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-pep420-package/foo/my_package/__init__.py
--rw-r--r--   0        0        0        3 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-pep420-package/foo/my_package/data.json
--rw-r--r--   0        0        0      464 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-pep420-package/pyproject.toml
--rw-r--r--   0        0        0       12 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-purelib-with-build/LICENSE
--rw-r--r--   0        0        0      277 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-purelib-with-build/my_build.py
--rw-r--r--   0        0        0       22 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-purelib-with-build/my_package/__init__.py
--rw-r--r--   0        0        0      138 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-purelib-with-build/pdm.lock
--rw-r--r--   0        0        0      549 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml
--rw-r--r--   0        0        0       26 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-reuse-spec/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0       24 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-reuse-spec/README.md
--rw-r--r--   0        0        0      413 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-reuse-spec/pyproject.toml
--rw-r--r--   0        0        0       36 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-reuse-spec/src/foo_module.py
--rw-r--r--   0        0        0       12 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-src-package-include/LICENSE
--rw-r--r--   0        0        0       24 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-src-package-include/README.md
--rw-r--r--   0        0        0       16 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-src-package-include/data_out.json
--rw-r--r--   0        0        0      500 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-src-package-include/pyproject.toml
--rw-r--r--   0        0        0       21 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-src-package-include/single_module.py
--rw-r--r--   0        0        0       22 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-src-package-include/sub/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-src-package-include/sub/my_package/data.json
--rw-r--r--   0        0        0       12 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-src-package/LICENSE
--rw-r--r--   0        0        0       24 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-src-package/README.md
--rw-r--r--   0        0        0       16 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-src-package/data_out.json
--rw-r--r--   0        0        0      395 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-src-package/pyproject.toml
--rw-r--r--   0        0        0       21 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-src-package/single_module.py
--rw-r--r--   0        0        0       22 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-src-package/src/my_package/data.json
--rw-r--r--   0        0        0       12 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-src-pymodule/LICENSE
--rw-r--r--   0        0        0       24 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-src-pymodule/README.md
--rw-r--r--   0        0        0      406 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-src-pymodule/pyproject.toml
--rw-r--r--   0        0        0       36 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-src-pymodule/src/foo_module.py
--rw-r--r--   0        0        0       36 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-using-scm/.gitignore
--rw-r--r--   0        0        0       12 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-using-scm/LICENSE
--rw-r--r--   0        0        0       24 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-using-scm/README.md
--rw-r--r--   0        0        0       36 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-using-scm/foo/__init__.py
--rw-r--r--   0        0        0      369 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/fixtures/projects/demo-using-scm/pyproject.toml
--rw-r--r--   0        0        0    18806 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/test_api.py
--rw-r--r--   0        0        0     5324 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/test_file_finder.py
--rw-r--r--   0        0        0     1632 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/test_hooks.py
--rw-r--r--   0        0        0     3058 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/test_metadata.py
--rw-r--r--   0        0        0      748 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/test_utils.py
--rw-r--r--   0        0        0     1176 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/test_wheel.py
--rw-r--r--   0        0        0      318 2023-12-27 07:00:03.143141 pdm_backend-2.1.8/tests/testutils.py
--rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 pdm_backend-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-14 07:54:30.319984 pdm_backend-2.2.0/LICENSE
+-rw-r--r--   0        0        0     1711 2024-04-14 07:54:30.319984 pdm_backend-2.2.0/README.md
+-rw-r--r--   0        0        0     2326 2024-04-14 07:54:48.572017 pdm_backend-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3286 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/__init__.py
+-rw-r--r--   0        0        0      197 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/LICENSE
+-rw-r--r--   0        0        0    10174 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/LICENSE.BSD
+-rw-r--r--   0        0        0      496 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_elffile.py
+-rw-r--r--   0        0        0     9590 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2676 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0    10347 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     5292 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8208 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0    33036 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/metadata.py
+-rw-r--r--   0        0        0        0 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/py.typed
+-rw-r--r--   0        0        0     2933 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    39824 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    18950 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     5268 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16256 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     1113 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/pyproject_metadata/LICENSE
+-rw-r--r--   0        0        0    20891 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/pyproject_metadata/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/pyproject_metadata/py.typed
+-rw-r--r--   0        0        0     1072 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli/LICENSE
+-rw-r--r--   0        0        0      396 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0       26 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli/py.typed
+-rw-r--r--   0        0        0     1072 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli_w/LICENSE
+-rw-r--r--   0        0        0      177 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli_w/__init__.py
+-rw-r--r--   0        0        0     6132 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli_w/_writer.py
+-rw-r--r--   0        0        0       26 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli_w/py.typed
+-rw-r--r--   0        0        0       73 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/vendor.txt
+-rw-r--r--   0        0        0    12629 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/base.py
+-rw-r--r--   0        0        0     9872 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/config.py
+-rw-r--r--   0        0        0     3674 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/editable.py
+-rw-r--r--   0        0        0      452 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/exceptions.py
+-rw-r--r--   0        0        0      108 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/hooks/__init__.py
+-rw-r--r--   0        0        0     4593 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/hooks/base.py
+-rw-r--r--   0        0        0     6459 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/hooks/setuptools.py
+-rw-r--r--   0        0        0     5296 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/hooks/version/__init__.py
+-rw-r--r--   0        0        0    10153 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/hooks/version/scm.py
+-rw-r--r--   0        0        0     1037 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/intree.py
+-rw-r--r--   0        0        0    14959 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/macosx_platform.py
+-rw-r--r--   0        0        0        0 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/py.typed
+-rw-r--r--   0        0        0     3050 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/sdist.py
+-rw-r--r--   0        0        0     1381 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/structures.py
+-rw-r--r--   0        0        0     8985 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/utils.py
+-rw-r--r--   0        0        0    11818 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/src/pdm/backend/wheel.py
+-rw-r--r--   0        0        0       72 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      929 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/conftest.py
+-rw-r--r--   0        0        0      856 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/hooks/hook_class.py
+-rw-r--r--   0        0        0      599 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/hooks/hook_module.py
+-rw-r--r--   0        0        0      599 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/hooks/local_hook.py
+-rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension-in-src/LICENSE
+-rw-r--r--   0        0        0      138 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension-in-src/pdm.lock
+-rw-r--r--   0        0        0      234 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension-in-src/pdm_build.py
+-rw-r--r--   0        0        0      558 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension-in-src/src/my_package/__init__.py
+-rw-r--r--   0        0        0      478 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension-in-src/src/my_package/hellomodule.c
+-rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension/LICENSE
+-rw-r--r--   0        0        0       22 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension/my_package/__init__.py
+-rw-r--r--   0        0        0      478 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension/my_package/hellomodule.c
+-rw-r--r--   0        0        0      138 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension/pdm.lock
+-rw-r--r--   0        0        0      230 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension/pdm_build.py
+-rw-r--r--   0        0        0      554 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-combined-extras/LICENSE
+-rw-r--r--   0        0        0       26 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-combined-extras/demo.py
+-rw-r--r--   0        0        0      379 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-combined-extras/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-explicit-package-dir/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-explicit-package-dir/README.md
+-rw-r--r--   0        0        0       16 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-explicit-package-dir/data_out.json
+-rw-r--r--   0        0        0       22 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/data.json
+-rw-r--r--   0        0        0      433 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-explicit-package-dir/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-explicit-package-dir/single_module.py
+-rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-metadata-test/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-metadata-test/README.md
+-rw-r--r--   0        0        0      407 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-metadata-test/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-module/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-module/README.md
+-rw-r--r--   0        0        0       14 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-module/bar_module.py
+-rw-r--r--   0        0        0       60 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-module/foo_module.py
+-rw-r--r--   0        0        0      402 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-module/pyproject.toml
+-rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-no-license/README.md
+-rw-r--r--   0        0        0      406 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-no-license/pyproject.toml
+-rw-r--r--   0        0        0       36 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-no-license/src/foo_module.py
+-rw-r--r--   0        0        0        0 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-no-version/README.md
+lrwxr-xr-x   0        0        0        0 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-no-version/anothername.toml -> pyproject.toml
+-rw-r--r--   0        0        0      330 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-no-version/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/README.md
+-rw-r--r--   0        0        0       16 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/data_out.json
+-rw-r--r--   0        0        0       22 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/my_package/data.json
+-rw-r--r--   0        0        0     7700 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/pdm.lock
+-rw-r--r--   0        0        0      555 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/pyproject.toml
+-rw-r--r--   0        0        0     4259 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/requirements.txt
+-rw-r--r--   0        0        0      604 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt
+-rw-r--r--   0        0        0       21 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/single_module.py
+-rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/README.md
+-rw-r--r--   0        0        0       16 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/data_out.json
+-rw-r--r--   0        0        0       22 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/my_package/data.json
+-rw-r--r--   0        0        0     7700 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/pdm.lock
+-rw-r--r--   0        0        0      642 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/pyproject.toml
+-rw-r--r--   0        0        0     4259 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/requirements.txt
+-rw-r--r--   0        0        0      604 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/requirements_simple.txt
+-rwxr-xr-x   0        0        0       32 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/scripts/data/my_script.sh
+-rw-r--r--   0        0        0       21 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/single_module.py
+-rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-deep-path/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-deep-path/README.md
+-rw-r--r--   0        0        0       22 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-deep-path/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_a.json
+-rw-r--r--   0        0        0       16 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_inner/data_b.json
+-rw-r--r--   0        0        0      574 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-tests/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-tests/README.md
+-rw-r--r--   0        0        0       22 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-tests/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-tests/my_package/data.json
+-rw-r--r--   0        0        0     7700 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-tests/pdm.lock
+-rw-r--r--   0        0        0      513 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-tests/tests/__init__.py
+-rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package/README.md
+-rw-r--r--   0        0        0       16 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package/data_out.json
+-rw-r--r--   0        0        0       22 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package/my_package/data.json
+-rwxr-xr-x   0        0        0        0 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package/my_package/executable
+-rw-r--r--   0        0        0     2461 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package/pdm.lock
+-rw-r--r--   0        0        0      598 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package/pyproject.toml
+-rw-r--r--   0        0        0     4259 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package/requirements.txt
+-rw-r--r--   0        0        0      604 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package/requirements_simple.txt
+-rw-r--r--   0        0        0       21 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package/single_module.py
+-rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-pep420-package/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-pep420-package/README.md
+-rw-r--r--   0        0        0       22 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-pep420-package/foo/my_package/__init__.py
+-rw-r--r--   0        0        0        3 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-pep420-package/foo/my_package/data.json
+-rw-r--r--   0        0        0      464 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-pep420-package/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-purelib-with-build/LICENSE
+-rw-r--r--   0        0        0      277 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-purelib-with-build/my_build.py
+-rw-r--r--   0        0        0       22 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-purelib-with-build/my_package/__init__.py
+-rw-r--r--   0        0        0      138 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-purelib-with-build/pdm.lock
+-rw-r--r--   0        0        0      549 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml
+-rw-r--r--   0        0        0       26 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-reuse-spec/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0       24 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-reuse-spec/README.md
+-rw-r--r--   0        0        0      413 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-reuse-spec/pyproject.toml
+-rw-r--r--   0        0        0       36 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-reuse-spec/src/foo_module.py
+-rw-r--r--   0        0        0       12 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package-include/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package-include/README.md
+-rw-r--r--   0        0        0       16 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package-include/data_out.json
+-rw-r--r--   0        0        0      500 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package-include/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package-include/single_module.py
+-rw-r--r--   0        0        0       22 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package-include/sub/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package-include/sub/my_package/data.json
+-rw-r--r--   0        0        0       12 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package/README.md
+-rw-r--r--   0        0        0       16 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package/data_out.json
+-rw-r--r--   0        0        0      395 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package/single_module.py
+-rw-r--r--   0        0        0       22 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package/src/my_package/data.json
+-rw-r--r--   0        0        0       12 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-pymodule/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-pymodule/README.md
+-rw-r--r--   0        0        0      406 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-pymodule/pyproject.toml
+-rw-r--r--   0        0        0       36 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-pymodule/src/foo_module.py
+-rw-r--r--   0        0        0       36 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-using-scm/.gitignore
+-rw-r--r--   0        0        0       12 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-using-scm/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-using-scm/README.md
+-rw-r--r--   0        0        0       36 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-using-scm/foo/__init__.py
+-rw-r--r--   0        0        0      369 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-using-scm/pyproject.toml
+-rw-r--r--   0        0        0      156 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-using-scm/version.py
+-rw-r--r--   0        0        0    20060 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/test_api.py
+-rw-r--r--   0        0        0     5324 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/test_file_finder.py
+-rw-r--r--   0        0        0     1632 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/test_hooks.py
+-rw-r--r--   0        0        0     3058 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/test_metadata.py
+-rw-r--r--   0        0        0      748 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1176 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/test_wheel.py
+-rw-r--r--   0        0        0      318 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/testutils.py
+-rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 pdm_backend-2.2.0/PKG-INFO
```

### Comparing `pdm_backend-2.1.8/LICENSE` & `pdm_backend-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/README.md` & `pdm_backend-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/pyproject.toml` & `pdm_backend-2.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -21,60 +21,55 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "importlib-metadata>=3.6; python_version < \"3.10\"",
 ]
-version = "2.1.8"
+version = "2.2.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/pdm-project/pdm-backend"
 Repository = "https://github.com/pdm-project/pdm-backend"
 Documentation = "https://backend.pdm-project.org"
 
-[tool.pdm.version]
-source = "scm"
-
-[tool.pdm.build]
-includes = [
+[build-system]
+requires = []
+build-backend = "pdm.backend.intree"
+backend-path = [
     "src",
 ]
-package-dir = "src"
-source-includes = [
-    "tests",
-]
 
-[tool.pdm.dev-dependencies]
-test = [
-    "pytest",
-    "pytest-cov",
-    "pytest-xdist",
-    "setuptools",
+[tool.ruff]
+src = [
+    "src",
 ]
-dev = [
-    "editables",
-    "vendoring; python_version ~= '3.8'",
+target-version = "py38"
+exclude = [
+    "tests/fixtures",
 ]
-docs = [
-    "mkdocs>=1.4.2",
-    "mkdocstrings[python]>=0.19.0",
-    "mkdocs-material>=8.5.10",
+
+[tool.ruff.lint]
+extend-select = [
+    "I",
+    "C4",
+    "W",
+    "YTT",
 ]
 
-[tool.pdm.scripts]
-build = "python scripts/build.py"
-docs = "mkdocs serve"
+[tool.ruff.lint.mccabe]
+max-complexity = 10
 
-[tool.black]
-line-length = 88
-exclude = "/(\n    \\.eggs\n  | \\.git\n  | \\.mypy_cache\n  | build\n  | dist\n  | __pypackages__\n  | pdm/backend/_vendor\n)/\n"
+[tool.ruff.lint.isort]
+known-first-party = [
+    "pdm.backend",
+]
 
 [tool.vendoring]
 destination = "src/pdm/backend/_vendor/"
 requirements = "src/pdm/backend/_vendor/vendor.txt"
 namespace = "pdm.backend._vendor"
 patches-dir = "scripts/patches"
 protected-files = [
@@ -90,19 +85,40 @@
     "*.so",
     "typing.*",
     "*/tests/",
     "**/test_*.py",
     "**/*_test.py",
 ]
 
-[tool.vendoring.typing-stubs]
-
-[tool.vendoring.license.directories]
-
-[tool.vendoring.license.fallback-urls]
+[tool.pdm.version]
+source = "scm"
 
-[build-system]
-requires = []
-build-backend = "pdm.backend.intree"
-backend-path = [
+[tool.pdm.build]
+includes = [
     "src",
 ]
+package-dir = "src"
+source-includes = [
+    "tests",
+]
+
+[tool.pdm.dev-dependencies]
+test = [
+    "pytest",
+    "pytest-cov",
+    "pytest-xdist",
+    "setuptools",
+]
+dev = [
+    "editables",
+    "vendoring; python_version ~= '3.8'",
+]
+docs = [
+    "mkdocs>=1.4.2",
+    "mkdocstrings[python]>=0.19.0",
+    "mkdocs-material>=8.5.10",
+    "mkdocs-version-annotations>=1.0.0",
+]
+
+[tool.pdm.scripts]
+build = "python scripts/build.py"
+docs = "mkdocs serve"
```

### Comparing `pdm_backend-2.1.8/src/pdm/backend/__init__.py` & `pdm_backend-2.2.0/src/pdm/backend/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 PEP-517 compliant pyproject build-system API
 """
+
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Any, Mapping
 
 
 def get_requires_for_build_wheel(
-    config_settings: Mapping[str, Any] | None = None
+    config_settings: Mapping[str, Any] | None = None,
 ) -> list[str]:
     """
     Returns an additional list of requirements for building, as PEP508 strings,
     above and beyond those specified in the pyproject.toml file.
 
     When C-extension build is needed, setuptools should be required, otherwise
     just return an empty list.
@@ -22,15 +23,15 @@
     with WheelBuilder(Path.cwd(), config_settings) as builder:
         if builder.config.build_config.run_setuptools:
             return ["setuptools>=40.8.0"]
         return []
 
 
 def get_requires_for_build_sdist(
-    config_settings: Mapping[str, Any] | None = None
+    config_settings: Mapping[str, Any] | None = None,
 ) -> list[str]:
     """There isn't any requirement for building a sdist at this point."""
     return []
 
 
 def prepare_metadata_for_build_wheel(
     metadata_directory: str, config_settings: Mapping[str, Any] | None = None
@@ -63,15 +64,15 @@
     from pdm.backend.sdist import SdistBuilder
 
     with SdistBuilder(Path.cwd(), config_settings) as builder:
         return builder.build(sdist_directory).name
 
 
 def get_requires_for_build_editable(
-    config_settings: Mapping[str, Any] | None = None
+    config_settings: Mapping[str, Any] | None = None,
 ) -> list[str]:
     """
     Returns an additional list of requirements for building, as PEP508 strings,
     above and beyond those specified in the pyproject.toml file.
 
     When C-extension build is needed, setuptools should be required, otherwise
     just return an empty list.
```

### Comparing `pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/LICENSE.APACHE` & `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/LICENSE.BSD` & `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/_elffile.py` & `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_elffile.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         except struct.error:
             raise ELFInvalid("unable to parse identification")
         magic = bytes(ident[:4])
         if magic != b"\x7fELF":
             raise ELFInvalid(f"invalid magic: {magic!r}")
 
         self.capacity = ident[4]  # Format for program header (bitness).
-        self.encoding = ident[5]  # Data structure encoding (endianess).
+        self.encoding = ident[5]  # Data structure encoding (endianness).
 
         try:
             # e_fmt: Format for program header.
             # p_fmt: Format for section header.
             # p_idx: Indexes to find p_type, p_offset, and p_filesz.
             e_fmt, self._p_fmt, self._p_idx = {
                 (1, 1): ("<HHIIIIIHHH", "<IIIIIIII", (0, 1, 4)),  # 32-bit LSB.
```

### Comparing `pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/_manylinux.py` & `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_manylinux.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import collections
 import contextlib
 import functools
 import os
 import re
 import sys
 import warnings
-from typing import Dict, Generator, Iterator, NamedTuple, Optional, Tuple
+from typing import Dict, Generator, Iterator, NamedTuple, Optional, Sequence, Tuple
 
 from ._elffile import EIClass, EIData, ELFFile, EMachine
 
 EF_ARM_ABIMASK = 0xFF000000
 EF_ARM_ABI_VER5 = 0x05000000
 EF_ARM_ABI_FLOAT_HARD = 0x00000400
 
 
+# `os.PathLike` not a generic type until Python 3.9, so sticking with `str`
+# as the type for `path` until then.
 @contextlib.contextmanager
 def _parse_elf(path: str) -> Generator[Optional[ELFFile], None, None]:
     try:
         with open(path, "rb") as f:
             yield ELFFile(f)
     except (OSError, TypeError, ValueError):
         yield None
@@ -44,20 +46,29 @@
             f is not None
             and f.capacity == EIClass.C32
             and f.encoding == EIData.Lsb
             and f.machine == EMachine.I386
         )
 
 
-def _have_compatible_abi(executable: str, arch: str) -> bool:
-    if arch == "armv7l":
+def _have_compatible_abi(executable: str, archs: Sequence[str]) -> bool:
+    if "armv7l" in archs:
         return _is_linux_armhf(executable)
-    if arch == "i686":
+    if "i686" in archs:
         return _is_linux_i686(executable)
-    return arch in {"x86_64", "aarch64", "ppc64", "ppc64le", "s390x"}
+    allowed_archs = {
+        "x86_64",
+        "aarch64",
+        "ppc64",
+        "ppc64le",
+        "s390x",
+        "loongarch64",
+        "riscv64",
+    }
+    return any(arch in allowed_archs for arch in archs)
 
 
 # If glibc ever changes its major version, we need to know what the last
 # minor version was, so we can build the complete list of all versions.
 # For now, guess what the highest minor version might be, assume it will
 # be 50 for testing. Once this actually happens, update the dictionary
 # with the actual value.
@@ -75,15 +86,15 @@
     """
     # os.confstr is quite a bit faster than ctypes.DLL. It's also less likely
     # to be broken or missing. This strategy is used in the standard library
     # platform module.
     # https://github.com/python/cpython/blob/fcf1d003bf4f0100c/Lib/platform.py#L175-L183
     try:
         # Should be a string like "glibc 2.17".
-        version_string: str = getattr(os, "confstr")("CS_GNU_LIBC_VERSION")
+        version_string: Optional[str] = os.confstr("CS_GNU_LIBC_VERSION")
         assert version_string is not None
         _, version = version_string.rsplit()
     except (AssertionError, AttributeError, OSError, ValueError):
         # os.confstr() or CS_GNU_LIBC_VERSION not available (or a bad value)...
         return None
     return version
 
@@ -161,21 +172,21 @@
     version_str = _glibc_version_string()
     if version_str is None:
         return (-1, -1)
     return _parse_glibc_version(version_str)
 
 
 # From PEP 513, PEP 600
-def _is_compatible(name: str, arch: str, version: _GLibCVersion) -> bool:
+def _is_compatible(arch: str, version: _GLibCVersion) -> bool:
     sys_glibc = _get_glibc_version()
     if sys_glibc < version:
         return False
     # Check for presence of _manylinux module.
     try:
-        import _manylinux  # noqa
+        import _manylinux
     except ImportError:
         return True
     if hasattr(_manylinux, "manylinux_compatible"):
         result = _manylinux.manylinux_compatible(version[0], version[1], arch)
         if result is not None:
             return bool(result)
         return True
@@ -197,42 +208,53 @@
     # CentOS 6 w/ glibc 2.12 (PEP 571)
     (2, 12): "manylinux2010",
     # CentOS 5 w/ glibc 2.5 (PEP 513)
     (2, 5): "manylinux1",
 }
 
 
-def platform_tags(linux: str, arch: str) -> Iterator[str]:
-    if not _have_compatible_abi(sys.executable, arch):
+def platform_tags(archs: Sequence[str]) -> Iterator[str]:
+    """Generate manylinux tags compatible to the current platform.
+
+    :param archs: Sequence of compatible architectures.
+        The first one shall be the closest to the actual architecture and be the part of
+        platform tag after the ``linux_`` prefix, e.g. ``x86_64``.
+        The ``linux_`` prefix is assumed as a prerequisite for the current platform to
+        be manylinux-compatible.
+
+    :returns: An iterator of compatible manylinux tags.
+    """
+    if not _have_compatible_abi(sys.executable, archs):
         return
     # Oldest glibc to be supported regardless of architecture is (2, 17).
     too_old_glibc2 = _GLibCVersion(2, 16)
-    if arch in {"x86_64", "i686"}:
+    if set(archs) & {"x86_64", "i686"}:
         # On x86/i686 also oldest glibc to be supported is (2, 5).
         too_old_glibc2 = _GLibCVersion(2, 4)
     current_glibc = _GLibCVersion(*_get_glibc_version())
     glibc_max_list = [current_glibc]
     # We can assume compatibility across glibc major versions.
     # https://sourceware.org/bugzilla/show_bug.cgi?id=24636
     #
     # Build a list of maximum glibc versions so that we can
     # output the canonical list of all glibc from current_glibc
     # down to too_old_glibc2, including all intermediary versions.
     for glibc_major in range(current_glibc.major - 1, 1, -1):
         glibc_minor = _LAST_GLIBC_MINOR[glibc_major]
         glibc_max_list.append(_GLibCVersion(glibc_major, glibc_minor))
-    for glibc_max in glibc_max_list:
-        if glibc_max.major == too_old_glibc2.major:
-            min_minor = too_old_glibc2.minor
-        else:
-            # For other glibc major versions oldest supported is (x, 0).
-            min_minor = -1
-        for glibc_minor in range(glibc_max.minor, min_minor, -1):
-            glibc_version = _GLibCVersion(glibc_max.major, glibc_minor)
-            tag = "manylinux_{}_{}".format(*glibc_version)
-            if _is_compatible(tag, arch, glibc_version):
-                yield linux.replace("linux", tag)
-            # Handle the legacy manylinux1, manylinux2010, manylinux2014 tags.
-            if glibc_version in _LEGACY_MANYLINUX_MAP:
-                legacy_tag = _LEGACY_MANYLINUX_MAP[glibc_version]
-                if _is_compatible(legacy_tag, arch, glibc_version):
-                    yield linux.replace("linux", legacy_tag)
+    for arch in archs:
+        for glibc_max in glibc_max_list:
+            if glibc_max.major == too_old_glibc2.major:
+                min_minor = too_old_glibc2.minor
+            else:
+                # For other glibc major versions oldest supported is (x, 0).
+                min_minor = -1
+            for glibc_minor in range(glibc_max.minor, min_minor, -1):
+                glibc_version = _GLibCVersion(glibc_max.major, glibc_minor)
+                tag = "manylinux_{}_{}".format(*glibc_version)
+                if _is_compatible(arch, glibc_version):
+                    yield f"{tag}_{arch}"
+                # Handle the legacy manylinux1, manylinux2010, manylinux2014 tags.
+                if glibc_version in _LEGACY_MANYLINUX_MAP:
+                    legacy_tag = _LEGACY_MANYLINUX_MAP[glibc_version]
+                    if _is_compatible(arch, glibc_version):
+                        yield f"{legacy_tag}_{arch}"
```

### Comparing `pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/_musllinux.py` & `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_musllinux.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 linked against musl, and what musl version is used.
 """
 
 import functools
 import re
 import subprocess
 import sys
-from typing import Iterator, NamedTuple, Optional
+from typing import Iterator, NamedTuple, Optional, Sequence
 
 from ._elffile import ELFFile
 
 
 class _MuslVersion(NamedTuple):
     major: int
     minor: int
@@ -43,32 +43,35 @@
     try:
         with open(executable, "rb") as f:
             ld = ELFFile(f).interpreter
     except (OSError, TypeError, ValueError):
         return None
     if ld is None or "musl" not in ld:
         return None
-    proc = subprocess.run([ld], stderr=subprocess.PIPE, universal_newlines=True)
+    proc = subprocess.run([ld], stderr=subprocess.PIPE, text=True)
     return _parse_musl_version(proc.stderr)
 
 
-def platform_tags(arch: str) -> Iterator[str]:
+def platform_tags(archs: Sequence[str]) -> Iterator[str]:
     """Generate musllinux tags compatible to the current platform.
 
-    :param arch: Should be the part of platform tag after the ``linux_``
-        prefix, e.g. ``x86_64``. The ``linux_`` prefix is assumed as a
-        prerequisite for the current platform to be musllinux-compatible.
+    :param archs: Sequence of compatible architectures.
+        The first one shall be the closest to the actual architecture and be the part of
+        platform tag after the ``linux_`` prefix, e.g. ``x86_64``.
+        The ``linux_`` prefix is assumed as a prerequisite for the current platform to
+        be musllinux-compatible.
 
     :returns: An iterator of compatible musllinux tags.
     """
     sys_musl = _get_musl_version(sys.executable)
     if sys_musl is None:  # Python not dynamically linked against musl.
         return
-    for minor in range(sys_musl.minor, -1, -1):
-        yield f"musllinux_{sys_musl.major}_{minor}_{arch}"
+    for arch in archs:
+        for minor in range(sys_musl.minor, -1, -1):
+            yield f"musllinux_{sys_musl.major}_{minor}_{arch}"
 
 
 if __name__ == "__main__":  # pragma: no cover
     import sysconfig
 
     plat = sysconfig.get_platform()
     assert plat.startswith("linux-"), "not linux"
```

### Comparing `pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/_parser.py` & `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         return str(self)
 
 
 MarkerVar = Union[Variable, Value]
 MarkerItem = Tuple[MarkerVar, Op, MarkerVar]
 # MarkerAtom = Union[MarkerItem, List["MarkerAtom"]]
 # MarkerList = List[Union["MarkerList", MarkerAtom, str]]
-# mypy does not suport recursive type definition
+# mypy does not support recursive type definition
 # https://github.com/python/mypy/issues/731
 MarkerAtom = Any
 MarkerList = List[Any]
 
 
 class ParsedRequirement(NamedTuple):
     name: str
@@ -85,15 +85,15 @@
     return ParsedRequirement(name, url, extras, specifier, marker)
 
 
 def _parse_requirement_details(
     tokenizer: Tokenizer,
 ) -> Tuple[str, str, Optional[MarkerList]]:
     """
-    requirement_details = AT URL (WS requirement_marker)?
+    requirement_details = AT URL (WS requirement_marker?)?
                         | specifier WS? (requirement_marker)?
     """
 
     specifier = ""
     url = ""
     marker = None
 
@@ -104,14 +104,18 @@
         url_start = tokenizer.position
         url = tokenizer.expect("URL", expected="URL after @").text
         if tokenizer.check("END", peek=True):
             return (url, specifier, marker)
 
         tokenizer.expect("WS", expected="whitespace after URL")
 
+        # The input might end after whitespace.
+        if tokenizer.check("END", peek=True):
+            return (url, specifier, marker)
+
         marker = _parse_requirement_marker(
             tokenizer, span_start=url_start, after="URL and whitespace"
         )
     else:
         specifier_start = tokenizer.position
         specifier = _parse_specifier(tokenizer)
         tokenizer.consume("WS")
@@ -140,31 +144,34 @@
     """
 
     if not tokenizer.check("SEMICOLON"):
         tokenizer.raise_syntax_error(
             f"Expected end or semicolon (after {after})",
             span_start=span_start,
         )
-    else:
-        tokenizer.read()
+    tokenizer.read()
 
     marker = _parse_marker(tokenizer)
     tokenizer.consume("WS")
 
     return marker
 
 
 def _parse_extras(tokenizer: Tokenizer) -> List[str]:
     """
     extras = (LEFT_BRACKET wsp* extras_list? wsp* RIGHT_BRACKET)?
     """
     if not tokenizer.check("LEFT_BRACKET", peek=True):
         return []
 
-    with tokenizer.enclosing_tokens("LEFT_BRACKET", "RIGHT_BRACKET"):
+    with tokenizer.enclosing_tokens(
+        "LEFT_BRACKET",
+        "RIGHT_BRACKET",
+        around="extras",
+    ):
         tokenizer.consume("WS")
         extras = _parse_extras_list(tokenizer)
         tokenizer.consume("WS")
 
     return extras
 
 
@@ -196,51 +203,66 @@
 
 
 def _parse_specifier(tokenizer: Tokenizer) -> str:
     """
     specifier = LEFT_PARENTHESIS WS? version_many WS? RIGHT_PARENTHESIS
               | WS? version_many WS?
     """
-    with tokenizer.enclosing_tokens("LEFT_PARENTHESIS", "RIGHT_PARENTHESIS"):
+    with tokenizer.enclosing_tokens(
+        "LEFT_PARENTHESIS",
+        "RIGHT_PARENTHESIS",
+        around="version specifier",
+    ):
         tokenizer.consume("WS")
         parsed_specifiers = _parse_version_many(tokenizer)
         tokenizer.consume("WS")
 
     return parsed_specifiers
 
 
 def _parse_version_many(tokenizer: Tokenizer) -> str:
     """
-    version_many = (OP VERSION (COMMA OP VERSION)*)?
+    version_many = (SPECIFIER (WS? COMMA WS? SPECIFIER)*)?
     """
     parsed_specifiers = ""
-    while tokenizer.check("OP"):
+    while tokenizer.check("SPECIFIER"):
+        span_start = tokenizer.position
         parsed_specifiers += tokenizer.read().text
-
-        # We intentionally do not consume whitespace here, since the regular expression
-        # for `VERSION` uses a lookback for the operator, to determine what
-        # corresponding syntax is permitted.
-
-        version_token = tokenizer.expect("VERSION", expected="version after operator")
-        parsed_specifiers += version_token.text
+        if tokenizer.check("VERSION_PREFIX_TRAIL", peek=True):
+            tokenizer.raise_syntax_error(
+                ".* suffix can only be used with `==` or `!=` operators",
+                span_start=span_start,
+                span_end=tokenizer.position + 1,
+            )
+        if tokenizer.check("VERSION_LOCAL_LABEL_TRAIL", peek=True):
+            tokenizer.raise_syntax_error(
+                "Local version label can only be used with `==` or `!=` operators",
+                span_start=span_start,
+                span_end=tokenizer.position,
+            )
         tokenizer.consume("WS")
-
         if not tokenizer.check("COMMA"):
             break
         parsed_specifiers += tokenizer.read().text
         tokenizer.consume("WS")
 
     return parsed_specifiers
 
 
 # --------------------------------------------------------------------------------------
 # Recursive descent parser for marker expression
 # --------------------------------------------------------------------------------------
 def parse_marker(source: str) -> MarkerList:
-    return _parse_marker(Tokenizer(source, rules=DEFAULT_RULES))
+    return _parse_full_marker(Tokenizer(source, rules=DEFAULT_RULES))
+
+
+def _parse_full_marker(tokenizer: Tokenizer) -> MarkerList:
+    retval = _parse_marker(tokenizer)
+    tokenizer.expect("END", expected="end of marker expression")
+    return retval
 
 
 def _parse_marker(tokenizer: Tokenizer) -> MarkerList:
     """
     marker = marker_atom (BOOLOP marker_atom)+
     """
     expression = [_parse_marker_atom(tokenizer)]
@@ -255,15 +277,19 @@
     """
     marker_atom = WS? LEFT_PARENTHESIS WS? marker WS? RIGHT_PARENTHESIS WS?
                 | WS? marker_item WS?
     """
 
     tokenizer.consume("WS")
     if tokenizer.check("LEFT_PARENTHESIS", peek=True):
-        with tokenizer.enclosing_tokens("LEFT_PARENTHESIS", "RIGHT_PARENTHESIS"):
+        with tokenizer.enclosing_tokens(
+            "LEFT_PARENTHESIS",
+            "RIGHT_PARENTHESIS",
+            around="marker expression",
+        ):
             tokenizer.consume("WS")
             marker: MarkerAtom = _parse_marker(tokenizer)
             tokenizer.consume("WS")
     else:
         marker = _parse_marker_item(tokenizer)
     tokenizer.consume("WS")
     return marker
@@ -294,18 +320,15 @@
     else:
         tokenizer.raise_syntax_error(
             message="Expected a marker variable or quoted string"
         )
 
 
 def process_env_var(env_var: str) -> Variable:
-    if (
-        env_var == "platform_python_implementation"
-        or env_var == "python_implementation"
-    ):
+    if env_var in ("platform_python_implementation", "python_implementation"):
         return Variable("platform_python_implementation")
     else:
         return Variable(env_var)
 
 
 def process_python_str(python_str: str) -> Value:
     value = ast.literal_eval(python_str)
```

### Comparing `pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/_structures.py` & `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/_tokenizer.py` & `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
     def __str__(self) -> str:
         marker = " " * self.span[0] + "~" * (self.span[1] - self.span[0]) + "^"
         return "\n    ".join([self.message, self.source, marker])
 
 
 DEFAULT_RULES: "Dict[str, Union[str, re.Pattern[str]]]" = {
-    "LPAREN": r"\s*\(",
     "LEFT_PARENTHESIS": r"\(",
     "RIGHT_PARENTHESIS": r"\)",
     "LEFT_BRACKET": r"\[",
     "RIGHT_BRACKET": r"\]",
     "SEMICOLON": r";",
     "COMMA": r",",
     "QUOTED_STRING": re.compile(
@@ -68,18 +67,23 @@
                 |python_implementation
                 |implementation_(name|version)
                 |extra
             )\b
         """,
         re.VERBOSE,
     ),
-    "VERSION": re.compile(Specifier._version_regex_str, re.VERBOSE | re.IGNORECASE),
+    "SPECIFIER": re.compile(
+        Specifier._operator_regex_str + Specifier._version_regex_str,
+        re.VERBOSE | re.IGNORECASE,
+    ),
     "AT": r"\@",
     "URL": r"[^ \t]+",
     "IDENTIFIER": r"\b[a-zA-Z0-9][a-zA-Z0-9._-]*\b",
+    "VERSION_PREFIX_TRAIL": r"\.\*",
+    "VERSION_LOCAL_LABEL_TRAIL": r"\+[a-z0-9]+(?:[-_\.][a-z0-9]+)*",
     "WS": r"[ \t]+",
     "END": r"$",
 }
 
 
 class Tokenizer:
     """Context-sensitive token parsing.
@@ -161,26 +165,28 @@
         raise ParserSyntaxError(
             message,
             source=self.source,
             span=span,
         )
 
     @contextlib.contextmanager
-    def enclosing_tokens(self, open_token: str, close_token: str) -> Iterator[bool]:
+    def enclosing_tokens(
+        self, open_token: str, close_token: str, *, around: str
+    ) -> Iterator[None]:
         if self.check(open_token):
             open_position = self.position
             self.read()
         else:
             open_position = None
 
-        yield open_position is not None
+        yield
 
         if open_position is None:
             return
 
         if not self.check(close_token):
             self.raise_syntax_error(
-                f"Expected closing {close_token}",
+                f"Expected matching {close_token} for {open_token}, after {around}",
                 span_start=open_position,
             )
 
         self.read()
```

### Comparing `pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/markers.py` & `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/markers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,22 @@
 
 import operator
 import os
 import platform
 import sys
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
-from ._parser import MarkerAtom, MarkerList, Op, Value, Variable, parse_marker
+from ._parser import (
+    MarkerAtom,
+    MarkerList,
+    Op,
+    Value,
+    Variable,
+    parse_marker as _parse_marker,
+)
 from ._tokenizer import ParserSyntaxError
 from .specifiers import InvalidSpecifier, Specifier
 from .utils import canonicalize_name
 
 __all__ = [
     "InvalidMarker",
     "UndefinedComparison",
@@ -185,15 +192,15 @@
 
 class Marker:
     def __init__(self, marker: str) -> None:
         # Note: We create a Marker object without calling this constructor in
         #       packaging.requirements.Requirement. If any additional logic is
         #       added here, make sure to mirror/adapt Requirement.
         try:
-            self._markers = _normalize_extra_values(parse_marker(marker))
+            self._markers = _normalize_extra_values(_parse_marker(marker))
             # The attribute `_markers` can be described in terms of a recursive type:
             # MarkerList = List[Union[Tuple[Node, ...], str, MarkerList]]
             #
             # For example, the following expression:
             # python_version > "3.6" or (python_version == "3.6" and os_name == "unix")
             #
             # is parsed into:
@@ -233,9 +240,13 @@
 
         The environment is determined from the current Python process.
         """
         current_environment = default_environment()
         current_environment["extra"] = ""
         if environment is not None:
             current_environment.update(environment)
+            # The API used to allow setting extra to None. We need to handle this
+            # case for backwards compatibility.
+            if current_environment["extra"] is None:
+                current_environment["extra"] = ""
 
         return _evaluate_markers(self._markers, current_environment)
```

### Comparing `pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/specifiers.py` & `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/specifiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,21 @@
     from pdm.backend._vendor.packaging.specifiers import Specifier, SpecifierSet, InvalidSpecifier
     from pdm.backend._vendor.packaging.version import Version
 """
 
 import abc
 import itertools
 import re
-from typing import Callable, Iterable, Iterator, List, Optional, Set, Tuple, Union
+from typing import Callable, Iterable, Iterator, List, Optional, Tuple, TypeVar, Union
 
 from .utils import canonicalize_version
 from .version import Version
 
 UnparsedVersion = Union[Version, str]
+UnparsedVersionVar = TypeVar("UnparsedVersionVar", bound=UnparsedVersion)
 CallableOperator = Callable[[Version, str], bool]
 
 
 def _coerce_version(version: UnparsedVersion) -> Version:
     if not isinstance(version, Version):
         version = Version(version)
     return version
@@ -81,16 +82,16 @@
     def contains(self, item: str, prereleases: Optional[bool] = None) -> bool:
         """
         Determines if the given item is contained within this specifier.
         """
 
     @abc.abstractmethod
     def filter(
-        self, iterable: Iterable[UnparsedVersion], prereleases: Optional[bool] = None
-    ) -> Iterator[UnparsedVersion]:
+        self, iterable: Iterable[UnparsedVersionVar], prereleases: Optional[bool] = None
+    ) -> Iterator[UnparsedVersionVar]:
         """
         Takes an iterable of items and filters them so that only items which
         are contained within this specifier are allowed in it.
         """
 
 
 class Specifier(BaseSpecifier):
@@ -136,15 +137,15 @@
                 # You cannot use a wild card and a pre-release, post-release, a dev or
                 # local version together so group them with a | and make them optional.
                 (?:
                     \.\*  # Wild card syntax of .*
                     |
                     (?:                                  # pre release
                         [-_\.]?
-                        (a|b|c|rc|alpha|beta|pre|preview)
+                        (alpha|beta|preview|pre|a|b|c|rc)
                         [-_\.]?
                         [0-9]*
                     )?
                     (?:                                  # post release
                         (?:-[0-9]+)|(?:[-_\.]?(post|rev|r)[-_\.]?[0-9]*)
                     )?
                     (?:[-_\.]?dev[-_\.]?[0-9]*)?         # dev release
@@ -159,15 +160,15 @@
 
                 \s*
                 v?
                 (?:[0-9]+!)?          # epoch
                 [0-9]+(?:\.[0-9]+)+   # release  (We have a + instead of a *)
                 (?:                   # pre release
                     [-_\.]?
-                    (a|b|c|rc|alpha|beta|pre|preview)
+                    (alpha|beta|preview|pre|a|b|c|rc)
                     [-_\.]?
                     [0-9]*
                 )?
                 (?:                                   # post release
                     (?:-[0-9]+)|(?:[-_\.]?(post|rev|r)[-_\.]?[0-9]*)
                 )?
                 (?:[-_\.]?dev[-_\.]?[0-9]*)?          # dev release
@@ -184,15 +185,15 @@
 
                 \s*
                 v?
                 (?:[0-9]+!)?          # epoch
                 [0-9]+(?:\.[0-9]+)*   # release
                 (?:                   # pre release
                     [-_\.]?
-                    (a|b|c|rc|alpha|beta|pre|preview)
+                    (alpha|beta|preview|pre|a|b|c|rc)
                     [-_\.]?
                     [0-9]*
                 )?
                 (?:                                   # post release
                     (?:-[0-9]+)|(?:[-_\.]?(post|rev|r)[-_\.]?[0-9]*)
                 )?
                 (?:[-_\.]?dev[-_\.]?[0-9]*)?          # dev release
@@ -237,15 +238,16 @@
             match.group("operator").strip(),
             match.group("version").strip(),
         )
 
         # Store whether or not this Specifier should accept prereleases
         self._prereleases = prereleases
 
-    @property
+    # https://github.com/python/mypy/pull/13475#pullrequestreview-1079784515
+    @property  # type: ignore[override]
     def prereleases(self) -> bool:
         # If there is an explicit prereleases set for this, then we'll just
         # blindly use that.
         if self._prereleases is not None:
             return self._prereleases
 
         # Look at all of our specifiers and determine if they are inclusive
@@ -367,15 +369,15 @@
         # is that ~=2.2 is equivalent to >=2.2,==2.*. This allows us to
         # implement this in terms of the other specifiers instead of
         # implementing it ourselves. The only thing we need to do is construct
         # the other specifiers.
 
         # We want everything but the last item in the version, but we want to
         # ignore suffix segments.
-        prefix = ".".join(
+        prefix = _version_join(
             list(itertools.takewhile(_is_not_suffix, _version_split(spec)))[:-1]
         )
 
         # Add the prefix notation to the end of our string
         prefix += ".*"
 
         return self._get_operator(">=")(prospective, spec) and self._get_operator("==")(
@@ -383,24 +385,26 @@
         )
 
     def _compare_equal(self, prospective: Version, spec: str) -> bool:
 
         # We need special logic to handle prefix matching
         if spec.endswith(".*"):
             # In the case of prefix matching we want to ignore local segment.
-            normalized_prospective = canonicalize_version(prospective.public)
+            normalized_prospective = canonicalize_version(
+                prospective.public, strip_trailing_zero=False
+            )
             # Get the normalized version string ignoring the trailing .*
             normalized_spec = canonicalize_version(spec[:-2], strip_trailing_zero=False)
-            # Split the spec out by dots, and pretend that there is an implicit
-            # dot in between a release segment and a pre-release segment.
+            # Split the spec out by bangs and dots, and pretend that there is
+            # an implicit dot in between a release segment and a pre-release segment.
             split_spec = _version_split(normalized_spec)
 
-            # Split the prospective version out by dots, and pretend that there
-            # is an implicit dot in between a release segment and a pre-release
-            # segment.
+            # Split the prospective version out by bangs and dots, and pretend
+            # that there is an implicit dot in between a release segment and
+            # a pre-release segment.
             split_prospective = _version_split(normalized_prospective)
 
             # 0-pad the prospective version before shortening it to get the correct
             # shortened version.
             padded_prospective, _ = _pad_version(split_prospective, split_spec)
 
             # Shorten the prospective version to be the same length as the spec
@@ -561,16 +565,16 @@
 
         # Actually do the comparison to determine if this item is contained
         # within this Specifier or not.
         operator_callable: CallableOperator = self._get_operator(self.operator)
         return operator_callable(normalized_item, self.version)
 
     def filter(
-        self, iterable: Iterable[UnparsedVersion], prereleases: Optional[bool] = None
-    ) -> Iterator[UnparsedVersion]:
+        self, iterable: Iterable[UnparsedVersionVar], prereleases: Optional[bool] = None
+    ) -> Iterator[UnparsedVersionVar]:
         """Filter items in the given iterable, that match the specifier.
 
         :param iterable:
             An iterable that can contain version strings and :class:`Version` instances.
             The items in the iterable will be filtered according to the specifier.
         :param prereleases:
             Whether or not to allow prereleases in the returned iterator. If set to
@@ -602,15 +606,15 @@
         # Attempt to iterate over all the values in the iterable and if any of
         # them match, yield them.
         for version in iterable:
             parsed_version = _coerce_version(version)
 
             if self.contains(parsed_version, **kw):
                 # If our version is a prerelease, and we were not set to allow
-                # prereleases, then we'll store it for later incase nothing
+                # prereleases, then we'll store it for later in case nothing
                 # else matches this specifier.
                 if parsed_version.is_prerelease and not (
                     prereleases or self.prereleases
                 ):
                     found_prereleases.append(version)
                 # Either this is not a prerelease, or we should have been
                 # accepting prereleases from the beginning.
@@ -626,24 +630,46 @@
                 yield version
 
 
 _prefix_regex = re.compile(r"^([0-9]+)((?:a|b|c|rc)[0-9]+)$")
 
 
 def _version_split(version: str) -> List[str]:
+    """Split version into components.
+
+    The split components are intended for version comparison. The logic does
+    not attempt to retain the original version string, so joining the
+    components back with :func:`_version_join` may not produce the original
+    version string.
+    """
     result: List[str] = []
-    for item in version.split("."):
+
+    epoch, _, rest = version.rpartition("!")
+    result.append(epoch or "0")
+
+    for item in rest.split("."):
         match = _prefix_regex.search(item)
         if match:
             result.extend(match.groups())
         else:
             result.append(item)
     return result
 
 
+def _version_join(components: List[str]) -> str:
+    """Join split version components into a version string.
+
+    This function assumes the input came from :func:`_version_split`, where the
+    first component must be the epoch (either empty or numeric), and all other
+    components numeric.
+    """
+    epoch, *rest = components
+    return f"{epoch}!{'.'.join(rest)}"
+
+
 def _is_not_suffix(segment: str) -> bool:
     return not any(
         segment.startswith(prefix) for prefix in ("dev", "a", "b", "rc", "post")
     )
 
 
 def _pad_version(left: List[str], right: List[str]) -> Tuple[List[str], List[str]]:
@@ -657,15 +683,18 @@
     left_split.append(left[len(left_split[0]) :])
     right_split.append(right[len(right_split[0]) :])
 
     # Insert our padding
     left_split.insert(1, ["0"] * max(0, len(right_split[0]) - len(left_split[0])))
     right_split.insert(1, ["0"] * max(0, len(left_split[0]) - len(right_split[0])))
 
-    return (list(itertools.chain(*left_split)), list(itertools.chain(*right_split)))
+    return (
+        list(itertools.chain.from_iterable(left_split)),
+        list(itertools.chain.from_iterable(right_split)),
+    )
 
 
 class SpecifierSet(BaseSpecifier):
     """This class abstracts handling of a set of version specifiers.
 
     It can be passed a single specifier (``>=3.0``), a comma-separated list of
     specifiers (``>=3.0,!=3.1``), or no specifier at all.
@@ -689,22 +718,16 @@
             raised.
         """
 
         # Split on `,` to break each individual specifier into it's own item, and
         # strip each item to remove leading/trailing whitespace.
         split_specifiers = [s.strip() for s in specifiers.split(",") if s.strip()]
 
-        # Parsed each individual specifier, attempting first to make it a
-        # Specifier.
-        parsed: Set[Specifier] = set()
-        for specifier in split_specifiers:
-            parsed.add(Specifier(specifier))
-
-        # Turn our parsed specifiers into a frozen set and save them for later.
-        self._specs = frozenset(parsed)
+        # Make each individual specifier a Specifier and save in a frozen set for later.
+        self._specs = frozenset(map(Specifier, split_specifiers))
 
         # Store our prereleases value so we can use it later to determine if
         # we accept prereleases or not.
         self._prereleases = prereleases
 
     @property
     def prereleases(self) -> Optional[bool]:
@@ -911,16 +934,16 @@
         # We simply dispatch to the underlying specs here to make sure that the
         # given version is contained within all of them.
         # Note: This use of all() here means that an empty set of specifiers
         #       will always return True, this is an explicit design decision.
         return all(s.contains(item, prereleases=prereleases) for s in self._specs)
 
     def filter(
-        self, iterable: Iterable[UnparsedVersion], prereleases: Optional[bool] = None
-    ) -> Iterator[UnparsedVersion]:
+        self, iterable: Iterable[UnparsedVersionVar], prereleases: Optional[bool] = None
+    ) -> Iterator[UnparsedVersionVar]:
         """Filter items in the given iterable, that match the specifiers in this set.
 
         :param iterable:
             An iterable that can contain version strings and :class:`Version` instances.
             The items in the iterable will be filtered according to the specifier.
         :param prereleases:
             Whether or not to allow prereleases in the returned iterator. If set to
@@ -968,16 +991,16 @@
             for spec in self._specs:
                 iterable = spec.filter(iterable, prereleases=bool(prereleases))
             return iter(iterable)
         # If we do not have any specifiers, then we need to have a rough filter
         # which will filter out any pre-releases, unless there are no final
         # releases.
         else:
-            filtered: List[UnparsedVersion] = []
-            found_prereleases: List[UnparsedVersion] = []
+            filtered: List[UnparsedVersionVar] = []
+            found_prereleases: List[UnparsedVersionVar] = []
 
             for item in iterable:
                 parsed_version = _coerce_version(item)
 
                 # Store any item which is a pre-release for later unless we've
                 # already found a final version or we are accepting prereleases
                 if parsed_version.is_prerelease and not prereleases:
```

### Comparing `pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/tags.py` & `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/tags.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
 import logging
 import platform
+import re
+import struct
 import subprocess
 import sys
 import sysconfig
 from importlib.machinery import EXTENSION_SUFFIXES
 from typing import (
     Dict,
     FrozenSet,
@@ -33,15 +35,15 @@
     "cpython": "cp",
     "pypy": "pp",
     "ironpython": "ip",
     "jython": "jy",
 }
 
 
-_32_BIT_INTERPRETER = sys.maxsize <= 2**32
+_32_BIT_INTERPRETER = struct.calcsize("P") == 4
 
 
 class Tag:
     """
     A representation of the tag triple for a wheel.
 
     Instances are considered immutable and thus are hashable. Equality checking
@@ -107,68 +109,82 @@
         for abi in abis.split("."):
             for platform_ in platforms.split("."):
                 tags.add(Tag(interpreter, abi, platform_))
     return frozenset(tags)
 
 
 def _get_config_var(name: str, warn: bool = False) -> Union[int, str, None]:
-    value = sysconfig.get_config_var(name)
+    value: Union[int, str, None] = sysconfig.get_config_var(name)
     if value is None and warn:
         logger.debug(
             "Config variable '%s' is unset, Python ABI tag may be incorrect", name
         )
     return value
 
 
 def _normalize_string(string: str) -> str:
-    return string.replace(".", "_").replace("-", "_")
+    return string.replace(".", "_").replace("-", "_").replace(" ", "_")
 
 
-def _abi3_applies(python_version: PythonVersion) -> bool:
+def _is_threaded_cpython(abis: List[str]) -> bool:
+    """
+    Determine if the ABI corresponds to a threaded (`--disable-gil`) build.
+
+    The threaded builds are indicated by a "t" in the abiflags.
+    """
+    if len(abis) == 0:
+        return False
+    # expect e.g., cp313
+    m = re.match(r"cp\d+(.*)", abis[0])
+    if not m:
+        return False
+    abiflags = m.group(1)
+    return "t" in abiflags
+
+
+def _abi3_applies(python_version: PythonVersion, threading: bool) -> bool:
     """
     Determine if the Python version supports abi3.
 
-    PEP 384 was first implemented in Python 3.2.
+    PEP 384 was first implemented in Python 3.2. The threaded (`--disable-gil`)
+    builds do not support abi3.
     """
-    return len(python_version) > 1 and tuple(python_version) >= (3, 2)
+    return len(python_version) > 1 and tuple(python_version) >= (3, 2) and not threading
 
 
 def _cpython_abis(py_version: PythonVersion, warn: bool = False) -> List[str]:
     py_version = tuple(py_version)  # To allow for version comparison.
     abis = []
     version = _version_nodot(py_version[:2])
-    debug = pymalloc = ucs4 = ""
+    threading = debug = pymalloc = ucs4 = ""
     with_debug = _get_config_var("Py_DEBUG", warn)
     has_refcount = hasattr(sys, "gettotalrefcount")
     # Windows doesn't set Py_DEBUG, so checking for support of debug-compiled
     # extension modules is the best option.
     # https://github.com/pypa/pip/issues/3383#issuecomment-173267692
     has_ext = "_d.pyd" in EXTENSION_SUFFIXES
     if with_debug or (with_debug is None and (has_refcount or has_ext)):
         debug = "d"
+    if py_version >= (3, 13) and _get_config_var("Py_GIL_DISABLED", warn):
+        threading = "t"
     if py_version < (3, 8):
         with_pymalloc = _get_config_var("WITH_PYMALLOC", warn)
         if with_pymalloc or with_pymalloc is None:
             pymalloc = "m"
         if py_version < (3, 3):
             unicode_size = _get_config_var("Py_UNICODE_SIZE", warn)
             if unicode_size == 4 or (
                 unicode_size is None and sys.maxunicode == 0x10FFFF
             ):
                 ucs4 = "u"
     elif debug:
         # Debug builds can also load "normal" extension modules.
         # We can also assume no UCS-4 or pymalloc requirement.
-        abis.append(f"cp{version}")
-    abis.insert(
-        0,
-        "cp{version}{debug}{pymalloc}{ucs4}".format(
-            version=version, debug=debug, pymalloc=pymalloc, ucs4=ucs4
-        ),
-    )
+        abis.append(f"cp{version}{threading}")
+    abis.insert(0, f"cp{version}{threading}{debug}{pymalloc}{ucs4}")
     return abis
 
 
 def cpython_tags(
     python_version: Optional[PythonVersion] = None,
     abis: Optional[Iterable[str]] = None,
     platforms: Optional[Iterable[str]] = None,
@@ -208,31 +224,69 @@
         except ValueError:
             pass
 
     platforms = list(platforms or platform_tags())
     for abi in abis:
         for platform_ in platforms:
             yield Tag(interpreter, abi, platform_)
-    if _abi3_applies(python_version):
+
+    threading = _is_threaded_cpython(abis)
+    use_abi3 = _abi3_applies(python_version, threading)
+    if use_abi3:
         yield from (Tag(interpreter, "abi3", platform_) for platform_ in platforms)
     yield from (Tag(interpreter, "none", platform_) for platform_ in platforms)
 
-    if _abi3_applies(python_version):
+    if use_abi3:
         for minor_version in range(python_version[1] - 1, 1, -1):
             for platform_ in platforms:
                 interpreter = "cp{version}".format(
                     version=_version_nodot((python_version[0], minor_version))
                 )
                 yield Tag(interpreter, "abi3", platform_)
 
 
-def _generic_abi() -> Iterator[str]:
-    abi = sysconfig.get_config_var("SOABI")
-    if abi:
-        yield _normalize_string(abi)
+def _generic_abi() -> List[str]:
+    """
+    Return the ABI tag based on EXT_SUFFIX.
+    """
+    # The following are examples of `EXT_SUFFIX`.
+    # We want to keep the parts which are related to the ABI and remove the
+    # parts which are related to the platform:
+    # - linux:   '.cpython-310-x86_64-linux-gnu.so' => cp310
+    # - mac:     '.cpython-310-darwin.so'           => cp310
+    # - win:     '.cp310-win_amd64.pyd'             => cp310
+    # - win:     '.pyd'                             => cp37 (uses _cpython_abis())
+    # - pypy:    '.pypy38-pp73-x86_64-linux-gnu.so' => pypy38_pp73
+    # - graalpy: '.graalpy-38-native-x86_64-darwin.dylib'
+    #                                               => graalpy_38_native
+
+    ext_suffix = _get_config_var("EXT_SUFFIX", warn=True)
+    if not isinstance(ext_suffix, str) or ext_suffix[0] != ".":
+        raise SystemError("invalid sysconfig.get_config_var('EXT_SUFFIX')")
+    parts = ext_suffix.split(".")
+    if len(parts) < 3:
+        # CPython3.7 and earlier uses ".pyd" on Windows.
+        return _cpython_abis(sys.version_info[:2])
+    soabi = parts[1]
+    if soabi.startswith("cpython"):
+        # non-windows
+        abi = "cp" + soabi.split("-")[1]
+    elif soabi.startswith("cp"):
+        # windows
+        abi = soabi.split("-")[0]
+    elif soabi.startswith("pypy"):
+        abi = "-".join(soabi.split("-")[:2])
+    elif soabi.startswith("graalpy"):
+        abi = "-".join(soabi.split("-")[:3])
+    elif soabi:
+        # pyston, ironpython, others?
+        abi = soabi
+    else:
+        return []
+    return [_normalize_string(abi)]
 
 
 def generic_tags(
     interpreter: Optional[str] = None,
     abis: Optional[Iterable[str]] = None,
     platforms: Optional[Iterable[str]] = None,
     *,
@@ -248,16 +302,17 @@
     """
     if not interpreter:
         interp_name = interpreter_name()
         interp_version = interpreter_version(warn=warn)
         interpreter = "".join([interp_name, interp_version])
     if abis is None:
         abis = _generic_abi()
+    else:
+        abis = list(abis)
     platforms = list(platforms or platform_tags())
-    abis = list(abis)
     if "none" not in abis:
         abis.append("none")
     for abi in abis:
         for platform_ in platforms:
             yield Tag(interpreter, abi, platform_)
 
 
@@ -366,15 +421,15 @@
                     "-sS",
                     "-c",
                     "import platform; print(platform.mac_ver()[0])",
                 ],
                 check=True,
                 env={"SYSTEM_VERSION_COMPAT": "0"},
                 stdout=subprocess.PIPE,
-                universal_newlines=True,
+                text=True,
             ).stdout
             version = cast("MacVersion", tuple(map(int, version_str.split(".")[:2])))
     else:
         version = version
     if arch is None:
         arch = _mac_arch(cpu_arch)
     else:
@@ -429,23 +484,29 @@
                     minor=compat_version[1],
                     binary_format=binary_format,
                 )
 
 
 def _linux_platforms(is_32bit: bool = _32_BIT_INTERPRETER) -> Iterator[str]:
     linux = _normalize_string(sysconfig.get_platform())
+    if not linux.startswith("linux_"):
+        # we should never be here, just yield the sysconfig one and return
+        yield linux
+        return
     if is_32bit:
         if linux == "linux_x86_64":
             linux = "linux_i686"
         elif linux == "linux_aarch64":
-            linux = "linux_armv7l"
+            linux = "linux_armv8l"
     _, arch = linux.split("_", 1)
-    yield from _manylinux.platform_tags(linux, arch)
-    yield from _musllinux.platform_tags(arch)
-    yield linux
+    archs = {"armv8l": ["armv8l", "armv7l"]}.get(arch, [arch])
+    yield from _manylinux.platform_tags(archs)
+    yield from _musllinux.platform_tags(archs)
+    for arch in archs:
+        yield f"linux_{arch}"
 
 
 def _generic_platforms() -> Iterator[str]:
     yield _normalize_string(sysconfig.get_platform())
 
 
 def platform_tags() -> Iterator[str]:
@@ -459,14 +520,17 @@
     else:
         return _generic_platforms()
 
 
 def interpreter_name() -> str:
     """
     Returns the name of the running interpreter.
+
+    Some implementations have a reserved, two-letter abbreviation which will
+    be returned when appropriate.
     """
     name = sys.implementation.name
     return INTERPRETER_SHORT_NAMES.get(name) or name
 
 
 def interpreter_version(*, warn: bool = False) -> str:
     """
```

### Comparing `pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/utils.py` & `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,37 +8,54 @@
 from .tags import Tag, parse_tag
 from .version import InvalidVersion, Version
 
 BuildTag = Union[Tuple[()], Tuple[int, str]]
 NormalizedName = NewType("NormalizedName", str)
 
 
+class InvalidName(ValueError):
+    """
+    An invalid distribution name; users should refer to the packaging user guide.
+    """
+
+
 class InvalidWheelFilename(ValueError):
     """
     An invalid wheel filename was found, users should refer to PEP 427.
     """
 
 
 class InvalidSdistFilename(ValueError):
     """
     An invalid sdist filename was found, users should refer to the packaging user guide.
     """
 
 
+# Core metadata spec for `Name`
+_validate_regex = re.compile(
+    r"^([A-Z0-9]|[A-Z0-9][A-Z0-9._-]*[A-Z0-9])$", re.IGNORECASE
+)
 _canonicalize_regex = re.compile(r"[-_.]+")
+_normalized_regex = re.compile(r"^([a-z0-9]|[a-z0-9]([a-z0-9-](?!--))*[a-z0-9])$")
 # PEP 427: The build number must start with a digit.
 _build_tag_regex = re.compile(r"(\d+)(.*)")
 
 
-def canonicalize_name(name: str) -> NormalizedName:
+def canonicalize_name(name: str, *, validate: bool = False) -> NormalizedName:
+    if validate and not _validate_regex.match(name):
+        raise InvalidName(f"name is invalid: {name!r}")
     # This is taken from PEP 503.
     value = _canonicalize_regex.sub("-", name).lower()
     return cast(NormalizedName, value)
 
 
+def is_normalized_name(name: str) -> bool:
+    return _normalized_regex.match(name) is not None
+
+
 def canonicalize_version(
     version: Union[Version, str], *, strip_trailing_zero: bool = True
 ) -> str:
     """
     This is very similar to Version.__str__, but has one subtle difference
     with the way it handles the release segment.
     """
@@ -96,19 +113,26 @@
     if dashes not in (4, 5):
         raise InvalidWheelFilename(
             f"Invalid wheel filename (wrong number of parts): {filename}"
         )
 
     parts = filename.split("-", dashes - 2)
     name_part = parts[0]
-    # See PEP 427 for the rules on escaping the project name
+    # See PEP 427 for the rules on escaping the project name.
     if "__" in name_part or re.match(r"^[\w\d._]*$", name_part, re.UNICODE) is None:
         raise InvalidWheelFilename(f"Invalid project name: {filename}")
     name = canonicalize_name(name_part)
-    version = Version(parts[1])
+
+    try:
+        version = Version(parts[1])
+    except InvalidVersion as e:
+        raise InvalidWheelFilename(
+            f"Invalid wheel filename (invalid version): {filename}"
+        ) from e
+
     if dashes == 5:
         build_part = parts[2]
         build_match = _build_tag_regex.match(build_part)
         if build_match is None:
             raise InvalidWheelFilename(
                 f"Invalid build number: {build_part} in '{filename}'"
             )
@@ -133,9 +157,16 @@
     # We are requiring a PEP 440 version, which cannot contain dashes,
     # so we split on the last dash.
     name_part, sep, version_part = file_stem.rpartition("-")
     if not sep:
         raise InvalidSdistFilename(f"Invalid sdist filename: {filename}")
 
     name = canonicalize_name(name_part)
-    version = Version(version_part)
+
+    try:
+        version = Version(version_part)
+    except InvalidVersion as e:
+        raise InvalidSdistFilename(
+            f"Invalid sdist filename (invalid version): {filename}"
+        ) from e
+
     return (name, version)
```

### Comparing `pdm_backend-2.1.8/src/pdm/backend/_vendor/packaging/version.py` & `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,45 +3,47 @@
 # for complete details.
 """
 .. testsetup::
 
     from pdm.backend._vendor.packaging.version import parse, Version
 """
 
-import collections
 import itertools
 import re
-from typing import Callable, Optional, SupportsInt, Tuple, Union
+from typing import Any, Callable, NamedTuple, Optional, SupportsInt, Tuple, Union
 
 from ._structures import Infinity, InfinityType, NegativeInfinity, NegativeInfinityType
 
 __all__ = ["VERSION_PATTERN", "parse", "Version", "InvalidVersion"]
 
-InfiniteTypes = Union[InfinityType, NegativeInfinityType]
-PrePostDevType = Union[InfiniteTypes, Tuple[str, int]]
-SubLocalType = Union[InfiniteTypes, int, str]
-LocalType = Union[
+LocalType = Tuple[Union[int, str], ...]
+
+CmpPrePostDevType = Union[InfinityType, NegativeInfinityType, Tuple[str, int]]
+CmpLocalType = Union[
     NegativeInfinityType,
-    Tuple[
-        Union[
-            SubLocalType,
-            Tuple[SubLocalType, str],
-            Tuple[NegativeInfinityType, SubLocalType],
-        ],
-        ...,
-    ],
+    Tuple[Union[Tuple[int, str], Tuple[NegativeInfinityType, Union[int, str]]], ...],
 ]
 CmpKey = Tuple[
-    int, Tuple[int, ...], PrePostDevType, PrePostDevType, PrePostDevType, LocalType
+    int,
+    Tuple[int, ...],
+    CmpPrePostDevType,
+    CmpPrePostDevType,
+    CmpPrePostDevType,
+    CmpLocalType,
 ]
 VersionComparisonMethod = Callable[[CmpKey, CmpKey], bool]
 
-_Version = collections.namedtuple(
-    "_Version", ["epoch", "release", "dev", "pre", "post", "local"]
-)
+
+class _Version(NamedTuple):
+    epoch: int
+    release: Tuple[int, ...]
+    dev: Optional[Tuple[str, int]]
+    pre: Optional[Tuple[str, int]]
+    post: Optional[Tuple[str, int]]
+    local: Optional[LocalType]
 
 
 def parse(version: str) -> "Version":
     """Parse the given version string.
 
     >>> parse('1.0.dev1')
     <Version('1.0.dev1')>
@@ -59,15 +61,15 @@
     Traceback (most recent call last):
         ...
     packaging.version.InvalidVersion: Invalid version: 'invalid'
     """
 
 
 class _BaseVersion:
-    _key: CmpKey
+    _key: Tuple[Any, ...]
 
     def __hash__(self) -> int:
         return hash(self._key)
 
     # Please keep the duplicated `isinstance` check
     # in the six comparisons hereunder
     # unless you find a way to avoid adding overhead function calls.
@@ -113,15 +115,15 @@
 _VERSION_PATTERN = r"""
     v?
     (?:
         (?:(?P<epoch>[0-9]+)!)?                           # epoch
         (?P<release>[0-9]+(?:\.[0-9]+)*)                  # release segment
         (?P<pre>                                          # pre-release
             [-_\.]?
-            (?P<pre_l>(a|b|c|rc|alpha|beta|pre|preview))
+            (?P<pre_l>alpha|a|beta|b|preview|pre|c|rc)
             [-_\.]?
             (?P<pre_n>[0-9]+)?
         )?
         (?P<post>                                         # post release
             (?:-(?P<post_n1>[0-9]+))
             |
             (?:
@@ -175,14 +177,15 @@
     >>> v1 >= v2
     False
     >>> v1 <= v2
     True
     """
 
     _regex = re.compile(r"^\s*" + VERSION_PATTERN + r"\s*$", re.VERBOSE | re.IGNORECASE)
+    _key: CmpKey
 
     def __init__(self, version: str) -> None:
         """Initialize a Version object.
 
         :param version:
             The string representation of a version which will be parsed and normalized
             before use.
@@ -264,16 +267,15 @@
         """The epoch of the version.
 
         >>> Version("2.0.0").epoch
         0
         >>> Version("1!2.0.0").epoch
         1
         """
-        _epoch: int = self._version.epoch
-        return _epoch
+        return self._version.epoch
 
     @property
     def release(self) -> Tuple[int, ...]:
         """The components of the "release" segment of the version.
 
         >>> Version("1.2.3").release
         (1, 2, 3)
@@ -281,32 +283,30 @@
         (2, 0, 0)
         >>> Version("1!2.0.0.post0").release
         (2, 0, 0)
 
         Includes trailing zeroes but not the epoch or any pre-release / development /
         post-release suffixes.
         """
-        _release: Tuple[int, ...] = self._version.release
-        return _release
+        return self._version.release
 
     @property
     def pre(self) -> Optional[Tuple[str, int]]:
         """The pre-release segment of the version.
 
         >>> print(Version("1.2.3").pre)
         None
         >>> Version("1.2.3a1").pre
         ('a', 1)
         >>> Version("1.2.3b1").pre
         ('b', 1)
         >>> Version("1.2.3rc1").pre
         ('rc', 1)
         """
-        _pre: Optional[Tuple[str, int]] = self._version.pre
-        return _pre
+        return self._version.pre
 
     @property
     def post(self) -> Optional[int]:
         """The post-release number of the version.
 
         >>> print(Version("1.2.3").post)
         None
@@ -446,15 +446,15 @@
         >>> Version("1").micro
         0
         """
         return self.release[2] if len(self.release) >= 3 else 0
 
 
 def _parse_letter_version(
-    letter: str, number: Union[str, bytes, SupportsInt]
+    letter: Optional[str], number: Union[str, bytes, SupportsInt, None]
 ) -> Optional[Tuple[str, int]]:
 
     if letter:
         # We consider there to be an implicit 0 in a pre-release if there is
         # not a numeral associated with it.
         if number is None:
             number = 0
@@ -484,15 +484,15 @@
 
     return None
 
 
 _local_version_separators = re.compile(r"[\._-]")
 
 
-def _parse_local_version(local: str) -> Optional[LocalType]:
+def _parse_local_version(local: Optional[str]) -> Optional[LocalType]:
     """
     Takes a string like abc.1.twelve and turns it into ("abc", 1, "twelve").
     """
     if local is not None:
         return tuple(
             part.lower() if not part.isdigit() else int(part)
             for part in _local_version_separators.split(local)
@@ -502,15 +502,15 @@
 
 def _cmpkey(
     epoch: int,
     release: Tuple[int, ...],
     pre: Optional[Tuple[str, int]],
     post: Optional[Tuple[str, int]],
     dev: Optional[Tuple[str, int]],
-    local: Optional[Tuple[SubLocalType]],
+    local: Optional[LocalType],
 ) -> CmpKey:
 
     # When we compare a release version, we want to compare it with all of the
     # trailing zeros removed. So we'll use a reverse the list, drop all the now
     # leading zeros until we come to something non zero, then take the rest
     # re-reverse it back into the correct order and make it a tuple and use
     # that for our sorting key.
@@ -519,39 +519,39 @@
     )
 
     # We need to "trick" the sorting algorithm to put 1.0.dev0 before 1.0a0.
     # We'll do this by abusing the pre segment, but we _only_ want to do this
     # if there is not a pre or a post segment. If we have one of those then
     # the normal sorting rules will handle this case correctly.
     if pre is None and post is None and dev is not None:
-        _pre: PrePostDevType = NegativeInfinity
+        _pre: CmpPrePostDevType = NegativeInfinity
     # Versions without a pre-release (except as noted above) should sort after
     # those with one.
     elif pre is None:
         _pre = Infinity
     else:
         _pre = pre
 
     # Versions without a post segment should sort before those with one.
     if post is None:
-        _post: PrePostDevType = NegativeInfinity
+        _post: CmpPrePostDevType = NegativeInfinity
 
     else:
         _post = post
 
     # Versions without a development segment should sort after those with one.
     if dev is None:
-        _dev: PrePostDevType = Infinity
+        _dev: CmpPrePostDevType = Infinity
 
     else:
         _dev = dev
 
     if local is None:
         # Versions without a local segment should sort before those with one.
-        _local: LocalType = NegativeInfinity
+        _local: CmpLocalType = NegativeInfinity
     else:
         # Versions with a local segment need that segment parsed to implement
         # the sorting rules in PEP440.
         # - Alpha numeric segments sort before numeric segments
         # - Alpha numeric segments sort lexicographically
         # - Numeric segments sort numerically
         # - Shorter versions sort before longer versions when the prefixes
```

### Comparing `pdm_backend-2.1.8/src/pdm/backend/_vendor/pyproject_metadata/LICENSE` & `pdm_backend-2.2.0/src/pdm/backend/_vendor/pyproject_metadata/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/src/pdm/backend/_vendor/pyproject_metadata/__init__.py` & `pdm_backend-2.2.0/src/pdm/backend/_vendor/pyproject_metadata/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import collections
+import copy
 import dataclasses
+import email.utils
 import os
 import os.path
 import pathlib
-import re
 import typing
 
-from collections.abc import Mapping
-from typing import Any
+
+if typing.TYPE_CHECKING:
+    from collections.abc import Mapping
+    from typing import Any
+
+    from pdm.backend._vendor.packaging.requirements import Requirement
 
 import pdm.backend._vendor.packaging.markers as pkg_markers
 import pdm.backend._vendor.packaging.requirements as pkg_requirements
 import pdm.backend._vendor.packaging.specifiers as pkg_specifiers
+import pdm.backend._vendor.packaging.utils as pkg_utils
 import pdm.backend._vendor.packaging.version as pkg_version
 
 
-__version__ = '0.7.1'
+__version__ = '0.8.0rc1'
+
+KNOWN_METADATA_VERSIONS = {'2.1', '2.2', '2.3'}
 
 
 class ConfigurationError(Exception):
     '''Error in the backend metadata.'''
     def __init__(self, msg: str, *, key: str | None = None):
         super().__init__(msg)
         self._key = key
 
     @property
     def key(self) -> str | None:  # pragma: no cover
         return self._key
 
 
-class RFC822Message():
+class RFC822Message:
     '''Python-flavored RFC 822 message implementation.'''
 
     def __init__(self) -> None:
         self.headers: collections.OrderedDict[str, list[str]] = collections.OrderedDict()
         self.body: str | None = None
 
     def __setitem__(self, name: str, value: str | None) -> None:
@@ -59,15 +67,15 @@
             text += '\n' + self.body
         return text
 
     def __bytes__(self) -> bytes:
         return str(self).encode()
 
 
-class DataFetcher():
+class DataFetcher:
     def __init__(self, data: Mapping[str, Any]) -> None:
         self._data = data
 
     def __contains__(self, key: Any) -> bool:
         if not isinstance(key, str):
             return False
         val = self._data
@@ -84,59 +92,44 @@
             val = val[part]
         return val
 
     def get_str(self, key: str) -> str | None:
         try:
             val = self.get(key)
             if not isinstance(val, str):
-                raise ConfigurationError(
-                    f'Field `{key}` has an invalid type, '
-                    f'expecting a string (got `{val}`)',
-                    key=key,
-                )
+                msg = f'Field "{key}" has an invalid type, expecting a string (got "{val}")'
+                raise ConfigurationError(msg, key=key)
             return val
         except KeyError:
             return None
 
     def get_list(self, key: str) -> list[str]:
         try:
             val = self.get(key)
             if not isinstance(val, list):
-                raise ConfigurationError(
-                    f'Field `{key}` has an invalid type, '
-                    f'expecting a list of strings (got `{val}`)',
-                    key=val,
-                )
+                msg = f'Field "{key}" has an invalid type, expecting a list of strings (got "{val}")'
+                raise ConfigurationError(msg, key=val)
             for item in val:
                 if not isinstance(item, str):
-                    raise ConfigurationError(
-                        f'Field `{key}` contains item with invalid type, '
-                        f'expecting a string (got `{item}`)',
-                        key=key,
-                    )
+                    msg = f'Field "{key}" contains item with invalid type, expecting a string (got "{item}")'
+                    raise ConfigurationError(msg, key=key)
             return val
         except KeyError:
             return []
 
     def get_dict(self, key: str) -> dict[str, str]:
         try:
             val = self.get(key)
             if not isinstance(val, dict):
-                raise ConfigurationError(
-                    f'Field `{key}` has an invalid type, '
-                    f'expecting a dictionary of strings (got `{val}`)',
-                    key=key,
-                )
+                msg = f'Field "{key}" has an invalid type, expecting a dictionary of strings (got "{val}")'
+                raise ConfigurationError(msg, key=key)
             for subkey, item in val.items():
                 if not isinstance(item, str):
-                    raise ConfigurationError(
-                        f'Field `{key}.{subkey}` has an invalid type, '
-                        f'expecting a string (got `{item}`)',
-                        key=f'{key}.{subkey}',
-                    )
+                    msg = f'Field "{key}.{subkey}" has an invalid type, expecting a string (got "{item}")'
+                    raise ConfigurationError(msg, key=f'{key}.{subkey}')
             return val
         except KeyError:
             return {}
 
     def get_people(self, key: str) -> list[tuple[str, str]]:
         try:
             val = self.get(key)
@@ -145,19 +138,19 @@
                 and all(isinstance(x, dict) for x in val)
                 and all(
                     isinstance(item, str)
                     for items in [_dict.values() for _dict in val]
                     for item in items
                 )
             ):
-                raise ConfigurationError(
-                    f'Field `{key}` has an invalid type, expecting a list of '
-                    f'dictionaries containing the `name` and/or `email` keys (got `{val}`)',
-                    key=key,
+                msg = (
+                    f'Field "{key}" has an invalid type, expecting a list of '
+                    f'dictionaries containing the "name" and/or "email" keys (got "{val}")'
                 )
+                raise ConfigurationError(msg, key=key)
             return [
                 (entry.get('name', 'Unknown'), entry.get('email'))
                 for entry in val
             ]
         except KeyError:
             return []
 
@@ -170,114 +163,140 @@
 class Readme(typing.NamedTuple):
     text: str
     file: pathlib.Path | None
     content_type: str
 
 
 @dataclasses.dataclass
-class StandardMetadata():
+class StandardMetadata:
     name: str
     version: pkg_version.Version | None = None
     description: str | None = None
     license: License | None = None
     readme: Readme | None = None
     requires_python: pkg_specifiers.SpecifierSet | None = None
-    dependencies: list[pkg_requirements.Requirement] = dataclasses.field(default_factory=list)
-    optional_dependencies: dict[str, list[pkg_requirements.Requirement]] = dataclasses.field(default_factory=dict)
+    dependencies: list[Requirement] = dataclasses.field(default_factory=list)
+    optional_dependencies: dict[str, list[Requirement]] = dataclasses.field(default_factory=dict)
     entrypoints: dict[str, dict[str, str]] = dataclasses.field(default_factory=dict)
     authors: list[tuple[str, str]] = dataclasses.field(default_factory=list)
     maintainers: list[tuple[str, str]] = dataclasses.field(default_factory=list)
     urls: dict[str, str] = dataclasses.field(default_factory=dict)
     classifiers: list[str] = dataclasses.field(default_factory=list)
     keywords: list[str] = dataclasses.field(default_factory=list)
     scripts: dict[str, str] = dataclasses.field(default_factory=dict)
     gui_scripts: dict[str, str] = dataclasses.field(default_factory=dict)
     dynamic: list[str] = dataclasses.field(default_factory=list)
 
-    def __post_init__(self) -> None:
-        self.name = re.sub(r'[-_.]+', '-', self.name).lower()
-        self._update_dynamic(self.version)
+    _metadata_version: str | None = None
+
+    @property
+    def metadata_version(self) -> str:
+        if self._metadata_version is None:
+            return '2.2' if self.dynamic else '2.1'
+        return self._metadata_version
+
+    @property
+    def canonical_name(self) -> str:
+        return pkg_utils.canonicalize_name(self.name)
 
     @classmethod
     def from_pyproject(
         cls,
         data: Mapping[str, Any],
         project_dir: str | os.PathLike[str] = os.path.curdir,
+        metadata_version: str | None = None,
     ) -> StandardMetadata:
         fetcher = DataFetcher(data)
         project_dir = pathlib.Path(project_dir)
 
         if 'project' not in fetcher:
-            raise ConfigurationError('Section `project` missing in pyproject.toml')
+            msg = 'Section "project" missing in pyproject.toml'
+            raise ConfigurationError(msg)
 
         dynamic = fetcher.get_list('project.dynamic')
         if 'name' in dynamic:
-            raise ConfigurationError('Unsupported field `name` in `project.dynamic`')
+            msg = 'Unsupported field "name" in "project.dynamic"'
+            raise ConfigurationError(msg)
 
         for field in dynamic:
             if field in data['project']:
-                raise ConfigurationError(
-                    f'Field `project.{field}` declared as dynamic in but is defined'
-                )
+                msg = f'Field "project.{field}" declared as dynamic in but is defined'
+                raise ConfigurationError(msg)
 
         name = fetcher.get_str('project.name')
         if not name:
-            raise ConfigurationError('Field `project.name` missing')
+            msg = 'Field "project.name" missing'
+            raise ConfigurationError(msg)
 
         version_string = fetcher.get_str('project.version')
         requires_python_string = fetcher.get_str('project.requires-python')
+        version = pkg_version.Version(version_string) if version_string else None
+
+        if version is None and 'version' not in dynamic:
+            msg = 'Field "project.version" missing and "version" not specified in "project.dynamic"'
+            raise ConfigurationError(msg)
+
+        # Description can't be multiline
+        description = fetcher.get_str('project.description')
+        if description and '\n' in description:
+            msg = 'The description must be a single line'
+            raise ConfigurationError(msg)
+
+        if metadata_version and metadata_version not in KNOWN_METADATA_VERSIONS:
+            msg = f'The metadata_version must be one of {KNOWN_METADATA_VERSIONS} or None (default)'
+            raise ConfigurationError(msg)
 
         return cls(
             name,
-            pkg_version.Version(version_string) if version_string else None,
-            fetcher.get_str('project.description'),
+            version,
+            description,
             cls._get_license(fetcher, project_dir),
             cls._get_readme(fetcher, project_dir),
             pkg_specifiers.SpecifierSet(requires_python_string) if requires_python_string else None,
             cls._get_dependencies(fetcher),
             cls._get_optional_dependencies(fetcher),
             cls._get_entrypoints(fetcher),
             fetcher.get_people('project.authors'),
             fetcher.get_people('project.maintainers'),
             fetcher.get_dict('project.urls'),
             fetcher.get_list('project.classifiers'),
             fetcher.get_list('project.keywords'),
             fetcher.get_dict('project.scripts'),
             fetcher.get_dict('project.gui-scripts'),
             dynamic,
+            metadata_version,
         )
 
     def _update_dynamic(self, value: Any) -> None:
         if value and 'version' in self.dynamic:
             self.dynamic.remove('version')
-        elif not value and 'version' not in self.dynamic:
-            self.dynamic.append('version')
 
     def __setattr__(self, name: str, value: Any) -> None:
         # update dynamic when version is set
         if name == 'version' and hasattr(self, 'dynamic'):
             self._update_dynamic(value)
         super().__setattr__(name, value)
 
     def as_rfc822(self) -> RFC822Message:
         message = RFC822Message()
         self.write_to_rfc822(message)
         return message
 
     def write_to_rfc822(self, message: RFC822Message) -> None:  # noqa: C901
-        message['Metadata-Version'] = '2.2' if self.dynamic else '2.1'
+        message['Metadata-Version'] = self.metadata_version
         message['Name'] = self.name
         if not self.version:
-            raise ConfigurationError('Missing version field')
+            msg = 'Missing version field'
+            raise ConfigurationError(msg)
         message['Version'] = str(self.version)
         # skip 'Platform'
         # skip 'Supported-Platform'
         if self.description:
             message['Summary'] = self.description
-        message['Keywords'] = ' '.join(self.keywords)
+        message['Keywords'] = ','.join(self.keywords)
         if 'homepage' in self.urls:
             message['Home-page'] = self.urls['homepage']
         # skip 'Download-URL'
         message['Author'] = self._name_list(self.authors)
         message['Author-Email'] = self._email_list(self.authors)
         message['Maintainer'] = self._name_list(self.maintainers)
         message['Maintainer-Email'] = self._email_list(self.maintainers)
@@ -291,84 +310,88 @@
         for name, url in self.urls.items():
             message['Project-URL'] = f'{name.capitalize()}, {url}'
         if self.requires_python:
             message['Requires-Python'] = str(self.requires_python)
         for dep in self.dependencies:
             message['Requires-Dist'] = str(dep)
         for extra, requirements in self.optional_dependencies.items():
-            message['Provides-Extra'] = extra
+            norm_extra = extra.replace('.', '-').replace('_', '-').lower()
+            message['Provides-Extra'] = norm_extra
             for requirement in requirements:
-                message['Requires-Dist'] = str(self._build_extra_req(extra, requirement))
+                message['Requires-Dist'] = str(self._build_extra_req(norm_extra, requirement))
         if self.readme:
             if self.readme.content_type:
                 message['Description-Content-Type'] = self.readme.content_type
             message.body = self.readme.text
         # Core Metadata 2.2
-        for field in self.dynamic:
-            if field in ('name', 'version'):
-                raise ConfigurationError(f'Field cannot be dynamic: {field}')
-            message['Dynamic'] = field
+        if self.metadata_version != '2.1':
+            for field in self.dynamic:
+                if field in ('name', 'version'):
+                    msg = f'Field cannot be dynamic: {field}'
+                    raise ConfigurationError(msg)
+                message['Dynamic'] = field
 
     def _name_list(self, people: list[tuple[str, str]]) -> str:
         return ', '.join(
             name
             for name, email_ in people
             if not email_
         )
 
     def _email_list(self, people: list[tuple[str, str]]) -> str:
-        return ', '.join([
-            '{}{}'.format(name, f' <{_email}>' if _email else '')
+        return ', '.join(
+            email.utils.formataddr((name, _email))
             for name, _email in people
             if _email
-        ])
+        )
 
     def _build_extra_req(
         self,
         extra: str,
-        requirement: pkg_requirements.Requirement,
-    ) -> pkg_requirements.Requirement:
-        if requirement.marker:  # append our extra to the marker
-            requirement.marker = pkg_markers.Marker(
-                str(requirement.marker) + f' and extra == "{extra}"'
-            )
-        else:  # add our extra marker
+        requirement: Requirement,
+    ) -> Requirement:
+        # append or add our extra marker
+        requirement = copy.copy(requirement)
+        if requirement.marker:
+            if 'or' in requirement.marker._markers:
+                requirement.marker = pkg_markers.Marker(
+                    f'({requirement.marker}) and extra == "{extra}"'
+                )
+            else:
+                requirement.marker = pkg_markers.Marker(
+                    f'{requirement.marker} and extra == "{extra}"'
+                )
+        else:
             requirement.marker = pkg_markers.Marker(f'extra == "{extra}"')
         return requirement
 
     @staticmethod
     def _get_license(fetcher: DataFetcher, project_dir: pathlib.Path) -> License | None:
         if 'project.license' not in fetcher:
             return None
 
         _license = fetcher.get_dict('project.license')
         for field in _license:
             if field not in ('file', 'text'):
-                raise ConfigurationError(
-                    f'Unexpected field `project.license.{field}`',
-                    key=f'project.license.{field}',
-                )
+                msg = f'Unexpected field "project.license.{field}"'
+                raise ConfigurationError(msg, key=f'project.license.{field}')
 
         file: pathlib.Path | None = None
         filename = fetcher.get_str('project.license.file')
         text = fetcher.get_str('project.license.text')
 
         if (filename and text) or (not filename and not text):
-            raise ConfigurationError(
-                f'Invalid `project.license` value, expecting either `file` or `text` (got `{_license}`)',
-                key='project.license',
-            )
+            msg = f'Invalid "project.license" value, expecting either "file" or "text" (got "{_license}")'
+            raise ConfigurationError(msg, key='project.license')
 
         if filename:
             file = project_dir.joinpath(filename)
             if not file.is_file():
-                raise ConfigurationError(
-                    f'License file not found (`{filename}`)',
-                    key='project.license.file',
-                )
+                msg = f'License file not found ("{filename}")'
+                raise ConfigurationError(msg, key='project.license.file')
             text = file.read_text(encoding='utf-8')
 
         assert text is not None
         return License(text, file)
 
     @staticmethod
     def _get_readme(fetcher: DataFetcher, project_dir: pathlib.Path) -> Readme | None:  # noqa: C901
@@ -386,130 +409,129 @@
             text = None
             filename = readme
             if filename.endswith('.md'):
                 content_type = 'text/markdown'
             elif filename.endswith('.rst'):
                 content_type = 'text/x-rst'
             else:
-                raise ConfigurationError(
-                    f'Could not infer content type for readme file `{filename}`',
-                    key='project.readme',
-                )
+                msg = f'Could not infer content type for readme file "{filename}"'
+                raise ConfigurationError(msg, key='project.readme')
         elif isinstance(readme, dict):
             # readme is a dict containing either 'file' or 'text', and content-type
             for field in readme:
                 if field not in ('content-type', 'file', 'text'):
-                    raise ConfigurationError(
-                        f'Unexpected field `project.readme.{field}`',
-                        key=f'project.readme.{field}',
-                    )
+                    msg = f'Unexpected field "project.readme.{field}"'
+                    raise ConfigurationError(msg, key=f'project.readme.{field}')
             content_type = fetcher.get_str('project.readme.content-type')
             filename = fetcher.get_str('project.readme.file')
             text = fetcher.get_str('project.readme.text')
             if (filename and text) or (not filename and not text):
-                raise ConfigurationError(
-                    f'Invalid `project.readme` value, expecting either `file` or `text` (got `{readme}`)',
-                    key='project.license',
-                )
+                msg = f'Invalid "project.readme" value, expecting either "file" or "text" (got "{readme}")'
+                raise ConfigurationError(msg, key='project.readme')
             if not content_type:
-                raise ConfigurationError(
-                    'Field `project.readme.content-type` missing',
-                    key='project.readme.content-type',
-                )
+                msg = 'Field "project.readme.content-type" missing'
+                raise ConfigurationError(msg, key='project.readme.content-type')
         else:
-            raise ConfigurationError(
-                f'Field `project.readme` has an invalid type, expecting either, '
-                f'a string or dictionary of strings (got `{readme}`)',
-                key='project.readme',
+            msg = (
+                f'Field "project.readme" has an invalid type, expecting either, '
+                f'a string or dictionary of strings (got "{readme}")'
             )
+            raise ConfigurationError(msg, key='project.readme')
 
         if filename:
             file = project_dir.joinpath(filename)
             if not file.is_file():
-                raise ConfigurationError(
-                    f'Readme file not found (`{filename}`)',
-                    key='project.license.file',
-                )
+                msg = f'Readme file not found ("{filename}")'
+                raise ConfigurationError(msg, key='project.readme.file')
             text = file.read_text(encoding='utf-8')
 
         assert text is not None
         return Readme(text, file, content_type)
 
     @staticmethod
-    def _get_dependencies(fetcher: DataFetcher) -> list[pkg_requirements.Requirement]:
+    def _get_dependencies(fetcher: DataFetcher) -> list[Requirement]:
         try:
             requirement_strings = fetcher.get_list('project.dependencies')
         except KeyError:
             return []
 
-        requirements: list[pkg_requirements.Requirement] = []
+        requirements: list[Requirement] = []
         for req in requirement_strings:
             try:
                 requirements.append(pkg_requirements.Requirement(req))
             except pkg_requirements.InvalidRequirement as e:
-                raise ConfigurationError(
-                    'Field `project.dependencies` contains an invalid PEP 508 '
-                    f'requirement string `{req}` (`{str(e)}`)'
+                msg = (
+                    'Field "project.dependencies" contains an invalid PEP 508 '
+                    f'requirement string "{req}" ("{e}")'
                 )
+                raise ConfigurationError(msg) from None
         return requirements
 
     @staticmethod
-    def _get_optional_dependencies(fetcher: DataFetcher) -> dict[str, list[pkg_requirements.Requirement]]:
+    def _get_optional_dependencies(fetcher: DataFetcher) -> dict[str, list[Requirement]]:
         try:
             val = fetcher.get('project.optional-dependencies')
         except KeyError:
             return {}
 
-        requirements_dict: collections.defaultdict[str, list[pkg_requirements.Requirement]] = collections.defaultdict(list)
+        requirements_dict: dict[str, list[Requirement]] = {}
         if not isinstance(val, dict):
-            raise ConfigurationError(
-                'Field `project.optional-dependencies` has an invalid type, expecting a '
-                f'dictionary of PEP 508 requirement strings (got `{val}`)'
+            msg = (
+                'Field "project.optional-dependencies" has an invalid type, expecting a '
+                f'dictionary of PEP 508 requirement strings (got "{val}")'
             )
+            raise ConfigurationError(msg)
         for extra, requirements in val.copy().items():
             assert isinstance(extra, str)
             if not isinstance(requirements, list):
-                raise ConfigurationError(
-                    f'Field `project.optional-dependencies.{extra}` has an invalid type, expecting a '
-                    f'dictionary PEP 508 requirement strings (got `{requirements}`)'
-                )
-            for i, req in enumerate(requirements):
+                msg = (
+                    f'Field "project.optional-dependencies.{extra}" has an invalid type, expecting a '
+                    f'dictionary PEP 508 requirement strings (got "{requirements}")'
+                )
+                raise ConfigurationError(msg)
+            requirements_dict[extra] = []
+            for req in requirements:
                 if not isinstance(req, str):
-                    raise ConfigurationError(
-                        f'Field `project.optional-dependencies.{extra}` has an invalid type, '
-                        f'expecting a PEP 508 requirement string (got `{req}`)'
+                    msg = (
+                        f'Field "project.optional-dependencies.{extra}" has an invalid type, '
+                        f'expecting a PEP 508 requirement string (got "{req}")'
                     )
+                    raise ConfigurationError(msg)
                 try:
                     requirements_dict[extra].append(pkg_requirements.Requirement(req))
                 except pkg_requirements.InvalidRequirement as e:
-                    raise ConfigurationError(
-                        f'Field `project.optional-dependencies.{extra}` contains '
-                        f'an invalid PEP 508 requirement string `{req}` (`{str(e)}`)'
+                    msg = (
+                        f'Field "project.optional-dependencies.{extra}" contains '
+                        f'an invalid PEP 508 requirement string "{req}" ("{e}")'
                     )
+                    raise ConfigurationError(msg) from None
         return dict(requirements_dict)
 
     @staticmethod
     def _get_entrypoints(fetcher: DataFetcher) -> dict[str, dict[str, str]]:
         try:
             val = fetcher.get('project.entry-points')
         except KeyError:
             return {}
         if not isinstance(val, dict):
-            raise ConfigurationError(
-                'Field `project.entry-points` has an invalid type, expecting a '
-                f'dictionary of entrypoint sections (got `{val}`)'
+            msg = (
+                'Field "project.entry-points" has an invalid type, expecting a '
+                f'dictionary of entrypoint sections (got "{val}")'
             )
+            raise ConfigurationError(msg)
         for section, entrypoints in val.items():
             assert isinstance(section, str)
             if not isinstance(entrypoints, dict):
-                raise ConfigurationError(
-                    f'Field `project.entry-points.{section}` has an invalid type, expecting a '
-                    f'dictionary of entrypoints (got `{entrypoints}`)'
+                msg = (
+                    f'Field "project.entry-points.{section}" has an invalid type, expecting a '
+                    f'dictionary of entrypoints (got "{entrypoints}")'
                 )
+                raise ConfigurationError(msg)
             for name, entrypoint in entrypoints.items():
                 assert isinstance(name, str)
                 if not isinstance(entrypoint, str):
-                    raise ConfigurationError(
-                        f'Field `project.entry-points.{section}.{name}` has an invalid type, '
-                        f'expecting a string (got `{entrypoint}`)'
+                    msg = (
+                        f'Field "project.entry-points.{section}.{name}" has an invalid type, '
+                        f'expecting a string (got "{entrypoint}")'
                     )
+                    raise ConfigurationError(msg)
         return val
```

### Comparing `pdm_backend-2.1.8/src/pdm/backend/_vendor/tomli/LICENSE` & `pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/src/pdm/backend/_vendor/tomli/_parser.py` & `pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/src/pdm/backend/_vendor/tomli/_re.py` & `pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/src/pdm/backend/_vendor/tomli_w/LICENSE` & `pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli_w/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/src/pdm/backend/_vendor/tomli_w/_writer.py` & `pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli_w/_writer.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/src/pdm/backend/base.py` & `pdm_backend-2.2.0/src/pdm/backend/base.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/src/pdm/backend/config.py` & `pdm_backend-2.2.0/src/pdm/backend/config.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/src/pdm/backend/editable.py` & `pdm_backend-2.2.0/src/pdm/backend/editable.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,27 +14,19 @@
 
 
 def is_subpath(path: str, parent: str) -> bool:
     return os.path.normcase(path).startswith(os.path.normcase(parent))
 
 
 class EditableBuildHook:
-    @staticmethod
-    def editable_version(version: str) -> str:
-        if "+" in version:
-            return f"{version}.editable"
-        return f"{version}+editable"
-
     def pdm_build_initialize(self, context: Context) -> None:
         editables = self._prepare_editable(context)
         context.config.metadata.setdefault("dependencies", []).extend(
             editables.dependencies()
         )
-        version = context.config.metadata["version"]
-        context.config.metadata["version"] = self.editable_version(version)
         context.editables = editables
 
     def pdm_build_update_files(self, context: Context, files: dict[str, Path]) -> None:
         packages: list[str] = context.config.convert_package_paths()["packages"]
         proxied = {p.replace(".", "/") for p in packages}
         for relpath in list(files):
             if os.path.splitext(relpath)[1] in (".py", ".pyc", ".pyo"):
```

### Comparing `pdm_backend-2.1.8/src/pdm/backend/hooks/base.py` & `pdm_backend-2.2.0/src/pdm/backend/hooks/base.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/src/pdm/backend/hooks/setuptools.py` & `pdm_backend-2.2.0/src/pdm/backend/hooks/setuptools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A built-in hook to generate setup.py and run the script"""
+
 from __future__ import annotations
 
 import atexit
 import pickle
 import shutil
 import subprocess
 import sys
```

### Comparing `pdm_backend-2.1.8/src/pdm/backend/hooks/version/scm.py` & `pdm_backend-2.2.0/src/pdm/backend/hooks/version/scm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 module to get version from tag of SCM repository.
 Adapted from setuptools-scm. Currently only support git and hg.
 """
+
 from __future__ import annotations
 
 import os
 import re
 import shlex
 import shutil
 import subprocess
 import warnings
 from dataclasses import dataclass
-from datetime import datetime
+from datetime import datetime, timezone
 from pathlib import Path
-from typing import TYPE_CHECKING, Iterable, NamedTuple
+from typing import TYPE_CHECKING, Callable, Iterable, NamedTuple
 
 from pdm.backend._vendor.packaging.version import Version
 
 if TYPE_CHECKING:
     from _typeshed import StrPath
 
 DEFAULT_TAG_REGEX = re.compile(
@@ -56,33 +57,33 @@
     return (
         proc.returncode,
         out.decode("utf-8", "surrogateescape").strip(),
         err.decode("utf-8", "surrogateescape").strip(),
     )
 
 
-class VersionInfo(NamedTuple):
+class SCMVersion(NamedTuple):
     version: Version
     distance: int | None
     dirty: bool
     node: str | None
     branch: str | None
 
 
 def meta(
     config: Config,
     tag: str | Version,
     distance: int | None = None,
     dirty: bool = False,
     node: str | None = None,
     branch: str | None = None,
-) -> VersionInfo:
+) -> SCMVersion:
     if isinstance(tag, str):
         tag = tag_to_version(config, tag)
-    return VersionInfo(tag, distance, dirty, node, branch)
+    return SCMVersion(tag, distance, dirty, node, branch)
 
 
 def _git_get_branch(root: StrPath) -> str | None:
     ret, out, _ = _subprocess_call("git rev-parse --abbrev-ref HEAD", root)
     if not ret:
         return out
     return None
@@ -168,15 +169,15 @@
     take tags that might be prefixed with a keyword and return only the version part
     :param tags: an iterable of tags
     :param config: optional configuration object
     """
     return [tag_to_version(config, tag) for tag in tags if tag]
 
 
-def git_parse_version(root: StrPath, config: Config) -> VersionInfo | None:
+def git_parse_version(root: StrPath, config: Config) -> SCMVersion | None:
     GIT = shutil.which("git")
     if not GIT:
         return None
 
     ret, repo, _ = _subprocess_call([GIT, "rev-parse", "--show-toplevel"], root)
     if ret or not repo:
         return None
@@ -222,15 +223,15 @@
     cmd = ["hg", "log", "-q", "-r", f"{rev1}::{rev2}"]
     _, out, _ = _subprocess_call(cmd, root)
     return len(out.strip().splitlines()) - 1
 
 
 def _hg_tagdist_normalize_tagcommit(
     config: Config, root: StrPath, tag: str, dist: int, node: str, branch: str
-) -> VersionInfo:
+) -> SCMVersion:
     dirty = node.endswith("+")
     node = "h" + node.strip("+")
 
     # Detect changes since the specified tag
     revset = (
         "(branch(.)"  # look for revisions in this branch only
         " and tag({tag!r})::."  # after the last tag
@@ -274,15 +275,15 @@
 def _bump_regex(version: str) -> str:
     match = re.match(r"(.*?)(\d+)$", version)
     assert match is not None
     prefix, tail = match.groups()
     return "%s%d" % (prefix, int(tail) + 1)
 
 
-def hg_parse_version(root: StrPath, config: Config) -> VersionInfo | None:
+def hg_parse_version(root: StrPath, config: Config) -> SCMVersion | None:
     if not shutil.which("hg"):
         return None
     _, output, _ = _subprocess_call("hg id -i -b -t", root)
     identity_data = output.split()
     if not identity_data:
         return None
     node = identity_data.pop(0)
@@ -305,36 +306,39 @@
             tag = "0.0"
             dist = int(dist) + 1
         return _hg_tagdist_normalize_tagcommit(config, root, tag, dist, node, branch)
     except ValueError:
         return None  # unpacking failed, old hg
 
 
-def format_version(version: VersionInfo) -> str:
+def format_version(version: SCMVersion) -> str:
     if version.distance is None:
         main_version = str(version.version)
     else:
         guessed = guess_next_version(version.version)
         main_version = f"{guessed}.dev{version.distance}"
 
     if version.distance is None or version.node is None:
         clean_format = ""
         dirty_format = "+d{time:%Y%m%d}"
     else:
         clean_format = "+{node}"
         dirty_format = "+{node}.d{time:%Y%m%d}"
     fmt = dirty_format if version.dirty else clean_format
-    local_version = fmt.format(node=version.node, time=datetime.utcnow())
+    local_version = fmt.format(node=version.node, time=datetime.now(tz=timezone.utc))
     return main_version + local_version
 
 
-def get_version_from_scm(root: str | Path, *, tag_regex: str | None = None) -> str:
+def get_version_from_scm(
+    root: str | Path,
+    *,
+    tag_regex: str | None = None,
+    version_formatter: Callable[[SCMVersion], str] | None = None,
+) -> str | None:
     config = Config(tag_regex=re.compile(tag_regex) if tag_regex else DEFAULT_TAG_REGEX)
     for func in (git_parse_version, hg_parse_version):
         version = func(root, config)  # type: ignore
         if version:
-            return format_version(version)
-    raise ValueError(
-        "Cannot find the version from SCM or SCM isn't detected. \n"
-        "You can still specify the version via environment variable "
-        "`PDM_BUILD_SCM_VERSION`."
-    )
+            if version_formatter is None:
+                version_formatter = format_version
+            return version_formatter(version)
+    return None
```

### Comparing `pdm_backend-2.1.8/src/pdm/backend/macosx_platform.py` & `pdm_backend-2.2.0/src/pdm/backend/macosx_platform.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 headers to extract system information
 
 Currently only for MacOSX
 
 Adapted from
 https://github.com/pypa/wheel/blob/6e86e6b886/src/wheel/macosx_libfile.py
 """
+
 from __future__ import annotations
 
 import ctypes
 import os
 import sys
 from pathlib import Path
 from typing import TYPE_CHECKING, BinaryIO, TypeVar, no_type_check
```

### Comparing `pdm_backend-2.1.8/src/pdm/backend/sdist.py` & `pdm_backend-2.2.0/src/pdm/backend/sdist.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/src/pdm/backend/structures.py` & `pdm_backend-2.2.0/src/pdm/backend/structures.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/src/pdm/backend/utils.py` & `pdm_backend-2.2.0/src/pdm/backend/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from __future__ import annotations
 
+import ast
+import contextlib
+import functools
 import importlib.util
 import os
 import re
 import sys
 import sysconfig
 import types
 import urllib.parse
 import warnings
 from contextlib import contextmanager
 from fnmatch import fnmatchcase
 from pathlib import Path
-from typing import Callable, Generator, Iterable, Match
+from typing import Any, Callable, Generator, Iterable, Match
 
 from pdm.backend._vendor.packaging import tags
 from pdm.backend._vendor.packaging.markers import Marker
 from pdm.backend._vendor.packaging.requirements import Requirement
 from pdm.backend._vendor.packaging.version import InvalidVersion, Version
+from pdm.backend.exceptions import ConfigError
 from pdm.backend.macosx_platform import calculate_macosx_platform_tag
 
 
 def safe_version(version: str) -> str:
     """
     Convert an arbitrary string to a standard version string
     """
@@ -230,7 +234,50 @@
     """
     # Set 644 permissions, leaving higher bits of st_mode unchanged
     new_mode = (st_mode | 0o644) & ~0o133
     if st_mode & 0o100:
         new_mode |= 0o111  # Executable: 644 -> 755
 
     return new_mode
+
+
+@contextlib.contextmanager
+def patch_sys_path(path: str | Path) -> Generator[None, None, None]:
+    old_path = sys.path[:]
+    sys.path.insert(0, str(path))
+    try:
+        yield
+    finally:
+        sys.path[:] = old_path
+
+
+_attr_regex = re.compile(r"([\w.]+):([\w.]+)\s*(\([^)]+\))?")
+
+
+def evaluate_module_attribute(
+    expression: str, context: Path | None = None
+) -> tuple[Any, tuple[Any, ...]]:
+    """Evaluate the value of an expression like '<module>:<attribute>'
+
+    Returns:
+        the object and the calling arguments if any
+    """
+    if context is None:
+        cm = contextlib.nullcontext()
+    else:
+        cm = patch_sys_path(context)  # type: ignore[assignment]
+
+    matched = _attr_regex.match(expression)
+    if matched is None:
+        raise ConfigError(
+            "Invalid expression, must be in the format of " "`module:attribute`."
+        )
+    with cm:
+        module = importlib.import_module(matched.group(1))
+        attrs = matched.group(2).split(".")
+        obj: Any = functools.reduce(getattr, attrs, module)
+        args_group = matched.group(3)
+        if args_group:
+            args = ast.literal_eval(args_group)
+        else:
+            args = ()
+        return obj, args
```

### Comparing `pdm_backend-2.1.8/src/pdm/backend/wheel.py` & `pdm_backend-2.2.0/src/pdm/backend/wheel.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/conftest.py` & `pdm_backend-2.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/fixtures/hooks/hook_class.py` & `pdm_backend-2.2.0/tests/fixtures/hooks/hook_class.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/fixtures/hooks/hook_module.py` & `pdm_backend-2.2.0/tests/fixtures/hooks/hook_module.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/fixtures/hooks/local_hook.py` & `pdm_backend-2.2.0/tests/fixtures/hooks/local_hook.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml` & `pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/fixtures/projects/demo-cextension/pyproject.toml` & `pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include-error/pdm.lock` & `pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include-error/pyproject.toml` & `pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include-error/requirements.txt` & `pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt` & `pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include/pdm.lock` & `pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include/pyproject.toml` & `pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include/requirements.txt` & `pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/fixtures/projects/demo-package-include/requirements_simple.txt` & `pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml` & `pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/fixtures/projects/demo-package-with-tests/pdm.lock` & `pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-tests/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/fixtures/projects/demo-package-with-tests/pyproject.toml` & `pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-tests/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/fixtures/projects/demo-package/pdm.lock` & `pdm_backend-2.2.0/tests/fixtures/projects/demo-package/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/fixtures/projects/demo-package/pyproject.toml` & `pdm_backend-2.2.0/tests/fixtures/projects/demo-package/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/fixtures/projects/demo-package/requirements.txt` & `pdm_backend-2.2.0/tests/fixtures/projects/demo-package/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/fixtures/projects/demo-package/requirements_simple.txt` & `pdm_backend-2.2.0/tests/fixtures/projects/demo-package/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml` & `pdm_backend-2.2.0/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/test_api.py` & `pdm_backend-2.2.0/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import email
 import os
 import sys
+import tarfile
 import zipfile
 from pathlib import Path
 
 import pytest
 
 import pdm.backend as api
 from pdm.backend.wheel import WheelBuilder
@@ -159,14 +160,35 @@
     assert "demo_package-0.1.0/foo/my_package/__init__.py" in tar_names
     assert "demo_package-0.1.0/foo/my_package/data.json" in tar_names
 
     assert "my_package/__init__.py" in zip_names
     assert "my_package/data.json" in zip_names
 
 
+@pytest.mark.parametrize("name", ["demo-metadata-test"])
+def test_demo_metadata_test__sdist__pkg_info(
+    dist: Path, name: str, tmp_path: Path
+) -> None:
+    filename = api.build_sdist(dist.as_posix())
+    with tarfile.open(dist / filename) as archive:
+        archive.extractall(tmp_path)
+    pkg_info_path = next(tmp_path.rglob("PKG-INFO"))
+    parsed_pkg_info = email.message_from_bytes(pkg_info_path.read_bytes())
+    assert dict(parsed_pkg_info) == {
+        "Author-Email": '"Corporation, Inc." <corporation@example.com>, Example '
+        "<example@example.com>",
+        "Description-Content-Type": "text/markdown",
+        "License": "MIT",
+        "Metadata-Version": "2.1",
+        "Name": name,
+        "Requires-Python": ">=3.8",
+        "Version": "3.2.1",
+    }
+
+
 @pytest.mark.parametrize("name", ["demo-package"])
 def test_prepare_metadata(dist: Path) -> None:
     dist_info = api.prepare_metadata_for_build_wheel(dist.as_posix())
     assert dist_info == "demo_package-0.1.0.dist-info"
     for filename in ("WHEEL", "METADATA"):
         assert (dist / dist_info / filename).is_file()
 
@@ -249,18 +271,18 @@
 def test_build_editable(dist: Path, fixture_project: Path) -> None:
     wheel_name = api.build_editable(dist.as_posix())
     assert api.get_requires_for_build_editable() == ["editables"]
     with zipfile.ZipFile(dist / wheel_name) as zf:
         namelist = zf.namelist()
         assert "demo_package.pth" in namelist
         assert "_editable_impl_demo_package.py" in namelist
-        assert "demo_package-0.1.0+editable.dist-info/licenses/LICENSE" in namelist
+        assert "demo_package-0.1.0.dist-info/licenses/LICENSE" in namelist
 
         metadata = email.message_from_bytes(
-            zf.read("demo_package-0.1.0+editable.dist-info/METADATA")
+            zf.read("demo_package-0.1.0.dist-info/METADATA")
         )
         assert "editables" in metadata.get_all("Requires-Dist", [])
 
         pth_content = zf.read("demo_package.pth").decode("utf-8").strip()
         assert pth_content == "import _editable_impl_demo_package"
 
         proxy_module = zf.read("_editable_impl_demo_package.py").decode("utf-8").strip()
@@ -309,26 +331,26 @@
 
     with zipfile.ZipFile(dist / wheel_name) as zf:
         namelist = zf.namelist()
         assert "demo_package.pth" in namelist
         assert "__editables_demo_package.py" not in namelist
 
         metadata = email.message_from_bytes(
-            zf.read("demo_package-0.1.0+editable.dist-info/METADATA")
+            zf.read("demo_package-0.1.0.dist-info/METADATA")
         )
         assert "editables" not in metadata.get_all("Requires-Dist", [])
 
         pth_content = zf.read("demo_package.pth").decode("utf-8").strip()
         assert pth_content == str(fixture_project.resolve())
 
 
 @pytest.mark.parametrize("name", ["demo-package"])
 def test_prepare_metadata_for_editable(dist: Path) -> None:
     dist_info = api.prepare_metadata_for_build_editable(dist.as_posix())
-    assert dist_info == "demo_package-0.1.0+editable.dist-info"
+    assert dist_info == "demo_package-0.1.0.dist-info"
     with (dist / dist_info / "METADATA").open("rb") as metadata:
         deps = email.message_from_binary_file(metadata).get_all("Requires-Dist")
     assert "editables" in deps
 
 
 @pytest.mark.parametrize("name", ["demo-purelib-with-build"])
 def test_build_purelib_project_with_build(dist: Path) -> None:
@@ -395,14 +417,27 @@
 ) -> None:
     monkeypatch.setenv("PDM_BUILD_SCM_VERSION", "1.0.0")
     wheel_name = api.build_wheel(dist.as_posix())
     assert wheel_name == "foo-1.0.0-py3-none-any.whl"
 
 
 @pytest.mark.usefixtures("scm")
+@pytest.mark.parametrize("name", ["demo-using-scm"])
+def test_build_wheel_custom_version_format(fixture_project: Path, dist) -> None:
+    builder = WheelBuilder(fixture_project)
+    builder.config.data.setdefault("tool", {}).setdefault("pdm", {})["version"] = {
+        "source": "scm",
+        "version_format": "version:format_version",
+    }
+    with builder:
+        wheel = builder.build(dist)
+        assert wheel.name == "foo-0.1.0rc0-py3-none-any.whl"
+
+
+@pytest.mark.usefixtures("scm")
 @pytest.mark.parametrize("getter", ["get_version:run", "get_version:run()"])
 @pytest.mark.parametrize("name", ["demo-using-scm"])
 def test_get_version_from_call(fixture_project: Path, getter: str, dist: Path) -> None:
     builder = WheelBuilder(fixture_project)
     builder.config.data.setdefault("tool", {}).setdefault("pdm", {})["version"] = {
         "source": "call",
         "write_to": "foo/__version__.py",
```

### Comparing `pdm_backend-2.1.8/tests/test_file_finder.py` & `pdm_backend-2.2.0/tests/test_file_finder.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/test_hooks.py` & `pdm_backend-2.2.0/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/test_metadata.py` & `pdm_backend-2.2.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/test_utils.py` & `pdm_backend-2.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/tests/test_wheel.py` & `pdm_backend-2.2.0/tests/test_wheel.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.8/PKG-INFO` & `pdm_backend-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pdm-backend
-Version: 2.1.8
+Version: 2.2.0
 Summary: The build backend used by PDM that supports latest packaging standards
-Keywords: packaging PEP 517 build
+Keywords: packaging,PEP 517,build
 Author-Email: Frost Ming <me@frostming.com>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pdm-backend Version: 2.1.8 Summary: The build
+Metadata-Version: 2.1 Name: pdm-backend Version: 2.2.0 Summary: The build
 backend used by PDM that supports latest packaging standards Keywords:
-packaging PEP 517 build Author-Email: Frost Ming
+packaging,PEP 517,build Author-Email: Frost Ming
 frostming.com> License: MIT Classifier: Development Status :: 5 - Production/
 Stable Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Project-URL:
 Homepage, https://github.com/pdm-project/pdm-backend Project-URL: Repository,
```


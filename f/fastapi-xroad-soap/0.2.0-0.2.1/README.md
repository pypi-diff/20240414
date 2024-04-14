# Comparing `tmp/fastapi_xroad_soap-0.2.0.tar.gz` & `tmp/fastapi_xroad_soap-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_xroad_soap-0.2.0.tar", max compression
+gzip compressed data, was "fastapi_xroad_soap-0.2.1.tar", max compression
```

## Comparing `fastapi_xroad_soap-0.2.0.tar` & `fastapi_xroad_soap-0.2.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0    13749 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/LICENSE
--rw-r--r--   0        0        0     2813 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/README.md
--rw-r--r--   0        0        0      524 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/__init__.py
--rw-r--r--   0        0        0      567 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/elements.py
--rw-r--r--   0        0        0      471 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/faults.py
--rw-r--r--   0        0        0      340 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/__init__.py
--rw-r--r--   0        0        0      579 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/base/__init__.py
--rw-r--r--   0        0        0     4024 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/base/body.py
--rw-r--r--   0        0        0     1181 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/base/meta.py
--rw-r--r--   0        0        0     3024 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/base/spec.py
--rw-r--r--   0        0        0      955 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/cid_gen.py
--rw-r--r--   0        0        0     1119 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/constants.py
--rw-r--r--   0        0        0     1031 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/__init__.py
--rw-r--r--   0        0        0     1120 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/boolean.py
--rw-r--r--   0        0        0     2205 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/common.py
--rw-r--r--   0        0        0     1146 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/date.py
--rw-r--r--   0        0        0     1194 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/datetime.py
--rw-r--r--   0        0        0     1131 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/float.py
--rw-r--r--   0        0        0     1278 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/integer.py
--rw-r--r--   0        0        0     1201 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/netres.py
--rw-r--r--   0        0        0     1235 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/string.py
--rw-r--r--   0        0        0     5104 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/swaref.py
--rw-r--r--   0        0        0     1146 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/time.py
--rw-r--r--   0        0        0     3157 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/validators.py
--rw-r--r--   0        0        0      679 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/envelope/__init__.py
--rw-r--r--   0        0        0     2783 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/envelope/factory.py
--rw-r--r--   0        0        0     1401 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/envelope/generics.py
--rw-r--r--   0        0        0     1910 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/envelope/header.py
--rw-r--r--   0        0        0     1910 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/file_size.py
--rw-r--r--   0        0        0      732 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/multipart/__init__.py
--rw-r--r--   0        0        0     2801 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/multipart/bodypart.py
--rw-r--r--   0        0        0     2124 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/multipart/decoder.py
--rw-r--r--   0        0        0     2502 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/multipart/encoder.py
--rw-r--r--   0        0        0     1025 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/multipart/errors.py
--rw-r--r--   0        0        0      901 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/soap/__init__.py
--rw-r--r--   0        0        0     4627 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/soap/action.py
--rw-r--r--   0        0        0     4064 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/soap/faults.py
--rw-r--r--   0        0        0     2517 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/soap/response.py
--rw-r--r--   0        0        0     4822 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/soap/service.py
--rw-r--r--   0        0        0     1938 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/soap/service.pyi
--rw-r--r--   0        0        0     4957 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/storage.py
--rw-r--r--   0        0        0      874 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/utils/__init__.py
--rw-r--r--   0        0        0     1750 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/utils/content_utils.py
--rw-r--r--   0        0        0     2673 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/utils/path_utils.py
--rw-r--r--   0        0        0     2233 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/utils/route_utils.py
--rw-r--r--   0        0        0     2487 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/__init__.py
--rw-r--r--   0        0        0     2840 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/binding.py
--rw-r--r--   0        0        0     1558 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/conditions.py
--rw-r--r--   0        0        0     1334 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/definitions.py
--rw-r--r--   0        0        0      574 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/generator.py
--rw-r--r--   0        0        0     1534 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/port_type.py
--rw-r--r--   0        0        0     4947 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/restrictions.py
--rw-r--r--   0        0        0     2264 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/schema.py
--rw-r--r--   0        0        0     1335 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/service.py
--rw-r--r--   0        0        0      506 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/utils.py
--rw-r--r--   0        0        0     2579 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4534 1970-01-01 00:00:00.000000 fastapi_xroad_soap-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    13749 2024-04-13 21:13:46.321086 fastapi_xroad_soap-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2825 2024-04-13 21:13:46.321086 fastapi_xroad_soap-0.2.1/README.md
+-rw-r--r--   0        0        0      524 2024-04-13 21:13:46.321086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/__init__.py
+-rw-r--r--   0        0        0      567 2024-04-13 21:13:46.321086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/elements.py
+-rw-r--r--   0        0        0      471 2024-04-13 21:13:46.321086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/faults.py
+-rw-r--r--   0        0        0      340 2024-04-13 21:13:46.321086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/__init__.py
+-rw-r--r--   0        0        0      579 2024-04-13 21:13:46.321086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/base/__init__.py
+-rw-r--r--   0        0        0     4024 2024-04-13 21:13:46.321086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/base/body.py
+-rw-r--r--   0        0        0     1181 2024-04-13 21:13:46.321086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/base/meta.py
+-rw-r--r--   0        0        0     3024 2024-04-13 21:13:46.321086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/base/spec.py
+-rw-r--r--   0        0        0      955 2024-04-13 21:13:46.321086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/cid_gen.py
+-rw-r--r--   0        0        0     1119 2024-04-13 21:13:46.321086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/constants.py
+-rw-r--r--   0        0        0     1031 2024-04-13 21:13:46.321086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/__init__.py
+-rw-r--r--   0        0        0     1120 2024-04-13 21:13:46.321086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/boolean.py
+-rw-r--r--   0        0        0     2205 2024-04-13 21:13:46.321086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/common.py
+-rw-r--r--   0        0        0     1146 2024-04-13 21:13:46.321086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/date.py
+-rw-r--r--   0        0        0     1194 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/datetime.py
+-rw-r--r--   0        0        0     1131 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/float.py
+-rw-r--r--   0        0        0     1278 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/integer.py
+-rw-r--r--   0        0        0     1201 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/netres.py
+-rw-r--r--   0        0        0     1235 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/string.py
+-rw-r--r--   0        0        0     5104 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/swaref.py
+-rw-r--r--   0        0        0     1146 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/time.py
+-rw-r--r--   0        0        0     3157 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/validators.py
+-rw-r--r--   0        0        0      679 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/envelope/__init__.py
+-rw-r--r--   0        0        0     2783 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/envelope/factory.py
+-rw-r--r--   0        0        0     1401 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/envelope/generics.py
+-rw-r--r--   0        0        0     1910 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/envelope/header.py
+-rw-r--r--   0        0        0     1910 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/file_size.py
+-rw-r--r--   0        0        0      732 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/multipart/__init__.py
+-rw-r--r--   0        0        0     2801 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/multipart/bodypart.py
+-rw-r--r--   0        0        0     2124 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/multipart/decoder.py
+-rw-r--r--   0        0        0     2502 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/multipart/encoder.py
+-rw-r--r--   0        0        0     1025 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/multipart/errors.py
+-rw-r--r--   0        0        0      901 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/soap/__init__.py
+-rw-r--r--   0        0        0     4627 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/soap/action.py
+-rw-r--r--   0        0        0     4064 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/soap/faults.py
+-rw-r--r--   0        0        0     2517 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/soap/response.py
+-rw-r--r--   0        0        0     4822 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/soap/service.py
+-rw-r--r--   0        0        0     1938 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/soap/service.pyi
+-rw-r--r--   0        0        0     4957 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/storage.py
+-rw-r--r--   0        0        0      874 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/utils/__init__.py
+-rw-r--r--   0        0        0     1750 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/utils/content_utils.py
+-rw-r--r--   0        0        0     2673 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/utils/path_utils.py
+-rw-r--r--   0        0        0     2233 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/utils/route_utils.py
+-rw-r--r--   0        0        0     2487 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/wsdl/__init__.py
+-rw-r--r--   0        0        0     2840 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/wsdl/binding.py
+-rw-r--r--   0        0        0     1558 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/wsdl/conditions.py
+-rw-r--r--   0        0        0     1334 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/wsdl/definitions.py
+-rw-r--r--   0        0        0      574 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/wsdl/generator.py
+-rw-r--r--   0        0        0     1534 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/wsdl/port_type.py
+-rw-r--r--   0        0        0     4947 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/wsdl/restrictions.py
+-rw-r--r--   0        0        0     2264 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/wsdl/schema.py
+-rw-r--r--   0        0        0     1335 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/wsdl/service.py
+-rw-r--r--   0        0        0      506 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/utils.py
+-rw-r--r--   0        0        0     2579 2024-04-13 21:13:46.325086 fastapi_xroad_soap-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4546 1970-01-01 00:00:00.000000 fastapi_xroad_soap-0.2.1/PKG-INFO
```

### Comparing `fastapi_xroad_soap-0.2.0/LICENSE` & `fastapi_xroad_soap-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/README.md` & `fastapi_xroad_soap-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # FastAPI X-Road SOAP
 
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fastapi-xroad-soap)](https://pypi.org/project/fastapi-xroad-soap/)
-[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/rik-ee/fastapi-xroad-soap/publish.yaml)](https://github.com/rik-ee/fastapi-xroad-soap/actions/workflows/publish.yaml)
-[![codecov](https://codecov.io/gh/rik-ee/fastapi-xroad-soap/graph/badge.svg?token=jymcRynp2P)](https://codecov.io/gh/rik-ee/fastapi-xroad-soap)
+[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/rik-ee/fastapi-xroad-soap/build-publish.yaml)](https://github.com/rik-ee/fastapi-xroad-soap/actions/workflows/build-publish.yaml)
+[![codecov](https://codecov.io/gh/rik-ee/fastapi-xroad-soap/graph/badge.svg?token=KB58NGDC1N)](https://codecov.io/gh/rik-ee/fastapi-xroad-soap)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/fastapi-xroad-soap)](https://pypistats.org/packages/fastapi-xroad-soap)
 
 
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=rik-ee_fastapi-xroad-soap&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=rik-ee_fastapi-xroad-soap)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=rik-ee_fastapi-xroad-soap&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=rik-ee_fastapi-xroad-soap)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=rik-ee_fastapi-xroad-soap&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=rik-ee_fastapi-xroad-soap)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=rik-ee_fastapi-xroad-soap&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=rik-ee_fastapi-xroad-soap)<br/>
```

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/__init__.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/elements.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/elements.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/base/__init__.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/base/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/base/body.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/base/body.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/base/meta.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/base/meta.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/base/spec.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/base/spec.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/cid_gen.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/cid_gen.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/constants.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/constants.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/__init__.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/boolean.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/boolean.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/common.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/common.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/date.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/date.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/datetime.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/datetime.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/float.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/float.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/integer.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/integer.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/netres.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/netres.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/string.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/string.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/swaref.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/swaref.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/time.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/time.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/validators.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/elements/validators.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/envelope/__init__.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/envelope/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/envelope/factory.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/envelope/factory.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/envelope/generics.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/envelope/generics.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/envelope/header.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/envelope/header.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/file_size.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/file_size.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/multipart/__init__.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/multipart/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/multipart/bodypart.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/multipart/bodypart.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/multipart/decoder.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/multipart/decoder.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/multipart/encoder.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/multipart/encoder.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/multipart/errors.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/multipart/errors.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/soap/__init__.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/soap/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/soap/action.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/soap/action.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/soap/faults.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/soap/faults.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/soap/response.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/soap/response.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/soap/service.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/soap/service.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/soap/service.pyi` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/soap/service.pyi`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/storage.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/storage.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/utils/__init__.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/utils/content_utils.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/utils/content_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/utils/path_utils.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/utils/route_utils.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/utils/route_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/__init__.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/wsdl/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/binding.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/wsdl/binding.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/conditions.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/wsdl/conditions.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/definitions.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/wsdl/definitions.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/generator.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/wsdl/generator.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/port_type.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/wsdl/port_type.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/restrictions.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/wsdl/restrictions.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/schema.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/wsdl/schema.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/service.py` & `fastapi_xroad_soap-0.2.1/fastapi_xroad_soap/internal/wsdl/service.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.0/pyproject.toml` & `fastapi_xroad_soap-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-xroad-soap"
-version = "0.2.0"
+version = "0.2.1"
 description = "FastAPI Extension for X-Road SOAP"
 authors = ["Zero Reports Team <zero.dev@rik.ee>"]
 license = "EUPL-1.2"
 readme = "README.md"
 keywords = ["fastapi", "xroad", "soap"]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `fastapi_xroad_soap-0.2.0/PKG-INFO` & `fastapi_xroad_soap-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-xroad-soap
-Version: 0.2.0
+Version: 0.2.1
 Summary: FastAPI Extension for X-Road SOAP
 License: EUPL-1.2
 Keywords: fastapi,xroad,soap
 Author: Zero Reports Team
 Author-email: zero.dev@rik.ee
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -38,16 +38,16 @@
 Project-URL: Repository, https://github.com/rik-ee/fastapi-xroad-soap
 Description-Content-Type: text/markdown
 
 # FastAPI X-Road SOAP
 
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fastapi-xroad-soap)](https://pypi.org/project/fastapi-xroad-soap/)
-[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/rik-ee/fastapi-xroad-soap/publish.yaml)](https://github.com/rik-ee/fastapi-xroad-soap/actions/workflows/publish.yaml)
-[![codecov](https://codecov.io/gh/rik-ee/fastapi-xroad-soap/graph/badge.svg?token=jymcRynp2P)](https://codecov.io/gh/rik-ee/fastapi-xroad-soap)
+[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/rik-ee/fastapi-xroad-soap/build-publish.yaml)](https://github.com/rik-ee/fastapi-xroad-soap/actions/workflows/build-publish.yaml)
+[![codecov](https://codecov.io/gh/rik-ee/fastapi-xroad-soap/graph/badge.svg?token=KB58NGDC1N)](https://codecov.io/gh/rik-ee/fastapi-xroad-soap)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/fastapi-xroad-soap)](https://pypistats.org/packages/fastapi-xroad-soap)
 
 
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=rik-ee_fastapi-xroad-soap&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=rik-ee_fastapi-xroad-soap)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=rik-ee_fastapi-xroad-soap&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=rik-ee_fastapi-xroad-soap)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=rik-ee_fastapi-xroad-soap&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=rik-ee_fastapi-xroad-soap)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=rik-ee_fastapi-xroad-soap&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=rik-ee_fastapi-xroad-soap)<br/>
```


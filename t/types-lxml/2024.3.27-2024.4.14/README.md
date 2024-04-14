# Comparing `tmp/types-lxml-2024.3.27.tar.gz` & `tmp/types_lxml-2024.4.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-lxml-2024.3.27.tar", last modified: Wed Mar 27 16:40:34 2024, max compression
+gzip compressed data, was "types_lxml-2024.4.14.tar", last modified: Sun Apr 14 04:10:42 2024, max compression
```

## Comparing `types-lxml-2024.3.27.tar` & `types_lxml-2024.4.14.tar`

### file list

```diff
@@ -1,122 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:40:34.955053 types-lxml-2024.3.27/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:40:34.935053 types-lxml-2024.3.27/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:40:34.935053 types-lxml-2024.3.27/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/.github/workflows/compat.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/.github/workflows/pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/.github/workflows/test_inc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7863 2024-03-27 16:40:34.955053 types-lxml-2024.3.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:40:34.935053 types-lxml-2024.3.27/lxml-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/ElementInclude.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/_types.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/builder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/cssselect.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:40:34.939053 types-lxml-2024.3.27/lxml-stubs/etree/
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/etree/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/etree/_classlookup.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/etree/_cleanup.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/etree/_docloader.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/etree/_dtd.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17557 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/etree/_element.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/etree/_factory_func.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10348 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/etree/_iterparse.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/etree/_module_func.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/etree/_module_misc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/etree/_nsclasses.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/etree/_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/etree/_relaxng.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/etree/_saxparser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/etree/_serializer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/etree/_xinclude.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/etree/_xmlerror.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/etree/_xmlid.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/etree/_xmlschema.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/etree/_xpath.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/etree/_xslt.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:40:34.943053 types-lxml-2024.3.27/lxml-stubs/html/
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/html/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9762 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/html/_element.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/html/_form.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/html/_funcs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/html/_parse.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/html/builder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/html/clean.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/html/defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/html/diff.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/html/html5parser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/html/soupparser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/isoschematron.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:40:34.943053 types-lxml-2024.3.27/lxml-stubs/objectify/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/objectify/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8896 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/objectify/_annotate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/objectify/_element.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9175 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/objectify/_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/objectify/_misc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/lxml-stubs/sax.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 16:40:34.955053 types-lxml-2024.3.27/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:40:34.943053 types-lxml-2024.3.27/test-rt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-rt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:40:34.947053 types-lxml-2024.3.27/test-rt/_testutils/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-rt/_testutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-rt/_testutils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-rt/_testutils/pyright_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-rt/_testutils/rt_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-rt/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:40:34.947053 types-lxml-2024.3.27/test-rt/data/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-rt/data/mdn-sample.html
--rw-r--r--   0 runner    (1001) docker     (127)    44825 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-rt/data/sample.html
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-rt/data/shiporder.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-rt/data/shiporder.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-rt/data/w3c-example.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-rt/test_attrib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-rt/test_elem_class_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-rt/test_errorlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-rt/test_html5lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    11232 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-rt/test_html_link_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-rt/test_iterparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-rt/test_xinclude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:40:34.951053 types-lxml-2024.3.27/test-stub/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/mypy-pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/no-test-custom-target.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/test-annotations.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/test-builder.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/test-classlookup.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/test-cssselect.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/test-dtd.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16136 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/test-etree-element.yml
--rw-r--r--   0 runner    (1001) docker     (127)    13483 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/test-etree-et.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/test-etree.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/test-html-clean.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/test-html-element.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/test-mypy-bug.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/test-nsclasses.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/test-oe-element.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/test-oe.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/test-resolver.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/test-sax.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/test-serializer.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/test-soupparser.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/test-validator.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/test-xmlid.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/test-xpath.yml
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/test-stub/test-xslt.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-03-27 16:40:13.000000 types-lxml-2024.3.27/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:40:34.951053 types-lxml-2024.3.27/types_lxml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7863 2024-03-27 16:40:34.000000 types-lxml-2024.3.27/types_lxml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-03-27 16:40:34.000000 types-lxml-2024.3.27/types_lxml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 16:40:34.000000 types-lxml-2024.3.27/types_lxml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-27 16:40:34.000000 types-lxml-2024.3.27/types_lxml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-27 16:40:34.000000 types-lxml-2024.3.27/types_lxml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:10:42.288109 types_lxml-2024.4.14/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:10:42.268109 types_lxml-2024.4.14/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:10:42.268109 types_lxml-2024.4.14/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/.github/workflows/compat.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/.github/workflows/pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/.github/workflows/test_inc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-04-14 04:10:42.288109 types_lxml-2024.4.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:10:42.268109 types_lxml-2024.4.14/lxml-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/ElementInclude.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/_types.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/builder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/cssselect.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:10:42.272109 types_lxml-2024.4.14/lxml-stubs/etree/
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/etree/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/etree/_classlookup.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/etree/_cleanup.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/etree/_docloader.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/etree/_dtd.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18118 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/etree/_element.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/etree/_factory_func.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10406 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/etree/_iterparse.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/etree/_module_func.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/etree/_module_misc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/etree/_nsclasses.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/etree/_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/etree/_relaxng.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/etree/_saxparser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/etree/_serializer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/etree/_xinclude.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/etree/_xmlerror.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/etree/_xmlid.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/etree/_xmlschema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/etree/_xpath.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/etree/_xslt.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:10:42.276109 types_lxml-2024.4.14/lxml-stubs/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/html/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/html/_element.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/html/_form.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/html/_funcs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/html/_parse.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/html/builder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/html/clean.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/html/defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/html/diff.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/html/html5parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/html/soupparser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/isoschematron.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:10:42.276109 types_lxml-2024.4.14/lxml-stubs/objectify/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/objectify/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/objectify/_annotate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/objectify/_element.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/objectify/_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/objectify/_misc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/lxml-stubs/sax.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 04:10:42.288109 types_lxml-2024.4.14/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:10:42.280109 types_lxml-2024.4.14/test-rt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-rt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:10:42.280109 types_lxml-2024.4.14/test-rt/_testutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-rt/_testutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-rt/_testutils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-rt/_testutils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-rt/_testutils/pyright_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-rt/_testutils/rt_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-rt/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:10:42.280109 types_lxml-2024.4.14/test-rt/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-rt/data/mdn-sample.html
+-rw-r--r--   0 runner    (1001) docker     (127)    44825 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-rt/data/sample.html
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-rt/data/shiporder.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-rt/data/shiporder.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-rt/data/w3c-example.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-rt/test_attrib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-rt/test_beautifulsoup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-rt/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-rt/test_elem_class_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8126 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-rt/test_errorlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9917 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-rt/test_html5lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-rt/test_html_link_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-rt/test_iterparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-rt/test_xinclude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:10:42.284109 types_lxml-2024.4.14/test-stub/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/mypy-pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/no-test-custom-target.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/test-annotations.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/test-builder.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/test-classlookup.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/test-cssselect.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/test-dtd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16136 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/test-etree-element.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    13539 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/test-etree-et.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/test-etree.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/test-html-clean.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/test-html-element.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/test-mypy-bug.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/test-nsclasses.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/test-oe-element.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/test-oe.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/test-resolver.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/test-sax.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/test-serializer.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/test-validator.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/test-xmlid.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/test-xpath.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/test-stub/test-xslt.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-14 04:10:17.000000 types_lxml-2024.4.14/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:10:42.288109 types_lxml-2024.4.14/types_lxml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-04-14 04:10:42.000000 types_lxml-2024.4.14/types_lxml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-14 04:10:42.000000 types_lxml-2024.4.14/types_lxml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 04:10:42.000000 types_lxml-2024.4.14/types_lxml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-14 04:10:42.000000 types_lxml-2024.4.14/types_lxml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-14 04:10:42.000000 types_lxml-2024.4.14/types_lxml.egg-info/top_level.txt
```

### Comparing `types-lxml-2024.3.27/.github/workflows/compat.yml` & `types_lxml-2024.4.14/.github/workflows/compat.yml`

 * *Files 23% similar despite different names*

```diff
@@ -5,25 +5,14 @@
 
 jobs:
   mypy_compat:
     strategy:
       fail-fast: false
       matrix:
         myver:
-          - 1.2.0
-          - 1.3.0
-          - 1.4.0
-          - 1.4.1
-          - 1.5.0
-          - 1.5.1
-          # - 1.6.0
-          - 1.6.1
-          - 1.7.0
-          - 1.7.1
-          - 1.8.0
           - 1.9.0
     runs-on: ubuntu-22.04
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
           python-version: 3.11
@@ -101,14 +90,19 @@
           - 1.1.347
           - 1.1.348
           - 1.1.349
           - 1.1.350
           - 1.1.351
           - 1.1.352
           - 1.1.353
+          - 1.1.354
+          - 1.1.355
+          - 1.1.356
+          - 1.1.357
+          - 1.1.358
     runs-on: ubuntu-22.04
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
           python-version: 3.11
           cache: 'pip'
```

### Comparing `types-lxml-2024.3.27/.github/workflows/format.yml` & `types_lxml-2024.4.14/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/.github/workflows/pr.yml` & `types_lxml-2024.4.14/.github/workflows/pr.yml`

 * *Files 5% similar despite different names*

```diff
@@ -31,18 +31,18 @@
 
     - name: Mypy review
       id: mypy
       uses: tsuyoshicho/action-mypy@v4
       with:
         reporter: github-pr-review
         level: warning
-        workdir: lxml-stubs
+        target: lxml-stubs
         fail_on_error: true
         ignore_note: true
-        setup_command: pip install mypy==1.5.1
+        setup_command: pip install mypy==1.9.*
         setup_method: install
         install_types: false
 
     - name: Pyright review
       id: pyright
       if: success() || steps.mypy.conclusion == 'failure'
       uses: jordemort/action-pyright@v1
```

### Comparing `types-lxml-2024.3.27/.github/workflows/release.yml` & `types_lxml-2024.4.14/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/.github/workflows/test_inc.yml` & `types_lxml-2024.4.14/.github/workflows/test_inc.yml`

 * *Files 6% similar despite different names*

```diff
@@ -108,14 +108,17 @@
           - "3.10"
           - "3.11"
           - "3.12"
         os:
           - ubuntu-22.04
           - windows-2022
           - macos-13
+        exclude:
+          - pyver: "3.10"  # lxml package cache hash mismatch
+            os: "macos-13"
     runs-on: ${{ matrix.os }}
     steps:
     - uses: actions/checkout@v4
 
     - uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.pyver }}
@@ -170,10 +173,10 @@
       uses: actions/upload-artifact@v4
       with:
         name: all-logs
         path: all-logs
         if-no-files-found: error
 
     - name: Remove individual logs
-      uses: geekyeggo/delete-artifact@v4
+      uses: geekyeggo/delete-artifact@v5
       with:
         name: log-*
```

### Comparing `types-lxml-2024.3.27/.gitignore` & `types_lxml-2024.4.14/.gitignore`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/LICENSE` & `types_lxml-2024.4.14/LICENSE`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/PKG-INFO` & `types_lxml-2024.4.14/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-lxml
-Version: 2024.3.27
+Version: 2024.4.14
 Summary: Complete lxml external type annotation
 Author-email: Abel Cheung <abelcheung@gmail.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/abelcheung/types-lxml
 Keywords: lxml,typing,stubs,annotation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -15,46 +15,48 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Stubs Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: types-beautifulsoup4
+Requires-Dist: types-beautifulsoup4~=4.12
 Requires-Dist: typing_extensions~=4.5
 Requires-Dist: cssselect~=1.2
 Provides-Extra: test
 Requires-Dist: tox~=4.0; extra == "test"
-Requires-Dist: mypy==1.5.1; extra == "test"
+Requires-Dist: mypy==1.9.*; extra == "test"
 Requires-Dist: pyright>=1.1.289; extra == "test"
 Requires-Dist: typeguard<5,>=3.0; extra == "test"
 Requires-Dist: pytest<9,>=7.0; extra == "test"
 Requires-Dist: html5lib==1.1; extra == "test"
-Requires-Dist: pytest-mypy-plugins!=1.10.0,~=1.10; extra == "test"
-Requires-Dist: lxml==5.1.*; extra == "test"
+Requires-Dist: pytest-mypy-plugins==1.11.1; extra == "test"
+Requires-Dist: lxml>=4.9; extra == "test"
+Requires-Dist: beautifulsoup4~=4.8; extra == "test"
 
 [![PyPI version](https://img.shields.io/pypi/v/types-lxml.svg)](https://pypi.org/project/types-lxml/)
 ![Supported Python](https://img.shields.io/pypi/pyversions/types-lxml.svg)
 ![Wheel](https://img.shields.io/pypi/wheel/types-lxml.svg)
 
 ## Important note
 
-Currently `types-lxml` shouldn't be used with `mypy` ≥ 1.6. The untested 1.6.0 [simply segfaults](https://github.com/python/mypy/issues/16278), while all later versions don't support `@overload` with `@deprecation`, which is [scheduled for Python 3.13](https://peps.python.org/pep-0702/).
+- `types-lxml 2024.03.27` release requires [cssselect package](https://pypi.org/project/cssselect/) to work, since `lxml.cssselect` submodule utilises inline annotation from `cssselect 1.2.0`.
+- Next release (`2024.04.14`) requires `mypy 1.9`; `2024.03.27` is the last release supporting `mypy 1.5`.
 
 ## Introduction
 
 This repository contains [external type annotations](https://peps.python.org/pep-0561/) for [`lxml`](http://lxml.de/). It can be used by type-checking tools (currently supporting [`mypy`](https://pypi.org/project/mypy/) and [`pyright`](https://github.com/Microsoft/pyright)) to check code that uses `lxml`, or used within IDEs like [VSCode](https://code.visualstudio.com/) or [PyCharm](https://www.jetbrains.com/pycharm/) to facilitate development.
 
 ## Goal ① : Completion
 
 Now the coverage of `lxml` submodules is complete (unless intentionally rejected, see further below), thus no more [considered as `partial`](https://peps.python.org/pep-0561/#partial-stub-packages):
   - [x] `lxml.etree`
   - [x] `lxml.html`
     - [x] `lxml.html.builder`
-    - [x] `lxml.html.clean`
+    - [x] `lxml.html.clean` (already removed in lxml 5.2.0, this project will follow suite in future)
     - [x] `lxml.html.diff`
     - [x] `lxml.html.html5parser`
     - [x] `lxml.html.soupparser`
   - [x] `lxml.isoschematron`
   - [x] `lxml.objectify`
   - [x] `lxml.builder`
   - [x] `lxml.cssselect`
@@ -68,26 +70,26 @@
   - `lxml.html.usedoctest`
   - `lxml.html.formfill` (shouldn't have existed, this would belong to HTTP libraries like `requests` or `httpx`)
 
 Check out [project page](https://github.com/abelcheung/types-lxml/projects/1) for future plans and progress.
 
 ## Goal ② : Support multiple type checkers
 
-Currently the annotations are validated for both `mypy` and `pyright` strict mode.
+Currently the annotations are validated for both `mypy` and `pyright`.
 
 In the future, there is plan to bring even more type checker support.
 
 ## Goal ③: Review and test suite
 
 - [x] All prior `lxml-stubs` contributions are reviewed thoroughly, bringing coherency of annotation across the whole package
 - [x] Much more extensive test cases
   - [x] Mypy test suite already vastly expanded
   - [x] Perform runtime check, and compare against static type checker result; this guarantees annotations are indeed working in real code, not just in some cooked up test suite
     - [x] Proof of concept for incorporating `pyright` result under progress, currently just comparing `reveal_type()` results
-    - [ ] Migrate static `mypy` tests to runtime `pyright` tests in future
+    - [ ] Migrate static `mypy` tests to runtime `pyright` tests in future (under progress)
 - [x] Modernize package building infrastructure
 
 ## Goal ④ : Support for IDEs
 
 Despite having no official PEP, some IDEs support showing docstring from external annotations. This package tries to bring type annotation specific docstrings for some `lxml` classes and functions, explaining how they can be used. Following screenshots show what would look like in Visual Studio Code, behaving as if docstrings come from real python code:
 
 ![Stub docstring in VSCode mouseover tooltip](https://user-images.githubusercontent.com/83110/277119481-debbd929-afbd-4f59-b9e6-52a1f7f23241.png)
@@ -109,55 +111,13 @@
 
     pip install -U types-lxml*.whl
 
 ### Bleeding edge from GitHub
 
     pip install -U git+https://github.com/abelcheung/types-lxml.git
 
-## Special notes
-
-### Type checker support
-
-Actually, `pyright` is the preferred type checker to use for `lxml` code. `mypy` can be either too restrictive or doesn't support some feature needed by lxml.
-
-Here is one example: normalisation of element attributes.
-
-It is employed by many other projects, so that users can supply common type of value while setting object attributes, and the code internally canonicalise/converts supplied argument to specific type. This is a convenience for library users, so they don't always need to do internal conversion by themselves. Consider the example below:
-
-```python
-from typing_extensions import reveal_type
-from lxml.etree import fromstring, QName
-
-person = fromstring('<person><height>170</height></person>')
-reveal_type(person[0].tag)
-person[0].tag = QName('http://ns.prefix', person[0].tag)
-```
-
-Lxml supports stringify QNames when setting element tags. Of course, during runtime, everything work as expected:
-
-```pycon
->>> print(e.tostring(person, encoding=str))
-<person><ns0:height xmlns:ns0="http://ns.prefix">170</ns0:height></person>
-```
-
-`pyright` correctly reports element tag type, and don't complain about assignment:
-
-```
-information: Type of "person[0].tag" is "str"
-```
-
-But `mypy` barks loudly about the feature:
-
-```
-error: Incompatible types in assignment (expression has type "QName", variable has type "str")  [assignment]
-```
-
-There are many, many more places in lxml that employs such normalisation.
-
-### ParserTarget
-There is now only one stub-only classes that do not exist as concrete class in `lxml` &mdash; `lxml.etree.ParserTarget`. However the support of custom parser target is shelved, so this virtual class is not very relevant for now.
 
 ## History
 
-Type annotations for `lxml` were initially included in [typeshed](https://www.github.com/python/typeshed), but as it was still incomplete at that time, the stubs are [ripped out as a separate project](https://github.com/python/typeshed/issues/525). The code was extracted by Jelle Zijlstra and moved to `lxml-stubs` repository using `git filter-branch`.
+Type annotations for `lxml` were initially included in [typeshed](https://www.github.com/python/typeshed), but as it was still incomplete at that time, the stubs are [ripped out as a separate project](https://github.com/python/typeshed/issues/525). The code was since then under governance of lxml, until 2022 when this fork intended to revamp `lxml-stubs` completely and emerge into separate project.
 
 `types-lxml` is a fork of `lxml-stubs` that strives for the goals described above, so that most people would find it more useful.
```

### Comparing `types-lxml-2024.3.27/README.md` & `types_lxml-2024.4.14/types_lxml.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,62 @@
+Metadata-Version: 2.1
+Name: types-lxml
+Version: 2024.4.14
+Summary: Complete lxml external type annotation
+Author-email: Abel Cheung <abelcheung@gmail.com>
+License: Apache-2.0
+Project-URL: homepage, https://github.com/abelcheung/types-lxml
+Keywords: lxml,typing,stubs,annotation
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: types-beautifulsoup4~=4.12
+Requires-Dist: typing_extensions~=4.5
+Requires-Dist: cssselect~=1.2
+Provides-Extra: test
+Requires-Dist: tox~=4.0; extra == "test"
+Requires-Dist: mypy==1.9.*; extra == "test"
+Requires-Dist: pyright>=1.1.289; extra == "test"
+Requires-Dist: typeguard<5,>=3.0; extra == "test"
+Requires-Dist: pytest<9,>=7.0; extra == "test"
+Requires-Dist: html5lib==1.1; extra == "test"
+Requires-Dist: pytest-mypy-plugins==1.11.1; extra == "test"
+Requires-Dist: lxml>=4.9; extra == "test"
+Requires-Dist: beautifulsoup4~=4.8; extra == "test"
+
 [![PyPI version](https://img.shields.io/pypi/v/types-lxml.svg)](https://pypi.org/project/types-lxml/)
 ![Supported Python](https://img.shields.io/pypi/pyversions/types-lxml.svg)
 ![Wheel](https://img.shields.io/pypi/wheel/types-lxml.svg)
 
 ## Important note
 
-Currently `types-lxml` shouldn't be used with `mypy` ≥ 1.6. The untested 1.6.0 [simply segfaults](https://github.com/python/mypy/issues/16278), while all later versions don't support `@overload` with `@deprecation`, which is [scheduled for Python 3.13](https://peps.python.org/pep-0702/).
+- `types-lxml 2024.03.27` release requires [cssselect package](https://pypi.org/project/cssselect/) to work, since `lxml.cssselect` submodule utilises inline annotation from `cssselect 1.2.0`.
+- Next release (`2024.04.14`) requires `mypy 1.9`; `2024.03.27` is the last release supporting `mypy 1.5`.
 
 ## Introduction
 
 This repository contains [external type annotations](https://peps.python.org/pep-0561/) for [`lxml`](http://lxml.de/). It can be used by type-checking tools (currently supporting [`mypy`](https://pypi.org/project/mypy/) and [`pyright`](https://github.com/Microsoft/pyright)) to check code that uses `lxml`, or used within IDEs like [VSCode](https://code.visualstudio.com/) or [PyCharm](https://www.jetbrains.com/pycharm/) to facilitate development.
 
 ## Goal ① : Completion
 
 Now the coverage of `lxml` submodules is complete (unless intentionally rejected, see further below), thus no more [considered as `partial`](https://peps.python.org/pep-0561/#partial-stub-packages):
   - [x] `lxml.etree`
   - [x] `lxml.html`
     - [x] `lxml.html.builder`
-    - [x] `lxml.html.clean`
+    - [x] `lxml.html.clean` (already removed in lxml 5.2.0, this project will follow suite in future)
     - [x] `lxml.html.diff`
     - [x] `lxml.html.html5parser`
     - [x] `lxml.html.soupparser`
   - [x] `lxml.isoschematron`
   - [x] `lxml.objectify`
   - [x] `lxml.builder`
   - [x] `lxml.cssselect`
@@ -34,26 +70,26 @@
   - `lxml.html.usedoctest`
   - `lxml.html.formfill` (shouldn't have existed, this would belong to HTTP libraries like `requests` or `httpx`)
 
 Check out [project page](https://github.com/abelcheung/types-lxml/projects/1) for future plans and progress.
 
 ## Goal ② : Support multiple type checkers
 
-Currently the annotations are validated for both `mypy` and `pyright` strict mode.
+Currently the annotations are validated for both `mypy` and `pyright`.
 
 In the future, there is plan to bring even more type checker support.
 
 ## Goal ③: Review and test suite
 
 - [x] All prior `lxml-stubs` contributions are reviewed thoroughly, bringing coherency of annotation across the whole package
 - [x] Much more extensive test cases
   - [x] Mypy test suite already vastly expanded
   - [x] Perform runtime check, and compare against static type checker result; this guarantees annotations are indeed working in real code, not just in some cooked up test suite
     - [x] Proof of concept for incorporating `pyright` result under progress, currently just comparing `reveal_type()` results
-    - [ ] Migrate static `mypy` tests to runtime `pyright` tests in future
+    - [ ] Migrate static `mypy` tests to runtime `pyright` tests in future (under progress)
 - [x] Modernize package building infrastructure
 
 ## Goal ④ : Support for IDEs
 
 Despite having no official PEP, some IDEs support showing docstring from external annotations. This package tries to bring type annotation specific docstrings for some `lxml` classes and functions, explaining how they can be used. Following screenshots show what would look like in Visual Studio Code, behaving as if docstrings come from real python code:
 
 ![Stub docstring in VSCode mouseover tooltip](https://user-images.githubusercontent.com/83110/277119481-debbd929-afbd-4f59-b9e6-52a1f7f23241.png)
@@ -75,55 +111,13 @@
 
     pip install -U types-lxml*.whl
 
 ### Bleeding edge from GitHub
 
     pip install -U git+https://github.com/abelcheung/types-lxml.git
 
-## Special notes
-
-### Type checker support
-
-Actually, `pyright` is the preferred type checker to use for `lxml` code. `mypy` can be either too restrictive or doesn't support some feature needed by lxml.
-
-Here is one example: normalisation of element attributes.
-
-It is employed by many other projects, so that users can supply common type of value while setting object attributes, and the code internally canonicalise/converts supplied argument to specific type. This is a convenience for library users, so they don't always need to do internal conversion by themselves. Consider the example below:
-
-```python
-from typing_extensions import reveal_type
-from lxml.etree import fromstring, QName
-
-person = fromstring('<person><height>170</height></person>')
-reveal_type(person[0].tag)
-person[0].tag = QName('http://ns.prefix', person[0].tag)
-```
-
-Lxml supports stringify QNames when setting element tags. Of course, during runtime, everything work as expected:
-
-```pycon
->>> print(e.tostring(person, encoding=str))
-<person><ns0:height xmlns:ns0="http://ns.prefix">170</ns0:height></person>
-```
-
-`pyright` correctly reports element tag type, and don't complain about assignment:
-
-```
-information: Type of "person[0].tag" is "str"
-```
-
-But `mypy` barks loudly about the feature:
-
-```
-error: Incompatible types in assignment (expression has type "QName", variable has type "str")  [assignment]
-```
-
-There are many, many more places in lxml that employs such normalisation.
-
-### ParserTarget
-There is now only one stub-only classes that do not exist as concrete class in `lxml` &mdash; `lxml.etree.ParserTarget`. However the support of custom parser target is shelved, so this virtual class is not very relevant for now.
 
 ## History
 
-Type annotations for `lxml` were initially included in [typeshed](https://www.github.com/python/typeshed), but as it was still incomplete at that time, the stubs are [ripped out as a separate project](https://github.com/python/typeshed/issues/525). The code was extracted by Jelle Zijlstra and moved to `lxml-stubs` repository using `git filter-branch`.
+Type annotations for `lxml` were initially included in [typeshed](https://www.github.com/python/typeshed), but as it was still incomplete at that time, the stubs are [ripped out as a separate project](https://github.com/python/typeshed/issues/525). The code was since then under governance of lxml, until 2022 when this fork intended to revamp `lxml-stubs` completely and emerge into separate project.
 
 `types-lxml` is a fork of `lxml-stubs` that strives for the goals described above, so that most people would find it more useful.
```

### Comparing `types-lxml-2024.3.27/SECURITY.md` & `types_lxml-2024.4.14/SECURITY.md`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/lxml-stubs/_types.pyi` & `types_lxml-2024.4.14/lxml-stubs/_types.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 )
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:
     from typing_extensions import TypeAlias
 
-from .etree import QName, _Element, _ElementTree
+from .etree import HTMLParser, QName, XMLParser, _Element, _ElementTree
 
 # Dup but deviate from recent _typeshed
 Unused: TypeAlias = Any
 
 # ElementTree API is notable of canonicalizing byte / unicode input data.
 # This type alias should only be used for input arguments, while one would
 # expect plain str in return type for most part of API (except a few places),
@@ -98,43 +98,43 @@
 _ElemClsLookupArg = Literal["element", "comment", "PI", "entity"]
 
 # serializer.pxi _findOutputMethod()
 _OutputMethodArg = Literal[
     "html",
     "text",
     "xml",
-    "HTML",
-    "TEXT",
-    "XML",
 ]
 
 # saxparser.pxi _buildParseEventFilter()
 _SaxEventNames = Literal[
     "start",
     "end",
     "start-ns",
     "end-ns",
     "comment",
     "pi",
 ]
 
-_ET = TypeVar("_ET", bound=_Element)
-_ET_co = TypeVar("_ET_co", bound=_Element, covariant=True)
+_ET = TypeVar("_ET", bound=_Element, default=_Element)
+_ET_co = TypeVar("_ET_co", bound=_Element, default=_Element, covariant=True)
 
 # Generic element factory function type. Because arguments are
 # mostly optional, accurate typing can't be done.
 _ElemFactory: TypeAlias = Callable[..., _ET]
 
 # Note that _TagSelector filters element type not by classes,
 # but checks for exact element *factory functions* instead
 # (etree.Element() and friends). Python typing system doesn't
 # support such outlandish usage. Use a generic callable instead.
-_TagSelector: TypeAlias = _TagName | _ElemFactory[_Element]
+_TagSelector: TypeAlias = _TagName | _ElemFactory
 
-_ElementOrTree: TypeAlias = _Element | _ElementTree[_Element]
+_ElementOrTree: TypeAlias = _ET | _ElementTree[_ET]
+
+# The basic parsers bundled in lxml.etree
+_DefEtreeParsers = XMLParser[_ET_co] | HTMLParser[_ET_co]
 
 class SupportsLaxedItems(Protocol[_KT_co, _VT_co]):
     """Relaxed form of SupportsItems
 
     Original SupportsItems from typeshed returns generic set which
     is compatible with ItemsView. However, _Attrib doesn't conform
     and returns list instead. Gotta find a common ground here.
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/builder.pyi` & `types_lxml-2024.4.14/lxml-stubs/builder.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 from typing import Any, Callable, Generic, Mapping, overload
 
-from ._types import _ElemFactory, _ET_co, _NSMapArg
-from .etree import QName, _Element
+from ._types import _ElemFactory, _ET_co, _NSMapArg, _TagName
+from .etree import _Element
 
+# Mapping should have been something like
+# Mapping[type[_T], Callable[[_Element, _T], None]]
+# but invariant key/value causes it to be incompatible
+# with anything
 _TypeMapArg = Mapping[Any, Callable[[_Element, Any], None]]
 
 class ElementMaker(Generic[_ET_co]):
     @overload
     def __new__(
         cls,
-        typemap: _TypeMapArg | None = ...,
-        namespace: str | None = ...,
-        nsmap: _NSMapArg | None = ...,
+        typemap: _TypeMapArg | None = None,
+        namespace: str | None = None,
+        nsmap: _NSMapArg | None = None,
         *,
         makeelement: _ElemFactory[_ET_co],
     ) -> ElementMaker[_ET_co]: ...
     @overload
     def __new__(
         cls,
         typemap: _TypeMapArg | None,
         namespace: str | None,
         nsmap: _NSMapArg | None,
         makeelement: _ElemFactory[_ET_co],
     ) -> ElementMaker[_ET_co]: ...
     @overload
     def __new__(
         cls,
-        typemap: _TypeMapArg | None = ...,
-        namespace: str | None = ...,
-        nsmap: _NSMapArg | None = ...,
-        makeelement: None = ...,
-    ) -> ElementMaker[_Element]: ...
+        typemap: _TypeMapArg | None = None,
+        namespace: str | None = None,
+        nsmap: _NSMapArg | None = None,
+        makeelement: None = None,
+    ) -> ElementMaker: ...
     def __call__(
         self,
-        tag: str | QName,  # No bytes here
+        tag: _TagName,
         # Although, by default, the ElementMaker only accepts _Element and types
         # interpretable by the default typemap (that is str, CDATA and dict)
         # as children, the typemap can be expanded to make sure items of any
         # type are accepted.
         *children: object,
         **attrib: str,
     ) -> _ET_co: ...
     # __getattr__ here is special. ElementMaker is a factory that generates
     # elements with any tag provided as attribute name, as long as the name
     # does not conflict with the basic object methods (including python keywords
     # like "class" and "for", which are common in HTML)
     def __getattr__(self, name: str) -> _ElemFactory[_ET_co]: ...
 
-E: ElementMaker[_Element]
+E: ElementMaker
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/cssselect.pyi` & `types_lxml-2024.4.14/lxml-stubs/cssselect.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Literal
 
 import cssselect as _csel
 from cssselect.parser import Function
 from cssselect.xpath import XPathExpr
 
-from ._types import _ET, _NonDefaultNSMapArg, _XPathVarArg
-from .etree import XPath, _ElementTree
+from ._types import _ET, _ElementOrTree, _NonDefaultNSMapArg, _XPathVarArg
+from .etree import XPath
 
 _CSSTransArg = LxmlTranslator | Literal["xml", "html", "xhtml"]
 
 SelectorError = _csel.SelectorError
 SelectorSyntaxError = _csel.SelectorSyntaxError
 ExpressionError = _csel.ExpressionError
 
@@ -29,20 +29,20 @@
     # CSS expression and the underlying XPath expression don't
     # match.
     @property
     def css(self) -> str: ...
     def __init__(
         self,
         css: str,
-        namespaces: _NonDefaultNSMapArg | None = ...,
-        translator: _CSSTransArg = ...,
+        namespaces: _NonDefaultNSMapArg | None = None,
+        translator: _CSSTransArg = "xml",
     ) -> None: ...
     # It is safe to assume cssselect always selects element
     # representable in original element tree, because CSS expression
     # is transformed into XPath via css_to_xpath() which doesn't support
     # pseudo-element by default.
     def __call__(
         self,
-        _etree_or_element: _ET | _ElementTree[_ET],
+        _etree_or_element: _ElementOrTree[_ET],
         /,
         **_variables: _XPathVarArg,
     ) -> list[_ET]: ...
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/etree/__init__.pyi` & `types_lxml-2024.4.14/lxml-stubs/etree/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/lxml-stubs/etree/_classlookup.pyi` & `types_lxml-2024.4.14/lxml-stubs/etree/_classlookup.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,16 @@
     hierarchies that implement a common namespace.
     """
 
     @final
     def __init__(
         self,
         *children: object,
-        attrib: SupportsLaxedItems[str, _AnyStr] | None = ...,
-        nsmap: _NSMapArg | None = ...,
+        attrib: SupportsLaxedItems[str, _AnyStr] | None = None,
+        nsmap: _NSMapArg | None = None,
         **_extra: _AnyStr,
     ) -> None: ...
     def _init(self) -> None: ...
 
 class CommentBase(_Comment):
     """All custom Comment classes must inherit from this one
 
@@ -77,15 +77,15 @@
     destroyed.  All persistent state of Comments must be stored in the
     underlying XML.  If you really need to initialize the object after
     creation, you can implement an ``_init(self)`` method that will be
     called after object creation.
     """
 
     @final
-    def __init__(self, text: _AnyStr | None = ...) -> None: ...
+    def __init__(self, text: _AnyStr | None) -> None: ...
     def _init(self) -> None: ...
 
 class PIBase(_ProcessingInstruction):
     """All custom Processing Instruction classes must inherit from this one.
 
     Original Docstring
     ------------------
@@ -97,15 +97,15 @@
     destroyed.  All persistent state of PIs must be stored in the
     underlying XML.  If you really need to initialize the object after
     creation, you can implement an ``_init(self)`` method that will be
     called after object creation.
     """
 
     @final
-    def __init__(self, target: _AnyStr, text: _AnyStr | None = ...) -> None: ...
+    def __init__(self, target: _AnyStr, text: _AnyStr | None = None) -> None: ...
     def _init(self) -> None: ...
 
 class EntityBase(_Entity):
     """All custom Entity classes must inherit from this one.
 
     To create an XML Entity instance, use the ``Entity()`` factory.
 
@@ -130,15 +130,15 @@
     """Superclass of Element class lookups"""
 
 class FallbackElementClassLookup(ElementClassLookup):
     """Superclass of Element class lookups with additional fallback"""
 
     @property
     def fallback(self) -> ElementClassLookup | None: ...
-    def __init__(self, fallback: ElementClassLookup | None = ...) -> None: ...
+    def __init__(self, fallback: ElementClassLookup | None = None) -> None: ...
     def set_fallback(self, lookup: ElementClassLookup) -> None:
         """Sets the fallback scheme for this lookup method"""
 
 class ElementDefaultClassLookup(ElementClassLookup):
     """Element class lookup scheme that always returns the default Element
     class.
 
@@ -151,18 +151,18 @@
     def comment_class(self) -> type[_Comment]: ...
     @property
     def pi_class(self) -> type[_ProcessingInstruction]: ...
     @property
     def entity_class(self) -> type[_Entity]: ...
     def __init__(
         self,
-        element: type[ElementBase] | None = ...,
-        comment: type[CommentBase] | None = ...,
-        pi: type[PIBase] | None = ...,
-        entity: type[EntityBase] | None = ...,
+        element: type[ElementBase] | None = None,
+        comment: type[CommentBase] | None = None,
+        pi: type[PIBase] | None = None,
+        entity: type[EntityBase] | None = None,
     ) -> None: ...
 
 class AttributeBasedElementClassLookup(FallbackElementClassLookup):
     """Checks an attribute of an Element and looks up the value in a
     class dictionary.
 
     Arguments
@@ -176,17 +176,18 @@
 
     A None key in the class mapping will be checked if the attribute is
     missing."""
 
     def __init__(
         self,
         attribute_name: _AttrName,
-        class_mapping: Mapping[str, type[_Element]]
-        | Mapping[str | None, type[_Element]],
-        fallback: ElementClassLookup | None = ...,
+        class_mapping: (
+            Mapping[str, type[_Element]] | Mapping[str | None, type[_Element]]
+        ),
+        fallback: ElementClassLookup | None = None,
     ) -> None: ...
 
 class ParserBasedElementClassLookup(FallbackElementClassLookup):
     """Element class lookup based on the XML parser"""
 
 # Though Cython has no notion of abstract method, it is giving
 # enough hints that all subclasses should implement lookup method
@@ -271,15 +272,15 @@
     @abstractmethod
     def lookup(
         self,
         doc: object,
         element: _Element,  # quasi-Element with all attributes read-only
     ) -> type[_Element] | None: ...
 
-def set_element_class_lookup(lookup: ElementClassLookup | None = ...) -> None:
+def set_element_class_lookup(lookup: ElementClassLookup | None = None) -> None:
     """Set the global element class lookup method
 
     Original Docstring
     ------------------
     This defines the main entry point for looking up element implementations.
     The standard implementation uses the :class:`ParserBasedElementClassLookup`
     to delegate to different lookup schemes for each parser.
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/etree/_cleanup.pyi` & `types_lxml-2024.4.14/lxml-stubs/etree/_cleanup.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Iterable, overload
 
 from .._types import _AnyStr, _ElementOrTree, _NSMapArg, _TagSelector
 
 def cleanup_namespaces(
     tree_or_element: _ElementOrTree,
-    top_nsmap: _NSMapArg | None = ...,
-    keep_ns_prefixes: Iterable[_AnyStr] | None = ...,
+    top_nsmap: _NSMapArg | None = None,
+    keep_ns_prefixes: Iterable[_AnyStr] | None = None,
 ) -> None: ...
 
 # For functions below, the first `tree_or_element` argument
 # can never be keyword argument, since tag/attribute names
 # that followed are considered positional arguments in
 # all possible function signature overloads.
 
@@ -22,22 +22,22 @@
 def strip_attributes(
     __tree_or_elem: _ElementOrTree, __attrib: Iterable[str] | None, /
 ) -> None: ...
 @overload
 def strip_elements(
     __tree_or_elem: _ElementOrTree,
     *tag_names: _TagSelector,
-    with_tail: bool = ...,
+    with_tail: bool = True,
 ) -> None: ...
 @overload
 def strip_elements(
     __tree_or_elem: _ElementOrTree,
     __tag: Iterable[_TagSelector] | None,
     /,
-    with_tail: bool = ...,
+    with_tail: bool = True,
 ) -> None: ...
 @overload
 def strip_tags(
     __tree_or_elem: _ElementOrTree,
     *tag_names: _TagSelector,
 ) -> None: ...
 @overload
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/etree/_docloader.pyi` & `types_lxml-2024.4.14/lxml-stubs/etree/_docloader.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     ) -> _InputDocument | None: ...
     def resolve_empty(self, context: _ResolverContext) -> _InputDocument | None: ...
     def resolve_string(
         self,
         string: _AnyStr,
         context: _ResolverContext,
         *,
-        base_url: _AnyStr | None = ...,
+        base_url: _AnyStr | None = None,
     ) -> _InputDocument | None: ...
     def resolve_filename(
         self, filename: _AnyStr, context: _ResolverContext
     ) -> _InputDocument | None: ...
     def resolve_file(
         self,
         f: SupportsRead[Any],
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/etree/_dtd.pyi` & `types_lxml-2024.4.14/lxml-stubs/etree/_dtd.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 class DTD(_Validator):
     # external_id is effective only when file is None, and
     # native string raises exception
     @overload
     def __init__(self, file: _FileReadSource) -> None: ...
     @overload
-    def __init__(self, file: None = ..., *, external_id: bytes) -> None: ...
+    def __init__(self, file: None = None, *, external_id: bytes) -> None: ...
     @property
     def name(self) -> str | None: ...
     @property
     def external_id(self) -> str | None: ...
     @property
     def system_url(self) -> str | None: ...
     def iterelements(self) -> Iterator[_DTDElementDecl]: ...
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/etree/_element.pyi` & `types_lxml-2024.4.14/lxml-stubs/etree/_element.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     from typing import deprecated
 else:
     from typing_extensions import deprecated
 
 from .. import _types as _t
 from ..cssselect import _CSSTransArg
 from ._module_misc import CDATA, DocInfo, QName
-from ._parser import _DefEtreeParsers
 from ._xslt import XSLTAccessControl, XSLTExtension, _Stylesheet_Param, _XSLTResultTree
 
 # The base of _Element is *almost* an amalgam of MutableSequence[_Element]
 # plus mixin methods for _Attrib.
 # Extra methods follow the order of _Element source approximately
 class _Element:
     #
@@ -73,19 +72,19 @@
     # There are a hoard of element iterators used in lxml, but
     # they only differ in implementation detail and don't affect typing.
     def __iter__(self) -> Iterator[Self]: ...
     def __reversed__(self) -> Iterator[Self]: ...
     def set(self, key: _t._AttrName, value: _t._AttrVal) -> None: ...
     def append(self, element: Self) -> None: ...
     def extend(self, elements: Iterable[Self]) -> None: ...
-    def clear(self, keep_tail: bool = ...) -> None: ...
+    def clear(self, keep_tail: bool = False) -> None: ...
     def insert(self, index: int, element: Self) -> None: ...
     def remove(self, element: Self) -> None: ...
     def index(
-        self, child: Self, start: int | None = ..., end: int | None = ...
+        self, child: Self, start: int | None = None, end: int | None = None
     ) -> int: ...
     @overload
     def get(self, key: _t._AttrName) -> str | None: ...
     @overload
     def get(self, key: _t._AttrName, default: _T) -> str | _T: ...
     def keys(self) -> list[str]: ...
     def values(self) -> list[str]: ...
@@ -98,133 +97,142 @@
     def replace(self, old_element: Self, new_element: Self) -> None: ...
     def getparent(self) -> Self | None: ...
     def getnext(self) -> Self | None: ...
     def getprevious(self) -> Self | None: ...
     def getroottree(self) -> _ElementTree[Self]: ...
     @overload
     def itersiblings(
-        self, *tags: _t._TagSelector, preceding: bool = ...
+        self, *tags: _t._TagSelector, preceding: bool = False
     ) -> Iterator[Self]: ...
     @overload
     def itersiblings(
-        self, *, tag: Iterable[_t._TagSelector] | None = ..., preceding: bool = ...
+        self,
+        *,
+        tag: _t._TagSelector | Iterable[_t._TagSelector] | None = None,
+        preceding: bool = False,
     ) -> Iterator[Self]: ...
     @overload
     def iterancestors(self, *tags: _t._TagSelector) -> Iterator[Self]: ...
     @overload
     def iterancestors(
-        self, *, tag: Iterable[_t._TagSelector] | None = ...
+        self, *, tag: _t._TagSelector | Iterable[_t._TagSelector] | None = None
     ) -> Iterator[Self]: ...
     @overload
     def iterdescendants(self, *tags: _t._TagSelector) -> Iterator[Self]: ...
     @overload
     def iterdescendants(
-        self, *, tag: Iterable[_t._TagSelector] | None = ...
+        self, *, tag: _t._TagSelector | Iterable[_t._TagSelector] | None = None
     ) -> Iterator[Self]: ...
     @overload
     def iterchildren(
-        self, *tags: _t._TagSelector, reversed: bool = ...
+        self, *tags: _t._TagSelector, reversed: bool = False
     ) -> Iterator[Self]: ...
     @overload
     def iterchildren(
-        self, *, tag: Iterable[_t._TagSelector] | None = ..., reversed: bool = ...
+        self,
+        *,
+        tag: _t._TagSelector | Iterable[_t._TagSelector] | None = None,
+        reversed: bool = False,
     ) -> Iterator[Self]: ...
     @overload
     def iter(self, *tags: _t._TagSelector) -> Iterator[Self]: ...
     @overload
     def iter(
-        self, *, tag: Iterable[_t._TagSelector] | None = ...
+        self, *, tag: _t._TagSelector | Iterable[_t._TagSelector] | None = None
     ) -> Iterator[Self]: ...
     @overload
     def itertext(
-        self, *tags: _t._TagSelector, with_tail: bool = ...
+        self, *tags: _t._TagSelector, with_tail: bool = True
     ) -> Iterator[str]: ...
     @overload
     def itertext(
-        self, *, tag: Iterable[_t._TagSelector] | None = ..., with_tail: bool = ...
+        self,
+        *,
+        tag: _t._TagSelector | Iterable[_t._TagSelector] | None = None,
+        with_tail: bool = True,
     ) -> Iterator[str]: ...
     def makeelement(
         self,
         _tag: _t._TagName,
         /,
         # Final result is sort of like {**attrib, **_extra}
-        attrib: _t.SupportsLaxedItems[str, _t._AnyStr] | None = ...,
-        nsmap: _t._NSMapArg | None = ...,
+        attrib: _t.SupportsLaxedItems[str, _t._AnyStr] | None = None,
+        nsmap: _t._NSMapArg | None = None,
         **_extra: _t._AnyStr,
     ) -> Self: ...
     def find(
-        self, path: _t._ElemPathArg, namespaces: _t._NSMapArg | None = ...
+        self, path: _t._ElemPathArg, namespaces: _t._NSMapArg | None = None
     ) -> Self | None: ...
     # Original method has no star. If somebody only supplies
     # 'path' and 'default' argument as positional one, it
     # would be misinterpreted as namespaces argument in first
     # overload form. Add star here to guard against such situation.
     @overload
     def findtext(
         self,
         path: _t._ElemPathArg,
         *,
-        namespaces: _t._NSMapArg | None = ...,
+        namespaces: _t._NSMapArg | None = None,
     ) -> str | None: ...
     @overload
     def findtext(
         self,
         path: _t._ElemPathArg,
         default: _T,
-        namespaces: _t._NSMapArg | None = ...,
+        namespaces: _t._NSMapArg | None = None,
     ) -> str | _T: ...
     def findall(
-        self, path: _t._ElemPathArg, namespaces: _t._NSMapArg | None = ...
+        self, path: _t._ElemPathArg, namespaces: _t._NSMapArg | None = None
     ) -> list[Self]: ...
     def iterfind(
-        self, path: _t._ElemPathArg, namespaces: _t._NSMapArg | None = ...
+        self, path: _t._ElemPathArg, namespaces: _t._NSMapArg | None = None
     ) -> Iterator[Self]: ...
     def xpath(
         self,
         _path: _t._AnyStr,
         /,
         *,
-        namespaces: _t._NonDefaultNSMapArg | None = ...,
-        extensions: _t._XPathExtFuncArg | None = ...,
-        smart_strings: bool = ...,
+        namespaces: _t._NonDefaultNSMapArg | None = None,
+        extensions: _t._XPathExtFuncArg | None = None,
+        smart_strings: bool = True,
         **_variables: _t._XPathVarArg,
     ) -> _t._XPathObject: ...
     def cssselect(
         self,
         expr: str,
         *,
-        translator: _CSSTransArg = ...,
+        translator: _CSSTransArg = "xml",
     ) -> list[Self]: ...
     @deprecated("Since v2.0 (2008); use list(element) or iterate over element")
     def getchildren(self) -> list[Self]: ...
     # Should have been overloaded for accuracy, but we can turn a blind eye
     # for something that is marked deprecated for 15 years
     @deprecated("Since v2.0 (2008); renamed to .iter()")
     def getiterator(
-        self, tag: _t._TagSelector | None = ..., *tags: _t._TagSelector
+        self, tag: _t._TagSelector | None = None, *tags: _t._TagSelector
     ) -> Iterator[Self]: ...
 
 # ET class notation is specialized, indicating the type of element
 # it is holding (e.g. XML element, HTML element or Objectified
 # Element).
 # Although it is also possible to be an empty tree containing no
 # element, the absolute majority of lxml API will fail to work.
 # It is considered harmful to support such corner case, which
 # adds much complexity without any benefit.
 class _ElementTree(Generic[_t._ET_co]):
     @property
-    def parser(self) -> _DefEtreeParsers[_t._ET_co] | None: ...
+    def parser(self) -> _t._DefEtreeParsers[_t._ET_co] | None: ...
     @property
     def docinfo(self) -> DocInfo: ...
     def parse(
         self,
         source: _t._FileReadSource,
-        parser: _DefEtreeParsers[_t._ET_co] | None = ...,
+        parser: _t._DefEtreeParsers[_t._ET_co] | None = None,
         *,
-        base_url: _t._AnyStr | None = ...,
+        base_url: _t._AnyStr | None = None,
     ) -> None: ...
     # Changes root node; in terms of typing, this means changing
     # specialization of ElementTree. This is not expressible in
     # current typing system.
     def _setroot(self, root: _Element) -> None: ...
     def getroot(self) -> _t._ET_co: ...
     # Special notes for write()
@@ -233,131 +241,132 @@
     # to handle in stub, so keep it simple and only divide
     # keyword usage by writing method as documented.
     # For example, following combination raises exception in lxml:
     #     - file argument is file name or path like, and
     #     - method is 'c14n2', and
     #     - no compression
     #
-    @overload  # deprecated usage of docstring param
+    @overload  # type: ignore[arg-type]  # mypy err since 1.6
+    # deprecated usage of docstring param
     @deprecated('Since v3.8.0; use "doctype" parameter instead')
     def write(
         self,
         file: Any,
         *,
         docstring: str,
         __kw: Any,
     ) -> None: ...
     @overload  # method=c14n
     def write(
         self,
         file: _t._FileWriteSource,
         *,
         method: Literal["c14n"],
-        exclusive: bool = ...,
-        with_comments: bool = ...,
-        compression: int | None = ...,
-        inclusive_ns_prefixes: Iterable[_t._AnyStr] | None = ...,
+        exclusive: bool = False,
+        with_comments: bool = True,
+        compression: int | None = 0,
+        inclusive_ns_prefixes: Iterable[_t._AnyStr] | None = None,
     ) -> None: ...
     @overload  # method=c14n2
     def write(
         self,
         file: _t._FileWriteSource,
         *,
         method: Literal["c14n2"],
-        with_comments: bool = ...,
-        compression: int | None = ...,
-        strip_text: bool = ...,
+        with_comments: bool = True,
+        compression: int | None = 0,
+        strip_text: bool = False,
     ) -> None: ...
     @overload  # other write methods
     def write(
         self,
         file: _t._FileWriteSource,
         *,
-        encoding: str | None = ...,  # unicode not allowed
-        method: _t._OutputMethodArg = ...,
-        pretty_print: bool = ...,
-        xml_declaration: bool | None = ...,
-        with_tail: bool = ...,
-        standalone: bool | None = ...,
-        doctype: str | None = ...,
-        compression: int | None = ...,
+        encoding: str | None = None,  # unicode not allowed
+        method: _t._OutputMethodArg = "xml",
+        pretty_print: bool = False,
+        xml_declaration: bool | None = None,
+        with_tail: bool = True,
+        standalone: bool | None = None,
+        doctype: str | None = None,
+        compression: int | None = 0,
     ) -> None: ...
     def getpath(self: _ElementTree[_t._ET], element: _t._ET) -> str: ...
     def getelementpath(self: _ElementTree[_t._ET], element: _t._ET) -> str: ...
     @overload
     def iter(self, *tags: _t._TagSelector) -> Iterator[_t._ET_co]: ...
     @overload
-    def iter(self, *, tag: _t._TagSelector | None = ...) -> Iterator[_t._ET_co]: ...
+    def iter(self, *, tag: _t._TagSelector | None = None) -> Iterator[_t._ET_co]: ...
     #
     # ElementPath methods calls the same method on root node,
     # so signature should be the same as _Element ones
     #
     def find(
-        self, path: _t._ElemPathArg, namespaces: _t._NSMapArg | None = ...
+        self, path: _t._ElemPathArg, namespaces: _t._NSMapArg | None = None
     ) -> _t._ET_co | None: ...
     @overload
     def findtext(
         self,
         path: _t._ElemPathArg,
         *,
-        namespaces: _t._NSMapArg | None = ...,
+        namespaces: _t._NSMapArg | None = None,
     ) -> str | None: ...
     @overload
     def findtext(
         self,
         path: _t._ElemPathArg,
         default: _T,
-        namespaces: _t._NSMapArg | None = ...,
+        namespaces: _t._NSMapArg | None = None,
     ) -> str | _T: ...
     def findall(
-        self, path: _t._ElemPathArg, namespaces: _t._NSMapArg | None = ...
+        self, path: _t._ElemPathArg, namespaces: _t._NSMapArg | None = None
     ) -> list[_t._ET_co]: ...
     def iterfind(
-        self, path: _t._ElemPathArg, namespaces: _t._NSMapArg | None = ...
+        self, path: _t._ElemPathArg, namespaces: _t._NSMapArg | None = None
     ) -> Iterator[_t._ET_co]: ...
     def xpath(
         self,
         _path: _t._AnyStr,
         /,
         *,
-        namespaces: _t._NonDefaultNSMapArg | None = ...,
-        extensions: _t._XPathExtFuncArg | None = ...,
-        smart_strings: bool = ...,
+        namespaces: _t._NonDefaultNSMapArg | None = None,
+        extensions: _t._XPathExtFuncArg | None = None,
+        smart_strings: bool = True,
         **_variables: _t._XPathVarArg,
     ) -> _t._XPathObject: ...
     def xslt(
         self,
         _xslt: _t._ElementOrTree,
         /,
         extensions: (
             _t.SupportsLaxedItems[tuple[_t._AnyStr, _t._AnyStr], XSLTExtension] | None
-        ) = ...,
-        access_control: XSLTAccessControl | None = ...,
+        ) = None,
+        access_control: XSLTAccessControl | None = None,
         *,  # all keywords are passed to XSLT.__call__
-        profile_run: bool = ...,
+        profile_run: bool = False,
         **__kw: _Stylesheet_Param,
     ) -> _XSLTResultTree: ...
     def relaxng(self, relaxng: _t._ElementOrTree) -> bool: ...
     def xmlschema(self, xmlschema: _t._ElementOrTree) -> bool: ...
     def xinclude(self) -> None: ...
     # Should have been overloaded for accuracy, but we can turn a blind eye
     # for something that is marked deprecated for 15 years
     @deprecated("Since v2.0 (2008); renamed to .iter()")
     def getiterator(
-        self, tag: _t._TagSelector | None = ..., *tags: _t._TagSelector
+        self, tag: _t._TagSelector | None = None, *tags: _t._TagSelector
     ) -> Iterator[_t._ET_co]: ...
     @deprecated('Since v4.4; use .write() with method="c14n" argument')
     def write_c14n(
         self,
         file: _t._FileWriteSource,
         *,
-        exclusive: bool = ...,
-        with_comments: bool = ...,
-        compression: int | None = ...,
-        inclusive_ns_prefixes: Iterable[_t._AnyStr] | None = ...,
+        exclusive: bool = False,
+        with_comments: bool = True,
+        compression: int | None = 0,
+        inclusive_ns_prefixes: Iterable[_t._AnyStr] | None = None,
     ) -> None: ...
 
 # Behaves like MutableMapping but deviates a lot in details
 class _Attrib:
     @property
     def _element(self) -> _Element: ...
     def __setitem__(self, __k: _t._AttrName, __v: _t._AttrVal) -> None: ...
@@ -416,24 +425,19 @@
 # throughout all element methods would cause great inconvenience
 # for me and all users alike -- using some _AnyHtmlElement alias
 # to represent union of all elements was a failure for users.
 # We opt for convenience and ease of use in the future.
 class __ContentOnlyElement(_Element):
     #
     # Useful properties
+    # .text and .tag are overridden in each concrete class below
     #
     @property
-    def text(self) -> str | None: ...
-    @text.setter
-    def text(  # pyright: ignore[reportIncompatibleMethodOverride]
-        self, value: _t._AnyStr | None
-    ) -> None: ...
-    @property
     def attrib(self) -> Mapping[_t.Unused, _t.Unused]: ...  # type: ignore[override]
-    def get(self, key: _t.Unused, default: _t.Unused = ...) -> None: ...  # type: ignore[override]
+    def get(self, key: _t.Unused, default: _t.Unused = None) -> None: ...  # type: ignore[override]
     def set(self, key: Never, value: Never) -> Never: ...  # type: ignore[override]
     def append(self, element: Never) -> Never: ...  # type: ignore[override]
     def insert(self, index: Never, value: Never) -> Never: ...  # type: ignore[override]
     def __setitem__(self, __k: Never, __v: Never) -> Never: ...  # type: ignore[override]
     # The intention is to forbid elem.__getitem__, allowing slice
     # doesn't make any sense
     def __getitem__(self, __k: Never) -> Never: ...  # type: ignore[override]
@@ -449,19 +453,31 @@
     # For example, append(elem) explicitly raises exception, yet
     # one can use extend([elem]) to circumvent restriction.
     # Go figure.
 
 class _Comment(__ContentOnlyElement):
     @property  # type: ignore[misc]
     def tag(self) -> _t._ElemFactory[_Comment]: ...  # type: ignore[override]
+    @property  # type: ignore[override]
+    def text(self) -> str: ...
+    @text.setter
+    def text(  # pyright: ignore[reportIncompatibleMethodOverride]
+        self, value: _t._AnyStr | None
+    ) -> None: ...
 
 # signature of .get() for _PI and _Element are the same
 class _ProcessingInstruction(__ContentOnlyElement):
     @property  # type: ignore[misc]
     def tag(self) -> _t._ElemFactory[_ProcessingInstruction]: ...  # type: ignore[override]
+    @property  # type: ignore[override]
+    def text(self) -> str: ...
+    @text.setter
+    def text(  # pyright: ignore[reportIncompatibleMethodOverride]
+        self, value: _t._AnyStr | None
+    ) -> None: ...
     @property
     def target(self) -> str: ...
     @target.setter
     def target(self, value: _t._AnyStr) -> None: ...
     @property
     def attrib(self) -> dict[str, str]: ...  # type: ignore[override]
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/etree/_iterparse.pyi` & `types_lxml-2024.4.14/lxml-stubs/etree/_iterparse.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 import sys
 from _typeshed import SupportsRead, _T_co
-from typing import IO, Iterable, Iterator, Literal, overload
+from typing import Iterable, Iterator, Literal, overload
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:
     from typing_extensions import TypeAlias
 
 if sys.version_info >= (3, 11):
     from typing import LiteralString
 else:
     from typing_extensions import LiteralString
 
 from .._types import (
     SupportsLaxedItems,
     _AnyStr,
+    _ElementOrTree,
     _ET_co,
     _FilePath,
     _NSMapArg,
     _SaxEventNames,
     _TagName,
     _TagSelector,
 )
 from ._classlookup import ElementClassLookup
 from ._docloader import _ResolverRegistry
-from ._element import _Element, _ElementTree
+from ._element import _Element
 from ._xmlerror import _ListErrorLog
 from ._xmlschema import XMLSchema
 
 # See https://lxml.de/parsing.html#event-types
 # Undocumented: 'comment' and 'pi' are actually supported!
 _NoNSEventNames: TypeAlias = Literal["start", "end", "comment", "pi"]
 _SaxNsEventValues: TypeAlias = tuple[str, str] | None  # for start-ns & end-ns event
 
 class iterparse(Iterator[_T_co]):
     """Incremental parser
 
     Annotation
     ----------
     Totally 5 function signatures are available:
-    - Default XML mode, where only `end` event is emitted
+    - HTML mode (`html=True`), where namespace events are ignored
     - `start`, `end`, `comment` and `pi` events, where only
       Element values are produced
-    - HTML mode (`html=True`), where namespace events are ignored
     - XML mode with `start-ns` or `end-ns` events, producing
       namespace tuple (for `start-ns`) or nothing (`end-ns`)
-    - Final catch-all signature for XML mode
+    - Catch-all signature where `events` arg is specified
+    - `events` arg absent, implying only `end` event is emitted
 
     Original Docstring
     ------------------
     Parses XML into a tree and generates tuples (event, element) in a
     SAX-like fashion. ``event`` is any of 'start', 'end', 'start-ns',
     'end-ns'.
 
@@ -68,160 +69,159 @@
     events are generated for all elements.  Note that the 'start-ns' and
     'end-ns' events are not impacted by this restriction.
 
     The other keyword arguments in the constructor are mainly based on the
     libxml2 parser configuration.  A DTD will also be loaded if validation or
     attribute default values are requested."""
 
-    @overload  # default values, only 'end' event emitted
-    def __new__(
+    @overload  # html mode -> namespace events suppressed
+    def __new__(  # type: ignore[overload-overlap]
         cls,
-        source: _FilePath | IO[bytes] | SupportsRead[bytes],
-        events: None = ...,
+        source: _FilePath | SupportsRead[bytes],
+        events: Iterable[_SaxEventNames] = ("end",),
         *,
-        tag: _TagSelector | Iterable[_TagSelector] | None = ...,
-        attribute_defaults: bool = ...,
-        dtd_validation: bool = ...,
-        load_dtd: bool = ...,
-        no_network: bool = ...,
-        remove_blank_text: bool = ...,
-        compact: bool = ...,
-        resolve_entities: bool = ...,
-        remove_comments: bool = ...,
-        remove_pis: bool = ...,
-        strip_cdata: bool = ...,
-        encoding: _AnyStr | None = ...,
-        html: bool = ...,
-        recover: bool | None = ...,
-        huge_tree: bool = ...,
-        collect_ids: bool = ...,
-        schema: XMLSchema | None = ...,
-    ) -> iterparse[tuple[Literal["end"], _Element]]: ...
+        tag: _TagSelector | Iterable[_TagSelector] | None = None,
+        attribute_defaults: bool = False,
+        dtd_validation: bool = False,
+        load_dtd: bool = False,
+        no_network: bool = True,
+        remove_blank_text: bool = False,
+        compact: bool = True,
+        resolve_entities: bool = True,
+        remove_comments: bool = False,
+        remove_pis: bool = False,
+        strip_cdata: bool = True,
+        encoding: _AnyStr | None = None,
+        html: Literal[True],
+        recover: bool | None = None,
+        huge_tree: bool = False,
+        collect_ids: bool = True,
+        schema: XMLSchema | None = None,
+    ) -> iterparse[tuple[_NoNSEventNames, _Element]]: ...
     @overload  # element-only events
     def __new__(
         cls,
-        source: _FilePath | IO[bytes] | SupportsRead[bytes],
+        source: _FilePath | SupportsRead[bytes],
         events: Iterable[_NoNSEventNames],
         *,
-        tag: _TagSelector | Iterable[_TagSelector] | None = ...,
-        attribute_defaults: bool = ...,
-        dtd_validation: bool = ...,
-        load_dtd: bool = ...,
-        no_network: bool = ...,
-        remove_blank_text: bool = ...,
-        compact: bool = ...,
-        resolve_entities: bool = ...,
-        remove_comments: bool = ...,
-        remove_pis: bool = ...,
-        strip_cdata: bool = ...,
-        encoding: _AnyStr | None = ...,
-        html: bool = ...,
-        recover: bool | None = ...,
-        huge_tree: bool = ...,
-        collect_ids: bool = ...,
-        schema: XMLSchema | None = ...,
+        tag: _TagSelector | Iterable[_TagSelector] | None = None,
+        attribute_defaults: bool = False,
+        dtd_validation: bool = False,
+        load_dtd: bool = False,
+        no_network: bool = True,
+        remove_blank_text: bool = False,
+        compact: bool = True,
+        resolve_entities: bool = True,
+        remove_comments: bool = False,
+        remove_pis: bool = False,
+        strip_cdata: bool = True,
+        encoding: _AnyStr | None = None,
+        html: bool = False,
+        recover: bool | None = None,
+        huge_tree: bool = False,
+        collect_ids: bool = True,
+        schema: XMLSchema | None = None,
     ) -> iterparse[tuple[_NoNSEventNames, _Element]]: ...
-    @overload  # html mode -> namespace events suppressed
+    @overload  # NS-only events
     def __new__(
         cls,
-        source: _FilePath | IO[bytes] | SupportsRead[bytes],
-        events: Iterable[_SaxEventNames],
-        *,
-        tag: _TagSelector | Iterable[_TagSelector] | None = ...,
-        attribute_defaults: bool = ...,
-        dtd_validation: bool = ...,
-        load_dtd: bool = ...,
-        no_network: bool = ...,
-        remove_blank_text: bool = ...,
-        compact: bool = ...,
-        resolve_entities: bool = ...,
-        remove_comments: bool = ...,
-        remove_pis: bool = ...,
-        strip_cdata: bool = ...,
-        encoding: _AnyStr | None = ...,
-        html: Literal[True],
-        recover: bool | None = ...,
-        huge_tree: bool = ...,
-        collect_ids: bool = ...,
-        schema: XMLSchema | None = ...,
-    ) -> iterparse[tuple[_NoNSEventNames, _Element]]: ...
-    @overload  # xml mode & NS-only events
-    def __new__(
-        cls,
-        source: _FilePath | IO[bytes] | SupportsRead[bytes],
+        source: _FilePath | SupportsRead[bytes],
         events: Iterable[Literal["start-ns", "end-ns"]],
         *,
-        tag: _TagSelector | Iterable[_TagSelector] | None = ...,
-        attribute_defaults: bool = ...,
-        dtd_validation: bool = ...,
-        load_dtd: bool = ...,
-        no_network: bool = ...,
-        remove_blank_text: bool = ...,
-        compact: bool = ...,
-        resolve_entities: bool = ...,
-        remove_comments: bool = ...,
-        remove_pis: bool = ...,
-        strip_cdata: bool = ...,
-        encoding: _AnyStr | None = ...,
-        html: Literal[False] = ...,
-        recover: bool | None = ...,
-        huge_tree: bool = ...,
-        collect_ids: bool = ...,
-        schema: XMLSchema | None = ...,
+        tag: _TagSelector | Iterable[_TagSelector] | None = None,
+        attribute_defaults: bool = False,
+        dtd_validation: bool = False,
+        load_dtd: bool = False,
+        no_network: bool = True,
+        remove_blank_text: bool = False,
+        compact: bool = True,
+        resolve_entities: bool = True,
+        remove_comments: bool = False,
+        remove_pis: bool = False,
+        strip_cdata: bool = True,
+        encoding: _AnyStr | None = None,
+        html: bool = False,
+        recover: bool | None = None,
+        huge_tree: bool = False,
+        collect_ids: bool = True,
+        schema: XMLSchema | None = None,
     ) -> iterparse[
         tuple[Literal["start-ns"], tuple[str, str]] | tuple[Literal["end-ns"], None]
     ]: ...
-    @overload  # xml mode, catch all
+    @overload  # other mixed events
     def __new__(
         cls,
-        source: _FilePath | IO[bytes] | SupportsRead[bytes],
+        source: _FilePath | SupportsRead[bytes],
         events: Iterable[_SaxEventNames],
         *,
-        tag: _TagSelector | Iterable[_TagSelector] | None = ...,
-        attribute_defaults: bool = ...,
-        dtd_validation: bool = ...,
-        load_dtd: bool = ...,
-        no_network: bool = ...,
-        remove_blank_text: bool = ...,
-        compact: bool = ...,
-        resolve_entities: bool = ...,
-        remove_comments: bool = ...,
-        remove_pis: bool = ...,
-        strip_cdata: bool = ...,
-        encoding: _AnyStr | None = ...,
-        html: Literal[False] = ...,
-        recover: bool | None = ...,
-        huge_tree: bool = ...,
-        collect_ids: bool = ...,
-        schema: XMLSchema | None = ...,
+        tag: _TagSelector | Iterable[_TagSelector] | None = None,
+        attribute_defaults: bool = False,
+        dtd_validation: bool = False,
+        load_dtd: bool = False,
+        no_network: bool = True,
+        remove_blank_text: bool = False,
+        compact: bool = True,
+        resolve_entities: bool = True,
+        remove_comments: bool = False,
+        remove_pis: bool = False,
+        strip_cdata: bool = True,
+        encoding: _AnyStr | None = None,
+        html: bool = False,
+        recover: bool | None = None,
+        huge_tree: bool = False,
+        collect_ids: bool = True,
+        schema: XMLSchema | None = None,
     ) -> iterparse[
         tuple[_NoNSEventNames, _Element]
         | tuple[Literal["start-ns"], tuple[str, str]]
         | tuple[Literal["end-ns"], None]
     ]: ...
+    @overload  # events absent -> only 'end' event emitted
+    def __new__(
+        cls,
+        source: _FilePath | SupportsRead[bytes],
+        *,
+        tag: _TagSelector | Iterable[_TagSelector] | None = None,
+        attribute_defaults: bool = False,
+        dtd_validation: bool = False,
+        load_dtd: bool = False,
+        no_network: bool = True,
+        remove_blank_text: bool = False,
+        compact: bool = True,
+        resolve_entities: bool = True,
+        remove_comments: bool = False,
+        remove_pis: bool = False,
+        strip_cdata: bool = True,
+        encoding: _AnyStr | None = None,
+        html: bool = False,
+        recover: bool | None = None,
+        huge_tree: bool = False,
+        collect_ids: bool = True,
+        schema: XMLSchema | None = None,
+    ) -> iterparse[tuple[Literal["end"], _Element]]: ...
     def __next__(self) -> _T_co: ...
     # root property only present after parsing is done
     @property
     def root(self) -> _Element | None: ...
     @property
     def error_log(self) -> _ListErrorLog: ...
     @property
     def resolvers(self) -> _ResolverRegistry: ...
     @property
     def version(self) -> LiteralString: ...
     def set_element_class_lookup(
         self,
-        lookup: ElementClassLookup | None = ...,
+        lookup: ElementClassLookup | None = None,
     ) -> None: ...
     def makeelement(
         self,
         _tag: _TagName,
         /,
-        attrib: SupportsLaxedItems[str, _AnyStr] | None = ...,
-        nsmap: _NSMapArg | None = ...,
+        attrib: SupportsLaxedItems[str, _AnyStr] | None = None,
+        nsmap: _NSMapArg | None = None,
         **_extra: _AnyStr,
     ) -> _Element: ...  # from etree pull parsers
 
 class iterwalk(Iterator[_T_co]):
     """Tree walker that generates events from an existing tree as if it
     was parsing XML data with ``iterparse()``
 
@@ -243,44 +243,44 @@
 
     After receiving a 'start' or 'start-ns' event, the children and
     descendants of the current element can be excluded from iteration
     by calling the ``skip_subtree()`` method.
     """
 
     # There is no concept of html mode in iterwalk; namespace events
-    # are not supressed like iterparse might do
-    @overload  # default events
-    def __new__(
-        cls,
-        element_or_tree: _ET_co | _ElementTree[_ET_co],
-        events: None = ...,
-        tag: _TagSelector | Iterable[_TagSelector] | None = ...,
-    ) -> iterwalk[tuple[Literal["end"], _ET_co]]: ...
+    # are not suppressed like iterparse()
     @overload  # element-only events
     def __new__(
         cls,
-        element_or_tree: _ET_co | _ElementTree[_ET_co],
+        element_or_tree: _ElementOrTree[_ET_co],
         events: Iterable[_NoNSEventNames],
-        tag: _TagSelector | Iterable[_TagSelector] | None = ...,
+        tag: _TagSelector | Iterable[_TagSelector] | None = None,
     ) -> iterwalk[tuple[_NoNSEventNames, _ET_co]]: ...
     @overload  # namespace-only events
     def __new__(
         cls,
-        element_or_tree: _ET_co | _ElementTree[_ET_co],
+        element_or_tree: _ElementOrTree[_ET_co],
         events: Iterable[Literal["start-ns", "end-ns"]],
-        tag: _TagSelector | Iterable[_TagSelector] | None = ...,
+        tag: _TagSelector | Iterable[_TagSelector] | None = None,
     ) -> iterwalk[
         tuple[Literal["start-ns"], tuple[str, str]] | tuple[Literal["end-ns"], None]
     ]: ...
-    @overload  # catch-all
+    @overload  # all other events combination
     def __new__(
         cls,
-        element_or_tree: _ET_co | _ElementTree[_ET_co],
+        element_or_tree: _ElementOrTree[_ET_co],
         events: Iterable[_SaxEventNames],
-        tag: _TagSelector | Iterable[_TagSelector] | None = ...,
+        tag: _TagSelector | Iterable[_TagSelector] | None = None,
     ) -> iterwalk[
         tuple[_NoNSEventNames, _ET_co]
         | tuple[Literal["start-ns"], tuple[str, str]]
         | tuple[Literal["end-ns"], None]
     ]: ...
+    @overload  # default events ('end' only)
+    def __new__(
+        cls,
+        element_or_tree: _ElementOrTree[_ET_co],
+        /,
+        tag: _TagSelector | Iterable[_TagSelector] | None = None,
+    ) -> iterwalk[tuple[Literal["end"], _ET_co]]: ...
     def __next__(self) -> _T_co: ...
     def skip_subtree(self) -> None: ...
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/etree/_module_func.pyi` & `types_lxml-2024.4.14/lxml-stubs/etree/_module_func.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -10,87 +10,88 @@
     from typing import deprecated
 else:
     from typing_extensions import deprecated
 
 from .._types import (
     _ET,
     _AnyStr,
+    _DefEtreeParsers,
     _ElementOrTree,
     _ET_co,
     _FileReadSource,
     _OutputMethodArg,
 )
 from ._element import _Element, _ElementTree
-from ._parser import HTMLParser, XMLParser, _DefEtreeParsers
+from ._parser import HTMLParser, XMLParser
 
 @overload
 def HTML(
     text: _AnyStr,
     parser: HTMLParser[_ET_co],
     *,
-    base_url: _AnyStr | None = ...,
+    base_url: _AnyStr | None = None,
 ) -> _ET_co: ...
 @overload
 def HTML(
     text: _AnyStr,
-    parser: None = ...,
+    parser: None = None,
     *,
-    base_url: _AnyStr | None = ...,
+    base_url: _AnyStr | None = None,
 ) -> _Element: ...
 @overload
 def XML(
     text: _AnyStr,
     parser: XMLParser[_ET_co],
     *,
-    base_url: _AnyStr | None = ...,
+    base_url: _AnyStr | None = None,
 ) -> _ET_co: ...
 @overload
 def XML(
     text: _AnyStr,
-    parser: None = ...,
+    parser: None = None,
     *,
-    base_url: _AnyStr | None = ...,
+    base_url: _AnyStr | None = None,
 ) -> _Element: ...
 @overload
 def parse(
     source: _FileReadSource,
     parser: _DefEtreeParsers[_ET_co],
     *,
-    base_url: _AnyStr | None = ...,
+    base_url: _AnyStr | None = None,
 ) -> _ElementTree[_ET_co]: ...
 @overload
 def parse(
     source: _FileReadSource,
-    parser: None = ...,
+    parser: None = None,
     *,
-    base_url: _AnyStr | None = ...,
-) -> _ElementTree[_Element]: ...
+    base_url: _AnyStr | None = None,
+) -> _ElementTree: ...
 @overload
 def fromstring(
     text: _AnyStr,
     parser: _DefEtreeParsers[_ET_co],
     *,
-    base_url: _AnyStr | None = ...,
+    base_url: _AnyStr | None = None,
 ) -> _ET_co: ...
 @overload
 def fromstring(
     text: _AnyStr,
-    parser: None = ...,
+    parser: None = None,
     *,
-    base_url: _AnyStr | None = ...,
+    base_url: _AnyStr | None = None,
 ) -> _Element: ...
 @overload
 def fromstringlist(
     strings: Iterable[_AnyStr],
     parser: _DefEtreeParsers[_ET_co],
 ) -> _ET_co: ...
 @overload
 def fromstringlist(
     strings: Iterable[_AnyStr],
-    parser: None = ...,
+    parser: None = None,
 ) -> _Element: ...
 
 # Under XML Canonicalization (C14N) mode, most arguments are ignored,
 # some arguments would even raise exception outright if specified.
 @overload  # method="c14n"
 def tostring(
     element_or_tree: _ElementOrTree,
@@ -105,15 +106,15 @@
     element_or_tree: _ElementOrTree,
     *,
     method: Literal["c14n2"],
     with_comments: bool = True,
     strip_text: bool = False,
 ) -> bytes: ...
 @overload  # Native str, no XML declaration
-def tostring(  # type: ignore[misc]
+def tostring(  # type: ignore[overload-overlap]
     element_or_tree: _ElementOrTree,
     *,
     encoding: type[str] | Literal["unicode"],
     method: _OutputMethodArg = "xml",
     pretty_print: bool = False,
     with_tail: bool = True,
     standalone: bool | None = None,
@@ -129,47 +130,47 @@
     pretty_print: bool = False,
     with_tail: bool = True,
     standalone: bool | None = None,
     doctype: str | None = None,
 ) -> bytes: ...
 def indent(
     element_or_tree: _ElementOrTree,
-    space: str = ...,
+    space: str = "  ",
     *,
-    level: int = ...,
+    level: int = 0,
 ) -> None: ...
 @deprecated(
     "For ElementTree 1.3 compat only; result is tostring() output wrapped inside a list"
 )
 def tostringlist(
     element_or_tree: _ElementOrTree, *args: Any, **__kw: Any
 ) -> list[str]: ...
 @deprecated('Since v3.3.2; use tostring() with encoding="unicode" argument')
 def tounicode(
     element_or_tree: _ElementOrTree,
     *,
-    method: str,
-    pretty_print: bool = ...,
-    with_tail: bool = ...,
-    doctype: str | None = ...,
+    method: str = "xml",
+    pretty_print: bool = False,
+    with_tail: bool = True,
+    doctype: str | None = None,
 ) -> None: ...
 def iselement(element: object) -> TypeGuard[_Element]: ...
 
-# XXX PyCapsule needs annotation of ctypes.pythonapi, which has no
+# HACK PyCapsule needs annotation of ctypes.pythonapi, which has no
 # annotation support currently. Use generic object for now.
 @overload
 def adopt_external_document(
     capsule: object,
     parser: _DefEtreeParsers[_ET],
 ) -> _ElementTree[_ET]: ...
 @overload
 def adopt_external_document(
     capsule: object,
-    parser: None = ...,
-) -> _ElementTree[_Element]:
+    parser: None = None,
+) -> _ElementTree:
     """
     Original Docstring
     ------------------
     Unpack a libxml2 document pointer from a PyCapsule and wrap it in an
     lxml ElementTree object.
 
     This allows external libraries to build XML/HTML trees using libxml2
@@ -201,15 +202,15 @@
 def register_namespace(prefix: _AnyStr, uri: _AnyStr) -> None:
     """Registers a namespace prefix that newly created Elements in that
     namespace will use.  The registry is global, and any existing
     mapping for either the given prefix or the namespace URI will be
     removed."""
 
 # Debugging only
-def dump(elem: _Element, *, pretty_print: bool = ..., with_tail: bool = ...) -> None:
+def dump(elem: _Element, *, pretty_print: bool = True, with_tail: bool = True) -> None:
     """Writes an element tree or element structure to sys.stdout.
     This function should be used for debugging only."""
 
 @final
 class _MemDebug:
     """Debugging support for the memory allocation in libxml2"""
 
@@ -236,27 +237,27 @@
         Returns
         -------
         int
             The current size of the global name dictionary used by libxml2
             for the current thread.  Each thread has its own dictionary.
         """
     def dump(
-        self, output_file: _AnyStr | None = ..., byte_count: int | None = ...
+        self, output_file: _AnyStr | None = None, byte_count: int | None = None
     ) -> None:
         """Dumps the current memory blocks allocated by libxml2 to a file
 
         Parameters
         ----------
         output_file : str or bytes, optional
             Output file path, default is ".memorylist" under current directory
         byte_count : int, optional
             Limits number of bytes in the dump, default is None (unlimited)
         """
     def show(
-        self, output_file: _AnyStr | None = ..., block_count: int | None = ...
+        self, output_file: _AnyStr | None = None, block_count: int | None = None
     ) -> None:
         """Dumps the current memory blocks allocated by libxml2 to a file
         The output file format is suitable for line diffing.
 
         Parameters
         ----------
         output_file : str or bytes, optional
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/etree/_module_misc.pyi` & `types_lxml-2024.4.14/lxml-stubs/etree/_module_misc.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     def clear(self) -> None: ...
 
 class QName:
     @overload
     def __init__(
         self,
         text_or_uri_or_element: _TagName | _Element,
-        tag: _TagName | None = ...,
+        tag: _TagName | None = None,
     ) -> None: ...
     @overload
     def __init__(
         self,
         text_or_uri_or_element: None,
         tag: _TagName,
     ) -> None: ...
@@ -79,15 +79,15 @@
 class CDATA:
     def __init__(self, data: _AnyStr) -> None: ...
 
 class Error(Exception): ...
 
 class LxmlError(Error):
     def __init__(
-        self, message: object, error_log: _BaseErrorLog | None = ...
+        self, message: object, error_log: _BaseErrorLog | None = None
     ) -> None: ...
     # Even when LxmlError is initiated with PyErrorLog, it fools
     # error_log property by creating a dummy _ListErrorLog object
     error_log: _ListErrorLog
 
 class DocumentInvalid(LxmlError): ...
 class LxmlSyntaxError(LxmlError, SyntaxError): ...
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/etree/_nsclasses.pyi` & `types_lxml-2024.4.14/lxml-stubs/etree/_nsclasses.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 # Element namespace
 #
 
 @final
 class _ClassNamespaceRegistry(_NamespaceRegistry[str | None, type[ElementBase]]):
     @overload  # @ns(None), @ns('tag')
     def __call__(
-        self, __tag: str | None, __cls: None = ...
+        self, __tag: str | None, __cls: None = None
     ) -> Callable[[type[_Public_ET]], type[_Public_ET]]: ...
     @overload  # plain @ns
     def __call__(self, __cls: type[_Public_ET]) -> type[_Public_ET]: ...
 
 class ElementNamespaceClassLookup(FallbackElementClassLookup):
     """Element class lookup scheme that searches the Element class in the
     Namespace registry
@@ -72,15 +72,15 @@
     @ns_elements("movie")
     class MovieElement(ElementBase):
       "Element implementation for 'movie' tag (explicit tag name) in schema namespace."
     """
 
     def __init__(
         self,
-        fallback: ElementClassLookup | None = ...,
+        fallback: ElementClassLookup | None = None,
     ) -> None: ...
     def get_namespace(self, ns_uri: str | None) -> _ClassNamespaceRegistry:
         """Retrieve the namespace object associated with the given URI
 
         Pass None for the empty namespace.
         Creates a new namespace object if it does not yet exist.
         """
@@ -93,13 +93,13 @@
 class _FunctionNamespaceRegistry(_NamespaceRegistry[str, Callable[..., Any]]):
     @property
     def prefix(self) -> str: ...
     @prefix.setter
     def prefix(self, __v: str | None) -> None: ...
     @overload  # @ns('name')
     def __call__(
-        self, __name: str, __func: None = ...
+        self, __name: str, __func: None = None
     ) -> Callable[[Callable[_P, _T]], Callable[_P, _T]]: ...
     @overload  # plain @ns
     def __call__(self, __func: Callable[_P, _T]) -> Callable[_P, _T]: ...
 
 def FunctionNamespace(ns_uri: str | None) -> _FunctionNamespaceRegistry: ...
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/etree/_parser.pyi` & `types_lxml-2024.4.14/lxml-stubs/etree/_parser.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 import sys
 from _typeshed import _T
-from typing import Any, Generic, Iterable, Iterator
+from typing import Any, Generic, Iterable, Iterator, Literal
 
 if sys.version_info >= (3, 11):
     from typing import LiteralString, Self
 else:
     from typing_extensions import LiteralString, Self
 
 if sys.version_info >= (3, 13):
     from typing import deprecated
 else:
     from typing_extensions import deprecated
 
 from .._types import (
     SupportsLaxedItems,
     _AnyStr,
+    _DefEtreeParsers,
     _ET_co,
     _NSMapArg,
     _SaxEventNames,
     _TagName,
     _TagSelector,
 )
 from ._classlookup import ElementClassLookup
 from ._docloader import _ResolverRegistry
 from ._element import _Element
 from ._module_misc import LxmlError, LxmlSyntaxError
 from ._saxparser import ParserTarget
 from ._xmlerror import _ListErrorLog
 from ._xmlschema import XMLSchema
 
-# The basic parsers bundled in lxml.etree
-_DefEtreeParsers = XMLParser[_ET_co] | HTMLParser[_ET_co]
-
 class ParseError(LxmlSyntaxError):
     lineno: int  # pyright: ignore[reportIncompatibleVariableOverride]
     offset: int  # pyright: ignore[reportIncompatibleVariableOverride]
     code: int
     filename: str | None
     position: tuple[int, int]
     def __init__(
         self,
         message: object,
         code: int,
         line: int,
         column: int,
-        filename: str | None = ...,
+        filename: str | None = None,
     ) -> None: ...
 
 class XMLSyntaxError(ParseError): ...
 class ParserError(LxmlError): ...
 
 # Includes most stuff in _BaseParser
 class _FeedParser(Generic[_ET_co]):
@@ -59,188 +57,186 @@
     @property
     def version(self) -> LiteralString: ...
     def copy(self) -> Self: ...
     def makeelement(
         self,
         _tag: _TagName,
         /,
-        attrib: SupportsLaxedItems[str, _AnyStr] | None = ...,
-        nsmap: _NSMapArg | None = ...,
+        attrib: SupportsLaxedItems[str, _AnyStr] | None = None,
+        nsmap: _NSMapArg | None = None,
         **_extra: _AnyStr,
     ) -> _ET_co: ...
-    # XXX: In terms of annotation, what setting class_lookup
-    # does is change _ET_co (type specialization), which can't be
+    # In terms of annotation, what setting class_lookup does
+    # is change _ET_co (type specialization), which can't be
     # done automatically with current python typing system.
     # One has to change it manually during type checking.
     # Very few people would do, if there were any at all.
-    def set_element_class_lookup(self, lookup: ElementClassLookup | None = ...) -> None:
+    def set_element_class_lookup(
+        self, lookup: ElementClassLookup | None = None
+    ) -> None:
         """
         Notes
         -----
         When calling this method, it is advised to also change typing
         specialization of concerned parser too, because current python
         typing system can't change it automatically.
 
         Example
         -------
         Following code demonstrates how to create ``lxml.html.HTMLParser``
         manually from ``lxml.etree.HTMLParser``::
 
         ```python
-        parser = lxml.etree.HTMLParser()  # type is HTMLParser[_Element]
+        parser = etree.HTMLParser()
+        reveal_type(parser)  # HTMLParser[_Element]
         if TYPE_CHECKING:
-            parser = cast('HTMLParser[HtmlElement]', parser)
+            parser = cast('etree.HTMLParser[HtmlElement]', parser)
         else:
-            parser.set_element_class_lookup(lxml.html.HtmlElementClassLookup())
+            parser.set_element_class_lookup(
+                html.HtmlElementClassLookup())
+        result = etree.fromstring(data, parser=parser)
+        reveal_type(result)  # HtmlElement
         ```
         """
         ...
-    @deprecated(
-        "Removed since 5.0; deprecated since v2.0 (2008); renamed to set_element_class_lookup()"
-    )
+    @deprecated("Removed since 5.0; renamed to set_element_class_lookup()")
     def setElementClassLookup(
-        self, lookup: ElementClassLookup | None = ...
+        self, lookup: ElementClassLookup | None = None
     ) -> None: ...
     @property
     def feed_error_log(self) -> _ListErrorLog: ...
     def feed(self, data: _AnyStr) -> None: ...
 
-# XXX: Custom parser target support is temporarily abandoned,
+# Custom parser target support is abandoned,
 # see comment in XMLParser
 class _ParserTargetMixin(Generic[_T]):
     @property
     def target(self) -> ParserTarget[_T] | None: ...
     def close(self) -> _T: ...
 
 class _PullParserMixin:
     # The iterated items from pull parser events may return anything.
     # Even etree.TreeBuilder, which produce element nodes by default, allows
     # overriding factory functions via arguments to generate anything.
-    def read_events(self) -> Iterator[tuple[str, Any]]: ...
+    def read_events(self) -> Iterator[tuple[str, _Element | Any]]: ...
 
-# XXX: Python doesn't support Higher Kinded Types, otherwise
-# it should have been something like _PT[_Element]. This means
-# one can't properly annotate subclassed XMLParser.
-# https://github.com/python/typing/issues/548
-# Same applies to all other parsers inherited from FeedParser.
-#
-# XXX: It is unfortunate that, in the end, it is decided to forfeit
+# It is unfortunate that, in the end, it is decided to forfeit
 # integration of custom target annotation (the 'target' parameter).
 # So far all attempts would cause usage of annotation unnecessarily
 # complex and convoluted, yet still can't get everything right.
 class XMLParser(_ParserTargetMixin[Any], _FeedParser[_ET_co]):
-    def __new__(
-        cls,
+    def __init__(
+        self,
         *,
-        encoding: _AnyStr | None = ...,
-        attribute_defaults: bool = ...,
-        dtd_validation: bool = ...,
-        load_dtd: bool = ...,
-        no_network: bool = ...,
-        ns_clean: bool = ...,
-        recover: bool = ...,
-        schema: XMLSchema | None = ...,
-        huge_tree: bool = ...,
-        remove_blank_text: bool = ...,
-        resolve_entities: bool = ...,
-        remove_comments: bool = ...,
-        remove_pis: bool = ...,
-        strip_cdata: bool = ...,
-        collect_ids: bool = ...,
-        target: ParserTarget[Any] | None = ...,
-        compact: bool = ...,
-    ) -> XMLParser[_Element]: ...
+        encoding: _AnyStr | None = None,
+        attribute_defaults: bool = False,
+        dtd_validation: bool = False,
+        load_dtd: bool = False,
+        no_network: bool = True,
+        ns_clean: bool = False,
+        recover: bool = False,
+        schema: XMLSchema | None = None,
+        huge_tree: bool = False,
+        remove_blank_text: bool = False,
+        resolve_entities: bool | Literal["internal"] = "internal",
+        remove_comments: bool = False,
+        remove_pis: bool = False,
+        strip_cdata: bool = True,
+        collect_ids: bool = True,
+        target: ParserTarget[Any] | None = None,
+        compact: bool = True,
+    ) -> None: ...
 
 class XMLPullParser(_PullParserMixin, XMLParser[_ET_co]):
-    def __new__(
-        cls,
-        events: Iterable[_SaxEventNames] | None = ...,
+    def __init__(
+        self,
+        events: Iterable[_SaxEventNames] | None = None,
         *,
-        tag: _TagSelector | Iterable[_TagSelector] | None = ...,
-        base_url: _AnyStr | None = ...,
+        tag: _TagSelector | Iterable[_TagSelector] | None = None,
+        base_url: _AnyStr | None = None,
         # All arguments from XMLParser
-        encoding: _AnyStr | None = ...,
-        attribute_defaults: bool = ...,
-        dtd_validation: bool = ...,
-        load_dtd: bool = ...,
-        no_network: bool = ...,
-        ns_clean: bool = ...,
-        recover: bool = ...,
-        schema: XMLSchema | None = ...,
-        huge_tree: bool = ...,
-        remove_blank_text: bool = ...,
-        resolve_entities: bool = ...,
-        remove_comments: bool = ...,
-        remove_pis: bool = ...,
-        strip_cdata: bool = ...,
-        collect_ids: bool = ...,
-        target: ParserTarget[Any] | None = ...,
-        compact: bool = ...,
-    ) -> XMLPullParser[_Element]: ...
+        encoding: _AnyStr | None = None,
+        attribute_defaults: bool = False,
+        dtd_validation: bool = False,
+        load_dtd: bool = False,
+        no_network: bool = True,
+        ns_clean: bool = False,
+        recover: bool = False,
+        schema: XMLSchema | None = None,
+        huge_tree: bool = False,
+        remove_blank_text: bool = False,
+        resolve_entities: bool | Literal["internal"] = "internal",
+        remove_comments: bool = False,
+        remove_pis: bool = False,
+        strip_cdata: bool = True,
+        collect_ids: bool = True,
+        target: ParserTarget[Any] | None = None,
+        compact: bool = True,
+    ) -> None: ...
 
 # This is XMLParser with some preset keyword arguments, and without
 # 'collect_ids' argument. Removing those keywords here, otherwise
 # ETCompatXMLParser has no reason to exist.
 class ETCompatXMLParser(XMLParser[_ET_co]):
-    def __new__(
-        cls,
+    def __init__(
+        self,
         *,
-        encoding: _AnyStr | None = ...,
-        attribute_defaults: bool = ...,
-        dtd_validation: bool = ...,
-        load_dtd: bool = ...,
-        no_network: bool = ...,
-        ns_clean: bool = ...,
-        recover: bool = ...,
-        schema: XMLSchema | None = ...,
-        huge_tree: bool = ...,
-        remove_blank_text: bool = ...,
-        resolve_entities: bool = ...,
-        strip_cdata: bool = ...,
-        target: ParserTarget[Any] | None = ...,
-        compact: bool = ...,
-    ) -> ETCompatXMLParser[_Element]: ...
+        encoding: _AnyStr | None = None,
+        attribute_defaults: bool = False,
+        dtd_validation: bool = False,
+        load_dtd: bool = False,
+        no_network: bool = True,
+        ns_clean: bool = False,
+        recover: bool = False,
+        schema: XMLSchema | None = None,
+        huge_tree: bool = False,
+        remove_blank_text: bool = False,
+        resolve_entities: bool | Literal["internal"] = True,
+        strip_cdata: bool = True,
+        target: ParserTarget[Any] | None = None,
+        compact: bool = True,
+    ) -> None: ...
 
 def set_default_parser(parser: _DefEtreeParsers[Any] | None) -> None: ...
 def get_default_parser() -> _DefEtreeParsers[Any]: ...
 
 class HTMLParser(_ParserTargetMixin[Any], _FeedParser[_ET_co]):
-    def __new__(
-        cls,
+    def __init__(
+        self,
         *,
-        encoding: _AnyStr | None = ...,
-        remove_blank_text: bool = ...,
-        remove_comments: bool = ...,
-        remove_pis: bool = ...,
-        strip_cdata: bool = ...,
-        no_network: bool = ...,
-        target: ParserTarget[Any] | None = ...,
-        schema: XMLSchema | None = ...,
-        recover: bool = ...,
-        compact: bool = ...,
-        default_doctype: bool = ...,
-        collect_ids: bool = ...,
-        huge_tree: bool = ...,
-    ) -> HTMLParser[_Element]: ...
+        encoding: _AnyStr | None = None,
+        remove_blank_text: bool = False,
+        remove_comments: bool = False,
+        remove_pis: bool = False,
+        strip_cdata: bool = True,
+        no_network: bool = True,
+        target: ParserTarget[Any] | None = None,
+        schema: XMLSchema | None = None,
+        recover: bool = True,
+        compact: bool = True,
+        default_doctype: bool = True,
+        collect_ids: bool = True,
+        huge_tree: bool = False,
+    ) -> None: ...
 
 class HTMLPullParser(_PullParserMixin, HTMLParser[_ET_co]):
-    def __new__(
-        cls,
-        events: Iterable[_SaxEventNames] | None = ...,
+    def __init__(
+        self,
+        events: Iterable[_SaxEventNames] | None = None,
         *,
-        tag: _TagSelector | Iterable[_TagSelector] | None = ...,
-        base_url: _AnyStr | None = ...,
+        tag: _TagSelector | Iterable[_TagSelector] | None = None,
+        base_url: _AnyStr | None = None,
         # All arguments from HTMLParser
-        encoding: _AnyStr | None = ...,
-        remove_blank_text: bool = ...,
-        remove_comments: bool = ...,
-        remove_pis: bool = ...,
-        strip_cdata: bool = ...,
-        no_network: bool = ...,
-        target: ParserTarget[Any] | None = ...,
-        schema: XMLSchema | None = ...,
-        recover: bool = ...,
-        compact: bool = ...,
-        default_doctype: bool = ...,
-        collect_ids: bool = ...,
-        huge_tree: bool = ...,
-    ) -> HTMLPullParser[_Element]: ...
+        encoding: _AnyStr | None = None,
+        remove_blank_text: bool = False,
+        remove_comments: bool = False,
+        remove_pis: bool = False,
+        strip_cdata: bool = True,
+        no_network: bool = True,
+        target: ParserTarget[Any] | None = None,
+        schema: XMLSchema | None = None,
+        recover: bool = True,
+        compact: bool = True,
+        default_doctype: bool = True,
+        collect_ids: bool = True,
+        huge_tree: bool = False,
+    ) -> None: ...
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/etree/_relaxng.pyi` & `types_lxml-2024.4.14/lxml-stubs/etree/_relaxng.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 
 class RelaxNG(_Validator):
     @overload
     def __init__(self, etree: _ElementOrTree) -> None: ...
     @overload
     def __init__(
         self,
-        etree: None = ...,
+        etree: None = None,
         *,
         file: _FileReadSource,
     ) -> None: ...
     def __call__(self, etree: _ElementOrTree) -> bool: ...
     @classmethod
-    def from_rnc_string(cls, src: str, base_url: str | None = ...) -> RelaxNG: ...
+    def from_rnc_string(cls, src: str, base_url: str | None = None) -> RelaxNG: ...
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/etree/_saxparser.pyi` & `types_lxml-2024.4.14/lxml-stubs/etree/_saxparser.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from _typeshed import _T_co
 from abc import abstractmethod
 from typing import Mapping, Protocol
 
-from .._types import _ElemFactory
+from .._types import _DefEtreeParsers, _ElemFactory
 from ._element import _Attrib, _Comment, _Element, _ProcessingInstruction
-from ._parser import XMLSyntaxError, _DefEtreeParsers
+from ._parser import XMLSyntaxError
 
 class XMLSyntaxAssertionError(XMLSyntaxError, AssertionError): ...
 
 class ParserTarget(Protocol[_T_co]):
     """This is a stub-only class representing parser target interface.
 
     - Because almost all methods are optional, ParserTarget should be
@@ -62,15 +62,15 @@
     def comment(self, text: str) -> None: ...
     def data(self, data: str) -> None: ...
     def end(self, tag: str) -> None: ...
     def start(
         self,
         tag: str,
         attrib: _Attrib | Mapping[str, str] | None,
-        nsmap: Mapping[str, str] | None = ...,
+        nsmap: Mapping[str, str] | None = None,
     ) -> None: ...
     # Methods below are undocumented. Lxml has described
     # 'start-ns' and 'end-ns' events however.
     def pi(self, target: str, data: str | None) -> None: ...
     # Default namespace prefix is empty string, not None
     def start_ns(self, prefix: str, uri: str) -> None: ...
     def end_ns(self, prefix: str) -> None: ...
@@ -81,15 +81,15 @@
         system_id: str | None,
     ) -> None: ...
 
 class TreeBuilder(ParserTarget[_Element]):
     def __init__(
         self,
         *,
-        element_factory: _ElemFactory[_Element] | None = ...,
-        parser: _DefEtreeParsers[_Element] | None = ...,
-        comment_factory: _ElemFactory[_Comment] | None = ...,
-        pi_factory: _ElemFactory[_ProcessingInstruction] | None = ...,
-        insert_comments: bool = ...,
-        insert_pis: bool = ...,
+        element_factory: _ElemFactory | None = None,
+        parser: _DefEtreeParsers | None = None,
+        comment_factory: _ElemFactory[_Comment] | None = None,
+        pi_factory: _ElemFactory[_ProcessingInstruction] | None = None,
+        insert_comments: bool = True,
+        insert_pis: bool = True,
     ) -> None: ...
     def close(self) -> _Element: ...
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/etree/_serializer.pyi` & `types_lxml-2024.4.14/lxml-stubs/etree/_serializer.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -28,21 +28,21 @@
 # Interface quite similar to a ParserTarget, but canonicalized output
 # is written during various stages before calling .close()
 class C14NWriterTarget:
     def __init__(
         self,
         write: Callable[[str], Any],
         *,
-        with_comments: bool = ...,
-        strip_text: bool = ...,
-        rewrite_prefixes: bool = ...,
-        qname_aware_tags: Iterable[str] | None = ...,
-        qname_aware_attrs: Iterable[str] | None = ...,
-        exclude_attrs: Iterable[str] | None = ...,
-        exclude_tags: Iterable[str] | None = ...,
+        with_comments: bool = False,
+        strip_text: bool = False,
+        rewrite_prefixes: bool = False,
+        qname_aware_tags: Iterable[str] | None = None,
+        qname_aware_attrs: Iterable[str] | None = None,
+        exclude_attrs: Iterable[str] | None = None,
+        exclude_tags: Iterable[str] | None = None,
     ) -> None: ...
     def data(self, data: str) -> None: ...
     def start_ns(self, prefix: str, uri: str) -> None: ...
     def start(self, tag: str, attrs: SupportsLaxedItems[str, str] | None) -> None: ...
     def end(self, tag: str) -> None: ...
     def comment(self, text: str) -> None: ...
     def pi(self, target: str, data: str | None) -> None: ...
@@ -53,62 +53,62 @@
 # 2x output (None, .write())
 # options keyword arguments come from C14NWriterTarget.__init__
 @overload
 def canonicalize(
     xml_data: _AnyStr | _ElementOrTree,
     *,
     out: SupportsWrite[str],
-    with_comments: bool = ...,
-    strip_text: bool = ...,
-    rewrite_prefixes: bool = ...,
-    qname_aware_tags: Iterable[str] | None = ...,
-    qname_aware_attrs: Iterable[str] | None = ...,
-    exclude_attrs: Iterable[str] | None = ...,
-    exclude_tags: Iterable[str] | None = ...,
+    with_comments: bool = False,
+    strip_text: bool = False,
+    rewrite_prefixes: bool = False,
+    qname_aware_tags: Iterable[str] | None = None,
+    qname_aware_attrs: Iterable[str] | None = None,
+    exclude_attrs: Iterable[str] | None = None,
+    exclude_tags: Iterable[str] | None = None,
 ) -> None: ...
 @overload
 def canonicalize(
-    xml_data: None = ...,
+    xml_data: None = None,
     *,
     out: SupportsWrite[str],
     from_file: _FileReadSource,
-    with_comments: bool = ...,
-    strip_text: bool = ...,
-    rewrite_prefixes: bool = ...,
-    qname_aware_tags: Iterable[str] | None = ...,
-    qname_aware_attrs: Iterable[str] | None = ...,
-    exclude_attrs: Iterable[str] | None = ...,
-    exclude_tags: Iterable[str] | None = ...,
+    with_comments: bool = False,
+    strip_text: bool = False,
+    rewrite_prefixes: bool = False,
+    qname_aware_tags: Iterable[str] | None = None,
+    qname_aware_attrs: Iterable[str] | None = None,
+    exclude_attrs: Iterable[str] | None = None,
+    exclude_tags: Iterable[str] | None = None,
 ) -> None: ...
 @overload
 def canonicalize(
     xml_data: _AnyStr | _ElementOrTree,
     *,
-    out: None = ...,
-    with_comments: bool = ...,
-    strip_text: bool = ...,
-    rewrite_prefixes: bool = ...,
-    qname_aware_tags: Iterable[str] | None = ...,
-    qname_aware_attrs: Iterable[str] | None = ...,
-    exclude_attrs: Iterable[str] | None = ...,
-    exclude_tags: Iterable[str] | None = ...,
+    out: None = None,
+    with_comments: bool = False,
+    strip_text: bool = False,
+    rewrite_prefixes: bool = False,
+    qname_aware_tags: Iterable[str] | None = None,
+    qname_aware_attrs: Iterable[str] | None = None,
+    exclude_attrs: Iterable[str] | None = None,
+    exclude_tags: Iterable[str] | None = None,
 ) -> str: ...
 @overload
 def canonicalize(
-    xml_data: None = ...,
+    xml_data: None = None,
     *,
-    out: None = ...,
+    out: None = None,
     from_file: _FileReadSource,
-    with_comments: bool = ...,
-    strip_text: bool = ...,
-    rewrite_prefixes: bool = ...,
-    qname_aware_tags: Iterable[str] | None = ...,
-    qname_aware_attrs: Iterable[str] | None = ...,
-    exclude_attrs: Iterable[str] | None = ...,
-    exclude_tags: Iterable[str] | None = ...,
+    with_comments: bool = False,
+    strip_text: bool = False,
+    rewrite_prefixes: bool = False,
+    qname_aware_tags: Iterable[str] | None = None,
+    qname_aware_attrs: Iterable[str] | None = None,
+    exclude_attrs: Iterable[str] | None = None,
+    exclude_tags: Iterable[str] | None = None,
 ) -> str: ...
 
 #
 # Incremental serializers
 # https://lxml.de/api.html#incremental-xml-generation
 #
 # Special notes:
@@ -117,75 +117,75 @@
 #    manager objects. For coherence, we distinguish their return type
 #    differently.
 #
 @final
 class _IncrementalFileWriter:
     def write_declaration(
         self,
-        version: _AnyStr | None = ...,
-        standalone: bool | None = ...,
-        doctype: _AnyStr | None = ...,
+        version: _AnyStr | None = None,
+        standalone: bool | None = None,
+        doctype: _AnyStr | None = None,
     ) -> None: ...
     def write_doctype(self, doctype: _AnyStr | None) -> None: ...
     def write(
         self,
         *args: _AnyStr | _Element,
-        with_tail: bool = ...,
-        pretty_print: bool = ...,
-        method: _OutputMethodArg | None = ...,
+        with_tail: bool = True,
+        pretty_print: bool = False,
+        method: _OutputMethodArg | None = None,
     ) -> None: ...
     def flush(self) -> None: ...
     def method(self, method: _OutputMethodArg | None) -> ContextManager[None]: ...
     def element(
         self,
         tag: _TagName,
-        attrib: SupportsLaxedItems[str, _AnyStr] | None = ...,
-        nsmap: _NSMapArg | None = ...,
-        method: _OutputMethodArg | None = ...,
+        attrib: SupportsLaxedItems[str, _AnyStr] | None = None,
+        nsmap: _NSMapArg | None = None,
+        method: _OutputMethodArg | None = None,
         **_extra: _AnyStr,
     ) -> ContextManager[None]: ...
 
 @final
 class _AsyncIncrementalFileWriter:
     async def write_declaration(
         self,
-        version: _AnyStr | None = ...,
-        standalone: bool | None = ...,
-        doctype: _AnyStr | None = ...,
+        version: _AnyStr | None = None,
+        standalone: bool | None = None,
+        doctype: _AnyStr | None = None,
     ) -> None: ...
     async def write_doctype(self, doctype: _AnyStr | None) -> None: ...
     async def write(
         self,
         *args: _AnyStr | _Element | None,
-        with_tail: bool = ...,
-        pretty_print: bool = ...,
-        method: _OutputMethodArg | None = ...,
+        with_tail: bool = True,
+        pretty_print: bool = False,
+        method: _OutputMethodArg | None = None,
     ) -> None: ...
     async def flush(self) -> None: ...
     def method(self, method: _OutputMethodArg | None) -> AsyncContextManager[None]: ...
     def element(
         self,
         tag: _TagName,
-        attrib: SupportsLaxedItems[str, _AnyStr] | None = ...,
-        nsmap: _NSMapArg | None = ...,
-        method: _OutputMethodArg | None = ...,
+        attrib: SupportsLaxedItems[str, _AnyStr] | None = None,
+        nsmap: _NSMapArg | None = None,
+        method: _OutputMethodArg | None = None,
         **_extra: _AnyStr,
     ) -> AsyncContextManager[None]: ...
 
 class xmlfile(
     AsyncContextManager[_AsyncIncrementalFileWriter],
     ContextManager[_IncrementalFileWriter],
 ):
     def __init__(
         self,
         output_file: _FileWriteSource,
-        encoding: _AnyStr | None = ...,
-        compression: int | None = ...,
-        close: bool = ...,
-        buffered: bool = ...,
+        encoding: _AnyStr | None = None,
+        compression: int | None = None,
+        close: bool = False,
+        buffered: bool = True,
     ) -> None: ...
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None: ...
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/etree/_xmlerror.pyi` & `types_lxml-2024.4.14/lxml-stubs/etree/_xmlerror.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -180,60 +180,64 @@
     Annotation notes
     ----------------
     These integer constants sementically fit int enum better, but
     in the end they are just integers. No enum properties and mechanics
     would work on them.
     """
 
-    NONE = ...
-    WARNING = ...
-    ERROR = ...
-    FATAL = ...
+    # fmt: off
+    NONE    = 0
+    WARNING = 1
+    ERROR   = 2
+    FATAL   = 3
+    # fmt: on
 
 class ErrorDomains(enum.IntEnum):
     """Part of the library that raised error
 
     Annotation notes
     ----------------
     These integer constants sementically fit int enum better, but
     in the end they are just integers. No enum properties and mechanics
     would work on them.
     """
 
-    NONE = ...
-    PARSER = ...
-    TREE = ...
-    NAMESPACE = ...
-    DTD = ...
-    HTML = ...
-    MEMORY = ...
-    OUTPUT = ...
-    IO = ...
-    FTP = ...
-    HTTP = ...
-    XINCLUDE = ...
-    XPATH = ...
-    XPOINTER = ...
-    REGEXP = ...
-    DATATYPE = ...
-    SCHEMASP = ...
-    SCHEMASV = ...
-    RELAXNGP = ...
-    RELAXNGV = ...
-    CATALOG = ...
-    C14N = ...
-    XSLT = ...
-    VALID = ...
-    CHECK = ...
-    WRITER = ...
-    MODULE = ...
-    I18N = ...
-    SCHEMATRONV = ...
-    BUFFER = ...
-    URI = ...
+    # fmt: off
+    NONE         = 0
+    PARSER       = 1
+    TREE         = 2
+    NAMESPACE    = 3
+    DTD          = 4
+    HTML         = 5
+    MEMORY       = 6
+    OUTPUT       = 7
+    IO           = 8
+    FTP          = 9
+    HTTP         = 10
+    XINCLUDE     = 11
+    XPATH        = 12
+    XPOINTER     = 13
+    REGEXP       = 14
+    DATATYPE     = 15
+    SCHEMASP     = 16
+    SCHEMASV     = 17
+    RELAXNGP     = 18
+    RELAXNGV     = 19
+    CATALOG      = 20
+    C14N         = 21
+    XSLT         = 22
+    VALID        = 23
+    CHECK        = 24
+    WRITER       = 25
+    MODULE       = 26
+    I18N         = 27
+    SCHEMATRONV  = 28
+    BUFFER       = 29
+    URI          = 30
+    # fmt: on
 
 # TODO implement ErrorTypes enum, looks like unavoidable
 class ErrorTypes(enum.IntEnum):
     """The actual libxml2 error code
 
     Annotation notes
     ----------------
@@ -254,47 +258,49 @@
     Annotation notes
     ----------------
     These integer constants sementically fit int enum better, but
     in the end they are just integers. No enum properties and mechanics
     would work on them.
     """
 
-    RELAXNG_OK = ...
-    RELAXNG_ERR_MEMORY = ...
-    RELAXNG_ERR_TYPE = ...
-    RELAXNG_ERR_TYPEVAL = ...
-    RELAXNG_ERR_DUPID = ...
-    RELAXNG_ERR_TYPECMP = ...
-    RELAXNG_ERR_NOSTATE = ...
-    RELAXNG_ERR_NODEFINE = ...
-    RELAXNG_ERR_LISTEXTRA = ...
-    RELAXNG_ERR_LISTEMPTY = ...
-    RELAXNG_ERR_INTERNODATA = ...
-    RELAXNG_ERR_INTERSEQ = ...
-    RELAXNG_ERR_INTEREXTRA = ...
-    RELAXNG_ERR_ELEMNAME = ...
-    RELAXNG_ERR_ATTRNAME = ...
-    RELAXNG_ERR_ELEMNONS = ...
-    RELAXNG_ERR_ATTRNONS = ...
-    RELAXNG_ERR_ELEMWRONGNS = ...
-    RELAXNG_ERR_ATTRWRONGNS = ...
-    RELAXNG_ERR_ELEMEXTRANS = ...
-    RELAXNG_ERR_ATTREXTRANS = ...
-    RELAXNG_ERR_ELEMNOTEMPTY = ...
-    RELAXNG_ERR_NOELEM = ...
-    RELAXNG_ERR_NOTELEM = ...
-    RELAXNG_ERR_ATTRVALID = ...
-    RELAXNG_ERR_CONTENTVALID = ...
-    RELAXNG_ERR_EXTRACONTENT = ...
-    RELAXNG_ERR_INVALIDATTR = ...
-    RELAXNG_ERR_DATAELEM = ...
-    RELAXNG_ERR_VALELEM = ...
-    RELAXNG_ERR_LISTELEM = ...
-    RELAXNG_ERR_DATATYPE = ...
-    RELAXNG_ERR_VALUE = ...
-    RELAXNG_ERR_LIST = ...
-    RELAXNG_ERR_NOGRAMMAR = ...
-    RELAXNG_ERR_EXTRADATA = ...
-    RELAXNG_ERR_LACKDATA = ...
-    RELAXNG_ERR_INTERNAL = ...
-    RELAXNG_ERR_ELEMWRONG = ...
-    RELAXNG_ERR_TEXTWRONG = ...
+    # fmt: off
+    RELAXNG_OK               = 0
+    RELAXNG_ERR_MEMORY       = 1
+    RELAXNG_ERR_TYPE         = 2
+    RELAXNG_ERR_TYPEVAL      = 3
+    RELAXNG_ERR_DUPID        = 4
+    RELAXNG_ERR_TYPECMP      = 5
+    RELAXNG_ERR_NOSTATE      = 6
+    RELAXNG_ERR_NODEFINE     = 7
+    RELAXNG_ERR_LISTEXTRA    = 8
+    RELAXNG_ERR_LISTEMPTY    = 9
+    RELAXNG_ERR_INTERNODATA  = 10
+    RELAXNG_ERR_INTERSEQ     = 11
+    RELAXNG_ERR_INTEREXTRA   = 12
+    RELAXNG_ERR_ELEMNAME     = 13
+    RELAXNG_ERR_ATTRNAME     = 14
+    RELAXNG_ERR_ELEMNONS     = 15
+    RELAXNG_ERR_ATTRNONS     = 16
+    RELAXNG_ERR_ELEMWRONGNS  = 17
+    RELAXNG_ERR_ATTRWRONGNS  = 18
+    RELAXNG_ERR_ELEMEXTRANS  = 19
+    RELAXNG_ERR_ATTREXTRANS  = 20
+    RELAXNG_ERR_ELEMNOTEMPTY = 21
+    RELAXNG_ERR_NOELEM       = 22
+    RELAXNG_ERR_NOTELEM      = 23
+    RELAXNG_ERR_ATTRVALID    = 24
+    RELAXNG_ERR_CONTENTVALID = 25
+    RELAXNG_ERR_EXTRACONTENT = 26
+    RELAXNG_ERR_INVALIDATTR  = 27
+    RELAXNG_ERR_DATAELEM     = 28
+    RELAXNG_ERR_VALELEM      = 29
+    RELAXNG_ERR_LISTELEM     = 30
+    RELAXNG_ERR_DATATYPE     = 31
+    RELAXNG_ERR_VALUE        = 32
+    RELAXNG_ERR_LIST         = 33
+    RELAXNG_ERR_NOGRAMMAR    = 34
+    RELAXNG_ERR_EXTRADATA    = 35
+    RELAXNG_ERR_LACKDATA     = 36
+    RELAXNG_ERR_INTERNAL     = 37
+    RELAXNG_ERR_ELEMWRONG    = 38
+    RELAXNG_ERR_TEXTWRONG    = 39
+    # fmt: on
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/etree/_xmlid.pyi` & `types_lxml-2024.4.14/lxml-stubs/etree/_xmlid.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -2,65 +2,64 @@
 from typing import Collection, Generic, Iterator, overload
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
-from .._types import _ET, _AnyStr, _FileReadSource
+from .._types import _ET, _AnyStr, _DefEtreeParsers, _FileReadSource
 from ._element import _Element, _ElementTree
-from ._parser import _DefEtreeParsers
 
 # arguments for these module funcs are the same as XML() and parse()
 
 @overload
 def XMLID(
     text: _AnyStr,
     parser: _DefEtreeParsers[_ET],
     *,
-    base_url: _AnyStr | None = ...,
+    base_url: _AnyStr | None = None,
 ) -> tuple[_ET, dict[str, _ET]]: ...
 @overload
 def XMLID(
     text: _AnyStr,
-    parser: None = ...,
+    parser: None = None,
     *,
-    base_url: _AnyStr | None = ...,
+    base_url: _AnyStr | None = None,
 ) -> tuple[_Element, dict[str, _Element]]: ...
 
 # It is interesting how _IDDict is used below but not above
 
 @overload
 def XMLDTDID(
     text: _AnyStr,
     parser: _DefEtreeParsers[_ET],
     *,
-    base_url: _AnyStr | None = ...,
+    base_url: _AnyStr | None = None,
 ) -> tuple[_ET, _IDDict[_ET]]: ...
 @overload
 def XMLDTDID(
     text: _AnyStr,
-    parser: None = ...,
+    parser: None = None,
     *,
-    base_url: _AnyStr | None = ...,
-) -> tuple[_Element, _IDDict[_Element]]: ...
+    base_url: _AnyStr | None = None,
+) -> tuple[_Element, _IDDict]: ...
 @overload
 def parseid(
     source: _FileReadSource,
     parser: _DefEtreeParsers[_ET],
     *,
-    base_url: _AnyStr | None = ...,
+    base_url: _AnyStr | None = None,
 ) -> tuple[_ElementTree[_ET], _IDDict[_ET]]: ...
 @overload
 def parseid(
     source: _FileReadSource,
-    parser: None = ...,
+    parser: None = None,
     *,
-    base_url: _AnyStr | None = ...,
-) -> tuple[_ElementTree[_Element], _IDDict[_Element]]: ...
+    base_url: _AnyStr | None = None,
+) -> tuple[_ElementTree, _IDDict]: ...
 
 class _IDDict(Collection[str], Generic[_ET]):
     """Dictionary-like proxy class that mapps ID attributes to elements
 
     Original Docstring
     ------------------
     The dictionary must be instantiated with the root element of a parsed XML
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/etree/_xmlschema.pyi` & `types_lxml-2024.4.14/lxml-stubs/etree/_xmlschema.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 class XMLSchema(_Validator):
     # file arg only useful when etree arg is None
     @overload
     def __init__(
         self,
         etree: _ElementOrTree,
         *,
-        file: None = ...,
-        attribute_defaults: bool = ...,
+        file: None = None,
+        attribute_defaults: bool = False,
     ) -> None: ...
     @overload
     def __init__(
         self,
-        etree: None = ...,
+        etree: None = None,
         *,
         file: _FileReadSource,
-        attribute_defaults: bool = ...,
+        attribute_defaults: bool = False,
     ) -> None: ...
     def __call__(self, etree: _ElementOrTree) -> bool: ...
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/etree/_xpath.pyi` & `types_lxml-2024.4.14/lxml-stubs/etree/_xpath.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -43,89 +43,87 @@
 class _XPathEvaluatorBase(Protocol):
     @property
     def error_log(self) -> _ListErrorLog: ...
     @abstractmethod
     def __call__(self, _arg: Any, /, **__var: _XPathVarArg) -> _XPathObject: ...
     # evaluate() should have been abstract like __call__(), but requiring all
     # subclasses to add deprecated method is idiocy
-    @deprecated(
-        "Removed since 5.0; deprecated since v2.0 (2008); call the object directly"
-    )
+    @deprecated("Removed since 5.0; call instance directly instead")
     def evaluate(self, _arg: Any, /, **__var: _XPathVarArg) -> _XPathObject: ...
 
 class XPath(_XPathEvaluatorBase):
     def __init__(
         self,
         path: _AnyStr,
         *,
-        namespaces: _NonDefaultNSMapArg | None = ...,
-        extensions: _XPathExtFuncArg | None = ...,
-        regexp: bool = ...,
-        smart_strings: bool = ...,
+        namespaces: _NonDefaultNSMapArg | None = None,
+        extensions: _XPathExtFuncArg | None = None,
+        regexp: bool = True,
+        smart_strings: bool = True,
     ) -> None: ...
     def __call__(
         self, _etree_or_element: _ElementOrTree, /, **_variables: _XPathVarArg
     ) -> _XPathObject: ...
     @property
     def path(self) -> str: ...
 
 class ETXPath(XPath):
     def __init__(
         self,
         path: _AnyStr,
         *,
-        extensions: _XPathExtFuncArg | None = ...,
-        regexp: bool = ...,
-        smart_strings: bool = ...,
+        extensions: _XPathExtFuncArg | None = None,
+        regexp: bool = True,
+        smart_strings: bool = True,
     ) -> None: ...
 
 class XPathElementEvaluator(_XPathEvaluatorBase):
     def __init__(
         self,
         element: _Element,
         *,
-        namespaces: _NonDefaultNSMapArg | None = ...,
-        extensions: _XPathExtFuncArg | None = ...,
-        regexp: bool = ...,
-        smart_strings: bool = ...,
+        namespaces: _NonDefaultNSMapArg | None = None,
+        extensions: _XPathExtFuncArg | None = None,
+        regexp: bool = True,
+        smart_strings: bool = True,
     ) -> None: ...
     def __call__(
         self, _path: _AnyStr, /, **_variables: _XPathVarArg
     ) -> _XPathObject: ...
     def register_namespace(self, prefix: _AnyStr, uri: _AnyStr) -> None: ...
     def register_namespaces(self, namespaces: _NonDefaultNSMapArg | None) -> None: ...
 
 class XPathDocumentEvaluator(XPathElementEvaluator):
     def __init__(
         self,
-        etree: _ElementTree[_Element],
+        etree: _ElementTree,
         *,
-        namespaces: _NonDefaultNSMapArg | None = ...,
-        extensions: _XPathExtFuncArg | None = ...,
-        regexp: bool = ...,
-        smart_strings: bool = ...,
+        namespaces: _NonDefaultNSMapArg | None = None,
+        extensions: _XPathExtFuncArg | None = None,
+        regexp: bool = True,
+        smart_strings: bool = True,
     ) -> None: ...
 
 @overload
 def XPathEvaluator(
     etree_or_element: _Element,
     *,
-    namespaces: _NonDefaultNSMapArg | None = ...,
-    extensions: _XPathExtFuncArg | None = ...,
-    regexp: bool = ...,
-    smart_strings: bool = ...,
+    namespaces: _NonDefaultNSMapArg | None = None,
+    extensions: _XPathExtFuncArg | None = None,
+    regexp: bool = True,
+    smart_strings: bool = True,
 ) -> XPathElementEvaluator: ...
 @overload
 def XPathEvaluator(
-    etree_or_element: _ElementTree[_Element],
+    etree_or_element: _ElementTree,
     *,
-    namespaces: _NonDefaultNSMapArg | None = ...,
-    extensions: _XPathExtFuncArg | None = ...,
-    regexp: bool = ...,
-    smart_strings: bool = ...,
+    namespaces: _NonDefaultNSMapArg | None = None,
+    extensions: _XPathExtFuncArg | None = None,
+    regexp: bool = True,
+    smart_strings: bool = True,
 ) -> XPathDocumentEvaluator: ...
 @final
 class _ElementUnicodeResult(str, Generic[_ET]):
     """Smart string is a private str subclass documented in
     [return types](https://lxml.de/xpathxslt.html#xpath-return-values)
     of XPath evaluation result.
 
@@ -141,17 +139,17 @@
     def is_text(self) -> bool: ...
     @property
     def attrname(self) -> str | None: ...
     def getparent(self: _ElementUnicodeResult[_ET]) -> _ET | None: ...
 
 def Extension(
     module: object,
-    function_mapping: Mapping[str, str] | None = ...,
+    function_mapping: Mapping[str, str] | None = None,
     *,
-    ns: str | None = ...,
+    ns: str | None = None,
 ) -> dict[tuple[str | None, str], Callable[..., Any]]:
     """Build a dictionary of extension functions from the functions
     defined in a module or the methods of an object.
 
     Original Docstring
     ------------------
     As second argument, you can pass an additional mapping of
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/etree/_xslt.pyi` & `types_lxml-2024.4.14/lxml-stubs/etree/_xslt.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,24 @@
     from typing_extensions import TypeAlias
 
 if sys.version_info >= (3, 13):
     from typing import deprecated
 else:
     from typing_extensions import deprecated
 
-from .._types import SupportsLaxedItems, _AnyStr, _ElementOrTree, _FileWriteSource
+from .._types import (
+    SupportsLaxedItems,
+    _AnyStr,
+    _DefEtreeParsers,
+    _ElementOrTree,
+    _FileWriteSource,
+)
 from ._classlookup import PIBase
 from ._element import _Element, _ElementTree
 from ._module_misc import LxmlError
-from ._parser import _DefEtreeParsers
 from ._serializer import SerialisationError
 from ._xmlerror import _ListErrorLog
 from ._xpath import XPath
 
 _Stylesheet_Param: TypeAlias = _XSLTQuotedStringParam | XPath | str
 
 # exported constants
@@ -43,25 +48,25 @@
 class XSLTSaveError(XSLTError, SerialisationError):
     """Error serialising an XSLT result"""
 
 class XSLTExtensionError(XSLTError):
     """Error registering an XSLT extension"""
 
 @final
-class _XSLTResultTree(_ElementTree[_Element]):
+class _XSLTResultTree(_ElementTree):
     """The result of an XSLT evaluation"""
 
-    def write_output(self, file: _FileWriteSource, *, compression: int = ...) -> None:
+    def write_output(self, file: _FileWriteSource, *, compression: int = 0) -> None:
         """Serialise the XSLT output to a file or file-like object
 
         As opposed to the generic ``.write()`` method, ``.write_output()`` serialises
         the result as defined by the ``<xsl:output>`` tag.
         """
     @property
-    def xslt_profile(self) -> _ElementTree[_Element] | None:
+    def xslt_profile(self) -> _ElementTree | None:
         """Return an ElementTree with profiling data for the stylesheet run"""
 
 @final
 class _XSLTQuotedStringParam:
     """A wrapper class for literal XSLT string parameters that require
     quote escaping"""
 
@@ -96,19 +101,19 @@
 
     DENY_ALL: ClassVar[XSLTAccessControl]
     DENY_WRITE: ClassVar[XSLTAccessControl]
 
     def __init__(
         self,
         *,
-        read_file: bool = ...,
-        write_file: bool = ...,
-        create_dir: bool = ...,
-        read_network: bool = ...,
-        write_network: bool = ...,
+        read_file: bool = True,
+        write_file: bool = True,
+        create_dir: bool = True,
+        read_network: bool = True,
+        write_network: bool = True,
     ) -> None: ...
     @property
     def options(self) -> __AccessControlConfig: ...
 
 class XSLT:
     """Turn an XSL document into an XSLT object.
 
@@ -136,51 +141,47 @@
     """
 
     def __init__(
         self,
         xslt_input: _ElementOrTree,
         extensions: (
             SupportsLaxedItems[tuple[_AnyStr, _AnyStr], XSLTExtension] | None
-        ) = ...,
-        regexp: bool = ...,
-        access_control: XSLTAccessControl | None = ...,
+        ) = None,
+        regexp: bool = True,
+        access_control: XSLTAccessControl | None = None,
     ) -> None: ...
     def __call__(
         self,
         _input: _ElementOrTree,
         /,
-        profile_run: bool = ...,
+        profile_run: bool = False,
         **__kw: _Stylesheet_Param,
     ) -> _XSLTResultTree: ...
     @property
     def error_log(self) -> _ListErrorLog: ...
     @staticmethod
     def strparam(strval: _AnyStr) -> _XSLTQuotedStringParam: ...
     @staticmethod
     def set_global_max_depth(max_depth: int) -> None: ...
-    @deprecated(
-        "Removed since 5.0; deprecated since v2.0 (2008); call instance directly instead"
-    )
+    @deprecated("Removed since 5.0; call instance directly instead")
     def apply(
         self,
         _input: _ElementOrTree,
         /,
-        profile_run: bool = ...,
+        profile_run: bool = False,
         **__kw: _Stylesheet_Param,
     ) -> _XSLTResultTree: ...
     @deprecated("Since v2.0 (2008); use str(result_tree) instead")
     def tostring(
         self,
-        result_tree: _ElementTree[_Element],
+        result_tree: _ElementTree,
     ) -> str: ...
 
 class _XSLTProcessingInstruction(PIBase):
-    def parseXSL(
-        self, parser: _DefEtreeParsers[_Element] | None = ...
-    ) -> _ElementTree[_Element]: ...
+    def parseXSL(self, parser: _DefEtreeParsers | None = None) -> _ElementTree: ...
     def set(self, key: Literal["href"], value: str) -> None: ...  # type: ignore[override]
 
 # Nodes are usually some opaque or read-only wrapper of _Element.
 # They provide access of varying attributes depending on node type,
 # which are not known to static typing. So use typing.Any here
 # to not prevent their access.
 class XSLTExtension(metaclass=abc.ABCMeta):
@@ -211,36 +212,36 @@
     @overload
     def apply_templates(
         self,
         context: Any,  # _XSLTContext,
         node: Any,
         output_parent: _Element,
         *,
-        elements_only: bool = ...,
-        remove_blank_text: bool = ...,
+        elements_only: bool = False,
+        remove_blank_text: bool = False,
     ) -> None: ...
     @overload
-    def apply_templates(
+    def apply_templates(  # type: ignore[overload-overlap]
         self,
         context: Any,
         node: Any,
-        output_parent: None = ...,
+        output_parent: None = None,
         *,
         elements_only: Literal[True],
-        remove_blank_text: bool = ...,
+        remove_blank_text: bool = False,
     ) -> list[_Element]: ...
     @overload
     def apply_templates(
         self,
         context: Any,
         node: Any,
-        output_parent: None = ...,
+        output_parent: None = None,
         *,
-        elements_only: Literal[False] = ...,
-        remove_blank_text: bool = ...,
+        elements_only: bool = False,
+        remove_blank_text: bool = False,
     ) -> list[str | _Element]:
         """Call this method to retrieve the result of applying templates
         to an element
 
         Original Docstring
         ------------------
         The return value is a list of elements or text strings that
@@ -260,34 +261,34 @@
         """
     @overload
     def process_children(
         self,
         context: Any,  # _XSLTContext,
         output_parent: _Element,
         *,
-        elements_only: bool = ...,
-        remove_blank_text: bool = ...,
+        elements_only: bool = False,
+        remove_blank_text: bool = False,
     ) -> None: ...
     @overload
-    def process_children(
+    def process_children(  # type: ignore[overload-overlap]
         self,
         context: Any,
-        output_parent: None = ...,
+        output_parent: None = None,
         *,
         elements_only: Literal[True],
-        remove_blank_text: bool = ...,
+        remove_blank_text: bool = False,
     ) -> list[_Element]: ...
     @overload
     def process_children(
         self,
         context: Any,
-        output_parent: None = ...,
+        output_parent: None = None,
         *,
-        elements_only: Literal[False] = ...,
-        remove_blank_text: bool = ...,
+        elements_only: bool = False,
+        remove_blank_text: bool = False,
     ) -> list[str | _Element]:
         """Call this method to process the XSLT content of the extension
         element itself.
 
         Original Docstring
         ------------------
         The return value is a list of elements or text strings that
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/html/__init__.pyi` & `types_lxml-2024.4.14/lxml-stubs/html/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/lxml-stubs/html/_element.pyi` & `types_lxml-2024.4.14/lxml-stubs/html/_element.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     def forms(self) -> list[FormElement]: ...
     @property
     def body(self) -> HtmlElement: ...
     @property
     def head(self) -> HtmlElement: ...
     # set() differs from _Element.set() -- value has default, can accept None,
     # which means boolean attribute without value, like <option selected>
-    def set(self, key: _AttrName, value: _AttrVal | None = ...) -> None: ...
+    def set(self, key: _AttrName, value: _AttrVal | None = None) -> None: ...
     def drop_tree(self) -> None: ...
     def drop_tag(self) -> None: ...
     def find_rel_links(
         self,
         rel: str,  # Can be bytes, but never match anything on py3
     ) -> list[HtmlElement]: ...
     def find_class(
@@ -83,38 +83,39 @@
     # similar to _Attrib.pop(); all defaults except the first
     # is discarded. No point to honor such useless signature.
     @overload
     def get_element_by_id(self, id: _AnyStr) -> HtmlElement: ...
     @overload
     def get_element_by_id(self, id: _AnyStr, default: _T) -> HtmlElement | _T: ...
     # text_content() uses XPath behind the scene, and smart string
-    # subscript should point to original element type
-    # XXX But acutally the result is always None, as it uses XPath
-    # string() to merge text content and destroy element heritage info
+    # subscript should point to original element type.
+    # But unfortunately, the getparent() result of HtmlElement.text_content()
+    # is always None, as it uses XPath string() to merge text content,
+    # thus destroying element heritage info
     def text_content(self) -> etree._ElementUnicodeResult[Self]: ...
     #
     # HtmlMixin Link functions
     #
     def make_links_absolute(
         self,
-        base_url: str | None = ...,  # not bytes
-        resolve_base_href: bool = ...,
-        handle_failures: _HANDLE_FAILURES | None = ...,
+        base_url: str | None = None,  # not bytes
+        resolve_base_href: bool = True,
+        handle_failures: _HANDLE_FAILURES | None = None,
     ) -> None: ...
     def resolve_base_href(
         self,
-        handle_failures: _HANDLE_FAILURES | None = ...,
+        handle_failures: _HANDLE_FAILURES | None = None,
     ) -> None: ...
     # (element, attribute, link, pos)
     def iterlinks(self) -> Iterator[tuple[HtmlElement, str | None, str, int]]: ...
     def rewrite_links(
         self,
         link_repl_func: Callable[[str], str | None],
-        resolve_base_href: bool = ...,
-        base_href: str | None = ...,
+        resolve_base_href: bool = True,
+        base_href: str | None = None,
     ) -> None: ...
     # Overriding of most _Element methods
     #
     # Subclassing of _Element should not go beyond HtmlElement. For example,
     # while children of HtmlElement are mostly HtmlElement, FormElement never
     # contains FormElement as child.
     @overload
@@ -128,85 +129,96 @@
     def __iter__(self) -> Iterator[HtmlElement]: ...
     def __reversed__(self) -> Iterator[HtmlElement]: ...
     def append(self, element: HtmlElement) -> None: ...
     def extend(self, elements: Iterable[HtmlElement]) -> None: ...
     def insert(self, index: int, element: HtmlElement) -> None: ...
     def remove(self, element: HtmlElement) -> None: ...
     def index(
-        self, child: HtmlElement, start: int | None = ..., end: int | None = ...
+        self, child: HtmlElement, start: int | None = None, end: int | None = None
     ) -> int: ...
     def addnext(self, element: HtmlElement) -> None: ...
     def addprevious(self, element: HtmlElement) -> None: ...
     def replace(self, old_element: HtmlElement, new_element: HtmlElement) -> None: ...
     def getparent(self) -> HtmlElement | None: ...
     def getnext(self) -> HtmlElement | None: ...
     def getprevious(self) -> HtmlElement | None: ...
     def getroottree(self) -> etree._ElementTree[HtmlElement]: ...
     @overload
     def itersiblings(
-        self, *tags: _TagSelector, preceding: bool = ...
+        self, *tags: _TagSelector, preceding: bool = False
     ) -> Iterator[HtmlElement]: ...
     @overload
     def itersiblings(
-        self, *, tag: Iterable[_TagSelector] | None = ..., preceding: bool = ...
+        self,
+        *,
+        tag: _TagSelector | Iterable[_TagSelector] | None = None,
+        preceding: bool = False,
     ) -> Iterator[HtmlElement]: ...
     @overload
     def iterancestors(self, *tags: _TagSelector) -> Iterator[HtmlElement]: ...
     @overload
     def iterancestors(
-        self, *, tag: Iterable[_TagSelector] | None = ...
+        self, *, tag: _TagSelector | Iterable[_TagSelector] | None = None
     ) -> Iterator[HtmlElement]: ...
     @overload
     def iterdescendants(self, *tags: _TagSelector) -> Iterator[HtmlElement]: ...
     @overload
     def iterdescendants(
-        self, *, tag: Iterable[_TagSelector] | None = ...
+        self, *, tag: _TagSelector | Iterable[_TagSelector] | None = None
     ) -> Iterator[HtmlElement]: ...
     @overload
     def iterchildren(
-        self, *tags: _TagSelector, reversed: bool = ...
+        self, *tags: _TagSelector, reversed: bool = False
     ) -> Iterator[HtmlElement]: ...
     @overload
     def iterchildren(
-        self, *, tag: Iterable[_TagSelector] | None = ..., reversed: bool = ...
+        self,
+        *,
+        tag: _TagSelector | Iterable[_TagSelector] | None = None,
+        reversed: bool = False,
     ) -> Iterator[HtmlElement]: ...
     @overload
     def iter(self, *tags: _TagSelector) -> Iterator[HtmlElement]: ...
     @overload
     def iter(
-        self, *, tag: Iterable[_TagSelector] | None = ...
+        self, *, tag: _TagSelector | Iterable[_TagSelector] | None = None
     ) -> Iterator[HtmlElement]: ...
     @overload
-    def itertext(self, *tags: _TagSelector, with_tail: bool = ...) -> Iterator[str]: ...
+    def itertext(
+        self, *tags: _TagSelector, with_tail: bool = True
+    ) -> Iterator[str]: ...
     @overload
     def itertext(
-        self, *, tag: Iterable[_TagSelector] | None = ..., with_tail: bool = ...
+        self,
+        *,
+        tag: _TagSelector | Iterable[_TagSelector] | None = None,
+        with_tail: bool = True,
     ) -> Iterator[str]: ...
     def makeelement(
         self,
         _tag: _TagName,
         /,
-        attrib: SupportsLaxedItems[str, _AnyStr] | None = ...,
-        nsmap: _NSMapArg | None = ...,
+        attrib: SupportsLaxedItems[str, _AnyStr] | None = None,
+        nsmap: _NSMapArg | None = None,
         **_extra: _AnyStr,
     ) -> HtmlElement: ...
     def find(
-        self, path: _ElemPathArg, namespaces: _NSMapArg | None = ...
+        self, path: _ElemPathArg, namespaces: _NSMapArg | None = None
     ) -> HtmlElement | None: ...
     def findall(
-        self, path: _ElemPathArg, namespaces: _NSMapArg | None = ...
+        self, path: _ElemPathArg, namespaces: _NSMapArg | None = None
     ) -> list[HtmlElement]: ...
     def iterfind(
-        self, path: _ElemPathArg, namespaces: _NSMapArg | None = ...
+        self, path: _ElemPathArg, namespaces: _NSMapArg | None = None
     ) -> Iterator[HtmlElement]: ...
     def cssselect(
         self,
         expr: str,
         *,
-        translator: _CSSTransArg = ...,
+        translator: _CSSTransArg = "xml",
     ) -> list[HtmlElement]: ...
 
 #
 # HTML element class attribute
 #
 class Classes(MutableSet[str]):
     # Theorectically, the internal structure need not be _Attrib,
@@ -247,11 +259,11 @@
 
 #
 # Factory func, signature same as etree.Element
 #
 def Element(
     _tag: _TagName,
     /,
-    attrib: SupportsLaxedItems[str, _AnyStr] | None = ...,
-    nsmap: _NSMapArg | None = ...,
+    attrib: SupportsLaxedItems[str, _AnyStr] | None = None,
+    nsmap: _NSMapArg | None = None,
     **extra: _AnyStr,
 ) -> HtmlElement: ...
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/html/_form.pyi` & `types_lxml-2024.4.14/lxml-stubs/html/_form.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import sys
+from _typeshed import _T
 from typing import (
     Any,
     Callable,
     Collection,
     Iterable,
     Iterator,
+    Literal,
     MutableMapping,
     MutableSet,
+    overload,
 )
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:
     from typing_extensions import TypeAlias
 
@@ -137,17 +140,31 @@
 
 class LabelElement(HtmlElement):
     @property
     def for_element(self) -> HtmlElement | None: ...
     @for_element.setter
     def for_element(self, __v: HtmlElement) -> None: ...
 
+# open_http argument has signature (method, url, values) -> Any
+@overload
 def submit_form(
     form: FormElement,
-    extra_values: _FormValues | SupportsLaxedItems[str, str] | None = ...,
-    # open_http(method, url, values)
-    open_http: Callable[[str, str, _FormValues], Any] | None = ...,
-) -> Any: ...  # result depends on open_http callback used
+    extra_values: _FormValues | SupportsLaxedItems[str, str] | None = None,
+    open_http: None = None,
+) -> Any: ...  # See typeshed _UrlOpenRet
+@overload  # open_http as positional argument
+def submit_form(
+    form: FormElement,
+    extra_values: _FormValues | SupportsLaxedItems[str, str] | None,
+    open_http: Callable[[Literal["GET", "POST"], str, _FormValues], _T],
+) -> _T: ...
+@overload  # open_http as keyword argument
+def submit_form(
+    form: FormElement,
+    extra_values: _FormValues | SupportsLaxedItems[str, str] | None = None,
+    *,
+    open_http: Callable[[Literal["GET", "POST"], str, _FormValues], _T],
+) -> _T: ...
 
 # No need to annotate open_http_urllib.
 # Only intended as callback func object in submit_form() argument,
 # and already used as default if open_http argument is absent.
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/html/_funcs.pyi` & `types_lxml-2024.4.14/lxml-stubs/html/_funcs.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,13 @@
-import sys
 from typing import AnyStr, Callable, Iterator, Literal, TypeVar, overload
 
-if sys.version_info >= (3, 10):
-    from typing import TypeAlias
-else:
-    from typing_extensions import TypeAlias
-
-from .._types import _AnyStr, _OutputMethodArg
-from ..etree import _ElementTree
+from .._types import _AnyStr, _ElementOrTree, _OutputMethodArg
 from ._element import _HANDLE_FAILURES, HtmlElement
 
 _HtmlDoc_T = TypeVar("_HtmlDoc_T", str, bytes, HtmlElement)
-_HtmlElemOrTree: TypeAlias = HtmlElement | _ElementTree[HtmlElement]
 
 # These are HtmlMixin methods converted to standard functions,
 # with element or HTML string as first argument followed by all
 # pre-existing args. Quoting from source:
 #
 #   ... the function takes either an element or an HTML string.  It
 #   returns whatever the function normally returns, or if the function
@@ -60,61 +52,61 @@
     doc: _AnyStr,
     class_name: _AnyStr,
     /,
 ) -> list[HtmlElement]: ...
 @overload
 def make_links_absolute(
     doc: HtmlElement,
-    base_url: str | None = ...,
-    resolve_base_href: bool = ...,
-    handle_failures: _HANDLE_FAILURES | None = ...,
+    base_url: str | None = None,
+    resolve_base_href: bool = True,
+    handle_failures: _HANDLE_FAILURES | None = None,
 ) -> HtmlElement: ...
 @overload
 def make_links_absolute(
     doc: AnyStr,
-    base_url: str | None = ...,
-    resolve_base_href: bool = ...,
-    handle_failures: _HANDLE_FAILURES | None = ...,
+    base_url: str | None = None,
+    resolve_base_href: bool = True,
+    handle_failures: _HANDLE_FAILURES | None = None,
     /,
 ) -> AnyStr: ...
 @overload
 def resolve_base_href(
     doc: HtmlElement,
-    handle_failures: _HANDLE_FAILURES | None = ...,
+    handle_failures: _HANDLE_FAILURES | None = None,
 ) -> HtmlElement: ...
 @overload
 def resolve_base_href(
     doc: AnyStr,
-    handle_failures: _HANDLE_FAILURES | None = ...,
+    handle_failures: _HANDLE_FAILURES | None = None,
     /,
 ) -> AnyStr: ...
 def iterlinks(
     doc: _HtmlDoc_T,
 ) -> Iterator[tuple[HtmlElement, str | None, str, int]]: ...
 @overload
 def rewrite_links(
     doc: HtmlElement,
     link_repl_func: Callable[[str], str | None],
-    resolve_base_href: bool = ...,
-    base_href: str | None = ...,
+    resolve_base_href: bool = True,
+    base_href: str | None = None,
 ) -> HtmlElement: ...
 @overload
 def rewrite_links(
     doc: AnyStr,
     link_repl_func: Callable[[str], str | None],
-    resolve_base_href: bool = ...,
-    base_href: str | None = ...,
+    resolve_base_href: bool = True,
+    base_href: str | None = None,
     /,
 ) -> AnyStr: ...
 
 #
 # Tree conversion
 #
-def html_to_xhtml(html: _HtmlElemOrTree) -> None: ...
-def xhtml_to_html(xhtml: _HtmlElemOrTree) -> None: ...
+def html_to_xhtml(html: _ElementOrTree[HtmlElement]) -> None: ...
+def xhtml_to_html(xhtml: _ElementOrTree[HtmlElement]) -> None: ...
 
 #
 # Tree output
 #
 # 1. Encoding issue is similar to etree.tostring().
 #
 # 2. Unlike etree.tostring(), all arguments here are not explicitly
@@ -125,35 +117,35 @@
 #
 # 3. Although html.tostring() does not forbid method="c14n" (or c14n2),
 #    calling tostring() this way would render almost all keyword arguments
 #    useless, defeating the purpose of existence of html.tostring().
 #    Besides, no c14n specific arguments are accepted here, so it is
 #    better to let etree.tostring() handle C14N.
 @overload  # encoding=str / "unicode"
-def tostring(  # type: ignore[misc]
-    doc: _HtmlElemOrTree,
+def tostring(  # type: ignore[overload-overlap]
+    doc: _ElementOrTree[HtmlElement],
     *,
-    pretty_print: bool = ...,
-    include_meta_content_type: bool = ...,
+    pretty_print: bool = False,
+    include_meta_content_type: bool = False,
     encoding: type[str] | Literal["unicode"],
-    method: _OutputMethodArg = ...,
-    with_tail: bool = ...,
-    doctype: str | None = ...,
+    method: _OutputMethodArg = "html",
+    with_tail: bool = True,
+    doctype: str | None = None,
 ) -> str: ...
 @overload  # encoding="..." / None, no encoding arg
 def tostring(
-    doc: _HtmlElemOrTree,
+    doc: _ElementOrTree[HtmlElement],
     *,
-    pretty_print: bool = ...,
-    include_meta_content_type: bool = ...,
-    encoding: str | None = ...,
-    method: _OutputMethodArg = ...,
-    with_tail: bool = ...,
-    doctype: str | None = ...,
+    pretty_print: bool = False,
+    include_meta_content_type: bool = False,
+    encoding: str | None = None,
+    method: _OutputMethodArg = "html",
+    with_tail: bool = True,
+    doctype: str | None = None,
 ) -> bytes: ...
 
 #
 # Debug
 #
 def open_in_browser(
-    doc: _HtmlElemOrTree, encoding: str | type[str] | None = ...
+    doc: _ElementOrTree[HtmlElement], encoding: str | type[str] | None = None
 ) -> None: ...
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/html/_parse.pyi` & `types_lxml-2024.4.14/lxml-stubs/html/_parse.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,58 @@
 import sys
-from typing import Any, Iterable, MutableMapping
+from typing import Any, Iterable, Literal, MutableMapping, overload
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:
     from typing_extensions import TypeAlias
 
 from .. import etree
-from .._types import Unused, _AnyStr, _ElemClsLookupArg, _FileReadSource
+from .._types import (
+    Unused,
+    _AnyStr,
+    _DefEtreeParsers,
+    _ElemClsLookupArg,
+    _FileReadSource,
+)
 from ._element import HtmlElement
 
-_HtmlElemParser: TypeAlias = etree._parser._DefEtreeParsers[HtmlElement]
+_HtmlElemParser: TypeAlias = _DefEtreeParsers[HtmlElement]
 
 #
 # Parser
 #
 
 # Stub version before March 2023 used to omit 'target' parameter, which
 # would nullify default HTML element lookup behavior, degenerating html
 # submodule parsers into etree ones. Since it is decided to not support
-# custom target parser for now, we just add back 'target' parameter for
+# custom target parser for now, we just use superclass constructor for
 # coherence. Same for XHTMLParser below.
 class HTMLParser(etree.HTMLParser[HtmlElement]):
     """An HTML parser configured to return ``lxml.html`` Element
     objects.
 
     Notes
     -----
     This subclass is not specialized, unlike the ``etree`` counterpart.
     They are designed to always handle ``HtmlElement``;
     for generating other kinds of ``_Elements``, one should use
     etree parsers with ``set_element_class_lookup()`` method instead.
     In that case, see ``_FeedParser.set_element_class_lookup()`` for more info.
     """
 
-    def __init__(
-        self,
-        *,
-        encoding: _AnyStr | None = ...,
-        remove_blank_text: bool = ...,
-        remove_comments: bool = ...,
-        remove_pis: bool = ...,
-        strip_cdata: bool = ...,
-        no_network: bool = ...,
-        target: etree.ParserTarget[Any] | None = ...,
-        schema: etree.XMLSchema | None = ...,
-        recover: bool = ...,
-        compact: bool = ...,
-        default_doctype: bool = ...,
-        collect_ids: bool = ...,
-        huge_tree: bool = ...,
-    ) -> None: ...
     @property
     def target(self) -> None: ...
 
 class XHTMLParser(etree.XMLParser[HtmlElement]):
     """An XML parser configured to return ``lxml.html`` Element
     objects.
 
-    Notes
-    -----
+    Annotation
+    ----------
     This subclass is not specialized, unlike the ``etree`` counterpart.
     They are designed to always handle ``HtmlElement``;
     for generating other kinds of ``_Elements``, one should use
     etree parsers with ``set_element_class_lookup()`` method instead.
     In that case, see ``_FeedParser.set_element_class_lookup()`` for more info.
 
     Original doc
@@ -78,96 +67,77 @@
     If you additionally want to validate the document, use this::
 
         >>> parser = XHTMLParser(dtd_validation=True)
 
     For catalog support, see http://www.xmlsoft.org/catalog.html.
     """
 
-    def __init__(
-        self,
-        *,
-        encoding: _AnyStr | None = ...,
-        attribute_defaults: bool = ...,
-        dtd_validation: bool = ...,
-        load_dtd: bool = ...,
-        no_network: bool = ...,
-        target: etree.ParserTarget[Any] | None = ...,
-        ns_clean: bool = ...,
-        recover: bool = ...,
-        schema: etree.XMLSchema | None = ...,
-        huge_tree: bool = ...,
-        remove_blank_text: bool = ...,
-        resolve_entities: bool = ...,
-        remove_comments: bool = ...,
-        remove_pis: bool = ...,
-        strip_cdata: bool = ...,
-        collect_ids: bool = ...,
-        compact: bool = ...,
-    ) -> None: ...
     @property
     def target(self) -> None: ...
 
 html_parser: HTMLParser
 xhtml_parser: XHTMLParser
 
 #
 # Parsing funcs
 #
 
 # Calls etree.fromstring(html, parser, **kw) which has signature
 # fromstring(text, parser, *, base_url)
 def document_fromstring(
     html: _AnyStr,
-    parser: _HtmlElemParser | None = ...,
-    ensure_head_body: bool = ...,
+    parser: _HtmlElemParser | None = None,
+    ensure_head_body: bool = False,
     *,
-    base_url: str | None = ...,
+    base_url: str | None = None,
 ) -> HtmlElement: ...
-def fragments_fromstring(
+@overload
+def fragments_fromstring(  # type: ignore[overload-overlap]
     html: _AnyStr,
-    no_leading_text: bool = ...,
-    base_url: str | None = ...,
-    parser: _HtmlElemParser | None = ...,
-    **kw: Unused,
+    no_leading_text: Literal[True],
+    base_url: str | None = None,
+    parser: _HtmlElemParser | None = None,
 ) -> list[HtmlElement]: ...
+@overload
+def fragments_fromstring(
+    html: _AnyStr,
+    no_leading_text: bool = False,
+    base_url: str | None = None,
+    parser: _HtmlElemParser | None = None,
+) -> list[str | HtmlElement]: ...
 def fragment_fromstring(
     html: _AnyStr,
-    create_parent: bool = ...,
-    base_url: str | None = ...,
-    parser: _HtmlElemParser | None = ...,
-    **kw: Unused,
+    create_parent: bool = False,
+    base_url: str | None = None,
+    parser: _HtmlElemParser | None = None,
 ) -> HtmlElement: ...
 def fromstring(
     html: _AnyStr,
-    base_url: str | None = ...,
-    parser: _HtmlElemParser | None = ...,
-    **kw: Unused,
+    base_url: str | None = None,
+    parser: _HtmlElemParser | None = None,
 ) -> HtmlElement: ...
 def parse(
     filename_or_url: _FileReadSource,
-    parser: _HtmlElemParser | None = ...,
-    base_url: str | None = ...,
-    **kw: Unused,
+    parser: _HtmlElemParser | None = None,
+    base_url: str | None = None,
 ) -> etree._ElementTree[HtmlElement]: ...
 
 #
 # Element Lookup
 #
 
 class HtmlElementClassLookup(etree.CustomElementClassLookup):
     def __init__(
         self,
         # Should have been something like Mapping[str, type[HtmlElement]],
         # but unfortunately classes mapping is required to be mutable
-        classes: MutableMapping[str, Any] | None = ...,
+        classes: MutableMapping[str, Any] | None = None,
         # docstring says mixins is mapping, but implementation says otherwise
-        mixins: Iterable[tuple[str, type[HtmlElement]]] = ...,
+        mixins: Iterable[tuple[str, type[HtmlElement]]] | None = None,
     ) -> None: ...
-    # Both argument names and types are incompatible with base class
-    # This is a standard practise for lxml
     def lookup(  # pyright: ignore[reportIncompatibleMethodOverride]
         self,
         node_type: _ElemClsLookupArg | None,
         document: Unused,
         namespace: Unused,
         name: str,  # type: ignore[override]
     ) -> type[HtmlElement] | None: ...
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/html/builder.pyi` & `types_lxml-2024.4.14/lxml-stubs/html/builder.pyi`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/lxml-stubs/html/defs.pyi` & `types_lxml-2024.4.14/lxml-stubs/html/defs.pyi`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/lxml-stubs/html/html5parser.pyi` & `types_lxml-2024.4.14/lxml-stubs/html/html5parser.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 from ..etree import _Element, _ElementTree
 
 # Note that tree arg is dropped, because the sole purpose of using
 # this parser is to generate lxml element tree with html5lib parser.
 # Other arguments good for html5lib >= 1.0
 class HTMLParser(_html5lib.HTMLParser):
     def __init__(
-        self, strict: bool = ..., namespaceHTMLElements: bool = ..., debug: bool = ...
+        self,
+        strict: bool = False,
+        namespaceHTMLElements: bool = True,
+        debug: bool = False,
     ) -> None: ...
 
 html_parser: HTMLParser
 
 # Notes:
 # - No XHTMLParser here. Lxml tries to probe for some hypothetical
 #   XHTMLParser class in html5lib which had never existed.
@@ -31,15 +34,15 @@
 #   but not reflected here. (TODO or?)
 # - Although other types of parser _might_ be usable (after implementing
 #   parse() method, that is), such usage completely defeats the purpose of
 #   creating this submodule. It is intended for subclassing or
 #   init argument tweaking instead.
 
 def document_fromstring(
-    html: _AnyStr, guess_charset: bool | None = ..., parser: HTMLParser | None = ...
+    html: _AnyStr, guess_charset: bool | None = None, parser: HTMLParser | None = None
 ) -> _Element: ...
 @overload
 def fragments_fromstring(  # type: ignore
     html: _AnyStr,
     no_leading_text: Literal[True],
     guess_charset: bool | None = None,
     parser: HTMLParser | None = None,
@@ -51,22 +54,22 @@
     html: _AnyStr,
     no_leading_text: bool = False,
     guess_charset: bool | None = None,
     parser: HTMLParser | None = None,
 ) -> list[str | _Element]: ...
 def fragment_fromstring(
     html: _AnyStr,
-    create_parent: bool | _AnyStr = ...,
-    guess_charset: bool | None = ...,
-    parser: HTMLParser | None = ...,
+    create_parent: bool | _AnyStr = False,
+    guess_charset: bool | None = None,
+    parser: HTMLParser | None = None,
 ) -> _Element: ...
 def fromstring(
     html: _AnyStr,
-    guess_charset: bool | None = ...,
-    parser: HTMLParser | None = ...,
+    guess_charset: bool | None = None,
+    parser: HTMLParser | None = None,
 ) -> _Element: ...
 def parse(
     # html5lib doesn't support pathlib
     filename_url_or_file: _AnyStr | SupportsRead[bytes] | SupportsRead[str],
-    guess_charset: bool | None = ...,
-    parser: HTMLParser | None = ...,
-) -> _ElementTree[_Element]: ...
+    guess_charset: bool | None = None,
+    parser: HTMLParser | None = None,
+) -> _ElementTree: ...
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/objectify/__init__.pyi` & `types_lxml-2024.4.14/lxml-stubs/objectify/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/lxml-stubs/objectify/_annotate.pyi` & `types_lxml-2024.4.14/lxml-stubs/objectify/_annotate.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -46,24 +46,24 @@
     @property
     def stringify(self) -> Callable[[Any], str]: ...
     def __init__(
         self,
         name: _AnyStr,
         type_check: Callable[[Any], None] | None,
         type_class: type[ObjectifiedDataElement],
-        stringify: Callable[[Any], str] | None = ...,
+        stringify: Callable[[Any], str] | None = None,
     ) -> None: ...
     def register(
         self,
-        before: Iterable[str] | None = ...,
-        after: Iterable[str] | None = ...,
+        before: Iterable[str] | None = None,
+        after: Iterable[str] | None = None,
     ) -> None: ...
     def unregister(self) -> None: ...
 
-def set_pytype_attribute_tag(attribute_tag: str | None = ...) -> None:
+def set_pytype_attribute_tag(attribute_tag: str | None = None) -> None:
     """Change name and namespace of the XML attribute that holds Python
     type information
 
     Original Docstring
     ------------------
     Do not use this unless you know what you are doing.
 
@@ -93,17 +93,17 @@
     check functions, you can simply `register()` it, which will append it to the
     end of the type list.
     """
 
 def pyannotate(
     element_or_tree: _ElementOrTree,
     *,
-    ignore_old: bool = ...,
-    ignore_xsi: bool = ...,
-    empty_pytype: _AnyStr | None = ...,
+    ignore_old: bool = False,
+    ignore_xsi: bool = False,
+    empty_pytype: _AnyStr | None = None,
 ) -> None:
     """Recursively annotates elements of an XML tree with `py:pytype` attributes
 
     Parameters
     ----------
     element_or_tree: `_Element` or `_ElementTree`
         The XML Element or XML Tree to be precessed
@@ -119,17 +119,17 @@
         for example, to annotate them as string elements. Default is None,
         which means not to process empty elements at all.
     """
 
 def xsiannotate(
     element_or_tree: _ElementOrTree,
     *,
-    ignore_old: bool = ...,
-    ignore_pytype: bool = ...,
-    empty_type: _AnyStr | None = ...,
+    ignore_old: bool = False,
+    ignore_pytype: bool = False,
+    empty_type: _AnyStr | None = None,
 ) -> None:
     """Recursively annotates elements of an XML tree with `xsi:type` attributes
 
     Note that the mapping from Python types to XSI types is usually ambiguous.
     Currently, only the first XSI type name in the corresponding PyType
     definition will be used for annotation.  Thus, you should consider naming
     the widest type first if you define additional types.
@@ -151,20 +151,21 @@
         is None, which means not to process empty elements at all. In particular,
         `xsi:nil` attribute is not added.
     """
 
 def annotate(
     element_or_tree: _ElementOrTree,
     *,
-    ignore_old: bool = ...,
-    ignore_xsi: bool = ...,
-    empty_pytype: _AnyStr | None = ...,
-    empty_type: _AnyStr | None = ...,
-    annotate_xsi: bool = ...,
-    annotate_pytype: bool = ...,
+    ignore_old: bool = True,
+    ignore_xsi: bool = False,
+    empty_pytype: _AnyStr | None = None,
+    empty_type: _AnyStr | None = None,
+    # following arguments are typed 'bint' in source
+    annotate_xsi: bool = False,
+    annotate_pytype: bool = True,
 ) -> None:
     """Recursively annotates elements of an XML tree with `py:pytype`
     and/or `xsi:type` attributes
 
     Annotation notice
     -----------------
     This function serves as a basis of both `pyannotate()` and
@@ -200,18 +201,18 @@
         Determines if `py:pytype` annotations would be updated or created,
         default is yes (True).
     """
 
 def deannotate(
     element_or_tree: _ElementOrTree,
     *,
-    pytype: bool = ...,
-    xsi: bool = ...,
-    xsi_nil: bool = ...,
-    cleanup_namespaces: bool = ...,
+    pytype: bool = True,
+    xsi: bool = True,
+    xsi_nil: bool = False,
+    cleanup_namespaces: bool = False,
 ) -> None:
     """Recursively de-annotate elements of an XML tree
 
     This is achieved by removing `py:pytype`, `xsi:type` and/or `xsi:nil` attributes.
 
     Parameters
     ----------
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/objectify/_element.pyi` & `types_lxml-2024.4.14/lxml-stubs/objectify/_element.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     @property  # type: ignore[misc]
     def text(  # pyright: ignore[reportIncompatibleMethodOverride]
         self,
     ) -> str | None: ...
     # addattr() value is stringified before adding to attribute
     def addattr(self, tag: _TagName, value: object) -> None: ...
     def countchildren(self) -> int: ...
-    def descendantpaths(self, prefix: str | list[str] | None = ...) -> list[str]: ...
+    def descendantpaths(self, prefix: str | list[str] | None = None) -> list[str]: ...
     def getchildren(self) -> list[ObjectifiedElement]: ...
     def __iter__(self) -> Iterator[ObjectifiedElement]: ...
     def __reversed__(self) -> Iterator[ObjectifiedElement]: ...
     def __getattr__(self, __name: str) -> ObjectifiedElement: ...
     # Input data or list need not be DataElements. They are internally
     # converted to DataElement on-the-fly. Same for __setitem__ below.
     def __setattr__(self, __name: str, __value: object) -> None: ...
@@ -171,15 +171,15 @@
     def text(self) -> str: ...  # type: ignore[override]
     def __bool__(self) -> bool: ...
     def __int__(self) -> int: ...
     def __float__(self) -> float: ...
     # FIXME Unlike arbitrary floating point / integer powers,
     # power involving bool always have fixed results (0 or 1).
     # However, python maintainers have delved into some disgusting
-    # sort of "type annotation arithmatics" -- like
+    # sort of half-arsed "type annotation arithmatics":
     # - int**0  = Literal[1]
     # - int**25 = int
     # - int**26 = Any
     # - int**-20 = float
     # - int**-21 = Any
     # It isn't a wise decision spending time to construct overloads
     # matching that idiocy, so let's skip implementing __pow__ for
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/objectify/_factory.pyi` & `types_lxml-2024.4.14/lxml-stubs/objectify/_factory.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from . import _element as _e
 
 _DataElem_T = TypeVar("_DataElem_T", bound=_e.ObjectifiedDataElement)
 
 def Element(
     _tag: _TagName,
     /,
-    attrib: SupportsLaxedItems[str, _AnyStr] | None = ...,
-    nsmap: _NSMapArg | None = ...,
+    attrib: SupportsLaxedItems[str, _AnyStr] | None = None,
+    nsmap: _NSMapArg | None = None,
     *,
-    _pytype: str | None = ...,
+    _pytype: str | None = None,
     **__attr: _AnyStr,
 ) -> _e.ObjectifiedElement:
     """Objectify specific version of `lxml.etree` `Element()` factory
 
     Original Docstring
     ------------------
     Requires parser based element class lookup activated in `lxml.etree`!
@@ -43,154 +43,154 @@
         The generated element.
     """
 
 def SubElement(
     _parent: _e.ObjectifiedElement,
     _tag: _TagName,
     /,
-    attrib: SupportsLaxedItems[str, _AnyStr] | None = ...,
-    nsmap: _NSMapArg | None = ...,
+    attrib: SupportsLaxedItems[str, _AnyStr] | None = None,
+    nsmap: _NSMapArg | None = None,
     **__attr: _AnyStr,
 ) -> _e.ObjectifiedElement: ...
 
 # TODO Current overload situation is unsatisfactory. Will decide
 # whether the list should be trimmed or extended in future.
 #
 # XXX Order matters! float can't be listed before int
 #
 @overload  # DataElement retains same type if no other hint given
 def DataElement(
     _value: _DataElem_T,
     /,
-    attrib: SupportsLaxedItems[str, _AnyStr] | None = ...,
-    nsmap: _NSMapArg | None = ...,
+    attrib: SupportsLaxedItems[str, _AnyStr] | None = None,
+    nsmap: _NSMapArg | None = None,
     *,
-    _pytype: None = ...,
-    _xsi: None = ...,
+    _pytype: None = None,
+    _xsi: None = None,
     **__attr: _AnyStr,
 ) -> _DataElem_T: ...
 @overload  # native type None
 def DataElement(
     _value: None,
     /,
-    attrib: SupportsLaxedItems[str, _AnyStr] | None = ...,
-    nsmap: _NSMapArg | None = ...,
+    attrib: SupportsLaxedItems[str, _AnyStr] | None = None,
+    nsmap: _NSMapArg | None = None,
     *,
-    _pytype: None = ...,
-    _xsi: None = ...,
+    _pytype: None = None,
+    _xsi: None = None,
     **__attr: _AnyStr,
 ) -> _e.NoneElement: ...
 @overload  # native type str
 def DataElement(
     _value: str,
     /,
-    attrib: SupportsLaxedItems[str, _AnyStr] | None = ...,
-    nsmap: _NSMapArg | None = ...,
+    attrib: SupportsLaxedItems[str, _AnyStr] | None = None,
+    nsmap: _NSMapArg | None = None,
     *,
-    _pytype: None = ...,
-    _xsi: None = ...,
+    _pytype: None = None,
+    _xsi: None = None,
     **__attr: _AnyStr,
 ) -> _e.StringElement: ...
 @overload  # native type bool
 def DataElement(  # pyright: ignore[reportOverlappingOverload]
     _value: bool,
     /,
-    attrib: SupportsLaxedItems[str, _AnyStr] | None = ...,
-    nsmap: _NSMapArg | None = ...,
+    attrib: SupportsLaxedItems[str, _AnyStr] | None = None,
+    nsmap: _NSMapArg | None = None,
     *,
-    _pytype: None = ...,
-    _xsi: None = ...,
+    _pytype: None = None,
+    _xsi: None = None,
     **__attr: _AnyStr,
 ) -> _e.BoolElement: ...
 @overload  # native type int
 def DataElement(
     _value: int,
     /,
-    attrib: SupportsLaxedItems[str, _AnyStr] | None = ...,
-    nsmap: _NSMapArg | None = ...,
+    attrib: SupportsLaxedItems[str, _AnyStr] | None = None,
+    nsmap: _NSMapArg | None = None,
     *,
-    _pytype: None = ...,
-    _xsi: None = ...,
+    _pytype: None = None,
+    _xsi: None = None,
     **__attr: _AnyStr,
 ) -> _e.IntElement: ...
 @overload  # native type float
 def DataElement(
     _value: float,
     /,
-    attrib: SupportsLaxedItems[str, _AnyStr] | None = ...,
-    nsmap: _NSMapArg | None = ...,
+    attrib: SupportsLaxedItems[str, _AnyStr] | None = None,
+    nsmap: _NSMapArg | None = None,
     *,
-    _pytype: None = ...,
-    _xsi: None = ...,
+    _pytype: None = None,
+    _xsi: None = None,
     **__attr: _AnyStr,
 ) -> _e.FloatElement: ...
 @overload  # pytype None
 def DataElement(
     _value: object,
     /,
-    attrib: SupportsLaxedItems[str, _AnyStr] | None = ...,
-    nsmap: _NSMapArg | None = ...,
+    attrib: SupportsLaxedItems[str, _AnyStr] | None = None,
+    nsmap: _NSMapArg | None = None,
     *,
     _pytype: Literal["NoneType", "none"],
-    _xsi: str | None = ...,
+    _xsi: str | None = None,
     **__attr: _AnyStr,
 ) -> _e.NoneElement: ...
 @overload  # pytype str
 def DataElement(
     _value: object,
     /,
-    attrib: SupportsLaxedItems[str, _AnyStr] | None = ...,
-    nsmap: _NSMapArg | None = ...,
+    attrib: SupportsLaxedItems[str, _AnyStr] | None = None,
+    nsmap: _NSMapArg | None = None,
     *,
     _pytype: Literal["str"],
-    _xsi: str | None = ...,
+    _xsi: str | None = None,
     **__attr: _AnyStr,
 ) -> _e.StringElement: ...
 @overload  # pytype bool
 def DataElement(
     _value: object,
     /,
-    attrib: SupportsLaxedItems[str, _AnyStr] | None = ...,
-    nsmap: _NSMapArg | None = ...,
+    attrib: SupportsLaxedItems[str, _AnyStr] | None = None,
+    nsmap: _NSMapArg | None = None,
     *,
     _pytype: Literal["bool"],
-    _xsi: str | None = ...,
+    _xsi: str | None = None,
     **__attr: _AnyStr,
 ) -> _e.BoolElement: ...
 @overload  # pytype int
 def DataElement(
     _value: object,
     /,
-    attrib: SupportsLaxedItems[str, _AnyStr] | None = ...,
-    nsmap: _NSMapArg | None = ...,
+    attrib: SupportsLaxedItems[str, _AnyStr] | None = None,
+    nsmap: _NSMapArg | None = None,
     *,
     _pytype: Literal["int"],
-    _xsi: str | None = ...,
+    _xsi: str | None = None,
     **__attr: _AnyStr,
 ) -> _e.IntElement: ...
 @overload  # pytype float
 def DataElement(
     _value: object,
     /,
-    attrib: SupportsLaxedItems[str, _AnyStr] | None = ...,
-    nsmap: _NSMapArg | None = ...,
+    attrib: SupportsLaxedItems[str, _AnyStr] | None = None,
+    nsmap: _NSMapArg | None = None,
     *,
     _pytype: Literal["float"],
-    _xsi: str | None = ...,
+    _xsi: str | None = None,
     **__attr: _AnyStr,
 ) -> _e.FloatElement: ...
 @overload  # Generic fallback
 def DataElement(
     _value: object,
     /,
-    attrib: SupportsLaxedItems[str, _AnyStr] | None = ...,
-    nsmap: _NSMapArg | None = ...,
+    attrib: SupportsLaxedItems[str, _AnyStr] | None = None,
+    nsmap: _NSMapArg | None = None,
     *,
-    _pytype: str | None = ...,
-    _xsi: str | None = ...,
+    _pytype: str | None = None,
+    _xsi: str | None = None,
     **__attr: _AnyStr,
 ) -> _e.ObjectifiedElement:
     """Create a new element from a Python value and XML attributes taken
     from keyword arguments or a dictionary passed as second argument.
 
     Annotation notice
     -----------------
@@ -276,18 +276,18 @@
     some text
     ```
     """
 
     def __init__(
         self,
         *,
-        namespace: str | None = ...,
-        nsmap: _NSMapArg | None = ...,
-        annotate: bool = ...,
-        makeelement: _ElemFactory[_e.ObjectifiedElement] | None = ...,
+        namespace: str | None = None,
+        nsmap: _NSMapArg | None = None,
+        annotate: bool = True,
+        makeelement: _ElemFactory[_e.ObjectifiedElement] | None = None,
     ) -> None: ...
     def __call__(
         self,
         tag: str,
         *args: Any,
         **kwargs: Any,
     ) -> _e.ObjectifiedElement: ...
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/objectify/_misc.pyi` & `types_lxml-2024.4.14/lxml-stubs/objectify/_misc.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #
 # Parsing and other module level funcs
 #
 
 from _typeshed import _T
-from typing import Iterable, overload
+from typing import Iterable, Literal, TypeVar, overload
 
 from .. import etree
-from .._types import _ET, _AnyStr, _FileReadSource
+from .._types import _AnyStr, _DefEtreeParsers, _FileReadSource
 from ._element import ObjectifiedDataElement, ObjectifiedElement
 
 #
 # Dumping tree and class lookup
 #
 
 def enable_recursive_str(on: bool) -> None:
@@ -21,16 +21,16 @@
     """Return a recursively generated string representation of an element"""
 
 class ObjectifyElementClassLookup(etree.ElementClassLookup):
     """Element class lookup method that uses the objectify classes"""
 
     def __init__(
         self,
-        tree_class: type[ObjectifiedElement] | None = ...,
-        empty_data_class: type[ObjectifiedDataElement] | None = ...,
+        tree_class: type[ObjectifiedElement] | None = None,
+        empty_data_class: type[ObjectifiedDataElement] | None = None,
     ) -> None:
         """
         Parameters
         ----------
         tree_class : `type[ObjectifiedElement]`, optional
             Defines inner tree classes; it can be replaced by subclass of
             `ObjectifiedElement`. Default is None, which implies `ObjectifiedElement`.
@@ -43,61 +43,63 @@
 #
 # Parser and parsing
 #
 
 def set_default_parser(
     # Not joking, it uses isinstance check
     new_parser: etree.XMLParser[ObjectifiedElement]
-    | None = ...,
+    | None = None,
 ) -> None:
     """Replace the default parser used by objectify's `Element()`
     and `fromstring()` functions.
 
     Parameters
     ----------
     new_parser: `etree.XMLParser`, optional
         The new parser intended to replace the default one. If not
         specified, defaults to `None`, which means reverting to
         original parser.
     """
 
+# All XMLParser() arguments, except that remove_black_text
+# default value is True
 def makeparser(
     *,
-    encoding: _AnyStr | None = ...,
-    attribute_defaults: bool = ...,
-    dtd_validation: bool = ...,
-    load_dtd: bool = ...,
-    no_network: bool = ...,
-    ns_clean: bool = ...,
-    recover: bool = ...,
-    schema: etree.XMLSchema | None = ...,
-    huge_tree: bool = ...,
-    remove_blank_text: bool = ...,
-    resolve_entities: bool = ...,
-    remove_comments: bool = ...,
-    remove_pis: bool = ...,
-    strip_cdata: bool = ...,
-    collect_ids: bool = ...,
-    compact: bool = ...,
+    encoding: _AnyStr | None = None,
+    attribute_defaults: bool = False,
+    dtd_validation: bool = False,
+    load_dtd: bool = False,
+    no_network: bool = True,
+    ns_clean: bool = False,
+    recover: bool = False,
+    schema: etree.XMLSchema | None = None,
+    huge_tree: bool = False,
+    remove_blank_text: bool = True,
+    resolve_entities: bool | Literal["internal"] = "internal",
+    remove_comments: bool = False,
+    remove_pis: bool = False,
+    strip_cdata: bool = True,
+    collect_ids: bool = True,
+    compact: bool = True,
 ) -> etree.XMLParser[ObjectifiedElement]:
     """Create a new XML parser for objectify trees.
 
     Original Docstring
     ------------------
     You can pass all keyword arguments that are supported by
     `etree.XMLParser()`.  Note that this parser defaults to
     removing blank text.  You can disable this by passing the
     `remove_blank_text` boolean keyword option yourself.
     """
 
 def parse(
     source: _FileReadSource,
-    parser: etree._parser._DefEtreeParsers[ObjectifiedElement] | None = ...,
+    parser: _DefEtreeParsers[ObjectifiedElement] | None = None,
     *,
-    base_url: _AnyStr | None = ...,
+    base_url: _AnyStr | None = None,
 ) -> etree._ElementTree[ObjectifiedElement]:
     """Parse a file or file-like object with objectify parser
 
     Parameters
     ----------
     parser: `etree.XMLParser` or `etree.HTMLParser`, optional
         Using different parser is allowed. If not specified, default
@@ -107,17 +109,17 @@
         Allows setting a URL for the document when parsing from a file-like
         object. This is needed when looking up external entities
         (DTD, XInclude, ...) with relative paths.
     """
 
 def fromstring(
     xml: _AnyStr,
-    parser: etree._parser._DefEtreeParsers[ObjectifiedElement] | None = ...,
+    parser: _DefEtreeParsers[ObjectifiedElement] | None = None,
     *,
-    base_url: _AnyStr | None = ...,
+    base_url: _AnyStr | None = None,
 ) -> ObjectifiedElement:
     """Variant of corresponding `lxml.etree` function that uses objectify parser
 
     Parameters
     ----------
     parser: `etree.XMLParser` or `etree.HTMLParser`, optional
         Using different parser is allowed. If not specified, default
@@ -127,14 +129,20 @@
         Allows setting a URL for the document when parsing from a file-like
         object. This is needed when looking up external entities
         (DTD, XInclude, ...) with relative paths.
     """
 
 XML = fromstring
 
+# Not using ._types._ET, which supports PEP 696, but causes
+# problem in 2nd overload of ObjectPath.__call__()
+# if _ET has a default type, then all subsequent argument
+# typevars need default type too (namely, _default: _T)
+_ET = TypeVar("_ET", bound=etree._Element)
+
 #
 # ObjectPath -- only used within lxml.objectify
 # lxml's own invention that behaves somewhat like Element Path
 # https://lxml.de/objectify.html#objectpath
 #
 class ObjectPath:
     """`objectify`'s own path language
```

### Comparing `types-lxml-2024.3.27/lxml-stubs/sax.pyi` & `types_lxml-2024.4.14/lxml-stubs/sax.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from typing import Generic, overload
 from xml.sax.handler import ContentHandler
 
 from ._types import _ElementOrTree, _ElemFactory, _ET_co
-from .etree import LxmlError, _Element, _ElementTree
+from .etree import LxmlError, _ElementTree
 
 class SaxError(LxmlError): ...
 
 # Most annotation should be done in xml.sax.handler,
 # which is unannotated as of writing. Only properties and methods
 # not present in superclass are listed here.
 class ElementTreeContentHandler(Generic[_ET_co], ContentHandler):
     @overload
     def __new__(
         cls, makeelement: _ElemFactory[_ET_co]
     ) -> ElementTreeContentHandler[_ET_co]: ...
     @overload
-    def __new__(
-        cls, makeelement: None = ...
-    ) -> ElementTreeContentHandler[_Element]: ...
+    def __new__(cls, makeelement: None = None) -> ElementTreeContentHandler: ...
     @property
     def etree(self) -> _ElementTree[_ET_co]: ...
 
 class ElementTreeProducer:
     def __init__(
         self,
         element_or_tree: _ElementOrTree,
```

### Comparing `types-lxml-2024.3.27/pyproject.toml` & `types_lxml-2024.4.14/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 name = 'types-lxml'
 dynamic = ['version']
 description = 'Complete lxml external type annotation'
 readme = 'README.md'
 requires-python = '>=3.8'
 license = {text = 'Apache-2.0'}
 dependencies = [
-    'types-beautifulsoup4',
+    'types-beautifulsoup4 ~= 4.12',
     'typing_extensions ~= 4.5',
     'cssselect ~= 1.2'  # cssselect uses inline annotation
 ]
 keywords = ['lxml', 'typing', 'stubs', 'annotation']
 authors = [
     { name = 'Abel Cheung', email = 'abelcheung@gmail.com' }
 ]
@@ -35,21 +35,22 @@
 
 [project.urls]
 homepage = 'https://github.com/abelcheung/types-lxml'
 
 [project.optional-dependencies]
 test = [
     'tox ~= 4.0',
-    'mypy == 1.5.1',
+    'mypy == 1.9.*',
     'pyright >= 1.1.289',
     'typeguard >= 3.0, < 5',
     'pytest >= 7.0, < 9',
     'html5lib == 1.1',
-    'pytest-mypy-plugins ~= 1.10, != 1.10.0',
-    'lxml == 5.1.*',
+    'pytest-mypy-plugins == 1.11.1',
+    'lxml >= 4.9',
+    'beautifulsoup4 ~= 4.8'
 ]
 
 [tool.pdm.version]
 source = 'scm'
 
 [tool.pdm.build]
 includes = [
```

### Comparing `types-lxml-2024.3.27/test-rt/_testutils/common.py` & `types_lxml-2024.4.14/test-rt/_testutils/common.py`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-rt/_testutils/pyright_adapter.py` & `types_lxml-2024.4.14/test-rt/_testutils/pyright_adapter.py`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-rt/_testutils/rt_wrapper.py` & `types_lxml-2024.4.14/test-rt/_testutils/rt_wrapper.py`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-rt/conftest.py` & `types_lxml-2024.4.14/test-rt/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 import pytest
 import typeguard
 from _testutils import run_pyright_on
 from lxml.etree import (
     XMLParser,
     XMLSyntaxError,
-    _Element,
     _ElementTree,
     _ListErrorLog,
     fromstring,
 )
 from lxml.html import HtmlElement, parse
 
 typeguard.config.forward_ref_policy = typeguard.ForwardRefPolicy.ERROR
@@ -42,14 +41,19 @@
 
 @pytest.fixture
 def h2_filepath() -> Path:
     return Path(__file__).parent / "data" / "mdn-sample.html"
 
 
 @pytest.fixture
+def h2_fileuri(h2_filepath: Path) -> str:
+    return "file:///" + str(h2_filepath)
+
+
+@pytest.fixture
 def h2_str(h2_filepath: Path) -> str:
     return h2_filepath.read_text()
 
 
 @pytest.fixture
 def h2_bytes(h2_filepath: Path) -> bytes:
     return h2_filepath.read_bytes()
@@ -69,15 +73,15 @@
 def html_tree(h1_filepath: Path) -> _ElementTree[HtmlElement]:
     with open(h1_filepath, "r", encoding="utf-8") as f:
         tree = parse(f)
     return tree
 
 
 @pytest.fixture
-def xml_tree(x2_filepath: Path) -> _ElementTree[_Element]:
+def xml_tree(x2_filepath: Path) -> _ElementTree:
     with open(x2_filepath, "r", encoding="ascii") as f:
         tree = parse(f)
     return tree
 
 
 @pytest.fixture
 def xinc_sample_data(x2_filepath: Path) -> str:
```

### Comparing `types-lxml-2024.3.27/test-rt/data/sample.html` & `types_lxml-2024.4.14/test-rt/data/sample.html`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-rt/data/shiporder.xml` & `types_lxml-2024.4.14/test-rt/data/shiporder.xml`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-rt/data/shiporder.xsd` & `types_lxml-2024.4.14/test-rt/data/shiporder.xsd`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-rt/data/w3c-example.svg` & `types_lxml-2024.4.14/test-rt/data/w3c-example.svg`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-rt/test_attrib.py` & `types_lxml-2024.4.14/test-rt/test_attrib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import copy
 from typing import Any, cast
 
 import _testutils
 import pytest
-from lxml.etree import _Element, _ElementTree
+from lxml.etree import _ElementTree
 
 reveal_type = getattr(_testutils, "reveal_type_wrapper")
 
 
 class TestXmlAttrib:
-    def test_behavior(self, xml_tree: _ElementTree[_Element]) -> None:
+    def test_behavior(self, xml_tree: _ElementTree) -> None:
         e = copy.deepcopy(xml_tree.getroot())
         attrib = e.attrib
         reveal_type(len(attrib))
         attrib.update([("foo", "foo"), (b"bar", b"bar")])
         attrib.update({"foo": "foo", b"bar": b"bar"})
         for k in attrib:
             reveal_type(k)
```

### Comparing `types-lxml-2024.3.27/test-rt/test_elem_class_lookup.py` & `types_lxml-2024.4.14/test-rt/test_elem_class_lookup.py`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-rt/test_errorlog.py` & `types_lxml-2024.4.14/test-rt/test_errorlog.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
-import inspect
 import logging
+from inspect import Parameter, Signature, signature
 from typing import Any, cast
 
 import _testutils
 import pytest
 from lxml.etree import (
     LXML_VERSION,
     ErrorDomains,
@@ -79,41 +79,38 @@
         e0 = list_log[0]
         reveal_type(len(list_log))
         reveal_type(e0)
         reveal_type(e0 in list_log)
         for e in list_log:
             reveal_type(e)
 
-    def test_filter_domains(self, list_log: _ListErrorLog) -> None:
-        sig = inspect.signature(list_log.filter_domains)
-        param = list(sig.parameters.values())
-        assert len(param) == 1
-        assert param[0].name == "domains"
-        assert param[0].kind == inspect.Parameter.POSITIONAL_OR_KEYWORD
-        del sig, param
 
-        filtered = list_log.filter_domains([ErrorDomains.PARSER, ErrorDomains.DTD])
+class TestListLogMethods:
+    # fmt: off
+    @_testutils.signature_tester(_ListErrorLog.filter_domains, (
+        None,
+        ("domains", Parameter.POSITIONAL_OR_KEYWORD, Parameter.empty),
+    ))  # fmt: on
+    def test_filter_domains(self, list_log: _ListErrorLog) -> None:
+        filtered = list_log.filter_domains([ErrorDomains.XINCLUDE, ErrorDomains.DTD])
         reveal_type(filtered)
         del filtered
 
         filtered = list_log.filter_domains(ErrorDomains.PARSER)
         reveal_type(filtered)
         del filtered
 
         with pytest.raises(TypeError, match=r"argument .+ is not iterable"):
             _ = list_log.filter_domains(cast(Any, None))
 
+    @_testutils.signature_tester(_ListErrorLog.filter_levels, (
+        None,
+        ("levels", Parameter.POSITIONAL_OR_KEYWORD, Parameter.empty),
+    ))
     def test_filter_levels(self, list_log: _ListErrorLog) -> None:
-        sig = inspect.signature(list_log.filter_levels)
-        param = list(sig.parameters.values())
-        assert len(param) == 1
-        assert param[0].name == "levels"
-        assert param[0].kind == inspect.Parameter.POSITIONAL_OR_KEYWORD
-        del sig, param
-
         new_log = list_log.filter_levels(ErrorLevels.ERROR)
         reveal_type(new_log)
         del new_log
 
         if _method_no_kwarg():
             new_log = list_log.filter_levels([ErrorLevels.ERROR, ErrorLevels.FATAL])
         else:
@@ -122,61 +119,58 @@
             )
         reveal_type(new_log)
         del new_log
 
         with pytest.raises(TypeError, match=r"argument .+ is not iterable"):
             _ = list_log.filter_levels(cast(Any, None))
 
-    def test_filter_levels_shortcut(self, list_log: _ListErrorLog) -> None:
-        sig = inspect.signature(list_log.filter_from_level)
-        param = list(sig.parameters.values())
-        assert len(param) == 1
-        assert param[0].name == "level"
-        assert param[0].kind == inspect.Parameter.POSITIONAL_OR_KEYWORD
-        del sig, param
-
+    @_testutils.signature_tester(_ListErrorLog.filter_from_level, (
+        None,
+        ("level", Parameter.POSITIONAL_OR_KEYWORD, Parameter.empty),
+    ))
+    def test_filter_from_level(self, list_log: _ListErrorLog) -> None:
         if _method_no_kwarg():
             new_log = list_log.filter_from_level(ErrorLevels.NONE)
         else:
             new_log = list_log.filter_from_level(level=ErrorLevels.NONE)
         reveal_type(new_log)
         del new_log
 
-        assert inspect.signature(list_log.filter_from_errors) == inspect.Signature()
+        assert signature(list_log.filter_from_errors) == Signature()
         reveal_type(list_log.filter_from_errors())
 
-        assert inspect.signature(list_log.filter_from_fatals) == inspect.Signature()
+        assert signature(list_log.filter_from_fatals) == Signature()
         reveal_type(list_log.filter_from_fatals())
 
-        assert inspect.signature(list_log.filter_from_warnings) == inspect.Signature()
+        assert signature(list_log.filter_from_warnings) == Signature()
         reveal_type(list_log.filter_from_warnings())
 
+    # TODO implement filter_types test when enums are completed in stub
     # def test_filter_types(self, list_log: _ListErrorLog) -> None:
     # new_log = list_log.filter_types(ErrorTypes.???)
 
-    def test_other_methods(self, list_log: _ListErrorLog) -> None:
-        sig = inspect.signature(list_log.receive)
-        param = list(sig.parameters.values())
-        assert len(param) == 1
-        assert param[0].name == "entry"
-        assert param[0].kind == inspect.Parameter.POSITIONAL_OR_KEYWORD
-        del sig, param
-
+    @_testutils.signature_tester(_ListErrorLog.receive, (
+        None,
+        ("entry", Parameter.POSITIONAL_OR_KEYWORD, Parameter.empty),
+    ))
+    def test_receive(self, list_log: _ListErrorLog) -> None:
         if _method_no_kwarg():
             ret = list_log.receive(list_log[0])
         else:
             ret = list_log.receive(entry=list_log[0])
         reveal_type(ret)
         del ret
         with pytest.raises(TypeError, match=r"expected .+\._LogEntry, got int"):
             list_log.receive(cast(Any, 1))
 
-        # BEWARE: vanilla _ListErrorLog has no clear() method,
-        # thus can't be inspected
-        assert inspect.signature(list_log.copy) == inspect.Signature()
+    # BEWARE: vanilla _ListErrorLog has no clear() method,
+    # thus can't be inspected
+
+    def test_copy(self, list_log: _ListErrorLog) -> None:
+        assert signature(list_log.copy) == Signature()
         err_copy = list_log.copy()
         reveal_type(err_copy)
 
 
 class TestEmptyLog:
     # validate some methods and props works for empty log too
     def test_create_empty_log(self) -> None:
@@ -190,28 +184,22 @@
         with pytest.raises(IndexError, match="out of range"):
             _ = e[0]
         e_copy = e.copy()
         reveal_type(e_copy)
 
 
 class TestModuleFunc:
-
+    @_testutils.signature_tester(
+        use_global_python_log,
+        (("log", Parameter.POSITIONAL_OR_KEYWORD, Parameter.empty),),
+    )
     def test_sig(self) -> None:
-        sig = inspect.signature(clear_error_log)
-        param = list(sig.parameters.values())
-        assert len(param) == 0
-        del sig, param
-
-        sig = inspect.signature(use_global_python_log)
-        param = list(sig.parameters.values())
-        assert len(param) == 1
-        assert param[0].name == "log"
-        assert param[0].kind == inspect.Parameter.POSITIONAL_OR_KEYWORD
-        del sig, param
+        assert signature(clear_error_log) == Signature()
 
+    def test_global_log_usage(self) -> None:
         with pytest.raises(
             TypeError, match=r"expected lxml\.etree\.PyErrorLog, got int"
         ):
             use_global_python_log(cast(Any, 1))
 
         # exception if used after use_global_python_log
         clear_error_log()
```

### Comparing `types-lxml-2024.3.27/test-rt/test_html5lib.py` & `types_lxml-2024.4.14/test-rt/test_html5lib.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
-import inspect
+from inspect import Parameter
 from io import BytesIO, StringIO
 from pathlib import Path
-from typing import Any, Sequence, cast
+from typing import Any, cast
 
 import _testutils
 import lxml.html.html5parser as h5
 import pytest
 from lxml.etree import (
     HTMLParser as WrongParser,
     _Element as _Element,
@@ -15,35 +15,36 @@
 )
 from lxml.html.html5parser import HTMLParser
 
 reveal_type = getattr(_testutils, "reveal_type_wrapper")
 
 
 class TestParserConstruct:
-    def test_no_args(self) -> None:
+    def test_default_parser(self) -> None:
         reveal_type(h5.html_parser)
-        p = HTMLParser()
-        reveal_type(p)
+
+    # fmt: off
+    @_testutils.signature_tester(HTMLParser.__init__, (
+        None,
+        ("strict", Parameter.POSITIONAL_OR_KEYWORD, False          ),
+        ("kwargs", Parameter.VAR_KEYWORD          , Parameter.empty),
+    ))  # fmt: on
+    def test_func_sig(self) -> None:
+        pass
 
     @pytest.mark.parametrize(
         ("args", "kw"),
         [
+            pytest.param((), {}),
             pytest.param((False,), {}),
             pytest.param((), {"strict": True, "debug": True}),
             pytest.param((True,), {"namespaceHTMLElements": True}),
         ],
     )
     def test_good_args(self, args: tuple[Any], kw: dict[str, Any]) -> None:
-        sig = inspect.signature(HTMLParser.__init__)
-        param = list(sig.parameters.values())
-        assert len(param) == 3
-        assert param[1].name == "strict"
-        assert param[1].kind == inspect.Parameter.POSITIONAL_OR_KEYWORD
-        assert param[2].kind == inspect.Parameter.VAR_KEYWORD
-
         p = HTMLParser(*args, **kw)
         reveal_type(p)
 
     # Stub signature is pretty strict in order to promote cleaner code;
     # but the params are just truthy/falsy values in runtime, so no test
     # is imposed on them
     @pytest.mark.parametrize(
@@ -55,52 +56,42 @@
     )
     def test_bad_args(self, args: tuple[Any], kw: dict[str, Any]) -> None:
         with pytest.raises(TypeError):
             _ = HTMLParser(*args, **kw)
 
 
 class TestFromstringFamily:
-    @pytest.mark.parametrize(
-        ("funcname", "argname"),
-        [
-            # fmt: off
-            ("document_fromstring",
-                ("html", "guess_charset", "parser")),
-            ("fragments_fromstring",
-                ("html", "no_leading_text", "guess_charset", "parser")),
-            ("fragment_fromstring",
-                ("html", "create_parent", "guess_charset", "parser")),
-            ("fromstring",
-                ("html", "guess_charset", "parser")),
-            ("parse",
-                ("filename_url_or_file", "guess_charset", "parser")),
-            # fmt: on
-        ],
-    )
-    def test_func_sig(self, funcname: str, argname: Sequence[str]) -> None:
-        sig = inspect.signature(getattr(h5, funcname))
-        param = list(sig.parameters.values())
-        assert len(param) == len(argname)
-        for i in range(len(argname)):
-            assert param[i].name == argname[i]
-            assert param[i].kind == inspect.Parameter.POSITIONAL_OR_KEYWORD
-            if i:
-                assert param[i].default != inspect.Parameter.empty
-            else:
-                assert param[i].default is inspect.Parameter.empty
+    # fmt: off
+    @_testutils.signature_tester(h5.document_fromstring, (
+        ("html"         , Parameter.POSITIONAL_OR_KEYWORD, Parameter.empty),
+        ("guess_charset", Parameter.POSITIONAL_OR_KEYWORD, None           ),
+        ("parser"       , Parameter.POSITIONAL_OR_KEYWORD, None           ),
+    ))  # fmt: on
+    def test_d_fs_sig(self) -> None:
+        pass
 
     def test_d_fs_src(self, h2_str: str, h2_bytes: bytes) -> None:
         elem = h5.document_fromstring(h2_str)
         reveal_type(elem)
         del elem
 
         elem = h5.document_fromstring(h2_bytes)
         reveal_type(elem)
         del elem
 
+    # fmt: off
+    @_testutils.signature_tester(h5.fragments_fromstring, (
+        ("html"           , Parameter.POSITIONAL_OR_KEYWORD, Parameter.empty),
+        ("no_leading_text", Parameter.POSITIONAL_OR_KEYWORD, False          ),
+        ("guess_charset"  , Parameter.POSITIONAL_OR_KEYWORD, None           ),
+        ("parser"         , Parameter.POSITIONAL_OR_KEYWORD, None           ),
+    ))  # fmt: on
+    def test_fs_fs_sig(self) -> None:
+        pass
+
     def test_fs_fs_src(self) -> None:
         src_s: str = '<div><img src=""/></div><span>nothing</span>'
         src_b: bytes = src_s.encode()
 
         elems = h5.fragments_fromstring(src_s)
         reveal_type(elems)
         for elem in elems:
@@ -115,26 +106,46 @@
 
         elems = h5.fragments_fromstring(src_b, no_leading_text=True)
         reveal_type(elems)
         for elem in elems:
             reveal_type(elem)
         del elems
 
+    # fmt: off
+    @_testutils.signature_tester(h5.fragment_fromstring, (
+        ("html"         , Parameter.POSITIONAL_OR_KEYWORD, Parameter.empty),
+        ("create_parent", Parameter.POSITIONAL_OR_KEYWORD, False          ),
+        ("guess_charset", Parameter.POSITIONAL_OR_KEYWORD, None           ),
+        ("parser"       , Parameter.POSITIONAL_OR_KEYWORD, None           ),
+    ))  # fmt: on
+    def test_f_fs_sig(self) -> None:
+        pass
+
     def test_f_fs_src(self) -> None:
         src_s: str = "<span>nothing</span>"
         src_b: bytes = src_s.encode()
 
         elem = h5.fragment_fromstring(src_s)
         reveal_type(elem)
         del elem
 
         elem = h5.fragment_fromstring(src_b)
         reveal_type(elem)
         del elem
 
+    # fmt: off
+    @_testutils.signature_tester(h5.fromstring, (
+        ("html"         , Parameter.POSITIONAL_OR_KEYWORD, Parameter.empty),
+        ("guess_charset", Parameter.POSITIONAL_OR_KEYWORD, None           ),
+        ("parser"       , Parameter.POSITIONAL_OR_KEYWORD, None           ),
+    ))  # fmt: on
+    def test_fs_sig(self) -> None:
+        pass
+
+
     def test_fs_src(self, h2_str: str, h2_bytes: bytes) -> None:
         elem = h5.fromstring(h2_str)
         reveal_type(elem)
         del elem
 
         elem = h5.fromstring(h2_bytes)
         reveal_type(elem)
@@ -154,14 +165,24 @@
         fh = open(h2_filepath, "rb")
         for src in (None, sio, fh):
             with pytest.raises(TypeError, match="string required"):
                 func = getattr(h5, funcname)
                 _ = func(cast(Any, src))
         fh.close()
 
+    # fmt: off
+    @_testutils.signature_tester(h5.parse, (
+        ("filename_url_or_file", Parameter.POSITIONAL_OR_KEYWORD, Parameter.empty),
+        ("guess_charset"       , Parameter.POSITIONAL_OR_KEYWORD, None           ),
+        ("parser"              , Parameter.POSITIONAL_OR_KEYWORD, None           ),
+    ))  # fmt: on
+    def test_parse_sig(self) -> None:
+        pass
+
+
     def test_parse_src(self, h2_filepath: Path) -> None:
         with open(h2_filepath, "rb") as fh:
             tree = h5.parse(fh)
         reveal_type(tree)
         reveal_type(tree.getroot())
         del tree
 
@@ -262,15 +283,15 @@
         del elem
 
         b_io = BytesIO(h2_bytes)
         tree = h5.parse(b_io, guess_charset=False)
         reveal_type(tree)
         del tree
 
-    # XXX Should this belong to application logic and not the domain
+    # TODO Should this belong to application logic and not the domain
     # of type annotation?
     def test_conflict(self, h2_str: str) -> None:
         with pytest.raises(TypeError, match="unexpected keyword argument"):
             _ = h5.document_fromstring(h2_str, guess_charset=True)
 
         with pytest.raises(TypeError, match="unexpected keyword argument"):
             _ = h5.fragments_fromstring(h2_str, guess_charset=True)
```

### Comparing `types-lxml-2024.3.27/test-rt/test_html_link_funcs.py` & `types_lxml-2024.4.14/test-rt/test_html_link_funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,18 +233,16 @@
         def repl_func(orig: bytes) -> bytes:
             return orig.replace(b"http", b"ftp")
 
         with pytest.raises(TypeError, match="argument 1 must be str, not bytes"):
             _ = rewrite_links(h1_str, cast(Any, repl_func))
 
     #
-    # XXX lxml bug
-    # For standalone link funcs,
     # non-Element input + keyword args = Exception
-    # See html/_funcs.pyi for detail
+    # See comment on module level functions in html/_funcs.pyi
     #
 
     def test_bad_methodfunc(
         self,
         h1_str: str,
         h1_bytes: bytes,
         h1_filepath: Path,
```

### Comparing `types-lxml-2024.3.27/test-rt/test_iterparse.py` & `types_lxml-2024.4.14/test-rt/test_iterparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Any, cast
 
 import _testutils
 import pytest
-from lxml.etree import _Element, _ElementTree, iterparse, iterwalk
+from lxml.etree import _Element as _Element, _ElementTree, iterparse, iterwalk
 from lxml.html import HtmlElement
 
 reveal_type = getattr(_testutils, "reveal_type_wrapper")
 
 
 class TestIterwalk:
-    def test_xml_default_event(self, xml_tree: _ElementTree[_Element]) -> None:
+    def test_xml_default_event(self, xml_tree: _ElementTree) -> None:
         walker = iterwalk(xml_tree)
         reveal_type(walker)
         for event, elem in walker:
             reveal_type(event)
             reveal_type(elem)
 
-    def test_xml_more_event(self, xml_tree: _ElementTree[_Element]) -> None:
+    def test_xml_more_event(self, xml_tree: _ElementTree) -> None:
         walker = iterwalk(xml_tree, ["start", "end", "start-ns", "end-ns", "comment"])
         reveal_type(walker)
         # Generated values are not unpacked here to test type narrowing
         # See issue #19 for more info
         for item in walker:
             if item[0] == "start-ns":
                 reveal_type(item[1])
```

### Comparing `types-lxml-2024.3.27/test-stub/no-test-custom-target.yml` & `types_lxml-2024.4.14/test-stub/no-test-custom-target.yml`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-stub/test-annotations.yml` & `types_lxml-2024.4.14/test-stub/test-annotations.yml`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   main: |
     from lxml import etree as e
 
     def tree_root(tree: e._ElementTree[e._Element]) -> None:
         el = tree.getroot()
         reveal_type(el)  # N: Revealed type is "lxml.etree._element._Element"
 
-    def tree_is_generic(et: e._ElementTree) -> None:  # E: Missing type parameters for generic type "_ElementTree"  [type-arg]
+    def tree_is_generic(et: e._ElementTree) -> None:
         pass
 
     def tree_of_int(et: e._ElementTree[int]) -> None:  # E: Type argument "int" of "_ElementTree" must be a subtype of "_Element"  [type-var]
         pass
 
     def get_tree(el: e._Element) -> None:
         tree = e.ElementTree(el)
```

### Comparing `types-lxml-2024.3.27/test-stub/test-builder.yml` & `types_lxml-2024.4.14/test-stub/test-builder.yml`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-stub/test-classlookup.yml` & `types_lxml-2024.4.14/test-stub/test-classlookup.yml`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-stub/test-cssselect.yml` & `types_lxml-2024.4.14/test-stub/test-cssselect.yml`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-stub/test-dtd.yml` & `types_lxml-2024.4.14/test-stub/test-dtd.yml`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-stub/test-etree-element.yml` & `types_lxml-2024.4.14/test-stub/test-etree-element.yml`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-stub/test-etree-et.yml` & `types_lxml-2024.4.14/test-stub/test-etree-et.yml`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     et.{{ prop }} = et.{{ prop }}  # E: Property "{{ prop }}" defined in "_ElementTree" is read-only  [misc]
 
 - case: no_arg_or_return_methods
   main: |
     from lxml.etree import _ElementTree, _Element
     root: _Element
     et: _ElementTree[_Element]
-    r = et.xinclude()  # E: "xinclude" of "_ElementTree" does not return a value  [func-returns-value]
-    r = et._setroot(root)  # E: "_setroot" of "_ElementTree" does not return a value  [func-returns-value]
+    r = et.xinclude()  # E: "xinclude" of "_ElementTree" does not return a value (it only ever returns None)  [func-returns-value]
+    r = et._setroot(root)  # E: "_setroot" of "_ElementTree" does not return a value (it only ever returns None)  [func-returns-value]
     reveal_type(et.getroot())  # NR: .+ "[\w\.]+\._Element"$
     et._setroot(et)  # E: Argument 1 to "_setroot" of "_ElementTree" has incompatible type "_ElementTree[_Element]"; expected "_Element"  [arg-type]
 
 - case: no_arg_or_return_methods_toomanyargs
   parametrized:
     - method: xinclude
       kwds: None
@@ -294,17 +294,17 @@
     tree.write(file=fileio, method="c14n2", {{ kwds }})
 
 - case: write_other_methods
   parametrized:
     - kwds: "method='xml', encoding='ASCII'"
     - kwds: "method='html', encoding='utf8'"
     - kwds: "method='text', compression=2"
-    - kwds: "method='XML', doctype=None"
-    - kwds: "method='HTML', doctype=doctype"
-    - kwds: "method='TEXT', compression=None"
+    - kwds: "method='xml', doctype=None"
+    - kwds: "method='html', doctype=doctype"
+    - kwds: "method='text', compression=None"
     - kwds: "xml_declaration=True"
     - kwds: "with_tail=True"
     - kwds: "standalone=True"
     - kwds: "pretty_print=True"
   main: |
     from lxml import etree
     tree: etree._ElementTree
```

### Comparing `types-lxml-2024.3.27/test-stub/test-etree.yml` & `types_lxml-2024.4.14/test-stub/test-etree.yml`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-stub/test-html-clean.yml` & `types_lxml-2024.4.14/test-stub/test-html-clean.yml`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,15 @@
   parametrized:
     - func: autolink
     - func: word_break
   main: |
     from lxml.html.clean import autolink, word_break
     from lxml.html import HtmlElement
     root: HtmlElement
-    _ = {{ func }}(root)  # E: "{{ func }}" does not return a value  [func-returns-value]
+    _ = {{ func }}(root)  # E: "{{ func }}" does not return a value (it only ever returns None)  [func-returns-value]
 
 - case: inplace_funcs_badargs
   expect_fail: true
   parametrized:
     - func: autolink
       args: None
     - func: autolink
@@ -215,15 +215,15 @@
     s: str
     pattern = re.compile(s)
     link_re = [pattern, pattern]
     avoid_el = (s, s)
     avoid_hosts = (pattern, pattern)
     avoid_cls = {s, s}
     root: HtmlElement
-    _ = autolink(root, {{ args }})  # E: "autolink" does not return a value  [func-returns-value]
+    _ = autolink(root, {{ args }})  # E: "autolink" does not return a value (it only ever returns None)  [func-returns-value]
 
 - case: autolink_html_goodargs
   parametrized:
     - args: "html=s, link_regexes=link_re"
     - args: "s, link_re"
     - args: "s, avoid_elements=avoid_el"
     - args: "s, avoid_hosts=avoid_hosts"
@@ -246,15 +246,15 @@
     - args: "break_character='s'"
     - args: 40
   main: |
     from lxml.html.clean import word_break
     from lxml.html import HtmlElement
     avoid_cls = {'x', 'y'}
     root: HtmlElement
-    _ = word_break(root, {{ args }})  # E: "word_break" does not return a value  [func-returns-value]
+    _ = word_break(root, {{ args }})  # E: "word_break" does not return a value (it only ever returns None)  [func-returns-value]
 
 - case: word_break_html_goodargs
   parametrized:
     - args: "s, 40"
     - args: "s, max_width=40"
     - args: "html=s, avoid_classes=avoid_cls"
     - args: "s, break_character='x'"
```

### Comparing `types-lxml-2024.3.27/test-stub/test-html-element.yml` & `types_lxml-2024.4.14/test-stub/test-html-element.yml`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-stub/test-mypy-bug.yml` & `types_lxml-2024.4.14/test-stub/test-mypy-bug.yml`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-stub/test-nsclasses.yml` & `types_lxml-2024.4.14/test-stub/test-nsclasses.yml`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-stub/test-oe-element.yml` & `types_lxml-2024.4.14/test-stub/test-oe-element.yml`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,16 @@
     reveal_type(int(be))  # NR: .+ "[\w\.]+\.int"$
     reveal_type(float(be))  # NR: .+ "[\w\.]+\.float"$
     reveal_type(abs(be))  # NR: .+ "[\w\.]+\.int"$
     reveal_type(bool(be))  # NR: .+ "[\w\.]+\.bool"$
     reveal_type(-be)  # NR: .+ "[\w\.]+\.int"$
     reveal_type(~be)  # NR: .+ "[\w\.]+\.int"$
 
-    # __pow__() Temporarily removed in stub
+    # Not testing __pow__() and reverse operators,
+    # see bug #13
     # reveal_type(be ** b )  # NR .+ "Union\[.+]"$
     # reveal_type(be ** i )  # NR .+ "Union\[.+]"$
     # reveal_type(be ** f )  # NR .+ "[\w\.]+\.float"$
 
     reveal_type(be +  i )  # NR: .+ "[\w\.]+\.int"$
     reveal_type(be %  i )  # NR: .+ "[\w\.]+\.int"$
     reveal_type(i  -  be)  # NR: .+ "[\w\.]+\.int"$
@@ -245,8 +246,7 @@
 
     reveal_type(be &  i )  # NR: .+ "[\w\.]+\.int"$
     reveal_type(be >  i )  # NR: .+ "[\w\.]+\.bool"$
     reveal_type(i  >  be)  # NR: .+ "[\w\.]+\.bool"$
     reveal_type(i  ^  be)  # NR: .+ "[\w\.]+\.int"$
     reveal_type(be >= be)  # NR: .+ "[\w\.]+\.bool"$
     reveal_type(be |  be)  # NR: .+ "[\w\.]+\.bool"$
-    # TODO Reverse operations don't work for now
```

### Comparing `types-lxml-2024.3.27/test-stub/test-oe.yml` & `types_lxml-2024.4.14/test-stub/test-oe.yml`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-stub/test-resolver.yml` & `types_lxml-2024.4.14/test-stub/test-resolver.yml`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-stub/test-sax.yml` & `types_lxml-2024.4.14/test-stub/test-sax.yml`

 * *Files 5% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     from lxml.sax import ElementTreeProducer
     from xml.sax.handler import ContentHandler
     from lxml.etree import _Element, _ElementTree
     ch: ContentHandler
     et: _ElementTree[_Element]
     el: _Element
     p = ElementTreeProducer(el, ch)
-    _ = p.saxify()  # E: "saxify" of "ElementTreeProducer" does not return a value  [func-returns-value]
+    _ = p.saxify()  # E: "saxify" of "ElementTreeProducer" does not return a value (it only ever returns None)  [func-returns-value]
     p.saxify(1)  # E: Too many arguments for "saxify" of "ElementTreeProducer"  [call-arg]
 
 - case: saxify_func_goodargs
   parametrized:
     - args: el, ch
     - args: et, ch
     - args: el, content_handler=ch
@@ -98,15 +98,15 @@
     from xml.sax.handler import ContentHandler
     from lxml.sax import saxify
     from lxml.etree import _Element, _ElementTree
     class MyHandler(ContentHandler): ...
     ch: MyHandler
     et: _ElementTree[_Element]
     el: _Element
-    _ = saxify({{ args }})  # E: "saxify" does not return a value  [func-returns-value]
+    _ = saxify({{ args }})  # E: "saxify" does not return a value (it only ever returns None)  [func-returns-value]
 
 - case: saxify_func_badargs
   expect_fail: true
   parametrized:
     - args: el
     - args: et, ch, 1
     - args: el, ch, badarg=None
```

### Comparing `types-lxml-2024.3.27/test-stub/test-serializer.yml` & `types_lxml-2024.4.14/test-stub/test-serializer.yml`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-stub/test-validator.yml` & `types_lxml-2024.4.14/test-stub/test-validator.yml`

 * *Files 2% similar despite different names*

```diff
@@ -145,9 +145,9 @@
     - obj: rng
     - obj: dtd
     - obj: schema
     - obj: tron
   main: |
     from inc import rng, dtd, schema, tron, tree, elem
     reveal_type({{ obj }}.error_log)  # NR: .+ "[\w\.]+\._ListErrorLog"
-    _ = {{ obj }}.assertValid(tree)  # E: "assertValid" of "_Validator" does not return a value  [func-returns-value]
-    _ = {{ obj }}.assert_(elem)  # E: "assert_" of "_Validator" does not return a value  [func-returns-value]
+    _ = {{ obj }}.assertValid(tree)  # E: "assertValid" of "_Validator" does not return a value (it only ever returns None)  [func-returns-value]
+    _ = {{ obj }}.assert_(elem)  # E: "assert_" of "_Validator" does not return a value (it only ever returns None)  [func-returns-value]
```

### Comparing `types-lxml-2024.3.27/test-stub/test-xmlid.yml` & `types_lxml-2024.4.14/test-stub/test-xmlid.yml`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-stub/test-xpath.yml` & `types_lxml-2024.4.14/test-stub/test-xpath.yml`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/test-stub/test-xslt.yml` & `types_lxml-2024.4.14/test-stub/test-xslt.yml`

 * *Files identical despite different names*

### Comparing `types-lxml-2024.3.27/tox.ini` & `types_lxml-2024.4.14/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,65 @@
 [tox]
-env_list = py{38,39,310,311,312}-stub, py{310,311,312}-rt-lxml{49,50,51}
+env_list = py{38,39,310,311,312}-stub, py{310,311,312}-rt-lxml{49,50,51,52}
 requires =
     tox >= 4
 
 [gh-actions]
 python =
     3.8: py38
     3.9: py39
     3.10: py310
     3.11: py311
     3.12: py312
 
 [common_dep]
 deps =
-    types-beautifulsoup4
-    typing_extensions ~= 4.5
-    cssselect ~= 1.2
+    types-beautifulsoup4 == 4.12.0.20240229
+    typing_extensions == 4.11.0
+    cssselect == 1.2.0
 
 [stub_test_dep]
 deps =
     {[common_dep]deps}
-    mypy == 1.5.1
-    pytest-mypy-plugins ~= 1.10, != 1.10.0
+    mypy == 1.9.0
+    pytest-mypy-plugins == 1.11.1
 
 [testenv:py{38,39,310,311,312}-stub]
 deps = {[stub_test_dep]deps}
 commands =
     pytest --mypy-ini-file=test-stub/mypy-pytest.ini {posargs:test-stub}
 
-[testenv:py{310,311,312}-rt-lxml{49,50,51}]
+[testenv:py{310,311,312}-rt-lxml{49,50,51,52}]
 deps =
     {[testenv:pyright]deps}
-    typeguard >= 3.0, < 5
-    pytest >= 7.0, < 9
+    typeguard == 4.2.1
+    pytest == 8.1.1
     html5lib == 1.1
-    py{310,311,312}-rt-lxml49: lxml == 4.9.*
-    py{310,311,312}-rt-lxml50: lxml == 5.0.*
-    py{310,311,312}-rt-lxml51: lxml == 5.1.*
+    beautifulsoup4 == 4.12.3
+    py{310,311,312}-rt-lxml49: lxml == 4.9.4
+    py{310,311,312}-rt-lxml50: lxml == 5.0.2
+    py{310,311,312}-rt-lxml51: lxml == 5.1.1
+    py{310,311,312}-rt-lxml52: lxml == 5.2.1
 setenv =
     PYTHONUTF8 = 1
 commands =
     pyright --level error test-rt
     pytest {posargs:test-rt}
 
 [testenv:mypy]
 deps =
     {[common_dep]deps}
-    mypy >= 1.2, < 1.6
+    mypy == 1.9.0
 package = skip
 commands = mypy {posargs:lxml-stubs}
 
 [testenv:pyright]
 deps =
     {[common_dep]deps}
-    pyright >= 1.1.289
+    pyright == 1.1.358
 package = skip
 commands = pyright {posargs:lxml-stubs}
 
 [testenv:build]
 deps =
     build
 package = skip
```

### Comparing `types-lxml-2024.3.27/types_lxml.egg-info/SOURCES.txt` & `types_lxml-2024.4.14/types_lxml.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -58,22 +58,25 @@
 lxml-stubs/objectify/_annotate.pyi
 lxml-stubs/objectify/_element.pyi
 lxml-stubs/objectify/_factory.pyi
 lxml-stubs/objectify/_misc.pyi
 test-rt/__init__.py
 test-rt/conftest.py
 test-rt/test_attrib.py
+test-rt/test_beautifulsoup.py
+test-rt/test_constants.py
 test-rt/test_elem_class_lookup.py
 test-rt/test_errorlog.py
 test-rt/test_html5lib.py
 test-rt/test_html_link_funcs.py
 test-rt/test_iterparse.py
 test-rt/test_xinclude.py
 test-rt/_testutils/__init__.py
 test-rt/_testutils/common.py
+test-rt/_testutils/decorator.py
 test-rt/_testutils/pyright_adapter.py
 test-rt/_testutils/rt_wrapper.py
 test-rt/data/mdn-sample.html
 test-rt/data/sample.html
 test-rt/data/shiporder.xml
 test-rt/data/shiporder.xsd
 test-rt/data/w3c-example.svg
@@ -92,15 +95,14 @@
 test-stub/test-mypy-bug.yml
 test-stub/test-nsclasses.yml
 test-stub/test-oe-element.yml
 test-stub/test-oe.yml
 test-stub/test-resolver.yml
 test-stub/test-sax.yml
 test-stub/test-serializer.yml
-test-stub/test-soupparser.yml
 test-stub/test-validator.yml
 test-stub/test-xmlid.yml
 test-stub/test-xpath.yml
 test-stub/test-xslt.yml
 types_lxml.egg-info/PKG-INFO
 types_lxml.egg-info/SOURCES.txt
 types_lxml.egg-info/dependency_links.txt
```


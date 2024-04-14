# Comparing `tmp/frozendict-2.4.1.tar.gz` & `tmp/frozendict-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frozendict-2.4.1.tar", last modified: Sun Mar 31 22:01:37 2024, max compression
+gzip compressed data, was "frozendict-2.4.2.tar", last modified: Sun Apr 14 11:11:34 2024, max compression
```

## Comparing `frozendict-2.4.1.tar` & `frozendict-2.4.2.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.814202 frozendict-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-03-31 22:01:34.000000 frozendict-2.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-31 22:01:34.000000 frozendict-2.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    23320 2024-03-31 22:01:37.814202 frozendict-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22191 2024-03-31 22:01:34.000000 frozendict-2.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-31 22:01:34.000000 frozendict-2.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 22:01:37.814202 frozendict-2.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     6182 2024-03-31 22:01:34.000000 frozendict-2.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.794202 frozendict-2.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.802202 frozendict-2.4.1/src/frozendict/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/_frozendict_py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.798202 frozendict-2.4.1/src/frozendict/c_src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.802202 frozendict-2.4.1/src/frozendict/c_src/3_10/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.802202 frozendict-2.4.1/src/frozendict/c_src/3_10/Include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.802202 frozendict-2.4.1/src/frozendict/c_src/3_10/Include/cpython/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_10/Include/cpython/frozendictobject.h
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_10/Include/frozendictobject.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.802202 frozendict-2.4.1/src/frozendict/c_src/3_10/cpython_src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.802202 frozendict-2.4.1/src/frozendict/c_src/3_10/cpython_src/Objects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.802202 frozendict-2.4.1/src/frozendict/c_src/3_10/cpython_src/Objects/clinic/
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_10/cpython_src/Objects/clinic/dictobject.c.h
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_10/cpython_src/Objects/dict-common.h
--rw-r--r--   0 runner    (1001) docker     (127)    57234 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject.c
--rw-r--r--   0 runner    (1001) docker     (127)   152447 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject_original.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.806202 frozendict-2.4.1/src/frozendict/c_src/3_10/cpython_src/Objects/stringlib/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_10/cpython_src/Objects/stringlib/eq.h
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_10/cpython_src/other.c
--rw-r--r--   0 runner    (1001) docker     (127)    60336 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_10/frozendictobject.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.806202 frozendict-2.4.1/src/frozendict/c_src/3_6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.806202 frozendict-2.4.1/src/frozendict/c_src/3_6/Include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.806202 frozendict-2.4.1/src/frozendict/c_src/3_6/Include/cpython/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_6/Include/cpython/frozendictobject.h
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_6/Include/frozendictobject.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.806202 frozendict-2.4.1/src/frozendict/c_src/3_6/cpython_src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.806202 frozendict-2.4.1/src/frozendict/c_src/3_6/cpython_src/Objects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.806202 frozendict-2.4.1/src/frozendict/c_src/3_6/cpython_src/Objects/clinic/
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_6/cpython_src/Objects/clinic/dictobject.c.h
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_6/cpython_src/Objects/dict-common.h
--rw-r--r--   0 runner    (1001) docker     (127)    63009 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject.c
--rw-r--r--   0 runner    (1001) docker     (127)   135061 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject_original.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.806202 frozendict-2.4.1/src/frozendict/c_src/3_6/cpython_src/Objects/stringlib/
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_6/cpython_src/Objects/stringlib/eq.h
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_6/cpython_src/other.c
--rw-r--r--   0 runner    (1001) docker     (127)    58155 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_6/frozendictobject.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.806202 frozendict-2.4.1/src/frozendict/c_src/3_7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.806202 frozendict-2.4.1/src/frozendict/c_src/3_7/Include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.806202 frozendict-2.4.1/src/frozendict/c_src/3_7/Include/cpython/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_7/Include/cpython/frozendictobject.h
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_7/Include/frozendictobject.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.806202 frozendict-2.4.1/src/frozendict/c_src/3_7/cpython_src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.806202 frozendict-2.4.1/src/frozendict/c_src/3_7/cpython_src/Objects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.806202 frozendict-2.4.1/src/frozendict/c_src/3_7/cpython_src/Objects/clinic/
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_7/cpython_src/Objects/clinic/dictobject.c.h
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_7/cpython_src/Objects/dict-common.h
--rw-r--r--   0 runner    (1001) docker     (127)    61834 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject.c
--rw-r--r--   0 runner    (1001) docker     (127)   132228 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject_original.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.806202 frozendict-2.4.1/src/frozendict/c_src/3_7/cpython_src/Objects/stringlib/
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_7/cpython_src/Objects/stringlib/eq.h
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_7/cpython_src/other.c
--rw-r--r--   0 runner    (1001) docker     (127)    58478 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_7/frozendictobject.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.810202 frozendict-2.4.1/src/frozendict/c_src/3_8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.810202 frozendict-2.4.1/src/frozendict/c_src/3_8/Include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.810202 frozendict-2.4.1/src/frozendict/c_src/3_8/Include/cpython/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_8/Include/cpython/frozendictobject.h
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_8/Include/frozendictobject.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.810202 frozendict-2.4.1/src/frozendict/c_src/3_8/cpython_src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.810202 frozendict-2.4.1/src/frozendict/c_src/3_8/cpython_src/Objects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.810202 frozendict-2.4.1/src/frozendict/c_src/3_8/cpython_src/Objects/clinic/
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_8/cpython_src/Objects/clinic/dictobject.c.h
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_8/cpython_src/Objects/dict-common.h
--rw-r--r--   0 runner    (1001) docker     (127)    58062 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject.c
--rw-r--r--   0 runner    (1001) docker     (127)   141374 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject_original.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.810202 frozendict-2.4.1/src/frozendict/c_src/3_8/cpython_src/Objects/stringlib/
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_8/cpython_src/Objects/stringlib/eq.h
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_8/cpython_src/other.c
--rw-r--r--   0 runner    (1001) docker     (127)    60418 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_8/frozendictobject.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.810202 frozendict-2.4.1/src/frozendict/c_src/3_9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.810202 frozendict-2.4.1/src/frozendict/c_src/3_9/Include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.810202 frozendict-2.4.1/src/frozendict/c_src/3_9/Include/cpython/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_9/Include/cpython/frozendictobject.h
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_9/Include/frozendictobject.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.810202 frozendict-2.4.1/src/frozendict/c_src/3_9/cpython_src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.810202 frozendict-2.4.1/src/frozendict/c_src/3_9/cpython_src/Objects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.810202 frozendict-2.4.1/src/frozendict/c_src/3_9/cpython_src/Objects/clinic/
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_9/cpython_src/Objects/clinic/dictobject.c.h
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_9/cpython_src/Objects/dict-common.h
--rw-r--r--   0 runner    (1001) docker     (127)    58099 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject.c
--rw-r--r--   0 runner    (1001) docker     (127)   145558 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject_original.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.810202 frozendict-2.4.1/src/frozendict/c_src/3_9/cpython_src/Objects/stringlib/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_9/cpython_src/Objects/stringlib/eq.h
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_9/cpython_src/other.c
--rw-r--r--   0 runner    (1001) docker     (127)    60489 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/c_src/3_9/frozendictobject.c
--rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/cool.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/monkeypatch.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-31 22:01:34.000000 frozendict-2.4.1/src/frozendict/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.814202 frozendict-2.4.1/src/frozendict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23320 2024-03-31 22:01:37.000000 frozendict-2.4.1/src/frozendict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-03-31 22:01:37.000000 frozendict-2.4.1/src/frozendict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 22:01:37.000000 frozendict-2.4.1/src/frozendict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-31 22:01:37.000000 frozendict-2.4.1/src/frozendict.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:37.814202 frozendict-2.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 22:01:34.000000 frozendict-2.4.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-03-31 22:01:34.000000 frozendict-2.4.1/test/base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7607 2024-03-31 22:01:34.000000 frozendict-2.4.1/test/bench.py
--rw-r--r--   0 runner    (1001) docker     (127)    14874 2024-03-31 22:01:34.000000 frozendict-2.4.1/test/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13501 2024-03-31 22:01:34.000000 frozendict-2.4.1/test/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-03-31 22:01:34.000000 frozendict-2.4.1/test/frozendict_only.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-03-31 22:01:34.000000 frozendict-2.4.1/test/subclass_only.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-03-31 22:01:34.000000 frozendict-2.4.1/test/test_freeze.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-31 22:01:34.000000 frozendict-2.4.1/test/test_frozendict.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-31 22:01:34.000000 frozendict-2.4.1/test/test_frozendict_subclass.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1888 2024-03-31 22:01:34.000000 frozendict-2.4.1/test/typed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.442635 frozendict-2.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-14 11:11:29.000000 frozendict-2.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-14 11:11:29.000000 frozendict-2.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23320 2024-04-14 11:11:34.442635 frozendict-2.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22191 2024-04-14 11:11:29.000000 frozendict-2.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-14 11:11:29.000000 frozendict-2.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 11:11:34.442635 frozendict-2.4.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6182 2024-04-14 11:11:29.000000 frozendict-2.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.422636 frozendict-2.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.430636 frozendict-2.4.2/src/frozendict/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/_frozendict_py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.426636 frozendict-2.4.2/src/frozendict/c_src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.430636 frozendict-2.4.2/src/frozendict/c_src/3_10/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.430636 frozendict-2.4.2/src/frozendict/c_src/3_10/Include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.430636 frozendict-2.4.2/src/frozendict/c_src/3_10/Include/cpython/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_10/Include/cpython/frozendictobject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_10/Include/frozendictobject.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.430636 frozendict-2.4.2/src/frozendict/c_src/3_10/cpython_src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.430636 frozendict-2.4.2/src/frozendict/c_src/3_10/cpython_src/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.430636 frozendict-2.4.2/src/frozendict/c_src/3_10/cpython_src/Objects/clinic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_10/cpython_src/Objects/clinic/dictobject.c.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_10/cpython_src/Objects/dict-common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    57234 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject.c
+-rw-r--r--   0 runner    (1001) docker     (127)   152447 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject_original.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.430636 frozendict-2.4.2/src/frozendict/c_src/3_10/cpython_src/Objects/stringlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_10/cpython_src/Objects/stringlib/eq.h
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_10/cpython_src/other.c
+-rw-r--r--   0 runner    (1001) docker     (127)    60336 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_10/frozendictobject.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.430636 frozendict-2.4.2/src/frozendict/c_src/3_6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.434635 frozendict-2.4.2/src/frozendict/c_src/3_6/Include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.434635 frozendict-2.4.2/src/frozendict/c_src/3_6/Include/cpython/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_6/Include/cpython/frozendictobject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_6/Include/frozendictobject.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.434635 frozendict-2.4.2/src/frozendict/c_src/3_6/cpython_src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.434635 frozendict-2.4.2/src/frozendict/c_src/3_6/cpython_src/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.434635 frozendict-2.4.2/src/frozendict/c_src/3_6/cpython_src/Objects/clinic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_6/cpython_src/Objects/clinic/dictobject.c.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_6/cpython_src/Objects/dict-common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    63009 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject.c
+-rw-r--r--   0 runner    (1001) docker     (127)   135061 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject_original.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.434635 frozendict-2.4.2/src/frozendict/c_src/3_6/cpython_src/Objects/stringlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_6/cpython_src/Objects/stringlib/eq.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_6/cpython_src/other.c
+-rw-r--r--   0 runner    (1001) docker     (127)    58155 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_6/frozendictobject.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.434635 frozendict-2.4.2/src/frozendict/c_src/3_7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.434635 frozendict-2.4.2/src/frozendict/c_src/3_7/Include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.434635 frozendict-2.4.2/src/frozendict/c_src/3_7/Include/cpython/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_7/Include/cpython/frozendictobject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_7/Include/frozendictobject.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.434635 frozendict-2.4.2/src/frozendict/c_src/3_7/cpython_src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.434635 frozendict-2.4.2/src/frozendict/c_src/3_7/cpython_src/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.434635 frozendict-2.4.2/src/frozendict/c_src/3_7/cpython_src/Objects/clinic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_7/cpython_src/Objects/clinic/dictobject.c.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_7/cpython_src/Objects/dict-common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    61834 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject.c
+-rw-r--r--   0 runner    (1001) docker     (127)   132228 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject_original.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.434635 frozendict-2.4.2/src/frozendict/c_src/3_7/cpython_src/Objects/stringlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_7/cpython_src/Objects/stringlib/eq.h
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_7/cpython_src/other.c
+-rw-r--r--   0 runner    (1001) docker     (127)    58478 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_7/frozendictobject.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.434635 frozendict-2.4.2/src/frozendict/c_src/3_8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.434635 frozendict-2.4.2/src/frozendict/c_src/3_8/Include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.434635 frozendict-2.4.2/src/frozendict/c_src/3_8/Include/cpython/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_8/Include/cpython/frozendictobject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_8/Include/frozendictobject.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.434635 frozendict-2.4.2/src/frozendict/c_src/3_8/cpython_src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.438635 frozendict-2.4.2/src/frozendict/c_src/3_8/cpython_src/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.438635 frozendict-2.4.2/src/frozendict/c_src/3_8/cpython_src/Objects/clinic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_8/cpython_src/Objects/clinic/dictobject.c.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_8/cpython_src/Objects/dict-common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    58062 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject.c
+-rw-r--r--   0 runner    (1001) docker     (127)   141374 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject_original.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.438635 frozendict-2.4.2/src/frozendict/c_src/3_8/cpython_src/Objects/stringlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_8/cpython_src/Objects/stringlib/eq.h
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_8/cpython_src/other.c
+-rw-r--r--   0 runner    (1001) docker     (127)    60418 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_8/frozendictobject.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.438635 frozendict-2.4.2/src/frozendict/c_src/3_9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.438635 frozendict-2.4.2/src/frozendict/c_src/3_9/Include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.438635 frozendict-2.4.2/src/frozendict/c_src/3_9/Include/cpython/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_9/Include/cpython/frozendictobject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_9/Include/frozendictobject.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.438635 frozendict-2.4.2/src/frozendict/c_src/3_9/cpython_src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.438635 frozendict-2.4.2/src/frozendict/c_src/3_9/cpython_src/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.438635 frozendict-2.4.2/src/frozendict/c_src/3_9/cpython_src/Objects/clinic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_9/cpython_src/Objects/clinic/dictobject.c.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_9/cpython_src/Objects/dict-common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    58099 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject.c
+-rw-r--r--   0 runner    (1001) docker     (127)   145558 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject_original.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.438635 frozendict-2.4.2/src/frozendict/c_src/3_9/cpython_src/Objects/stringlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_9/cpython_src/Objects/stringlib/eq.h
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_9/cpython_src/other.c
+-rw-r--r--   0 runner    (1001) docker     (127)    60489 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/c_src/3_9/frozendictobject.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/cool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/monkeypatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-14 11:11:29.000000 frozendict-2.4.2/src/frozendict/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.442635 frozendict-2.4.2/src/frozendict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23320 2024-04-14 11:11:34.000000 frozendict-2.4.2/src/frozendict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-14 11:11:34.000000 frozendict-2.4.2/src/frozendict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 11:11:34.000000 frozendict-2.4.2/src/frozendict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-14 11:11:34.000000 frozendict-2.4.2/src/frozendict.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:34.438635 frozendict-2.4.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 11:11:29.000000 frozendict-2.4.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-14 11:11:29.000000 frozendict-2.4.2/test/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7607 2024-04-14 11:11:29.000000 frozendict-2.4.2/test/bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14874 2024-04-14 11:11:29.000000 frozendict-2.4.2/test/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13501 2024-04-14 11:11:29.000000 frozendict-2.4.2/test/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-14 11:11:29.000000 frozendict-2.4.2/test/frozendict_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-14 11:11:29.000000 frozendict-2.4.2/test/subclass_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-14 11:11:29.000000 frozendict-2.4.2/test/test_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-14 11:11:29.000000 frozendict-2.4.2/test/test_frozendict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-14 11:11:29.000000 frozendict-2.4.2/test/test_frozendict_subclass.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1888 2024-04-14 11:11:29.000000 frozendict-2.4.2/test/typed.py
```

### Comparing `frozendict-2.4.1/LICENSE.txt` & `frozendict-2.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/PKG-INFO` & `frozendict-2.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frozendict
-Version: 2.4.1
+Version: 2.4.2
 Summary: A simple immutable dictionary
 Home-page: https://github.com/Marco-Sulla/python-frozendict
 Author: Marco Sulla
 Author-email: marcosullaroma@gmail.com
 License: LGPL v3
 Project-URL: Bug Reports, https://github.com/Marco-Sulla/python-frozendict/issues
 Project-URL: Source, https://github.com/Marco-Sulla/python-frozendict
```

### Comparing `frozendict-2.4.1/README.md` & `frozendict-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/setup.py` & `frozendict-2.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/__init__.py` & `frozendict-2.4.2/src/frozendict/__init__.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/__init__.pyi` & `frozendict-2.4.2/src/frozendict/__init__.pyi`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/_frozendict_py.py` & `frozendict-2.4.2/src/frozendict/_frozendict_py.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 
 _empty_frozendict = None
 
 
 class frozendict(dict):
     r"""
     A simple immutable dictionary.
-    
-    The API is the same as `dict`, without methods that can change the 
+
+    The API is the same as `dict`, without methods that can change the
     immutability. In addition, it supports __hash__().
     """
     
     __slots__ = (
-        "_hash", 
+        "_hash",
     )
     
     @classmethod
     def fromkeys(cls, *args, **kwargs):
         r"""
         Identical to dict.fromkeys().
         """
@@ -54,15 +54,15 @@
             
             dict.__init__(self, *args, **kwargs)
             
             # empty singleton - start
             
             if self.__class__ == frozendict and not len(self):
                 global _empty_frozendict
-
+                
                 if _empty_frozendict is None:
                     _empty_frozendict = self
                 else:
                     self = _empty_frozendict
                     continue_creation = False
             
             # empty singleton - end
@@ -123,40 +123,40 @@
         See copy().
         """
         
         return self.copy()
     
     def __deepcopy__(self, memo, *args, **kwargs):
         r"""
-        As for tuples, if hashable, see copy(); otherwise, it returns a 
+        As for tuples, if hashable, see copy(); otherwise, it returns a
         deepcopy.
         """
         
         klass = self.__class__
         return_copy = klass == frozendict
         
         if return_copy:
             try:
                 hash(self)
             except TypeError:
                 return_copy = False
         
         if return_copy:
             return self.copy()
-            
+        
         tmp = deepcopy(dict(self))
         
         return klass(tmp)
     
     def __reduce__(self, *args, **kwargs):
         r"""
         Support for `pickle`.
         """
         
-        return (self.__class__, (dict(self), ))
+        return (self.__class__, (dict(self),))
     
     def set(self, key, val):
         new_self = deepcopy(dict(self))
         new_self[key] = val
         
         return self.__class__(new_self)
     
@@ -174,15 +174,15 @@
         new_self = deepcopy(dict(self))
         del new_self[key]
         
         if new_self:
             return self.__class__(new_self)
         
         return self.__class__()
-        
+    
     def _get_by_index(self, collection, index):
         try:
             return collection[index]
         except IndexError:
             maxindex = len(collection) - 1
             name = self.__class__.__name__
             raise IndexError(
@@ -230,19 +230,19 @@
 
 try:
     frozendict.__reversed__
 except AttributeError:
     def frozendict_reversed(self, *args, **kwargs):
         return reversed(tuple(self))
     
-    frozendict.__reversed__ = frozendict_reversed
     
+    frozendict.__reversed__ = frozendict_reversed
 
 frozendict.clear = immutable
 frozendict.pop = immutable
 frozendict.popitem = immutable
 frozendict.update = immutable
 frozendict.__delattr__ = immutable
 frozendict.__setattr__ = immutable
 frozendict.__module__ = 'frozendict'
 
-__all__ = (frozendict.__name__, )
+__all__ = (frozendict.__name__,)
```

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_10/Include/frozendictobject.h` & `frozendict-2.4.2/src/frozendict/c_src/3_10/Include/frozendictobject.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_10/cpython_src/Objects/clinic/dictobject.c.h` & `frozendict-2.4.2/src/frozendict/c_src/3_10/cpython_src/Objects/clinic/dictobject.c.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_10/cpython_src/Objects/dict-common.h` & `frozendict-2.4.2/src/frozendict/c_src/3_10/cpython_src/Objects/dict-common.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject.c` & `frozendict-2.4.2/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject_original.c` & `frozendict-2.4.2/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject_original.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_10/cpython_src/Objects/stringlib/eq.h` & `frozendict-2.4.2/src/frozendict/c_src/3_10/cpython_src/Objects/stringlib/eq.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_10/cpython_src/other.c` & `frozendict-2.4.2/src/frozendict/c_src/3_10/cpython_src/other.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_10/frozendictobject.c` & `frozendict-2.4.2/src/frozendict/c_src/3_10/frozendictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_6/Include/frozendictobject.h` & `frozendict-2.4.2/src/frozendict/c_src/3_6/Include/frozendictobject.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_6/cpython_src/Objects/clinic/dictobject.c.h` & `frozendict-2.4.2/src/frozendict/c_src/3_6/cpython_src/Objects/clinic/dictobject.c.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_6/cpython_src/Objects/dict-common.h` & `frozendict-2.4.2/src/frozendict/c_src/3_6/cpython_src/Objects/dict-common.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject.c` & `frozendict-2.4.2/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject_original.c` & `frozendict-2.4.2/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject_original.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_6/cpython_src/Objects/stringlib/eq.h` & `frozendict-2.4.2/src/frozendict/c_src/3_6/cpython_src/Objects/stringlib/eq.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_6/cpython_src/other.c` & `frozendict-2.4.2/src/frozendict/c_src/3_6/cpython_src/other.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_6/frozendictobject.c` & `frozendict-2.4.2/src/frozendict/c_src/3_6/frozendictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_7/Include/frozendictobject.h` & `frozendict-2.4.2/src/frozendict/c_src/3_7/Include/frozendictobject.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_7/cpython_src/Objects/clinic/dictobject.c.h` & `frozendict-2.4.2/src/frozendict/c_src/3_7/cpython_src/Objects/clinic/dictobject.c.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_7/cpython_src/Objects/dict-common.h` & `frozendict-2.4.2/src/frozendict/c_src/3_7/cpython_src/Objects/dict-common.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject.c` & `frozendict-2.4.2/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject_original.c` & `frozendict-2.4.2/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject_original.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_7/cpython_src/Objects/stringlib/eq.h` & `frozendict-2.4.2/src/frozendict/c_src/3_7/cpython_src/Objects/stringlib/eq.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_7/frozendictobject.c` & `frozendict-2.4.2/src/frozendict/c_src/3_7/frozendictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_8/Include/frozendictobject.h` & `frozendict-2.4.2/src/frozendict/c_src/3_8/Include/frozendictobject.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_8/cpython_src/Objects/clinic/dictobject.c.h` & `frozendict-2.4.2/src/frozendict/c_src/3_8/cpython_src/Objects/clinic/dictobject.c.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_8/cpython_src/Objects/dict-common.h` & `frozendict-2.4.2/src/frozendict/c_src/3_8/cpython_src/Objects/dict-common.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject.c` & `frozendict-2.4.2/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject_original.c` & `frozendict-2.4.2/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject_original.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_8/cpython_src/Objects/stringlib/eq.h` & `frozendict-2.4.2/src/frozendict/c_src/3_8/cpython_src/Objects/stringlib/eq.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_8/cpython_src/other.c` & `frozendict-2.4.2/src/frozendict/c_src/3_8/cpython_src/other.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_8/frozendictobject.c` & `frozendict-2.4.2/src/frozendict/c_src/3_8/frozendictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_9/Include/frozendictobject.h` & `frozendict-2.4.2/src/frozendict/c_src/3_9/Include/frozendictobject.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_9/cpython_src/Objects/clinic/dictobject.c.h` & `frozendict-2.4.2/src/frozendict/c_src/3_9/cpython_src/Objects/clinic/dictobject.c.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_9/cpython_src/Objects/dict-common.h` & `frozendict-2.4.2/src/frozendict/c_src/3_9/cpython_src/Objects/dict-common.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject.c` & `frozendict-2.4.2/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject_original.c` & `frozendict-2.4.2/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject_original.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_9/cpython_src/Objects/stringlib/eq.h` & `frozendict-2.4.2/src/frozendict/c_src/3_9/cpython_src/Objects/stringlib/eq.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_9/cpython_src/other.c` & `frozendict-2.4.2/src/frozendict/c_src/3_9/cpython_src/other.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/c_src/3_9/frozendictobject.c` & `frozendict-2.4.2/src/frozendict/c_src/3_9/frozendictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict/cool.py` & `frozendict-2.4.2/src/frozendict/cool.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,30 +276,30 @@
     if frozen_type:
         o = freeze_conversion_inverse_map[base_type_o](o)
     
     from copy import copy
     
     o_copy = copy(o)
     
-    for k, v in getItems(o)(o_copy):
-        o[k] = deepfreeze(
+    for k, v in getItems(o_copy)(o_copy):
+        o_copy[k] = deepfreeze(
             v,
             custom_converters = custom_converters,
             custom_inverse_converters = custom_inverse_converters
         )
     
     try:
         freeze = freeze_conversion_map[base_type_o]
     except KeyError:
         if frozen_type:
             freeze = type_o
         else:
             raise
     
-    return freeze(o)
+    return freeze(o_copy)
 
 
 __all__ = (
     deepfreeze.__name__, 
     register.__name__, 
     unregister.__name__, 
     getFreezeConversionMap.__name__,
```

### Comparing `frozendict-2.4.1/src/frozendict/monkeypatch.py` & `frozendict-2.4.2/src/frozendict/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/src/frozendict.egg-info/PKG-INFO` & `frozendict-2.4.2/src/frozendict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frozendict
-Version: 2.4.1
+Version: 2.4.2
 Summary: A simple immutable dictionary
 Home-page: https://github.com/Marco-Sulla/python-frozendict
 Author: Marco Sulla
 Author-email: marcosullaroma@gmail.com
 License: LGPL v3
 Project-URL: Bug Reports, https://github.com/Marco-Sulla/python-frozendict/issues
 Project-URL: Source, https://github.com/Marco-Sulla/python-frozendict
```

### Comparing `frozendict-2.4.1/src/frozendict.egg-info/SOURCES.txt` & `frozendict-2.4.2/src/frozendict.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/test/base.py` & `frozendict-2.4.2/test/base.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/test/bench.py` & `frozendict-2.4.2/test/bench.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/test/common.py` & `frozendict-2.4.2/test/common.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/test/debug.py` & `frozendict-2.4.2/test/debug.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/test/frozendict_only.py` & `frozendict-2.4.2/test/frozendict_only.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/test/subclass_only.py` & `frozendict-2.4.2/test/subclass_only.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/test/test_freeze.py` & `frozendict-2.4.2/test/test_freeze.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,8 +177,18 @@
     assert isinstance(
         cool.deepfreeze(
             [FrozenSeqA((0, 1, 2))],
             custom_converters={FrozenSeqA: FrozenSeqB},
             custom_inverse_converters={FrozenSeqA: MutableSeq}
             )[0],
         FrozenSeqB
-        )
+        )
+
+def test_original_immutate():
+    unfrozen = {
+        "int": 1,
+        "nested": {"int": 1},
+    }
+
+    frozen = cool.deepfreeze(unfrozen)
+    
+    assert type(unfrozen["nested"]) is dict
```

### Comparing `frozendict-2.4.1/test/test_frozendict_subclass.py` & `frozendict-2.4.2/test/test_frozendict_subclass.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.1/test/typed.py` & `frozendict-2.4.2/test/typed.py`

 * *Files identical despite different names*


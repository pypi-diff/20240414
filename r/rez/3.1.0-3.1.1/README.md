# Comparing `tmp/rez-3.1.0.tar.gz` & `tmp/rez-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rez-3.1.0.tar", last modified: Sat Mar 30 16:27:16 2024, max compression
+gzip compressed data, was "rez-3.1.1.tar", last modified: Sun Apr 14 19:41:45 2024, max compression
```

## Comparing `rez-3.1.0.tar` & `rez-3.1.1.tar`

### file list

```diff
@@ -1,924 +1,929 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.867523 rez-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10176 2024-03-30 16:27:13.000000 rez-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-30 16:27:13.000000 rez-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13050 2024-03-30 16:27:16.867523 rez-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11864 2024-03-30 16:27:13.000000 rez-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-30 16:27:13.000000 rez-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 16:27:16.871523 rez-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-03-30 16:27:13.000000 rez-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.751522 rez-3.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.759522 rez-3.1.0/src/rez/
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.763522 rez-3.1.0/src/rez/bind/
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/bind/PyQt.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/bind/PySide.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/bind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/bind/_pymodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/bind/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/bind/arch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/bind/cmake.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/bind/gcc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/bind/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/bind/os.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/bind/pip.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/bind/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/bind/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/bind/rez.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/bind/rezgui.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/bind/setuptools.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/bind/sip.py
--rw-r--r--   0 runner    (1001) docker     (127)    17062 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/build_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    12103 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/build_system.py
--rw-r--r--   0 runner    (1001) docker     (127)    11755 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/bundle_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.771522 rez-3.1.0/src/rez/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/_complete_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10594 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/complete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/cp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/depends.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)    10300 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/forward.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/help.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/interpret.py
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/memcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/mv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/pip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/pkg-cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/pkg-ignore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/release.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/selftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/cli/yaml2py.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.771522 rez-3.1.0/src/rez/completion/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/completion/complete.csh
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/completion/complete.sh
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/completion/complete.zsh
--rw-r--r--   0 runner    (1001) docker     (127)    36899 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.727522 rez-3.1.0/src/rez/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.775523 rez-3.1.0/src/rez/data/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (127)   828630 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/benchmarking/packages.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)   194231 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/benchmarking/requests.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.743522 rez-3.1.0/src/rez/data/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.775523 rez-3.1.0/src/rez/data/tests/bind/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/bind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/bind/os.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.727522 rez-3.1.0/src/rez/data/tests/builds/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.731522 rez-3.1.0/src/rez/data/tests/builds/packages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.727522 rez-3.1.0/src/rez/data/tests/builds/packages/anti/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.775523 rez-3.1.0/src/rez/data/tests/builds/packages/anti/1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/anti/1.0.0/build.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/anti/1.0.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.727522 rez-3.1.0/src/rez/data/tests/builds/packages/bah/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.775523 rez-3.1.0/src/rez/data/tests/builds/packages/bah/2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.775523 rez-3.1.0/src/rez/data/tests/builds/packages/bah/2.1/bah/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/bah/2.1/bah/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/bah/2.1/build.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/bah/2.1/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.727522 rez-3.1.0/src/rez/data/tests/builds/packages/build_util/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.775523 rez-3.1.0/src/rez/data/tests/builds/packages/build_util/1/
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/build_util/1/build.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.775523 rez-3.1.0/src/rez/data/tests/builds/packages/build_util/1/build_util/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/build_util/1/build_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/build_util/1/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.775523 rez-3.1.0/src/rez/data/tests/builds/packages/floob/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/floob/build.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.775523 rez-3.1.0/src/rez/data/tests/builds/packages/floob/floob/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/floob/floob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/floob/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.731522 rez-3.1.0/src/rez/data/tests/builds/packages/foo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.775523 rez-3.1.0/src/rez/data/tests/builds/packages/foo/1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/foo/1.0.0/build.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.775523 rez-3.1.0/src/rez/data/tests/builds/packages/foo/1.0.0/foo/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/foo/1.0.0/foo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/foo/1.0.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.775523 rez-3.1.0/src/rez/data/tests/builds/packages/foo/1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/foo/1.1.0/build.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.775523 rez-3.1.0/src/rez/data/tests/builds/packages/foo/1.1.0/foo/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/foo/1.1.0/foo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/foo/1.1.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.731522 rez-3.1.0/src/rez/data/tests/builds/packages/hello/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.779523 rez-3.1.0/src/rez/data/tests/builds/packages/hello/1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/hello/1.0/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.779523 rez-3.1.0/src/rez/data/tests/builds/packages/hello/1.0/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/hello/1.0/lib/main.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/hello/1.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.731522 rez-3.1.0/src/rez/data/tests/builds/packages/loco/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.779523 rez-3.1.0/src/rez/data/tests/builds/packages/loco/3/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/loco/3/build.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/loco/3/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.731522 rez-3.1.0/src/rez/data/tests/builds/packages/sup_world/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.779523 rez-3.1.0/src/rez/data/tests/builds/packages/sup_world/3.8/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/sup_world/3.8/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.779523 rez-3.1.0/src/rez/data/tests/builds/packages/sup_world/3.8/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/sup_world/3.8/lib/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/sup_world/3.8/lib/spanish_greet.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/sup_world/3.8/lib/spanish_greet.h
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/sup_world/3.8/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.779523 rez-3.1.0/src/rez/data/tests/builds/packages/sup_world/3.8/util/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/sup_world/3.8/util/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/sup_world/3.8/util/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.731522 rez-3.1.0/src/rez/data/tests/builds/packages/translate_lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.779523 rez-3.1.0/src/rez/data/tests/builds/packages/translate_lib/2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/translate_lib/2.2.0/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.779523 rez-3.1.0/src/rez/data/tests/builds/packages/translate_lib/2.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/translate_lib/2.2.0/docs/a spaced document
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/translate_lib/2.2.0/docs/an_unspaced_document
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/translate_lib/2.2.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.779523 rez-3.1.0/src/rez/data/tests/builds/packages/translate_lib/2.2.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/translate_lib/2.2.0/src/lolTranslator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/translate_lib/2.2.0/src/lolTranslator.h
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/translate_lib/2.2.0/src/spanishTranslator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/translate_lib/2.2.0/src/spanishTranslator.h
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/translate_lib/2.2.0/src/translator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/translate_lib/2.2.0/src/translator.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.779523 rez-3.1.0/src/rez/data/tests/builds/packages/whack/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/whack/build.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/builds/packages/whack/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.731522 rez-3.1.0/src/rez/data/tests/commands/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.731522 rez-3.1.0/src/rez/data/tests/commands/packages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.731522 rez-3.1.0/src/rez/data/tests/commands/packages/rextest/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.783522 rez-3.1.0/src/rez/data/tests/commands/packages/rextest/1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/commands/packages/rextest/1.1/package.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.783522 rez-3.1.0/src/rez/data/tests/commands/packages/rextest/1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/commands/packages/rextest/1.2/package.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.783522 rez-3.1.0/src/rez/data/tests/commands/packages/rextest/1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/commands/packages/rextest/1.3/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.731522 rez-3.1.0/src/rez/data/tests/commands/packages/rextest2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.783522 rez-3.1.0/src/rez/data/tests/commands/packages/rextest2/2/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/commands/packages/rextest2/2/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.783522 rez-3.1.0/src/rez/data/tests/config/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/config/package.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/config/test1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/config/test2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.731522 rez-3.1.0/src/rez/data/tests/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.783522 rez-3.1.0/src/rez/data/tests/extensions/bar/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/extensions/bar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.783522 rez-3.1.0/src/rez/data/tests/extensions/bar/rezplugins/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/extensions/bar/rezplugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.783522 rez-3.1.0/src/rez/data/tests/extensions/bar/rezplugins/package_repository/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/extensions/bar/rezplugins/package_repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/extensions/bar/rezplugins/package_repository/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.783522 rez-3.1.0/src/rez/data/tests/extensions/foo/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/extensions/foo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.783522 rez-3.1.0/src/rez/data/tests/extensions/foo/rezplugins/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/extensions/foo/rezplugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.783522 rez-3.1.0/src/rez/data/tests/extensions/foo/rezplugins/package_repository/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/extensions/foo/rezplugins/package_repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/extensions/foo/rezplugins/package_repository/cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.735522 rez-3.1.0/src/rez/data/tests/extensions/non-mod/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.783522 rez-3.1.0/src/rez/data/tests/extensions/non-mod/rezplugins/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/extensions/non-mod/rezplugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.783522 rez-3.1.0/src/rez/data/tests/extensions/non-mod/rezplugins/package_repository/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/extensions/non-mod/rezplugins/package_repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/extensions/non-mod/rezplugins/package_repository/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.735522 rez-3.1.0/src/rez/data/tests/packages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.783522 rez-3.1.0/src/rez/data/tests/packages/developer/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/developer/package.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.783522 rez-3.1.0/src/rez/data/tests/packages/developer_changed/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/developer_changed/package.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.783522 rez-3.1.0/src/rez/data/tests/packages/developer_dynamic_global_preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/developer_dynamic_global_preprocess/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.783522 rez-3.1.0/src/rez/data/tests/packages/developer_dynamic_local_preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/developer_dynamic_local_preprocess/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.783522 rez-3.1.0/src/rez/data/tests/packages/developer_dynamic_local_preprocess_additive/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/developer_dynamic_local_preprocess_additive/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.787522 rez-3.1.0/src/rez/data/tests/packages/developer_novar/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/developer_novar/package.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.787522 rez-3.1.0/src/rez/data/tests/packages/developer_novar_changed/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/developer_novar_changed/package.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.787522 rez-3.1.0/src/rez/data/tests/packages/py_packages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.787522 rez-3.1.0/src/rez/data/tests/packages/py_packages/empty/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/py_packages/empty/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.735522 rez-3.1.0/src/rez/data/tests/packages/py_packages/late_binding/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.787522 rez-3.1.0/src/rez/data/tests/packages/py_packages/late_binding/1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/py_packages/late_binding/1.0/package.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/py_packages/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/py_packages/single_unversioned.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/py_packages/single_versioned.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.735522 rez-3.1.0/src/rez/data/tests/packages/py_packages/timestamped/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.787522 rez-3.1.0/src/rez/data/tests/packages/py_packages/timestamped/1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/py_packages/timestamped/1.0.5/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.787522 rez-3.1.0/src/rez/data/tests/packages/py_packages/timestamped/1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/py_packages/timestamped/1.0.6/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.787522 rez-3.1.0/src/rez/data/tests/packages/py_packages/timestamped/1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/py_packages/timestamped/1.1.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.787522 rez-3.1.0/src/rez/data/tests/packages/py_packages/timestamped/1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/py_packages/timestamped/1.1.1/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.787522 rez-3.1.0/src/rez/data/tests/packages/py_packages/timestamped/1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/py_packages/timestamped/1.2.0/package.py
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/py_packages/timestamped/1.2.0/stuff.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.787522 rez-3.1.0/src/rez/data/tests/packages/py_packages/timestamped/2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/py_packages/timestamped/2.0.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.787522 rez-3.1.0/src/rez/data/tests/packages/py_packages/timestamped/2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/py_packages/timestamped/2.1.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.787522 rez-3.1.0/src/rez/data/tests/packages/py_packages/timestamped/2.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/py_packages/timestamped/2.1.5/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.787522 rez-3.1.0/src/rez/data/tests/packages/py_packages/unversioned_py/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/py_packages/unversioned_py/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.735522 rez-3.1.0/src/rez/data/tests/packages/py_packages/variants_py/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.787522 rez-3.1.0/src/rez/data/tests/packages/py_packages/variants_py/2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/py_packages/variants_py/2.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.735522 rez-3.1.0/src/rez/data/tests/packages/py_packages/versioned/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.787522 rez-3.1.0/src/rez/data/tests/packages/py_packages/versioned/2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/py_packages/versioned/2.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.787522 rez-3.1.0/src/rez/data/tests/packages/py_packages/versioned/3.0/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/py_packages/versioned/3.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.787522 rez-3.1.0/src/rez/data/tests/packages/yaml_packages/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/yaml_packages/multi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/yaml_packages/single_unversioned.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/yaml_packages/single_versioned.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.791523 rez-3.1.0/src/rez/data/tests/packages/yaml_packages/unversioned/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/yaml_packages/unversioned/package.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.735522 rez-3.1.0/src/rez/data/tests/packages/yaml_packages/versioned/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.791523 rez-3.1.0/src/rez/data/tests/packages/yaml_packages/versioned/1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/yaml_packages/versioned/1.0/package.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.791523 rez-3.1.0/src/rez/data/tests/packages/yaml_packages/versioned/2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/packages/yaml_packages/versioned/2.0/package.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.735522 rez-3.1.0/src/rez/data/tests/pip/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.735522 rez-3.1.0/src/rez/data/tests/pip/installed_distributions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.791523 rez-3.1.0/src/rez/data/tests/pip/installed_distributions/six-1.12.0.dist-info/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/pip/installed_distributions/six-1.12.0.dist-info/INSTALLER
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/pip/installed_distributions/six-1.12.0.dist-info/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/pip/installed_distributions/six-1.12.0.dist-info/METADATA
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/pip/installed_distributions/six-1.12.0.dist-info/RECORD
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/pip/installed_distributions/six-1.12.0.dist-info/WHEEL
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/pip/installed_distributions/six-1.12.0.dist-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.739522 rez-3.1.0/src/rez/data/tests/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.791523 rez-3.1.0/src/rez/data/tests/python/early_bind/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/python/early_bind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/python/early_bind/early_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.791523 rez-3.1.0/src/rez/data/tests/python/late_bind/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/python/late_bind/late_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.791523 rez-3.1.0/src/rez/data/tests/python/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/python/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/python/preprocess/global_preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.791523 rez-3.1.0/src/rez/data/tests/release/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/release/build.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.791523 rez-3.1.0/src/rez/data/tests/release/data/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/release/data/data.txt
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/release/package.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.791523 rez-3.1.0/src/rez/data/tests/release/variants/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/release/variants/build.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/release/variants/package.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.739522 rez-3.1.0/src/rez/data/tests/release/variants/spangle/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.791523 rez-3.1.0/src/rez/data/tests/release/variants/spangle/1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/release/variants/spangle/1.0/package.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.791523 rez-3.1.0/src/rez/data/tests/release/variants/spangle/1.1/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/release/variants/spangle/1.1/package.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.791523 rez-3.1.0/src/rez/data/tests/release/variants/spangle/2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/release/variants/spangle/2.0/package.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.739522 rez-3.1.0/src/rez/data/tests/solver/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.791523 rez-3.1.0/src/rez/data/tests/solver/packages/
--rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/README
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.739522 rez-3.1.0/src/rez/data/tests/solver/packages/bahish/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/bahish/1/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/bahish/1/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/bahish/2/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/bahish/2/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.739522 rez-3.1.0/src/rez/data/tests/solver/packages/missing_variant_requires/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/missing_variant_requires/1/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/missing_variant_requires/1/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/nada/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/nada/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.739522 rez-3.1.0/src/rez/data/tests/solver/packages/nopy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/nopy/2.1/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/nopy/2.1/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.739522 rez-3.1.0/src/rez/data/tests/solver/packages/pybah/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/pybah/4/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/pybah/4/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/pybah/5/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/pybah/5/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.739522 rez-3.1.0/src/rez/data/tests/solver/packages/pydad/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/pydad/1/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/pydad/1/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/pydad/2/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/pydad/2/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/pydad/3/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/pydad/3/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.739522 rez-3.1.0/src/rez/data/tests/solver/packages/pyfoo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/pyfoo/3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/pyfoo/3.0.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/pyfoo/3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/pyfoo/3.1.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.739522 rez-3.1.0/src/rez/data/tests/solver/packages/pymum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/pymum/1/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/pymum/1/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/pymum/2/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/pymum/2/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/pymum/3/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/pymum/3/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.743522 rez-3.1.0/src/rez/data/tests/solver/packages/pyodd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/pyodd/1/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/pyodd/1/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/pyodd/2/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/pyodd/2/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.743522 rez-3.1.0/src/rez/data/tests/solver/packages/pyson/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/pyson/1/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/pyson/1/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/pyson/2/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/pyson/2/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.743522 rez-3.1.0/src/rez/data/tests/solver/packages/pysplit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/pysplit/5/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/pysplit/5/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/pysplit/6/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/pysplit/6/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/pysplit/7/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/pysplit/7/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.743522 rez-3.1.0/src/rez/data/tests/solver/packages/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.795523 rez-3.1.0/src/rez/data/tests/solver/packages/python/2.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/python/2.5.2/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.799522 rez-3.1.0/src/rez/data/tests/solver/packages/python/2.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/python/2.6.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.799522 rez-3.1.0/src/rez/data/tests/solver/packages/python/2.6.8/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/python/2.6.8/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.799522 rez-3.1.0/src/rez/data/tests/solver/packages/python/2.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/python/2.7.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.743522 rez-3.1.0/src/rez/data/tests/solver/packages/pyvariants/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.799522 rez-3.1.0/src/rez/data/tests/solver/packages/pyvariants/2/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/pyvariants/2/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.743522 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_end/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.799522 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_end/1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_end/1.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.799522 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_end/2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_end/2.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.799522 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_end/3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_end/3.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.799522 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_end/4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_end/4.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.743522 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_mid1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.799522 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_mid1/1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_mid1/1.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.799522 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_mid1/2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_mid1/2.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.743522 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_mid2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.799522 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_mid2/1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_mid2/1.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.799522 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_mid2/2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_mid2/2.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.743522 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_start/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.799522 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_start/1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_start/1.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.799522 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_start/2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/solver/packages/test_variant_split_start/2.0/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.743522 rez-3.1.0/src/rez/data/tests/suites/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.743522 rez-3.1.0/src/rez/data/tests/suites/packages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.799522 rez-3.1.0/src/rez/data/tests/suites/packages/bah/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/suites/packages/bah/package.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.799522 rez-3.1.0/src/rez/data/tests/suites/packages/eek/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/suites/packages/eek/package.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.799522 rez-3.1.0/src/rez/data/tests/suites/packages/foo/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/suites/packages/foo/package.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.799522 rez-3.1.0/src/rez/data/tests/suites/packages/pooh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.799522 rez-3.1.0/src/rez/data/tests/suites/packages/pooh/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)       33 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/suites/packages/pooh/bin/hunny
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/suites/packages/pooh/bin/hunny.bat
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/data/tests/suites/packages/pooh/package.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/deprecations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/developer_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/package_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)    30481 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/package_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    15911 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/package_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17076 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/package_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/package_help.py
--rw-r--r--   0 runner    (1001) docker     (127)     8227 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/package_maker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/package_move.py
--rw-r--r--   0 runner    (1001) docker     (127)    23145 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/package_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/package_py_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/package_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)    22302 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/package_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    16720 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/package_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/package_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/package_serialise.py
--rw-r--r--   0 runner    (1001) docker     (127)    24837 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/package_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    30902 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)    21612 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/pip.py
--rw-r--r--   0 runner    (1001) docker     (127)    18343 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/plugin_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/release_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     8168 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/release_vcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    81225 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/resolved_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    18018 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    46162 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/rex.py
--rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/rex_bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)    50764 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/rezconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    14111 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/serialise.py
--rw-r--r--   0 runner    (1001) docker     (127)    18753 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/shells.py
--rw-r--r--   0 runner    (1001) docker     (127)    86337 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    12433 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/status.py
--rw-r--r--   0 runner    (1001) docker     (127)    27452 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/suite.py
--rw-r--r--   0 runner    (1001) docker     (127)    10300 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.807523 rez-3.1.0/src/rez/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/README
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    14397 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9018 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    10926 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_copy_package.py
--rw-r--r--   0 runner    (1001) docker     (127)    12661 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_package_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_package_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    24355 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)    15216 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_packages_order.py
--rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_pip_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9393 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_release.py
--rw-r--r--   0 runner    (1001) docker     (127)    10116 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_resources_.py
--rw-r--r--   0 runner    (1001) docker     (127)    20569 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_rex.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    21842 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_shells.py
--rw-r--r--   0 runner    (1001) docker     (127)     9082 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_suites.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_utils_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_utils_resolve_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    18543 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12573 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.811523 rez-3.1.0/src/rez/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/amqp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/backcompat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/base26.py
--rw-r--r--   0 runner    (1001) docker     (127)     9620 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/colorize.py
--rw-r--r--   0 runner    (1001) docker     (127)    20355 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/diff_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/elf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    22262 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)    14957 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8415 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/installer.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/lint_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/logging_.py
--rw-r--r--   0 runner    (1001) docker     (127)    13868 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/memcached.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/patching.py
--rw-r--r--   0 runner    (1001) docker     (127)    24665 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/pip.py
--rw-r--r--   0 runner    (1001) docker     (127)    18302 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/platform_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/platform_mapped.py
--rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/py_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/resolve_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    10407 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     8613 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    11097 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/sourcecode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/which.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.811523 rez-3.1.0/src/rez/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.811523 rez-3.1.0/src/rez/vendor/argcomplete/
--rw-r--r--   0 runner    (1001) docker     (127)    21557 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/argcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/argcomplete/completers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13198 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/argcomplete/my_argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    11545 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/argcomplete/my_shlex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.811523 rez-3.1.0/src/rez/vendor/atomicwrites/
--rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/atomicwrites/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.815523 rez-3.1.0/src/rez/vendor/attr/
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/attr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/attr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/attr/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/attr/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/attr/_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    68317 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/attr/_make.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/attr/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/attr/converters.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/attr/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/attr/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/attr/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/attr/filters.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/attr/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/attr/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/attr/validators.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.815523 rez-3.1.0/src/rez/vendor/colorama/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/colorama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/colorama/ansi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/colorama/ansitowin32.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/colorama/initialise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.815523 rez-3.1.0/src/rez/vendor/colorama/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/colorama/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/colorama/tests/ansi_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/colorama/tests/ansitowin32_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/colorama/tests/initialise_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/colorama/tests/isatty_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/colorama/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/colorama/tests/winterm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/colorama/win32.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/colorama/winterm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.819523 rez-3.1.0/src/rez/vendor/distlib/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.819523 rez-3.1.0/src/rez/vendor/distlib/_backport/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distlib/_backport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distlib/_backport/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    25647 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distlib/_backport/shutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    26964 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distlib/_backport/sysconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    92628 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distlib/_backport/tarfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    41404 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distlib/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    51029 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distlib/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    21066 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distlib/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    51807 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distlib/locators.py
--rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distlib/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distlib/markers.py
--rw-r--r--   0 runner    (1001) docker     (127)    40234 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distlib/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distlib/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distlib/scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)    92672 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distlib/t32.exe
--rw-r--r--   0 runner    (1001) docker     (127)   102912 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distlib/t64.exe
--rw-r--r--   0 runner    (1001) docker     (127)    60091 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distlib/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    23391 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distlib/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    89088 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distlib/w32.exe
--rw-r--r--   0 runner    (1001) docker     (127)    99840 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distlib/w64.exe
--rw-r--r--   0 runner    (1001) docker     (127)    40437 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distlib/wheel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.819523 rez-3.1.0/src/rez/vendor/distro/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43628 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/distro/distro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.819523 rez-3.1.0/src/rez/vendor/enum/
--rw-r--r--   0 runner    (1001) docker     (127)    28578 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28578 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/enum/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.823523 rez-3.1.0/src/rez/vendor/lockfile/
--rw-r--r--   0 runner    (1001) docker     (127)     9418 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/lockfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/lockfile/linklockfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/lockfile/mkdirlockfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/lockfile/pidlockfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/lockfile/sqlitelockfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/lockfile/symlinklockfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.823523 rez-3.1.0/src/rez/vendor/memcache/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/memcache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54961 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/memcache/memcache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.823523 rez-3.1.0/src/rez/vendor/packaging/
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/packaging/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/packaging/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/packaging/_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/packaging/markers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/packaging/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)    27778 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/packaging/specifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/packaging/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11978 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/packaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.827523 rez-3.1.0/src/rez/vendor/pika/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.827523 rez-3.1.0/src/rez/vendor/pika/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9256 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/adapters/asyncio_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20544 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/adapters/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)   109577 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/adapters/blocking_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    45326 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/adapters/select_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.827523 rez-3.1.0/src/rez/vendor/pika/adapters/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/adapters/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33944 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/adapters/utils/connection_workflow.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    53724 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/adapters/utils/io_services_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17294 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/adapters/utils/nbio_interface.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19988 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/adapters/utils/selector_ioloop_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/amqp_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    14776 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)    62966 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    86718 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/data.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/delivery_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/diagnostic_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10117 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/exchange_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)    78619 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/tcp_socket_opts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pika/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.827523 rez-3.1.0/src/rez/vendor/progress/
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/progress/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/progress/counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/progress/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/progress/spinner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.831523 rez-3.1.0/src/rez/vendor/pydot/
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pydot/README
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pydot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pydot/dot_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    54309 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pydot/pydot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.831523 rez-3.1.0/src/rez/vendor/pygraph/
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.831523 rez-3.1.0/src/rez/vendor/pygraph/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/algorithms/accessibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/algorithms/critical.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/algorithms/cycles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.831523 rez-3.1.0/src/rez/vendor/pygraph/algorithms/filters/
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/algorithms/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/algorithms/filters/find.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/algorithms/filters/null.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/algorithms/filters/radius.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/algorithms/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.831523 rez-3.1.0/src/rez/vendor/pygraph/algorithms/heuristics/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/algorithms/heuristics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/algorithms/heuristics/chow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/algorithms/heuristics/euclidean.py
--rw-r--r--   0 runner    (1001) docker     (127)    16125 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/algorithms/minmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/algorithms/pagerank.py
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/algorithms/searching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/algorithms/sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/algorithms/traversal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/algorithms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.831523 rez-3.1.0/src/rez/vendor/pygraph/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/classes/digraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/classes/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/classes/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    10957 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/classes/hypergraph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.835523 rez-3.1.0/src/rez/vendor/pygraph/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/mixins/basegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/mixins/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/mixins/labeling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.835523 rez-3.1.0/src/rez/vendor/pygraph/readwrite/
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/readwrite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/readwrite/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pygraph/readwrite/markup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.835523 rez-3.1.0/src/rez/vendor/pyparsing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pyparsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   245356 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/pyparsing/pyparsing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.835523 rez-3.1.0/src/rez/vendor/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    16287 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/schema/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.835523 rez-3.1.0/src/rez/vendor/six/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/six/README
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/six/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32452 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/six/six.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.835523 rez-3.1.0/src/rez/vendor/yaml/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.839523 rez-3.1.0/src/rez/vendor/yaml/lib/
--rw-r--r--   0 runner    (1001) docker     (127)    12182 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib/composer.py
--rw-r--r--   0 runner    (1001) docker     (127)    26834 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib/constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib/cyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib/dumper.py
--rw-r--r--   0 runner    (1001) docker     (127)    43427 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib/emitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    25542 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    17791 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib/representer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9122 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    52027 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib/scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.843523 rez-3.1.0/src/rez/vendor/yaml/lib3/
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib3/composer.py
--rw-r--r--   0 runner    (1001) docker     (127)    27187 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib3/constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib3/cyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib3/dumper.py
--rw-r--r--   0 runner    (1001) docker     (127)    43006 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib3/emitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib3/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib3/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib3/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib3/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    25495 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib3/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib3/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    14189 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib3/representer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8970 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib3/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    51277 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib3/scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib3/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/vendor/yaml/lib3/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.843523 rez-3.1.0/src/rez/version/
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14250 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/version/_requirement.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/version/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    51286 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/version/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-03-30 16:27:13.000000 rez-3.1.0/src/rez/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.867523 rez-3.1.0/src/rez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13050 2024-03-30 16:27:16.000000 rez-3.1.0/src/rez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27629 2024-03-30 16:27:16.000000 rez-3.1.0/src/rez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 16:27:16.000000 rez-3.1.0/src/rez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-30 16:27:16.000000 rez-3.1.0/src/rez.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 16:27:16.000000 rez-3.1.0/src/rez.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-30 16:27:16.000000 rez-3.1.0/src/rez.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.843523 rez-3.1.0/src/rezgui/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.843523 rez-3.1.0/src/rezgui/dialogs/
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/dialogs/AboutDialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/dialogs/BrowsePackageDialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/dialogs/ImageViewerDialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/dialogs/ProcessDialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    11714 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/dialogs/ResolveDialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/dialogs/VariantVersionsDialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/dialogs/WriteGraphDialog.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/dialogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.851523 rez-3.1.0/src/rezgui/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/advanced_resolve.png
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/changelog.png
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/clock.png
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/clock_warning.png
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/cog.png
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/context.png
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/context_settings.png
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/depends.png
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/diff.png
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/diff_to_disk.png
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/diff_to_other.png
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/equal_to.png
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/equalish.png
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/error.png
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/excluded.png
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/find.png
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/github_32.png
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/graph.png
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/greater_than.png
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/greater_than_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/greater_than_2.png
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/greater_than_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/green_tick.png
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/green_white_tick.png
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/help.png
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/info.png
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/less_than.png
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/less_than_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/less_than_2.png
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/less_than_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/local.png
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/lock.png
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/lock_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/lock_2_faint.png
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/lock_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/lock_3_faint.png
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/lock_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/lock_4_faint.png
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/lock_faint.png
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/missing.png
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/new.png
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/no_lock.png
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/no_lock_faint.png
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/old_man.png
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/package.png
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/pink.png
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/resolve.png
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/revert.png
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/revert_to_diff.png
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/revert_to_disk.png
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/spanner.png
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/terminal.png
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/time_lock.png
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/tools.png
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/variant.png
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/versions.png
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/warning.png
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/yellow_tick.png
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/icons/yellow_white_tick.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.851523 rez-3.1.0/src/rezgui/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/mixins/ContextViewMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/mixins/StoreSizeMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/mixins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.851523 rez-3.1.0/src/rezgui/models/
--rw-r--r--   0 runner    (1001) docker     (127)     9406 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/models/ContextModel.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.855523 rez-3.1.0/src/rezgui/objects/
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/objects/App.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/objects/Config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/objects/LoadPackagesThread.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/objects/ProcessTrackerThread.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/objects/ResolveThread.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/rezguiconfig
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.859523 rez-3.1.0/src/rezgui/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/BrowsePackagePane.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/BrowsePackageWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/ChangelogEdit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/ConfiguredSplitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/ContextDetailsWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/ContextEnvironTable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/ContextEnvironWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)    15192 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/ContextManagerWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/ContextResolveTimeLabel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/ContextSettingsWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)    29408 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/ContextTableWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/ContextToolsWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/EffectivePackageCellWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/FindPopup.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/IconButton.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/ImageViewerWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/PackageLineEdit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/PackageLoadingWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/PackageSelectWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/PackageTabWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/PackageVersionsTable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/SearchableTextEdit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/StreamableTextEdit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/TimeSelecterPopup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/TimestampWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/ToolWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)    13740 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/VariantCellWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/VariantDetailsWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/VariantHelpWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/VariantSummaryWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/VariantToolsList.py
--rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/VariantVersionsTable.py
--rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/VariantVersionsWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/VariantsList.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/ViewGraphButton.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.859523 rez-3.1.0/src/rezgui/windows/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/windows/BrowsePackageSubWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/windows/ContextSubWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/windows/MainWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezgui/windows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.859523 rez-3.1.0/src/rezplugins/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.859523 rez-3.1.0/src/rezplugins/build_process/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19189 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_process/local.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_process/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_process/rezconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.863523 rez-3.1.0/src/rezplugins/build_system/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10935 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_system/cmake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.863523 rez-3.1.0/src/rezplugins/build_system/cmake_files/
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_system/cmake_files/Colorize.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_system/cmake_files/FindStaticLibs.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_system/cmake_files/InstallDirs.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_system/cmake_files/InstallFiles.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_system/cmake_files/InstallPython.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_system/cmake_files/RezBuild.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_system/cmake_files/RezFindPackages.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_system/cmake_files/RezInstallCMake.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_system/cmake_files/RezInstallContext.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     6502 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_system/cmake_files/RezInstallDoxygen.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_system/cmake_files/RezInstallPython.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_system/cmake_files/RezPipInstall.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_system/cmake_files/RezProject.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_system/cmake_files/RezRepository.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     6038 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_system/cmake_files/Utils.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     9112 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_system/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_system/make.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_system/rezconfig
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_system/rezconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.863523 rez-3.1.0/src/rezplugins/build_system/template_files/
--rw-r--r--   0 runner    (1001) docker     (127)    76664 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/build_system/template_files/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.863523 rez-3.1.0/src/rezplugins/command/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.863523 rez-3.1.0/src/rezplugins/package_repository/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/package_repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53530 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/package_repository/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/package_repository/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/package_repository/rezconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.867523 rez-3.1.0/src/rezplugins/release_hook/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/release_hook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/release_hook/amqp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/release_hook/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/release_hook/emailer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/release_hook/rezconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.867523 rez-3.1.0/src/rezplugins/release_vcs/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/release_vcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/release_vcs/git.py
--rw-r--r--   0 runner    (1001) docker     (127)    11217 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/release_vcs/hg.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/release_vcs/rezconfig
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/release_vcs/stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/release_vcs/svn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.867523 rez-3.1.0/src/rezplugins/shell/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.867523 rez-3.1.0/src/rezplugins/shell/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/shell/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11609 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/shell/_utils/powershell_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/shell/_utils/windows.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/shell/bash.py
--rw-r--r--   0 runner    (1001) docker     (127)    11561 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/shell/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/shell/csh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/shell/gitbash.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/shell/powershell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/shell/pwsh.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/shell/rezconfig
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/shell/sh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/shell/tcsh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-03-30 16:27:13.000000 rez-3.1.0/src/rezplugins/shell/zsh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:16.867523 rez-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-30 16:27:13.000000 rez-3.1.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.884031 rez-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10176 2024-04-14 19:41:41.000000 rez-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-14 19:41:41.000000 rez-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13050 2024-04-14 19:41:45.884031 rez-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11864 2024-04-14 19:41:41.000000 rez-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-14 19:41:41.000000 rez-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 19:41:45.884031 rez-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-14 19:41:41.000000 rez-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.760030 rez-3.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.772030 rez-3.1.1/src/rez/
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.776030 rez-3.1.1/src/rez/bind/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/bind/PyQt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/bind/PySide.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/bind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/bind/_pymodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/bind/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/bind/arch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/bind/cmake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/bind/gcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/bind/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/bind/os.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/bind/pip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/bind/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/bind/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/bind/rez.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/bind/rezgui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/bind/setuptools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/bind/sip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17062 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/build_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12103 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/build_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11755 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/bundle_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.784030 rez-3.1.1/src/rez/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/_complete_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10594 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/complete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/depends.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10300 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/interpret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/memcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/mv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/pip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/pkg-cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/pkg-ignore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/selftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/cli/yaml2py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.784030 rez-3.1.1/src/rez/completion/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/completion/complete.csh
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/completion/complete.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/completion/complete.zsh
+-rw-r--r--   0 runner    (1001) docker     (127)    36899 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.740030 rez-3.1.1/src/rez/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.784030 rez-3.1.1/src/rez/data/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (127)   828630 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/benchmarking/packages.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   194231 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/benchmarking/requests.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.756030 rez-3.1.1/src/rez/data/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.784030 rez-3.1.1/src/rez/data/tests/bind/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/bind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/bind/os.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.740030 rez-3.1.1/src/rez/data/tests/builds/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.744030 rez-3.1.1/src/rez/data/tests/builds/packages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.740030 rez-3.1.1/src/rez/data/tests/builds/packages/anti/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.784030 rez-3.1.1/src/rez/data/tests/builds/packages/anti/1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/anti/1.0.0/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/anti/1.0.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.740030 rez-3.1.1/src/rez/data/tests/builds/packages/bah/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.784030 rez-3.1.1/src/rez/data/tests/builds/packages/bah/2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.788030 rez-3.1.1/src/rez/data/tests/builds/packages/bah/2.1/bah/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/bah/2.1/bah/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/bah/2.1/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/bah/2.1/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.740030 rez-3.1.1/src/rez/data/tests/builds/packages/build_util/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.788030 rez-3.1.1/src/rez/data/tests/builds/packages/build_util/1/
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/build_util/1/build.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.788030 rez-3.1.1/src/rez/data/tests/builds/packages/build_util/1/build_util/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/build_util/1/build_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/build_util/1/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.788030 rez-3.1.1/src/rez/data/tests/builds/packages/floob/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/floob/build.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.788030 rez-3.1.1/src/rez/data/tests/builds/packages/floob/floob/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/floob/floob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/floob/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.740030 rez-3.1.1/src/rez/data/tests/builds/packages/foo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.788030 rez-3.1.1/src/rez/data/tests/builds/packages/foo/1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/foo/1.0.0/build.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.788030 rez-3.1.1/src/rez/data/tests/builds/packages/foo/1.0.0/foo/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/foo/1.0.0/foo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/foo/1.0.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.788030 rez-3.1.1/src/rez/data/tests/builds/packages/foo/1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/foo/1.1.0/build.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.788030 rez-3.1.1/src/rez/data/tests/builds/packages/foo/1.1.0/foo/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/foo/1.1.0/foo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/foo/1.1.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.740030 rez-3.1.1/src/rez/data/tests/builds/packages/hello/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.788030 rez-3.1.1/src/rez/data/tests/builds/packages/hello/1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/hello/1.0/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.788030 rez-3.1.1/src/rez/data/tests/builds/packages/hello/1.0/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/hello/1.0/lib/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/hello/1.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.740030 rez-3.1.1/src/rez/data/tests/builds/packages/loco/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.788030 rez-3.1.1/src/rez/data/tests/builds/packages/loco/3/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/loco/3/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/loco/3/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.740030 rez-3.1.1/src/rez/data/tests/builds/packages/sup_world/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.788030 rez-3.1.1/src/rez/data/tests/builds/packages/sup_world/3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/sup_world/3.8/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.788030 rez-3.1.1/src/rez/data/tests/builds/packages/sup_world/3.8/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/sup_world/3.8/lib/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/sup_world/3.8/lib/spanish_greet.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/sup_world/3.8/lib/spanish_greet.h
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/sup_world/3.8/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.792030 rez-3.1.1/src/rez/data/tests/builds/packages/sup_world/3.8/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/sup_world/3.8/util/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/sup_world/3.8/util/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.744030 rez-3.1.1/src/rez/data/tests/builds/packages/translate_lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.792030 rez-3.1.1/src/rez/data/tests/builds/packages/translate_lib/2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/translate_lib/2.2.0/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.792030 rez-3.1.1/src/rez/data/tests/builds/packages/translate_lib/2.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/translate_lib/2.2.0/docs/a spaced document
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/translate_lib/2.2.0/docs/an_unspaced_document
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/translate_lib/2.2.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.792030 rez-3.1.1/src/rez/data/tests/builds/packages/translate_lib/2.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/translate_lib/2.2.0/src/lolTranslator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/translate_lib/2.2.0/src/lolTranslator.h
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/translate_lib/2.2.0/src/spanishTranslator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/translate_lib/2.2.0/src/spanishTranslator.h
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/translate_lib/2.2.0/src/translator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/translate_lib/2.2.0/src/translator.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.792030 rez-3.1.1/src/rez/data/tests/builds/packages/whack/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/whack/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/builds/packages/whack/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.744030 rez-3.1.1/src/rez/data/tests/commands/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.744030 rez-3.1.1/src/rez/data/tests/commands/packages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.744030 rez-3.1.1/src/rez/data/tests/commands/packages/rextest/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.792030 rez-3.1.1/src/rez/data/tests/commands/packages/rextest/1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/commands/packages/rextest/1.1/package.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.792030 rez-3.1.1/src/rez/data/tests/commands/packages/rextest/1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/commands/packages/rextest/1.2/package.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.792030 rez-3.1.1/src/rez/data/tests/commands/packages/rextest/1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/commands/packages/rextest/1.3/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.744030 rez-3.1.1/src/rez/data/tests/commands/packages/rextest2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.792030 rez-3.1.1/src/rez/data/tests/commands/packages/rextest2/2/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/commands/packages/rextest2/2/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.792030 rez-3.1.1/src/rez/data/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/config/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/config/test1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/config/test2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.744030 rez-3.1.1/src/rez/data/tests/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.792030 rez-3.1.1/src/rez/data/tests/extensions/bar/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/extensions/bar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.792030 rez-3.1.1/src/rez/data/tests/extensions/bar/rezplugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/extensions/bar/rezplugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.792030 rez-3.1.1/src/rez/data/tests/extensions/bar/rezplugins/package_repository/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/extensions/bar/rezplugins/package_repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/extensions/bar/rezplugins/package_repository/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.792030 rez-3.1.1/src/rez/data/tests/extensions/foo/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/extensions/foo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.792030 rez-3.1.1/src/rez/data/tests/extensions/foo/rezplugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/extensions/foo/rezplugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.796030 rez-3.1.1/src/rez/data/tests/extensions/foo/rezplugins/package_repository/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/extensions/foo/rezplugins/package_repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/extensions/foo/rezplugins/package_repository/cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.744030 rez-3.1.1/src/rez/data/tests/extensions/non-mod/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.796030 rez-3.1.1/src/rez/data/tests/extensions/non-mod/rezplugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/extensions/non-mod/rezplugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.796030 rez-3.1.1/src/rez/data/tests/extensions/non-mod/rezplugins/package_repository/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/extensions/non-mod/rezplugins/package_repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/extensions/non-mod/rezplugins/package_repository/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.748030 rez-3.1.1/src/rez/data/tests/packages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.796030 rez-3.1.1/src/rez/data/tests/packages/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/developer/package.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.796030 rez-3.1.1/src/rez/data/tests/packages/developer_changed/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/developer_changed/package.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.796030 rez-3.1.1/src/rez/data/tests/packages/developer_dynamic_global_preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/developer_dynamic_global_preprocess/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.796030 rez-3.1.1/src/rez/data/tests/packages/developer_dynamic_local_preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/developer_dynamic_local_preprocess/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.796030 rez-3.1.1/src/rez/data/tests/packages/developer_dynamic_local_preprocess_additive/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/developer_dynamic_local_preprocess_additive/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.796030 rez-3.1.1/src/rez/data/tests/packages/developer_novar/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/developer_novar/package.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.796030 rez-3.1.1/src/rez/data/tests/packages/developer_novar_changed/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/developer_novar_changed/package.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.796030 rez-3.1.1/src/rez/data/tests/packages/py_packages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.796030 rez-3.1.1/src/rez/data/tests/packages/py_packages/empty/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/py_packages/empty/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.744030 rez-3.1.1/src/rez/data/tests/packages/py_packages/late_binding/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.796030 rez-3.1.1/src/rez/data/tests/packages/py_packages/late_binding/1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/py_packages/late_binding/1.0/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/py_packages/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/py_packages/single_unversioned.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/py_packages/single_versioned.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.748030 rez-3.1.1/src/rez/data/tests/packages/py_packages/timestamped/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.796030 rez-3.1.1/src/rez/data/tests/packages/py_packages/timestamped/1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/py_packages/timestamped/1.0.5/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.796030 rez-3.1.1/src/rez/data/tests/packages/py_packages/timestamped/1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/py_packages/timestamped/1.0.6/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.796030 rez-3.1.1/src/rez/data/tests/packages/py_packages/timestamped/1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/py_packages/timestamped/1.1.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.796030 rez-3.1.1/src/rez/data/tests/packages/py_packages/timestamped/1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/py_packages/timestamped/1.1.1/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.796030 rez-3.1.1/src/rez/data/tests/packages/py_packages/timestamped/1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/py_packages/timestamped/1.2.0/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/py_packages/timestamped/1.2.0/stuff.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.796030 rez-3.1.1/src/rez/data/tests/packages/py_packages/timestamped/2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/py_packages/timestamped/2.0.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.796030 rez-3.1.1/src/rez/data/tests/packages/py_packages/timestamped/2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/py_packages/timestamped/2.1.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.800030 rez-3.1.1/src/rez/data/tests/packages/py_packages/timestamped/2.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/py_packages/timestamped/2.1.5/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.800030 rez-3.1.1/src/rez/data/tests/packages/py_packages/unversioned_py/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/py_packages/unversioned_py/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.748030 rez-3.1.1/src/rez/data/tests/packages/py_packages/variants_py/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.800030 rez-3.1.1/src/rez/data/tests/packages/py_packages/variants_py/2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/py_packages/variants_py/2.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.748030 rez-3.1.1/src/rez/data/tests/packages/py_packages/versioned/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.800030 rez-3.1.1/src/rez/data/tests/packages/py_packages/versioned/2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/py_packages/versioned/2.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.800030 rez-3.1.1/src/rez/data/tests/packages/py_packages/versioned/3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/py_packages/versioned/3.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.800030 rez-3.1.1/src/rez/data/tests/packages/yaml_packages/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/yaml_packages/multi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/yaml_packages/single_unversioned.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/yaml_packages/single_versioned.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.800030 rez-3.1.1/src/rez/data/tests/packages/yaml_packages/unversioned/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/yaml_packages/unversioned/package.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.748030 rez-3.1.1/src/rez/data/tests/packages/yaml_packages/versioned/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.800030 rez-3.1.1/src/rez/data/tests/packages/yaml_packages/versioned/1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/yaml_packages/versioned/1.0/package.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.800030 rez-3.1.1/src/rez/data/tests/packages/yaml_packages/versioned/2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/packages/yaml_packages/versioned/2.0/package.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.748030 rez-3.1.1/src/rez/data/tests/pip/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.748030 rez-3.1.1/src/rez/data/tests/pip/installed_distributions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.800030 rez-3.1.1/src/rez/data/tests/pip/installed_distributions/six-1.12.0.dist-info/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/pip/installed_distributions/six-1.12.0.dist-info/INSTALLER
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/pip/installed_distributions/six-1.12.0.dist-info/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/pip/installed_distributions/six-1.12.0.dist-info/METADATA
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/pip/installed_distributions/six-1.12.0.dist-info/RECORD
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/pip/installed_distributions/six-1.12.0.dist-info/WHEEL
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/pip/installed_distributions/six-1.12.0.dist-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.748030 rez-3.1.1/src/rez/data/tests/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.800030 rez-3.1.1/src/rez/data/tests/python/early_bind/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/python/early_bind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/python/early_bind/early_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.800030 rez-3.1.1/src/rez/data/tests/python/late_bind/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/python/late_bind/late_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.800030 rez-3.1.1/src/rez/data/tests/python/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/python/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/python/preprocess/global_preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.800030 rez-3.1.1/src/rez/data/tests/release/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/release/build.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.800030 rez-3.1.1/src/rez/data/tests/release/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/release/data/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/release/package.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/release/variants/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/release/variants/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/release/variants/package.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.748030 rez-3.1.1/src/rez/data/tests/release/variants/spangle/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/release/variants/spangle/1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/release/variants/spangle/1.0/package.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/release/variants/spangle/1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/release/variants/spangle/1.1/package.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/release/variants/spangle/2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/release/variants/spangle/2.0/package.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.748030 rez-3.1.1/src/rez/data/tests/solver/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/solver/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/README
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.752030 rez-3.1.1/src/rez/data/tests/solver/packages/bahish/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/solver/packages/bahish/1/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/bahish/1/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/solver/packages/bahish/2/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/bahish/2/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.752030 rez-3.1.1/src/rez/data/tests/solver/packages/missing_variant_requires/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/solver/packages/missing_variant_requires/1/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/missing_variant_requires/1/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/solver/packages/nada/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/nada/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.752030 rez-3.1.1/src/rez/data/tests/solver/packages/nopy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/solver/packages/nopy/2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/nopy/2.1/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.752030 rez-3.1.1/src/rez/data/tests/solver/packages/pybah/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/solver/packages/pybah/4/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/pybah/4/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/solver/packages/pybah/5/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/pybah/5/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.752030 rez-3.1.1/src/rez/data/tests/solver/packages/pydad/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/solver/packages/pydad/1/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/pydad/1/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/solver/packages/pydad/2/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/pydad/2/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/solver/packages/pydad/3/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/pydad/3/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.752030 rez-3.1.1/src/rez/data/tests/solver/packages/pyfoo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/solver/packages/pyfoo/3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/pyfoo/3.0.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/solver/packages/pyfoo/3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/pyfoo/3.1.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.752030 rez-3.1.1/src/rez/data/tests/solver/packages/pymum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/solver/packages/pymum/1/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/pymum/1/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/solver/packages/pymum/2/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/pymum/2/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/solver/packages/pymum/3/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/pymum/3/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.752030 rez-3.1.1/src/rez/data/tests/solver/packages/pyodd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/solver/packages/pyodd/1/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/pyodd/1/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/solver/packages/pyodd/2/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/pyodd/2/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.752030 rez-3.1.1/src/rez/data/tests/solver/packages/pyson/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/solver/packages/pyson/1/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/pyson/1/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/solver/packages/pyson/2/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/pyson/2/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.752030 rez-3.1.1/src/rez/data/tests/solver/packages/pysplit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/solver/packages/pysplit/5/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/pysplit/5/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.804030 rez-3.1.1/src/rez/data/tests/solver/packages/pysplit/6/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/pysplit/6/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/solver/packages/pysplit/7/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/pysplit/7/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.752030 rez-3.1.1/src/rez/data/tests/solver/packages/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/solver/packages/python/2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/python/2.5.2/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/solver/packages/python/2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/python/2.6.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/solver/packages/python/2.6.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/python/2.6.8/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/solver/packages/python/2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/python/2.7.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.752030 rez-3.1.1/src/rez/data/tests/solver/packages/pyvariants/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/solver/packages/pyvariants/2/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/pyvariants/2/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.756030 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_end/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_end/1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_end/1.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_end/2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_end/2.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_end/3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_end/3.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_end/4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_end/4.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.756030 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_mid1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_mid1/1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_mid1/1.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_mid1/2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_mid1/2.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.756030 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_mid2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_mid2/1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_mid2/1.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_mid2/2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_mid2/2.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.756030 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_start/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_start/1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_start/1.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_start/2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/test_variant_split_start/2.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.756030 rez-3.1.1/src/rez/data/tests/solver/packages/test_weakly_reference_requires/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/solver/packages/test_weakly_reference_requires/2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/test_weakly_reference_requires/2.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.756030 rez-3.1.1/src/rez/data/tests/solver/packages/test_weakly_reference_variant/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/solver/packages/test_weakly_reference_variant/2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/solver/packages/test_weakly_reference_variant/2.0/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.756030 rez-3.1.1/src/rez/data/tests/suites/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.756030 rez-3.1.1/src/rez/data/tests/suites/packages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/suites/packages/bah/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/suites/packages/bah/package.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/suites/packages/eek/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/suites/packages/eek/package.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/suites/packages/foo/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/suites/packages/foo/package.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/suites/packages/pooh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.808030 rez-3.1.1/src/rez/data/tests/suites/packages/pooh/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       33 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/suites/packages/pooh/bin/hunny
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/suites/packages/pooh/bin/hunny.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/data/tests/suites/packages/pooh/package.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/developer_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/package_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30481 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/package_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15911 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/package_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17076 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/package_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/package_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8227 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/package_maker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/package_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23543 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/package_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/package_py_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/package_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22302 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/package_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16720 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/package_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/package_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/package_serialise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24837 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/package_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30902 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21612 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/pip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18343 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/plugin_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/release_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8168 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/release_vcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81225 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/resolved_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18018 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46162 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/rex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/rex_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50764 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/rezconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14111 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/serialise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18753 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/shells.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86337 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12433 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27452 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10300 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.816030 rez-3.1.1/src/rez/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/README
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14672 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9018 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10926 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_copy_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12661 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_package_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_package_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24439 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15216 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_packages_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_pip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9393 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10116 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_resources_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20569 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_rex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21842 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_shells.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10003 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_suites.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_utils_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_utils_resolve_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18543 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12573 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.820031 rez-3.1.1/src/rez/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/amqp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/backcompat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/base26.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9620 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20355 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/diff_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/elf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22262 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14957 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8415 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/lint_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/logging_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13868 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/memcached.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24665 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/pip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18302 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/platform_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/platform_mapped.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/py_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/resolve_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10407 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8613 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11097 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/sourcecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/which.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.820031 rez-3.1.1/src/rez/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.820031 rez-3.1.1/src/rez/vendor/argcomplete/
+-rw-r--r--   0 runner    (1001) docker     (127)    21557 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/argcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/argcomplete/completers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13198 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/argcomplete/my_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11545 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/argcomplete/my_shlex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.820031 rez-3.1.1/src/rez/vendor/atomicwrites/
+-rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/atomicwrites/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.824030 rez-3.1.1/src/rez/vendor/attr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/attr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/attr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/attr/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/attr/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/attr/_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68317 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/attr/_make.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/attr/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/attr/converters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/attr/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/attr/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/attr/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/attr/filters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/attr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/attr/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/attr/validators.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.824030 rez-3.1.1/src/rez/vendor/colorama/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/colorama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/colorama/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/colorama/ansitowin32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/colorama/initialise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.824030 rez-3.1.1/src/rez/vendor/colorama/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/colorama/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/colorama/tests/ansi_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/colorama/tests/initialise_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/colorama/tests/isatty_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/colorama/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/colorama/tests/winterm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/colorama/win32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/colorama/winterm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.828030 rez-3.1.1/src/rez/vendor/distlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.832030 rez-3.1.1/src/rez/vendor/distlib/_backport/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distlib/_backport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distlib/_backport/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25647 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distlib/_backport/shutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26964 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distlib/_backport/sysconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92628 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distlib/_backport/tarfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41404 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distlib/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51029 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distlib/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21066 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distlib/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51807 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distlib/locators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distlib/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distlib/markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40234 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distlib/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distlib/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distlib/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92672 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distlib/t32.exe
+-rw-r--r--   0 runner    (1001) docker     (127)   102912 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distlib/t64.exe
+-rw-r--r--   0 runner    (1001) docker     (127)    60091 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distlib/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23391 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distlib/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89088 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distlib/w32.exe
+-rw-r--r--   0 runner    (1001) docker     (127)    99840 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distlib/w64.exe
+-rw-r--r--   0 runner    (1001) docker     (127)    40437 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distlib/wheel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.832030 rez-3.1.1/src/rez/vendor/distro/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43628 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/distro/distro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.832030 rez-3.1.1/src/rez/vendor/enum/
+-rw-r--r--   0 runner    (1001) docker     (127)    28578 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28578 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/enum/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.832030 rez-3.1.1/src/rez/vendor/lockfile/
+-rw-r--r--   0 runner    (1001) docker     (127)     9418 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/lockfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/lockfile/linklockfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/lockfile/mkdirlockfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/lockfile/pidlockfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/lockfile/sqlitelockfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/lockfile/symlinklockfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.832030 rez-3.1.1/src/rez/vendor/memcache/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/memcache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54961 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/memcache/memcache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.836031 rez-3.1.1/src/rez/vendor/packaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/packaging/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/packaging/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/packaging/_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/packaging/markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/packaging/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27778 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/packaging/specifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/packaging/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11978 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/packaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.836031 rez-3.1.1/src/rez/vendor/pika/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.840031 rez-3.1.1/src/rez/vendor/pika/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9256 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/adapters/asyncio_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20544 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/adapters/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109577 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/adapters/blocking_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45326 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/adapters/select_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.840031 rez-3.1.1/src/rez/vendor/pika/adapters/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/adapters/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33944 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/adapters/utils/connection_workflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    53724 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/adapters/utils/io_services_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17294 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/adapters/utils/nbio_interface.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19988 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/adapters/utils/selector_ioloop_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/amqp_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14776 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62966 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86718 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/delivery_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/diagnostic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10117 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/exchange_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78619 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/tcp_socket_opts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pika/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.840031 rez-3.1.1/src/rez/vendor/progress/
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/progress/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/progress/counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/progress/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/progress/spinner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.840031 rez-3.1.1/src/rez/vendor/pydot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pydot/README
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pydot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pydot/dot_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54309 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pydot/pydot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.840031 rez-3.1.1/src/rez/vendor/pygraph/
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.844030 rez-3.1.1/src/rez/vendor/pygraph/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/algorithms/accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/algorithms/critical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/algorithms/cycles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.844030 rez-3.1.1/src/rez/vendor/pygraph/algorithms/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/algorithms/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/algorithms/filters/find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/algorithms/filters/null.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/algorithms/filters/radius.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/algorithms/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.844030 rez-3.1.1/src/rez/vendor/pygraph/algorithms/heuristics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/algorithms/heuristics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/algorithms/heuristics/chow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/algorithms/heuristics/euclidean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16125 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/algorithms/minmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/algorithms/pagerank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/algorithms/searching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/algorithms/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/algorithms/traversal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/algorithms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.844030 rez-3.1.1/src/rez/vendor/pygraph/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/classes/digraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/classes/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/classes/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10957 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/classes/hypergraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.844030 rez-3.1.1/src/rez/vendor/pygraph/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/mixins/basegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/mixins/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/mixins/labeling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.844030 rez-3.1.1/src/rez/vendor/pygraph/readwrite/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/readwrite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/readwrite/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pygraph/readwrite/markup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.848031 rez-3.1.1/src/rez/vendor/pyparsing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pyparsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   245356 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/pyparsing/pyparsing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.848031 rez-3.1.1/src/rez/vendor/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16287 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/schema/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.848031 rez-3.1.1/src/rez/vendor/six/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/six/README
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/six/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32452 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/six/six.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.848031 rez-3.1.1/src/rez/vendor/yaml/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.852031 rez-3.1.1/src/rez/vendor/yaml/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)    12182 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib/composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26834 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib/cyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43427 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25542 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17791 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib/representer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9122 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52027 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.852031 rez-3.1.1/src/rez/vendor/yaml/lib3/
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib3/composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27187 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib3/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib3/cyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib3/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43006 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib3/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib3/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib3/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib3/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib3/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25495 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib3/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib3/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14189 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib3/representer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8970 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib3/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51277 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib3/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib3/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/vendor/yaml/lib3/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.856031 rez-3.1.1/src/rez/version/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14250 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/version/_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/version/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51286 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/version/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-04-14 19:41:41.000000 rez-3.1.1/src/rez/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.884031 rez-3.1.1/src/rez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13050 2024-04-14 19:41:45.000000 rez-3.1.1/src/rez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27767 2024-04-14 19:41:45.000000 rez-3.1.1/src/rez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 19:41:45.000000 rez-3.1.1/src/rez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-14 19:41:45.000000 rez-3.1.1/src/rez.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 19:41:45.000000 rez-3.1.1/src/rez.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-14 19:41:45.000000 rez-3.1.1/src/rez.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.856031 rez-3.1.1/src/rezgui/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.856031 rez-3.1.1/src/rezgui/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/dialogs/AboutDialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/dialogs/BrowsePackageDialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/dialogs/ImageViewerDialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/dialogs/ProcessDialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11714 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/dialogs/ResolveDialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/dialogs/VariantVersionsDialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/dialogs/WriteGraphDialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/dialogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.864031 rez-3.1.1/src/rezgui/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/advanced_resolve.png
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/changelog.png
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/clock.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/clock_warning.png
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/cog.png
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/context.png
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/context_settings.png
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/depends.png
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/diff.png
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/diff_to_disk.png
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/diff_to_other.png
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/equal_to.png
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/equalish.png
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/error.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/excluded.png
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/find.png
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/github_32.png
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/graph.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/greater_than.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/greater_than_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/greater_than_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/greater_than_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/green_tick.png
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/green_white_tick.png
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/help.png
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/info.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/less_than.png
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/less_than_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/less_than_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/less_than_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/local.png
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/lock.png
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/lock_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/lock_2_faint.png
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/lock_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/lock_3_faint.png
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/lock_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/lock_4_faint.png
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/lock_faint.png
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/missing.png
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/new.png
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/no_lock.png
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/no_lock_faint.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/old_man.png
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/package.png
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/pink.png
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/resolve.png
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/revert.png
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/revert_to_diff.png
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/revert_to_disk.png
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/spanner.png
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/terminal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/time_lock.png
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/tools.png
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/variant.png
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/versions.png
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/warning.png
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/yellow_tick.png
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/icons/yellow_white_tick.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.868031 rez-3.1.1/src/rezgui/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/mixins/ContextViewMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/mixins/StoreSizeMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/mixins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.868031 rez-3.1.1/src/rezgui/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     9406 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/models/ContextModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.868031 rez-3.1.1/src/rezgui/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/objects/App.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/objects/Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/objects/LoadPackagesThread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/objects/ProcessTrackerThread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/objects/ResolveThread.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/rezguiconfig
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.872031 rez-3.1.1/src/rezgui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/BrowsePackagePane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/BrowsePackageWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/ChangelogEdit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/ConfiguredSplitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/ContextDetailsWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/ContextEnvironTable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/ContextEnvironWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15192 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/ContextManagerWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/ContextResolveTimeLabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/ContextSettingsWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29408 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/ContextTableWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/ContextToolsWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/EffectivePackageCellWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/FindPopup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/IconButton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/ImageViewerWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/PackageLineEdit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/PackageLoadingWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/PackageSelectWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/PackageTabWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/PackageVersionsTable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/SearchableTextEdit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/StreamableTextEdit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/TimeSelecterPopup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/TimestampWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/ToolWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13740 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/VariantCellWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/VariantDetailsWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/VariantHelpWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/VariantSummaryWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/VariantToolsList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/VariantVersionsTable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/VariantVersionsWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/VariantsList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/ViewGraphButton.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.872031 rez-3.1.1/src/rezgui/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/windows/BrowsePackageSubWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/windows/ContextSubWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/windows/MainWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezgui/windows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.872031 rez-3.1.1/src/rezplugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.876031 rez-3.1.1/src/rezplugins/build_process/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19189 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_process/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_process/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_process/rezconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.876031 rez-3.1.1/src/rezplugins/build_system/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10935 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_system/cmake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.876031 rez-3.1.1/src/rezplugins/build_system/cmake_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_system/cmake_files/Colorize.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_system/cmake_files/FindStaticLibs.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_system/cmake_files/InstallDirs.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_system/cmake_files/InstallFiles.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_system/cmake_files/InstallPython.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_system/cmake_files/RezBuild.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_system/cmake_files/RezFindPackages.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_system/cmake_files/RezInstallCMake.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_system/cmake_files/RezInstallContext.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     6502 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_system/cmake_files/RezInstallDoxygen.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_system/cmake_files/RezInstallPython.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_system/cmake_files/RezPipInstall.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_system/cmake_files/RezProject.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_system/cmake_files/RezRepository.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     6038 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_system/cmake_files/Utils.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     9112 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_system/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_system/make.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_system/rezconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.876031 rez-3.1.1/src/rezplugins/build_system/template_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    76664 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/build_system/template_files/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.880031 rez-3.1.1/src/rezplugins/command/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.880031 rez-3.1.1/src/rezplugins/package_repository/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/package_repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53681 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/package_repository/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/package_repository/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/package_repository/rezconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.880031 rez-3.1.1/src/rezplugins/release_hook/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/release_hook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/release_hook/amqp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/release_hook/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/release_hook/emailer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/release_hook/rezconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.880031 rez-3.1.1/src/rezplugins/release_vcs/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/release_vcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/release_vcs/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11217 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/release_vcs/hg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/release_vcs/rezconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/release_vcs/stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/release_vcs/svn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.884031 rez-3.1.1/src/rezplugins/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.884031 rez-3.1.1/src/rezplugins/shell/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/shell/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11609 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/shell/_utils/powershell_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/shell/_utils/windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/shell/bash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11561 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/shell/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/shell/csh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/shell/gitbash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/shell/powershell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/shell/pwsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/shell/rezconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/shell/sh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/shell/tcsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-14 19:41:41.000000 rez-3.1.1/src/rezplugins/shell/zsh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:41:45.884031 rez-3.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-14 19:41:41.000000 rez-3.1.1/tests/test.py
```

### Comparing `rez-3.1.0/LICENSE` & `rez-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/PKG-INFO` & `rez-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rez
-Version: 3.1.0
+Version: 3.1.1
 Summary: A cross-platform packaging system that can build and install multiple version of packages, and dynamically configure resolved environments at runtime.
 Home-page: https://github.com/AcademySoftwareFoundation/rez
 Author: Allan Johns
 Author-email: nerdvegas@gmail.com
 Maintainer: Contributors to the rez project
 Maintainer-email: rez-discussion@lists.aswf.io
 License: Apache-2.0
```

### Comparing `rez-3.1.0/README.md` & `rez-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/setup.py` & `rez-3.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,14 @@
         'rez':
             ['utils/logging.conf'] +
             ['README*'] +
             find_files('*', 'completion') +
             find_files('*', 'data') +
             find_files('*.exe', 'vendor/distlib'),
         'rezplugins':
-            find_files('rezconfig', root='rezplugins') +
             find_files('*.cmake', 'build_system', root='rezplugins') +
             find_files('*', 'build_system/template_files', root='rezplugins'),
         'rezgui':
             find_files('rezguiconfig', root='rezgui') +
             find_files('*', 'icons', root='rezgui')
     },
     classifiers=[
```

### Comparing `rez-3.1.0/src/rez/__init__.py` & `rez-3.1.1/src/rez/__init__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/bind/PyQt.py` & `rez-3.1.1/src/rez/bind/PyQt.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/bind/PySide.py` & `rez-3.1.1/src/rez/bind/PySide.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/bind/_pymodule.py` & `rez-3.1.1/src/rez/bind/_pymodule.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/bind/_utils.py` & `rez-3.1.1/src/rez/bind/_utils.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/bind/arch.py` & `rez-3.1.1/src/rez/bind/arch.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/bind/cmake.py` & `rez-3.1.1/src/rez/bind/cmake.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/bind/gcc.py` & `rez-3.1.1/src/rez/bind/gcc.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/bind/hello_world.py` & `rez-3.1.1/src/rez/bind/hello_world.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/bind/os.py` & `rez-3.1.1/src/rez/bind/os.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/bind/pip.py` & `rez-3.1.1/src/rez/bind/pip.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/bind/platform.py` & `rez-3.1.1/src/rez/bind/platform.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/bind/python.py` & `rez-3.1.1/src/rez/bind/python.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/bind/rez.py` & `rez-3.1.1/src/rez/bind/rez.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/bind/rezgui.py` & `rez-3.1.1/src/rez/bind/rezgui.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/bind/setuptools.py` & `rez-3.1.1/src/rez/bind/setuptools.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/bind/sip.py` & `rez-3.1.1/src/rez/bind/sip.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/build_process.py` & `rez-3.1.1/src/rez/build_process.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/build_system.py` & `rez-3.1.1/src/rez/build_system.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/bundle_context.py` & `rez-3.1.1/src/rez/bundle_context.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/_complete_util.py` & `rez-3.1.1/src/rez/cli/_complete_util.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/_entry_points.py` & `rez-3.1.1/src/rez/cli/_entry_points.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/_main.py` & `rez-3.1.1/src/rez/cli/_main.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/_util.py` & `rez-3.1.1/src/rez/cli/_util.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/benchmark.py` & `rez-3.1.1/src/rez/cli/benchmark.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/bind.py` & `rez-3.1.1/src/rez/cli/bind.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/build.py` & `rez-3.1.1/src/rez/cli/build.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/bundle.py` & `rez-3.1.1/src/rez/cli/bundle.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/complete.py` & `rez-3.1.1/src/rez/cli/complete.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/config.py` & `rez-3.1.1/src/rez/cli/config.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/context.py` & `rez-3.1.1/src/rez/cli/context.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/cp.py` & `rez-3.1.1/src/rez/cli/cp.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/depends.py` & `rez-3.1.1/src/rez/cli/depends.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/diff.py` & `rez-3.1.1/src/rez/cli/diff.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/env.py` & `rez-3.1.1/src/rez/cli/env.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/forward.py` & `rez-3.1.1/src/rez/cli/forward.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/gui.py` & `rez-3.1.1/src/rez/cli/gui.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/help.py` & `rez-3.1.1/src/rez/cli/help.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/interpret.py` & `rez-3.1.1/src/rez/cli/interpret.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/memcache.py` & `rez-3.1.1/src/rez/cli/memcache.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/mv.py` & `rez-3.1.1/src/rez/cli/mv.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/pip.py` & `rez-3.1.1/src/rez/cli/pip.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/pkg-cache.py` & `rez-3.1.1/src/rez/cli/pkg-cache.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/pkg-ignore.py` & `rez-3.1.1/src/rez/cli/pkg-ignore.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/plugins.py` & `rez-3.1.1/src/rez/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/python.py` & `rez-3.1.1/src/rez/cli/python.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/release.py` & `rez-3.1.1/src/rez/cli/release.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/rm.py` & `rez-3.1.1/src/rez/cli/rm.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/search.py` & `rez-3.1.1/src/rez/cli/search.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/selftest.py` & `rez-3.1.1/src/rez/cli/selftest.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/status.py` & `rez-3.1.1/src/rez/cli/status.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/suite.py` & `rez-3.1.1/src/rez/cli/suite.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/test.py` & `rez-3.1.1/src/rez/cli/test.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/view.py` & `rez-3.1.1/src/rez/cli/view.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/cli/yaml2py.py` & `rez-3.1.1/src/rez/cli/yaml2py.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/command.py` & `rez-3.1.1/src/rez/command.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/completion/complete.sh` & `rez-3.1.1/src/rez/completion/complete.sh`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/completion/complete.zsh` & `rez-3.1.1/src/rez/completion/complete.zsh`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/config.py` & `rez-3.1.1/src/rez/config.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/data/benchmarking/packages.tar.gz` & `rez-3.1.1/src/rez/data/benchmarking/packages.tar.gz`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/data/benchmarking/requests.json` & `rez-3.1.1/src/rez/data/benchmarking/requests.json`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/data/tests/builds/packages/anti/1.0.0/build.py` & `rez-3.1.1/src/rez/data/tests/builds/packages/anti/1.0.0/build.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/data/tests/builds/packages/bah/2.1/build.py` & `rez-3.1.1/src/rez/data/tests/builds/packages/bah/2.1/build.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/data/tests/builds/packages/build_util/1/build.py` & `rez-3.1.1/src/rez/data/tests/builds/packages/build_util/1/build.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/data/tests/builds/packages/build_util/1/build_util/__init__.py` & `rez-3.1.1/src/rez/data/tests/builds/packages/build_util/1/build_util/__init__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/data/tests/builds/packages/floob/build.py` & `rez-3.1.1/src/rez/data/tests/builds/packages/floob/build.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/data/tests/builds/packages/foo/1.0.0/build.py` & `rez-3.1.1/src/rez/data/tests/builds/packages/foo/1.0.0/build.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/data/tests/builds/packages/foo/1.1.0/build.py` & `rez-3.1.1/src/rez/data/tests/builds/packages/foo/1.1.0/build.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/data/tests/builds/packages/translate_lib/2.2.0/CMakeLists.txt` & `rez-3.1.1/src/rez/data/tests/builds/packages/translate_lib/2.2.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/data/tests/builds/packages/translate_lib/2.2.0/src/lolTranslator.cpp` & `rez-3.1.1/src/rez/data/tests/builds/packages/translate_lib/2.2.0/src/lolTranslator.cpp`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/data/tests/builds/packages/translate_lib/2.2.0/src/lolTranslator.h` & `rez-3.1.1/src/rez/data/tests/builds/packages/translate_lib/2.2.0/src/lolTranslator.h`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/data/tests/builds/packages/translate_lib/2.2.0/src/translator.h` & `rez-3.1.1/src/rez/data/tests/builds/packages/translate_lib/2.2.0/src/translator.h`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/data/tests/config/package.py` & `rez-3.1.1/src/rez/data/tests/config/package.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/data/tests/pip/installed_distributions/six-1.12.0.dist-info/LICENSE` & `rez-3.1.1/src/rez/data/tests/pip/installed_distributions/six-1.12.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/data/tests/pip/installed_distributions/six-1.12.0.dist-info/METADATA` & `rez-3.1.1/src/rez/data/tests/pip/installed_distributions/six-1.12.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/data/tests/pip/installed_distributions/six-1.12.0.dist-info/RECORD` & `rez-3.1.1/src/rez/data/tests/pip/installed_distributions/six-1.12.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/data/tests/release/build.py` & `rez-3.1.1/src/rez/data/tests/release/build.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/data/tests/solver/packages/README` & `rez-3.1.1/src/rez/data/tests/solver/packages/README`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/deprecations.py` & `rez-3.1.1/src/rez/deprecations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 
 import warnings
 
 
 def warn(message, category, pre_formatted=False, stacklevel=1, filename=None, **kwargs):
     """
-    Wrapper around warnings.warn that allows to passa a pre-formatter
+    Wrapper around warnings.warn that allows to pass a pre-formatter
     warning message. This allows to warn about things that aren't coming
     from python files, like environment variables, etc.
     """
     if not pre_formatted:
-        message = warnings.warn(
+        warnings.warn(
             message, category=category, stacklevel=stacklevel + 1, **kwargs
         )
         return
 
     original_formatwarning = warnings.formatwarning
     if pre_formatted:
```

### Comparing `rez-3.1.0/src/rez/developer_package.py` & `rez-3.1.1/src/rez/developer_package.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/exceptions.py` & `rez-3.1.1/src/rez/exceptions.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/package_bind.py` & `rez-3.1.1/src/rez/package_bind.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/package_cache.py` & `rez-3.1.1/src/rez/package_cache.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/package_copy.py` & `rez-3.1.1/src/rez/package_copy.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/package_filter.py` & `rez-3.1.1/src/rez/package_filter.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/package_help.py` & `rez-3.1.1/src/rez/package_help.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/package_maker.py` & `rez-3.1.1/src/rez/package_maker.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/package_move.py` & `rez-3.1.1/src/rez/package_move.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/package_order.py` & `rez-3.1.1/src/rez/package_order.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,39 +112,45 @@
         return key(item).name
 
     def sort_key(self, package_name, version_like):
         """Returns a sort key usable for sorting packages within the same family
 
         Args:
             package_name: (str) The family name of the package we are sorting
-            version_like: (Version|_LowerBound|_UpperBound|_Bound|VersionRange)
-                the version-like object you wish to generate a key for
+            version_like: (Version|_LowerBound|_UpperBound|_Bound|VersionRange|None)
+                The version-like object to be used as a basis for generating a sort key.
+                Note that 'None' is also a supported value, which maintains the default sorting order.
 
         Returns:
             Sortable object
                 The returned object must be sortable, which means that it must implement __lt__.
                 The specific return type is not important.
         """
         if isinstance(version_like, VersionRange):
             return tuple(self.sort_key(package_name, bound) for bound in version_like.bounds)
-        elif isinstance(version_like, _Bound):
+        if isinstance(version_like, _Bound):
             return (self.sort_key(package_name, version_like.lower),
                     self.sort_key(package_name, version_like.upper))
-        elif isinstance(version_like, _LowerBound):
+        if isinstance(version_like, _LowerBound):
             inclusion_key = -2 if version_like.inclusive else -1
             return self.sort_key(package_name, version_like.version), inclusion_key
-        elif isinstance(version_like, _UpperBound):
+        if isinstance(version_like, _UpperBound):
             inclusion_key = 2 if version_like.inclusive else 1
             return self.sort_key(package_name, version_like.version), inclusion_key
-        elif isinstance(version_like, Version):
+        if isinstance(version_like, Version):
             # finally, the bit that we actually use the sort_key_implementation for.
             return FallbackComparable(
                 self.sort_key_implementation(package_name, version_like), version_like)
-        else:
-            raise TypeError(version_like)
+        if version_like is None:
+            # As no version range is provided for this package,
+            # Python's sort preserves the order of equal elements.
+            # Thus, to maintain the original order,
+            # we return the same object for all None values.
+            return 0
+        raise TypeError(version_like)
 
     def sort_key_implementation(self, package_name, version):
         """Returns a sort key usable for sorting these packages within the
         same family
         Args:
             package_name: (str) The family name of the package we are sorting
             version: (Version) the version object you wish to generate a key for
```

### Comparing `rez-3.1.0/src/rez/package_py_utils.py` & `rez-3.1.1/src/rez/package_py_utils.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/package_remove.py` & `rez-3.1.1/src/rez/package_remove.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/package_repository.py` & `rez-3.1.1/src/rez/package_repository.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/package_resources.py` & `rez-3.1.1/src/rez/package_resources.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/package_search.py` & `rez-3.1.1/src/rez/package_search.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/package_serialise.py` & `rez-3.1.1/src/rez/package_serialise.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/package_test.py` & `rez-3.1.1/src/rez/package_test.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/packages.py` & `rez-3.1.1/src/rez/packages.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/pip.py` & `rez-3.1.1/src/rez/pip.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/plugin_managers.py` & `rez-3.1.1/src/rez/plugin_managers.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/release_hook.py` & `rez-3.1.1/src/rez/release_hook.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/release_vcs.py` & `rez-3.1.1/src/rez/release_vcs.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/resolved_context.py` & `rez-3.1.1/src/rez/resolved_context.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/resolver.py` & `rez-3.1.1/src/rez/resolver.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/rex.py` & `rez-3.1.1/src/rez/rex.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/rex_bindings.py` & `rez-3.1.1/src/rez/rex_bindings.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/rezconfig.py` & `rez-3.1.1/src/rez/rezconfig.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/serialise.py` & `rez-3.1.1/src/rez/serialise.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/shells.py` & `rez-3.1.1/src/rez/shells.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/solver.py` & `rez-3.1.1/src/rez/solver.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/status.py` & `rez-3.1.1/src/rez/status.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/suite.py` & `rez-3.1.1/src/rez/suite.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/system.py` & `rez-3.1.1/src/rez/system.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/README` & `rez-3.1.1/src/rez/tests/README`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_bind.py` & `rez-3.1.1/src/rez/tests/test_bind.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_build.py` & `rez-3.1.1/src/rez/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_cli.py` & `rez-3.1.1/src/rez/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_commands.py` & `rez-3.1.1/src/rez/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_completion.py` & `rez-3.1.1/src/rez/tests/test_completion.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,15 +48,16 @@
             completions = get_completions(prefix)
             self.assertEqual(set(completions), set(expected_completions))
 
         _eq("zzz", [])
         _eq("", ["bahish", "nada", "nopy", "pybah", "pydad", "pyfoo", "pymum",
                  "pyodd", "pyson", "pysplit", "python", "pyvariants",
                  "test_variant_split_start", "test_variant_split_mid1",
-                 "test_variant_split_mid2", "test_variant_split_end", "missing_variant_requires"])
+                 "test_variant_split_mid2", "test_variant_split_end", "missing_variant_requires",
+                 "test_weakly_reference_requires", "test_weakly_reference_variant"])
         _eq("py", ["pybah", "pydad", "pyfoo", "pymum", "pyodd", "pyson",
             "pysplit", "python", "pyvariants"])
         _eq("pys", ["pyson", "pysplit"])
         _eq("pyb", ["pybah", "pybah-4", "pybah-5"])
         _eq("pybah-", ["pybah-4", "pybah-5"])
         _eq("pyfoo-3.0", ["pyfoo-3.0.0"])
```

### Comparing `rez-3.1.0/src/rez/tests/test_config.py` & `rez-3.1.1/src/rez/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import unittest
 from rez.tests.util import TestBase, TempdirMixin, restore_os_environ
 from rez.exceptions import ConfigurationError
 from rez.config import Config, get_module_root_config, _replace_config, _Deprecation
 from rez.system import system
 from rez.utils.data_utils import RO_AttrDictWrapper
 from rez.packages import get_developer_package
-from rez.deprecations import RezDeprecationWarning
+from rez.deprecations import RezDeprecationWarning, warn
 import os
 import os.path
 import subprocess
 import functools
 import shutil
 import unittest.mock
 
@@ -328,21 +328,21 @@
                 os.environ["HOME"] = user_home
                 # On Windows, os.path.expanduser will read HOME and then USERPROFILE with Python 3.7.
                 # https://docs.python.org/3.7/library/os.path.html#os.path.expanduser
                 # Also on Windows but for Python 3.8+, it will look for USERPROFILE and then HOME.
                 # https://docs.python.org/3.8/library/os.path.html#os.path.expanduser
                 os.environ["USERPROFILE"] = user_home
                 config = Config._create_main_config()
-                with self.assertWarns(RezDeprecationWarning) as warn:
+                with self.assertWarns(RezDeprecationWarning) as warning:
                     _ = config.data
                     # Assert just to ensure the test was set up properly.
                     self.assertEqual(config.data["packages_path"], ["/tmp/asd"])
 
                 self.assertEqual(
-                    str(warn.warning),
+                    str(warning.warning),
                     "config setting named 'packages_path' is deprecated and will be removed in 0.0.0.",
                 )
 
     def test_deprecation_from_env_var(self):
         fake_deprecated_settings = {
             "packages_path": _Deprecation("0.0.0"),
         }
@@ -352,39 +352,44 @@
             fake_deprecated_settings
         ):
             with restore_os_environ():
                 # Test with non-json env var
                 os.environ["REZ_PACKAGES_PATH"] = "/tmp/asd2"
                 os.environ["REZ_DISABLE_HOME_CONFIG"] = "1"
                 config = Config._create_main_config()
-                with self.assertWarns(RezDeprecationWarning) as warn:
+                with self.assertWarns(RezDeprecationWarning) as warning:
                     _ = config.data
                     # Assert just to ensure the test was set up properly.
                     self.assertEqual(config.data["packages_path"], ["/tmp/asd2"])
 
                 self.assertEqual(
-                    str(warn.warning),
+                    str(warning.warning),
                     "config setting named 'packages_path' (configured through the "
                     "REZ_PACKAGES_PATH environment variable) is deprecated and will "
                     "be removed in 0.0.0.",
                 )
 
             with restore_os_environ():
                 # Test with json env var
                 os.environ["REZ_PACKAGES_PATH_JSON"] = '["/tmp/asd2"]'
                 os.environ["REZ_DISABLE_HOME_CONFIG"] = "1"
                 config = Config._create_main_config()
-                with self.assertWarns(RezDeprecationWarning) as warn:
+                with self.assertWarns(RezDeprecationWarning) as warning:
                     _ = config.data
                     # Assert just to ensure the test was set up properly.
                     self.assertEqual(config.data["packages_path"], ["/tmp/asd2"])
 
                 self.assertEqual(
-                    str(warn.warning),
+                    str(warning.warning),
                     "config setting named 'packages_path' (configured through the "
                     "REZ_PACKAGES_PATH_JSON environment variable) is deprecated and will "
                     "be removed in 0.0.0.",
                 )
 
+    def test_non_preformatted_warning(self):
+        with self.assertWarns(DeprecationWarning) as warning:
+            warn('Warning Message', DeprecationWarning, pre_formatted=False)
+        self.assertEqual(str(warning.warning), 'Warning Message')
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `rez-3.1.0/src/rez/tests/test_context.py` & `rez-3.1.1/src/rez/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_copy_package.py` & `rez-3.1.1/src/rez/tests/test_copy_package.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_formatter.py` & `rez-3.1.1/src/rez/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_imports.py` & `rez-3.1.1/src/rez/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_package_cache.py` & `rez-3.1.1/src/rez/tests/test_package_cache.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_package_filter.py` & `rez-3.1.1/src/rez/tests/test_package_filter.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_packages.py` & `rez-3.1.1/src/rez/tests/test_packages.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,17 @@
     'variants_py-2.0',
     'single_unversioned',
     'single_versioned-3.5',
     'late_binding-1.0',
     'timestamped-1.0.5', 'timestamped-1.0.6', 'timestamped-1.1.0', 'timestamped-1.1.1',
     'timestamped-1.2.0', 'timestamped-2.0.0', 'timestamped-2.1.0', 'timestamped-2.1.5',
     'multi-1.0', 'multi-1.1', 'multi-1.2', 'multi-2.0',
-    'missing_variant_requires-1'
+    'missing_variant_requires-1',
+    'test_weakly_reference_requires-2.0',
+    'test_weakly_reference_variant-2.0',
 ])
 
 
 ALL_FAMILIES = set(
     [x.split('-')[0] for x in ALL_PACKAGES]
     + ["empty"]
 )
```

### Comparing `rez-3.1.0/src/rez/tests/test_packages_order.py` & `rez-3.1.1/src/rez/tests/test_packages_order.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_pip_utils.py` & `rez-3.1.1/src/rez/tests/test_pip_utils.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_plugin_manager.py` & `rez-3.1.1/src/rez/tests/test_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_release.py` & `rez-3.1.1/src/rez/tests/test_release.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_resources_.py` & `rez-3.1.1/src/rez/tests/test_resources_.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_rex.py` & `rez-3.1.1/src/rez/tests/test_rex.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_shells.py` & `rez-3.1.1/src/rez/tests/test_shells.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_solver.py` & `rez-3.1.1/src/rez/tests/test_solver.py`

 * *Files 16% similar despite different names*

```diff
@@ -252,10 +252,27 @@
         config.override("error_on_missing_variant_requires", True)
         with self.assertRaises(rez.exceptions.PackageFamilyNotFoundError):
             self._solve(["missing_variant_requires"], [])
 
         config.override("error_on_missing_variant_requires", False)
         self._solve(["missing_variant_requires"], ["nada[]", "missing_variant_requires-1[1]"])
 
+    def test_13_resolve_weakly_reference_requires(self):
+        """Test resolving a package with a weakly referenced requirement."""
+        self._solve(["test_weakly_reference_requires", "test_variant_split_mid2-2"],
+                    ['test_weakly_reference_requires-2.0[]',
+                     'test_variant_split_end-3.0[0]',
+                     'test_variant_split_mid2-2.0[1]'])
+
+    def test_14_resolve_weakly_reference_variant(self):
+        """Test resolving a package with a weakly referenced variant."""
+        self._solve(["test_weakly_reference_variant-2.0", "test_variant_split_mid2-2", "pyfoo"],
+                    ['test_variant_split_end-1.0[1]',
+                     'test_variant_split_mid1-1.0[1]',
+                     'test_weakly_reference_variant-2.0[0]',
+                     'test_variant_split_mid2-2.0[0]',
+                     'python-2.6.8[]',
+                     'pyfoo-3.1.0[]'])
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `rez-3.1.0/src/rez/tests/test_suites.py` & `rez-3.1.1/src/rez/tests/test_suites.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_util.py` & `rez-3.1.1/src/rez/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_utils.py` & `rez-3.1.1/src/rez/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_utils_filesystem.py` & `rez-3.1.1/src/rez/tests/test_utils_filesystem.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_utils_resolve_graph.py` & `rez-3.1.1/src/rez/tests/test_utils_resolve_graph.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/test_version.py` & `rez-3.1.1/src/rez/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/tests/util.py` & `rez-3.1.1/src/rez/tests/util.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/util.py` & `rez-3.1.1/src/rez/util.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/__init__.py` & `rez-3.1.1/src/rez/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/amqp.py` & `rez-3.1.1/src/rez/utils/amqp.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/backcompat.py` & `rez-3.1.1/src/rez/utils/backcompat.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/base26.py` & `rez-3.1.1/src/rez/utils/base26.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/colorize.py` & `rez-3.1.1/src/rez/utils/colorize.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/data_utils.py` & `rez-3.1.1/src/rez/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/diff_packages.py` & `rez-3.1.1/src/rez/utils/diff_packages.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/elf.py` & `rez-3.1.1/src/rez/utils/elf.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/execution.py` & `rez-3.1.1/src/rez/utils/execution.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/filesystem.py` & `rez-3.1.1/src/rez/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/formatting.py` & `rez-3.1.1/src/rez/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/graph_utils.py` & `rez-3.1.1/src/rez/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/installer.py` & `rez-3.1.1/src/rez/utils/installer.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/lint_helper.py` & `rez-3.1.1/src/rez/utils/lint_helper.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/logging_.py` & `rez-3.1.1/src/rez/utils/logging_.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/memcached.py` & `rez-3.1.1/src/rez/utils/memcached.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/patching.py` & `rez-3.1.1/src/rez/utils/patching.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/pip.py` & `rez-3.1.1/src/rez/utils/pip.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/platform_.py` & `rez-3.1.1/src/rez/utils/platform_.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/platform_mapped.py` & `rez-3.1.1/src/rez/utils/platform_mapped.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/py_dist.py` & `rez-3.1.1/src/rez/utils/py_dist.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/resolve_graph.py` & `rez-3.1.1/src/rez/utils/resolve_graph.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/resources.py` & `rez-3.1.1/src/rez/utils/resources.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/schema.py` & `rez-3.1.1/src/rez/utils/schema.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/scope.py` & `rez-3.1.1/src/rez/utils/scope.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/sourcecode.py` & `rez-3.1.1/src/rez/utils/sourcecode.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/which.py` & `rez-3.1.1/src/rez/utils/which.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/utils/yaml.py` & `rez-3.1.1/src/rez/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/README.md` & `rez-3.1.1/src/rez/vendor/README.md`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/argcomplete/__init__.py` & `rez-3.1.1/src/rez/vendor/argcomplete/__init__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/argcomplete/completers.py` & `rez-3.1.1/src/rez/vendor/argcomplete/completers.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/argcomplete/my_argparse.py` & `rez-3.1.1/src/rez/vendor/argcomplete/my_argparse.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/argcomplete/my_shlex.py` & `rez-3.1.1/src/rez/vendor/argcomplete/my_shlex.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/atomicwrites/__init__.py` & `rez-3.1.1/src/rez/vendor/atomicwrites/__init__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/attr/__init__.py` & `rez-3.1.1/src/rez/vendor/attr/__init__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/attr/__init__.pyi` & `rez-3.1.1/src/rez/vendor/attr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/attr/_compat.py` & `rez-3.1.1/src/rez/vendor/attr/_compat.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/attr/_config.py` & `rez-3.1.1/src/rez/vendor/attr/_config.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/attr/_funcs.py` & `rez-3.1.1/src/rez/vendor/attr/_funcs.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/attr/_make.py` & `rez-3.1.1/src/rez/vendor/attr/_make.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/attr/converters.py` & `rez-3.1.1/src/rez/vendor/attr/converters.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/attr/exceptions.py` & `rez-3.1.1/src/rez/vendor/attr/exceptions.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/attr/filters.py` & `rez-3.1.1/src/rez/vendor/attr/filters.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/attr/validators.py` & `rez-3.1.1/src/rez/vendor/attr/validators.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/attr/validators.pyi` & `rez-3.1.1/src/rez/vendor/attr/validators.pyi`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/colorama/ansi.py` & `rez-3.1.1/src/rez/vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/colorama/ansitowin32.py` & `rez-3.1.1/src/rez/vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/colorama/initialise.py` & `rez-3.1.1/src/rez/vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/colorama/tests/ansi_test.py` & `rez-3.1.1/src/rez/vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/colorama/tests/ansitowin32_test.py` & `rez-3.1.1/src/rez/vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/colorama/tests/initialise_test.py` & `rez-3.1.1/src/rez/vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/colorama/tests/isatty_test.py` & `rez-3.1.1/src/rez/vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/colorama/tests/utils.py` & `rez-3.1.1/src/rez/vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/colorama/tests/winterm_test.py` & `rez-3.1.1/src/rez/vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/colorama/win32.py` & `rez-3.1.1/src/rez/vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/colorama/winterm.py` & `rez-3.1.1/src/rez/vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/distlib/__init__.py` & `rez-3.1.1/src/rez/vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/distlib/_backport/misc.py` & `rez-3.1.1/src/rez/vendor/distlib/_backport/misc.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/distlib/_backport/shutil.py` & `rez-3.1.1/src/rez/vendor/distlib/_backport/shutil.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/distlib/_backport/sysconfig.py` & `rez-3.1.1/src/rez/vendor/distlib/_backport/sysconfig.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/distlib/_backport/tarfile.py` & `rez-3.1.1/src/rez/vendor/distlib/_backport/tarfile.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/distlib/compat.py` & `rez-3.1.1/src/rez/vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/distlib/database.py` & `rez-3.1.1/src/rez/vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/distlib/index.py` & `rez-3.1.1/src/rez/vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/distlib/locators.py` & `rez-3.1.1/src/rez/vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/distlib/manifest.py` & `rez-3.1.1/src/rez/vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/distlib/markers.py` & `rez-3.1.1/src/rez/vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/distlib/metadata.py` & `rez-3.1.1/src/rez/vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/distlib/resources.py` & `rez-3.1.1/src/rez/vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/distlib/scripts.py` & `rez-3.1.1/src/rez/vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/distlib/t32.exe` & `rez-3.1.1/src/rez/vendor/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/distlib/t64.exe` & `rez-3.1.1/src/rez/vendor/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/distlib/util.py` & `rez-3.1.1/src/rez/vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/distlib/version.py` & `rez-3.1.1/src/rez/vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/distlib/w32.exe` & `rez-3.1.1/src/rez/vendor/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/distlib/w64.exe` & `rez-3.1.1/src/rez/vendor/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/distlib/wheel.py` & `rez-3.1.1/src/rez/vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/distro/distro.py` & `rez-3.1.1/src/rez/vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/enum/__init__.py` & `rez-3.1.1/src/rez/vendor/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/enum/enum.py` & `rez-3.1.1/src/rez/vendor/enum/enum.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/lockfile/__init__.py` & `rez-3.1.1/src/rez/vendor/lockfile/__init__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/lockfile/linklockfile.py` & `rez-3.1.1/src/rez/vendor/lockfile/linklockfile.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/lockfile/mkdirlockfile.py` & `rez-3.1.1/src/rez/vendor/lockfile/mkdirlockfile.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/lockfile/pidlockfile.py` & `rez-3.1.1/src/rez/vendor/lockfile/pidlockfile.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/lockfile/sqlitelockfile.py` & `rez-3.1.1/src/rez/vendor/lockfile/sqlitelockfile.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/lockfile/symlinklockfile.py` & `rez-3.1.1/src/rez/vendor/lockfile/symlinklockfile.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/memcache/memcache.py` & `rez-3.1.1/src/rez/vendor/memcache/memcache.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/packaging/__about__.py` & `rez-3.1.1/src/rez/vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/packaging/__init__.py` & `rez-3.1.1/src/rez/vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/packaging/_compat.py` & `rez-3.1.1/src/rez/vendor/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/packaging/_structures.py` & `rez-3.1.1/src/rez/vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/packaging/markers.py` & `rez-3.1.1/src/rez/vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/packaging/requirements.py` & `rez-3.1.1/src/rez/vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/packaging/specifiers.py` & `rez-3.1.1/src/rez/vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/packaging/utils.py` & `rez-3.1.1/src/rez/vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/packaging/version.py` & `rez-3.1.1/src/rez/vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/adapters/__init__.py` & `rez-3.1.1/src/rez/vendor/pika/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/adapters/asyncio_connection.py` & `rez-3.1.1/src/rez/vendor/pika/adapters/asyncio_connection.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/adapters/base_connection.py` & `rez-3.1.1/src/rez/vendor/pika/adapters/base_connection.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/adapters/blocking_connection.py` & `rez-3.1.1/src/rez/vendor/pika/adapters/blocking_connection.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/adapters/select_connection.py` & `rez-3.1.1/src/rez/vendor/pika/adapters/select_connection.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/adapters/utils/connection_workflow.py` & `rez-3.1.1/src/rez/vendor/pika/adapters/utils/connection_workflow.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/adapters/utils/io_services_utils.py` & `rez-3.1.1/src/rez/vendor/pika/adapters/utils/io_services_utils.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/adapters/utils/nbio_interface.py` & `rez-3.1.1/src/rez/vendor/pika/adapters/utils/nbio_interface.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/adapters/utils/selector_ioloop_adapter.py` & `rez-3.1.1/src/rez/vendor/pika/adapters/utils/selector_ioloop_adapter.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/amqp_object.py` & `rez-3.1.1/src/rez/vendor/pika/amqp_object.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/callback.py` & `rez-3.1.1/src/rez/vendor/pika/callback.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/channel.py` & `rez-3.1.1/src/rez/vendor/pika/channel.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/compat.py` & `rez-3.1.1/src/rez/vendor/pika/compat.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/connection.py` & `rez-3.1.1/src/rez/vendor/pika/connection.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/credentials.py` & `rez-3.1.1/src/rez/vendor/pika/credentials.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/data.py` & `rez-3.1.1/src/rez/vendor/pika/data.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/diagnostic_utils.py` & `rez-3.1.1/src/rez/vendor/pika/diagnostic_utils.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/exceptions.py` & `rez-3.1.1/src/rez/vendor/pika/exceptions.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/frame.py` & `rez-3.1.1/src/rez/vendor/pika/frame.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/heartbeat.py` & `rez-3.1.1/src/rez/vendor/pika/heartbeat.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/spec.py` & `rez-3.1.1/src/rez/vendor/pika/spec.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/tcp_socket_opts.py` & `rez-3.1.1/src/rez/vendor/pika/tcp_socket_opts.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pika/validators.py` & `rez-3.1.1/src/rez/vendor/pika/validators.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/progress/__init__.py` & `rez-3.1.1/src/rez/vendor/progress/__init__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/progress/bar.py` & `rez-3.1.1/src/rez/vendor/progress/bar.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/progress/counter.py` & `rez-3.1.1/src/rez/vendor/progress/counter.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/progress/helpers.py` & `rez-3.1.1/src/rez/vendor/progress/helpers.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/progress/spinner.py` & `rez-3.1.1/src/rez/vendor/progress/spinner.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pydot/README` & `rez-3.1.1/src/rez/vendor/pydot/README`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pydot/dot_parser.py` & `rez-3.1.1/src/rez/vendor/pydot/dot_parser.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pydot/pydot.py` & `rez-3.1.1/src/rez/vendor/pydot/pydot.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/__init__.py` & `rez-3.1.1/src/rez/vendor/pygraph/__init__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/algorithms/__init__.py` & `rez-3.1.1/src/rez/vendor/pygraph/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/algorithms/accessibility.py` & `rez-3.1.1/src/rez/vendor/pygraph/algorithms/accessibility.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/algorithms/critical.py` & `rez-3.1.1/src/rez/vendor/pygraph/algorithms/critical.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/algorithms/cycles.py` & `rez-3.1.1/src/rez/vendor/pygraph/algorithms/cycles.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/algorithms/filters/__init__.py` & `rez-3.1.1/src/rez/vendor/pygraph/algorithms/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/algorithms/filters/find.py` & `rez-3.1.1/src/rez/vendor/pygraph/algorithms/filters/find.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/algorithms/filters/null.py` & `rez-3.1.1/src/rez/vendor/pygraph/algorithms/filters/null.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/algorithms/filters/radius.py` & `rez-3.1.1/src/rez/vendor/pygraph/algorithms/filters/radius.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/algorithms/generators.py` & `rez-3.1.1/src/rez/vendor/pygraph/algorithms/generators.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/algorithms/heuristics/__init__.py` & `rez-3.1.1/src/rez/vendor/pygraph/algorithms/heuristics/__init__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/algorithms/heuristics/chow.py` & `rez-3.1.1/src/rez/vendor/pygraph/algorithms/heuristics/chow.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/algorithms/heuristics/euclidean.py` & `rez-3.1.1/src/rez/vendor/pygraph/algorithms/heuristics/euclidean.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/algorithms/minmax.py` & `rez-3.1.1/src/rez/vendor/pygraph/algorithms/minmax.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/algorithms/pagerank.py` & `rez-3.1.1/src/rez/vendor/pygraph/algorithms/pagerank.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/algorithms/searching.py` & `rez-3.1.1/src/rez/vendor/pygraph/algorithms/searching.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/algorithms/sorting.py` & `rez-3.1.1/src/rez/vendor/pygraph/algorithms/sorting.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/algorithms/traversal.py` & `rez-3.1.1/src/rez/vendor/pygraph/algorithms/traversal.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/algorithms/utils.py` & `rez-3.1.1/src/rez/vendor/pygraph/algorithms/utils.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/classes/__init__.py` & `rez-3.1.1/src/rez/vendor/pygraph/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/classes/digraph.py` & `rez-3.1.1/src/rez/vendor/pygraph/classes/digraph.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/classes/exceptions.py` & `rez-3.1.1/src/rez/vendor/pygraph/classes/exceptions.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/classes/graph.py` & `rez-3.1.1/src/rez/vendor/pygraph/classes/graph.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/classes/hypergraph.py` & `rez-3.1.1/src/rez/vendor/pygraph/classes/hypergraph.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/mixins/__init__.py` & `rez-3.1.1/src/rez/vendor/pygraph/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/mixins/basegraph.py` & `rez-3.1.1/src/rez/vendor/pygraph/mixins/basegraph.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/mixins/common.py` & `rez-3.1.1/src/rez/vendor/pygraph/mixins/common.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/mixins/labeling.py` & `rez-3.1.1/src/rez/vendor/pygraph/mixins/labeling.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/readwrite/__init__.py` & `rez-3.1.1/src/rez/vendor/pygraph/readwrite/__init__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/readwrite/dot.py` & `rez-3.1.1/src/rez/vendor/pygraph/readwrite/dot.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pygraph/readwrite/markup.py` & `rez-3.1.1/src/rez/vendor/pygraph/readwrite/markup.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/pyparsing/pyparsing.py` & `rez-3.1.1/src/rez/vendor/pyparsing/pyparsing.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/schema/schema.py` & `rez-3.1.1/src/rez/vendor/schema/schema.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/schema/test_schema.py` & `rez-3.1.1/src/rez/vendor/schema/test_schema.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/six/README` & `rez-3.1.1/src/rez/vendor/six/README`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/six/six.py` & `rez-3.1.1/src/rez/vendor/six/six.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib/__init__.py` & `rez-3.1.1/src/rez/vendor/yaml/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib/composer.py` & `rez-3.1.1/src/rez/vendor/yaml/lib/composer.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib/constructor.py` & `rez-3.1.1/src/rez/vendor/yaml/lib/constructor.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib/cyaml.py` & `rez-3.1.1/src/rez/vendor/yaml/lib/cyaml.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib/dumper.py` & `rez-3.1.1/src/rez/vendor/yaml/lib/dumper.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib/emitter.py` & `rez-3.1.1/src/rez/vendor/yaml/lib/emitter.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib/error.py` & `rez-3.1.1/src/rez/vendor/yaml/lib/error.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib/events.py` & `rez-3.1.1/src/rez/vendor/yaml/lib/events.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib/loader.py` & `rez-3.1.1/src/rez/vendor/yaml/lib/loader.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib/nodes.py` & `rez-3.1.1/src/rez/vendor/yaml/lib/nodes.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib/parser.py` & `rez-3.1.1/src/rez/vendor/yaml/lib/parser.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib/reader.py` & `rez-3.1.1/src/rez/vendor/yaml/lib/reader.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib/representer.py` & `rez-3.1.1/src/rez/vendor/yaml/lib/representer.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib/resolver.py` & `rez-3.1.1/src/rez/vendor/yaml/lib/resolver.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib/scanner.py` & `rez-3.1.1/src/rez/vendor/yaml/lib/scanner.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib/serializer.py` & `rez-3.1.1/src/rez/vendor/yaml/lib/serializer.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib/tokens.py` & `rez-3.1.1/src/rez/vendor/yaml/lib/tokens.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib3/__init__.py` & `rez-3.1.1/src/rez/vendor/yaml/lib3/__init__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib3/composer.py` & `rez-3.1.1/src/rez/vendor/yaml/lib3/composer.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib3/constructor.py` & `rez-3.1.1/src/rez/vendor/yaml/lib3/constructor.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib3/cyaml.py` & `rez-3.1.1/src/rez/vendor/yaml/lib3/cyaml.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib3/dumper.py` & `rez-3.1.1/src/rez/vendor/yaml/lib3/dumper.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib3/emitter.py` & `rez-3.1.1/src/rez/vendor/yaml/lib3/emitter.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib3/error.py` & `rez-3.1.1/src/rez/vendor/yaml/lib3/error.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib3/events.py` & `rez-3.1.1/src/rez/vendor/yaml/lib3/events.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib3/loader.py` & `rez-3.1.1/src/rez/vendor/yaml/lib3/loader.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib3/nodes.py` & `rez-3.1.1/src/rez/vendor/yaml/lib3/nodes.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib3/parser.py` & `rez-3.1.1/src/rez/vendor/yaml/lib3/parser.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib3/reader.py` & `rez-3.1.1/src/rez/vendor/yaml/lib3/reader.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib3/representer.py` & `rez-3.1.1/src/rez/vendor/yaml/lib3/representer.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib3/resolver.py` & `rez-3.1.1/src/rez/vendor/yaml/lib3/resolver.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib3/scanner.py` & `rez-3.1.1/src/rez/vendor/yaml/lib3/scanner.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib3/serializer.py` & `rez-3.1.1/src/rez/vendor/yaml/lib3/serializer.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/vendor/yaml/lib3/tokens.py` & `rez-3.1.1/src/rez/vendor/yaml/lib3/tokens.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/version/__init__.py` & `rez-3.1.1/src/rez/version/__init__.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/version/_requirement.py` & `rez-3.1.1/src/rez/version/_requirement.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/version/_util.py` & `rez-3.1.1/src/rez/version/_util.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/version/_version.py` & `rez-3.1.1/src/rez/version/_version.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez/wrapper.py` & `rez-3.1.1/src/rez/wrapper.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rez.egg-info/PKG-INFO` & `rez-3.1.1/src/rez.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rez
-Version: 3.1.0
+Version: 3.1.1
 Summary: A cross-platform packaging system that can build and install multiple version of packages, and dynamically configure resolved environments at runtime.
 Home-page: https://github.com/AcademySoftwareFoundation/rez
 Author: Allan Johns
 Author-email: nerdvegas@gmail.com
 Maintainer: Contributors to the rez project
 Maintainer-email: rez-discussion@lists.aswf.io
 License: Apache-2.0
```

### Comparing `rez-3.1.0/src/rez.egg-info/SOURCES.txt` & `rez-3.1.1/src/rez.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -255,14 +255,16 @@
 src/rez/data/tests/solver/packages/test_variant_split_end/4.0/package.py
 src/rez/data/tests/solver/packages/test_variant_split_mid1/1.0/package.py
 src/rez/data/tests/solver/packages/test_variant_split_mid1/2.0/package.py
 src/rez/data/tests/solver/packages/test_variant_split_mid2/1.0/package.py
 src/rez/data/tests/solver/packages/test_variant_split_mid2/2.0/package.py
 src/rez/data/tests/solver/packages/test_variant_split_start/1.0/package.py
 src/rez/data/tests/solver/packages/test_variant_split_start/2.0/package.py
+src/rez/data/tests/solver/packages/test_weakly_reference_requires/2.0/package.py
+src/rez/data/tests/solver/packages/test_weakly_reference_variant/2.0/package.py
 src/rez/data/tests/suites/packages/bah/package.yaml
 src/rez/data/tests/suites/packages/eek/package.yaml
 src/rez/data/tests/suites/packages/foo/package.yaml
 src/rez/data/tests/suites/packages/pooh/package.yaml
 src/rez/data/tests/suites/packages/pooh/bin/hunny
 src/rez/data/tests/suites/packages/pooh/bin/hunny.bat
 src/rez/tests/README
@@ -639,20 +641,19 @@
 src/rezgui/windows/ContextSubWindow.py
 src/rezgui/windows/MainWindow.py
 src/rezgui/windows/__init__.py
 src/rezplugins/__init__.py
 src/rezplugins/build_process/__init__.py
 src/rezplugins/build_process/local.py
 src/rezplugins/build_process/remote.py
-src/rezplugins/build_process/rezconfig
+src/rezplugins/build_process/rezconfig.py
 src/rezplugins/build_system/__init__.py
 src/rezplugins/build_system/cmake.py
 src/rezplugins/build_system/custom.py
 src/rezplugins/build_system/make.py
-src/rezplugins/build_system/rezconfig
 src/rezplugins/build_system/rezconfig.py
 src/rezplugins/build_system/cmake_files/Colorize.cmake
 src/rezplugins/build_system/cmake_files/FindStaticLibs.cmake
 src/rezplugins/build_system/cmake_files/InstallDirs.cmake
 src/rezplugins/build_system/cmake_files/InstallFiles.cmake
 src/rezplugins/build_system/cmake_files/InstallPython.cmake
 src/rezplugins/build_system/cmake_files/RezBuild.cmake
@@ -666,34 +667,34 @@
 src/rezplugins/build_system/cmake_files/RezRepository.cmake
 src/rezplugins/build_system/cmake_files/Utils.cmake
 src/rezplugins/build_system/template_files/Doxyfile
 src/rezplugins/command/__init__.py
 src/rezplugins/package_repository/__init__.py
 src/rezplugins/package_repository/filesystem.py
 src/rezplugins/package_repository/memory.py
-src/rezplugins/package_repository/rezconfig
+src/rezplugins/package_repository/rezconfig.py
 src/rezplugins/release_hook/__init__.py
 src/rezplugins/release_hook/amqp.py
 src/rezplugins/release_hook/command.py
 src/rezplugins/release_hook/emailer.py
-src/rezplugins/release_hook/rezconfig
+src/rezplugins/release_hook/rezconfig.py
 src/rezplugins/release_vcs/__init__.py
 src/rezplugins/release_vcs/git.py
 src/rezplugins/release_vcs/hg.py
-src/rezplugins/release_vcs/rezconfig
+src/rezplugins/release_vcs/rezconfig.py
 src/rezplugins/release_vcs/stub.py
 src/rezplugins/release_vcs/svn.py
 src/rezplugins/shell/__init__.py
 src/rezplugins/shell/bash.py
 src/rezplugins/shell/cmd.py
 src/rezplugins/shell/csh.py
 src/rezplugins/shell/gitbash.py
 src/rezplugins/shell/powershell.py
 src/rezplugins/shell/pwsh.py
-src/rezplugins/shell/rezconfig
+src/rezplugins/shell/rezconfig.py
 src/rezplugins/shell/sh.py
 src/rezplugins/shell/tcsh.py
 src/rezplugins/shell/zsh.py
 src/rezplugins/shell/_utils/__init__.py
 src/rezplugins/shell/_utils/powershell_base.py
 src/rezplugins/shell/_utils/windows.py
 tests/test.py
```

### Comparing `rez-3.1.0/src/rez.egg-info/entry_points.txt` & `rez-3.1.1/src/rez.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/app.py` & `rez-3.1.1/src/rezgui/app.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/dialogs/AboutDialog.py` & `rez-3.1.1/src/rezgui/dialogs/AboutDialog.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/dialogs/BrowsePackageDialog.py` & `rez-3.1.1/src/rezgui/dialogs/BrowsePackageDialog.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/dialogs/ImageViewerDialog.py` & `rez-3.1.1/src/rezgui/dialogs/ImageViewerDialog.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/dialogs/ProcessDialog.py` & `rez-3.1.1/src/rezgui/dialogs/ProcessDialog.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/dialogs/ResolveDialog.py` & `rez-3.1.1/src/rezgui/dialogs/ResolveDialog.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/dialogs/VariantVersionsDialog.py` & `rez-3.1.1/src/rezgui/dialogs/VariantVersionsDialog.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/dialogs/WriteGraphDialog.py` & `rez-3.1.1/src/rezgui/dialogs/WriteGraphDialog.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/advanced_resolve.png` & `rez-3.1.1/src/rezgui/icons/advanced_resolve.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/changelog.png` & `rez-3.1.1/src/rezgui/icons/changelog.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/clock.png` & `rez-3.1.1/src/rezgui/icons/clock.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/clock_warning.png` & `rez-3.1.1/src/rezgui/icons/clock_warning.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/context.png` & `rez-3.1.1/src/rezgui/icons/context.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/context_settings.png` & `rez-3.1.1/src/rezgui/icons/context_settings.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/diff.png` & `rez-3.1.1/src/rezgui/icons/diff.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/diff_to_disk.png` & `rez-3.1.1/src/rezgui/icons/diff_to_disk.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/diff_to_other.png` & `rez-3.1.1/src/rezgui/icons/diff_to_other.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/equal_to.png` & `rez-3.1.1/src/rezgui/icons/equal_to.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/equalish.png` & `rez-3.1.1/src/rezgui/icons/equalish.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/error.png` & `rez-3.1.1/src/rezgui/icons/error.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/excluded.png` & `rez-3.1.1/src/rezgui/icons/excluded.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/find.png` & `rez-3.1.1/src/rezgui/icons/find.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/github_32.png` & `rez-3.1.1/src/rezgui/icons/github_32.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/graph.png` & `rez-3.1.1/src/rezgui/icons/graph.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/greater_than.png` & `rez-3.1.1/src/rezgui/icons/greater_than.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/greater_than_1.png` & `rez-3.1.1/src/rezgui/icons/greater_than_1.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/greater_than_2.png` & `rez-3.1.1/src/rezgui/icons/greater_than_2.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/greater_than_3.png` & `rez-3.1.1/src/rezgui/icons/greater_than_3.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/green_tick.png` & `rez-3.1.1/src/rezgui/icons/green_tick.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/green_white_tick.png` & `rez-3.1.1/src/rezgui/icons/green_white_tick.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/help.png` & `rez-3.1.1/src/rezgui/icons/help.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/info.png` & `rez-3.1.1/src/rezgui/icons/info.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/less_than.png` & `rez-3.1.1/src/rezgui/icons/less_than.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/less_than_1.png` & `rez-3.1.1/src/rezgui/icons/less_than_1.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/less_than_2.png` & `rez-3.1.1/src/rezgui/icons/less_than_2.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/less_than_3.png` & `rez-3.1.1/src/rezgui/icons/less_than_3.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/local.png` & `rez-3.1.1/src/rezgui/icons/local.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/missing.png` & `rez-3.1.1/src/rezgui/icons/missing.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/new.png` & `rez-3.1.1/src/rezgui/icons/new.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/no_lock.png` & `rez-3.1.1/src/rezgui/icons/no_lock.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/no_lock_faint.png` & `rez-3.1.1/src/rezgui/icons/no_lock_faint.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/old_man.png` & `rez-3.1.1/src/rezgui/icons/old_man.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/package.png` & `rez-3.1.1/src/rezgui/icons/package.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/resolve.png` & `rez-3.1.1/src/rezgui/icons/resolve.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/revert.png` & `rez-3.1.1/src/rezgui/icons/revert.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/revert_to_diff.png` & `rez-3.1.1/src/rezgui/icons/revert_to_diff.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/revert_to_disk.png` & `rez-3.1.1/src/rezgui/icons/revert_to_disk.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/terminal.png` & `rez-3.1.1/src/rezgui/icons/terminal.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/versions.png` & `rez-3.1.1/src/rezgui/icons/versions.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/warning.png` & `rez-3.1.1/src/rezgui/icons/warning.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/yellow_tick.png` & `rez-3.1.1/src/rezgui/icons/yellow_tick.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/icons/yellow_white_tick.png` & `rez-3.1.1/src/rezgui/icons/yellow_white_tick.png`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/mixins/ContextViewMixin.py` & `rez-3.1.1/src/rezgui/mixins/ContextViewMixin.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/mixins/StoreSizeMixin.py` & `rez-3.1.1/src/rezgui/mixins/StoreSizeMixin.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/models/ContextModel.py` & `rez-3.1.1/src/rezgui/models/ContextModel.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/objects/App.py` & `rez-3.1.1/src/rezgui/objects/App.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/objects/Config.py` & `rez-3.1.1/src/rezgui/objects/Config.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/objects/LoadPackagesThread.py` & `rez-3.1.1/src/rezgui/objects/LoadPackagesThread.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/objects/ProcessTrackerThread.py` & `rez-3.1.1/src/rezgui/objects/ProcessTrackerThread.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/objects/ResolveThread.py` & `rez-3.1.1/src/rezgui/objects/ResolveThread.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/rezguiconfig` & `rez-3.1.1/src/rezgui/rezguiconfig`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/util.py` & `rez-3.1.1/src/rezgui/util.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/BrowsePackagePane.py` & `rez-3.1.1/src/rezgui/widgets/BrowsePackagePane.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/BrowsePackageWidget.py` & `rez-3.1.1/src/rezgui/widgets/BrowsePackageWidget.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/ChangelogEdit.py` & `rez-3.1.1/src/rezgui/widgets/ChangelogEdit.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/ConfiguredSplitter.py` & `rez-3.1.1/src/rezgui/widgets/ConfiguredSplitter.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/ContextDetailsWidget.py` & `rez-3.1.1/src/rezgui/widgets/ContextDetailsWidget.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/ContextEnvironTable.py` & `rez-3.1.1/src/rezgui/widgets/ContextEnvironTable.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/ContextEnvironWidget.py` & `rez-3.1.1/src/rezgui/widgets/ContextEnvironWidget.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/ContextManagerWidget.py` & `rez-3.1.1/src/rezgui/widgets/ContextManagerWidget.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/ContextResolveTimeLabel.py` & `rez-3.1.1/src/rezgui/widgets/ContextResolveTimeLabel.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/ContextSettingsWidget.py` & `rez-3.1.1/src/rezgui/widgets/ContextSettingsWidget.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/ContextTableWidget.py` & `rez-3.1.1/src/rezgui/widgets/ContextTableWidget.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/ContextToolsWidget.py` & `rez-3.1.1/src/rezgui/widgets/ContextToolsWidget.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/EffectivePackageCellWidget.py` & `rez-3.1.1/src/rezgui/widgets/EffectivePackageCellWidget.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/FindPopup.py` & `rez-3.1.1/src/rezgui/widgets/FindPopup.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/IconButton.py` & `rez-3.1.1/src/rezgui/widgets/IconButton.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/ImageViewerWidget.py` & `rez-3.1.1/src/rezgui/widgets/ImageViewerWidget.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/PackageLineEdit.py` & `rez-3.1.1/src/rezgui/widgets/PackageLineEdit.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/PackageLoadingWidget.py` & `rez-3.1.1/src/rezgui/widgets/PackageLoadingWidget.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/PackageSelectWidget.py` & `rez-3.1.1/src/rezgui/widgets/PackageSelectWidget.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/PackageTabWidget.py` & `rez-3.1.1/src/rezgui/widgets/PackageTabWidget.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/PackageVersionsTable.py` & `rez-3.1.1/src/rezgui/widgets/PackageVersionsTable.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/SearchableTextEdit.py` & `rez-3.1.1/src/rezgui/widgets/SearchableTextEdit.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/StreamableTextEdit.py` & `rez-3.1.1/src/rezgui/widgets/StreamableTextEdit.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/TimeSelecterPopup.py` & `rez-3.1.1/src/rezgui/widgets/TimeSelecterPopup.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/TimestampWidget.py` & `rez-3.1.1/src/rezgui/widgets/TimestampWidget.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/ToolWidget.py` & `rez-3.1.1/src/rezgui/widgets/ToolWidget.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/VariantCellWidget.py` & `rez-3.1.1/src/rezgui/widgets/VariantCellWidget.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/VariantDetailsWidget.py` & `rez-3.1.1/src/rezgui/widgets/VariantDetailsWidget.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/VariantHelpWidget.py` & `rez-3.1.1/src/rezgui/widgets/VariantHelpWidget.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/VariantSummaryWidget.py` & `rez-3.1.1/src/rezgui/widgets/VariantSummaryWidget.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/VariantToolsList.py` & `rez-3.1.1/src/rezgui/widgets/VariantToolsList.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/VariantVersionsTable.py` & `rez-3.1.1/src/rezgui/widgets/VariantVersionsTable.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/VariantVersionsWidget.py` & `rez-3.1.1/src/rezgui/widgets/VariantVersionsWidget.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/VariantsList.py` & `rez-3.1.1/src/rezgui/widgets/VariantsList.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/widgets/ViewGraphButton.py` & `rez-3.1.1/src/rezgui/widgets/ViewGraphButton.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/windows/BrowsePackageSubWindow.py` & `rez-3.1.1/src/rezgui/windows/BrowsePackageSubWindow.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/windows/ContextSubWindow.py` & `rez-3.1.1/src/rezgui/windows/ContextSubWindow.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezgui/windows/MainWindow.py` & `rez-3.1.1/src/rezgui/windows/MainWindow.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/build_process/local.py` & `rez-3.1.1/src/rezplugins/build_process/local.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/build_process/remote.py` & `rez-3.1.1/src/rezplugins/build_process/remote.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/build_system/cmake.py` & `rez-3.1.1/src/rezplugins/build_system/cmake.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/build_system/cmake_files/Colorize.cmake` & `rez-3.1.1/src/rezplugins/build_system/cmake_files/Colorize.cmake`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/build_system/cmake_files/FindStaticLibs.cmake` & `rez-3.1.1/src/rezplugins/build_system/cmake_files/FindStaticLibs.cmake`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/build_system/cmake_files/InstallDirs.cmake` & `rez-3.1.1/src/rezplugins/build_system/cmake_files/InstallDirs.cmake`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/build_system/cmake_files/InstallFiles.cmake` & `rez-3.1.1/src/rezplugins/build_system/cmake_files/InstallFiles.cmake`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/build_system/cmake_files/InstallPython.cmake` & `rez-3.1.1/src/rezplugins/build_system/cmake_files/InstallPython.cmake`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/build_system/cmake_files/RezBuild.cmake` & `rez-3.1.1/src/rezplugins/build_system/cmake_files/RezBuild.cmake`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/build_system/cmake_files/RezFindPackages.cmake` & `rez-3.1.1/src/rezplugins/build_system/cmake_files/RezFindPackages.cmake`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/build_system/cmake_files/RezInstallCMake.cmake` & `rez-3.1.1/src/rezplugins/build_system/cmake_files/RezInstallCMake.cmake`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/build_system/cmake_files/RezInstallContext.cmake` & `rez-3.1.1/src/rezplugins/build_system/cmake_files/RezInstallContext.cmake`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/build_system/cmake_files/RezInstallDoxygen.cmake` & `rez-3.1.1/src/rezplugins/build_system/cmake_files/RezInstallDoxygen.cmake`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/build_system/cmake_files/RezInstallPython.cmake` & `rez-3.1.1/src/rezplugins/build_system/cmake_files/RezInstallPython.cmake`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/build_system/cmake_files/RezPipInstall.cmake` & `rez-3.1.1/src/rezplugins/build_system/cmake_files/RezPipInstall.cmake`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/build_system/cmake_files/RezProject.cmake` & `rez-3.1.1/src/rezplugins/build_system/cmake_files/RezProject.cmake`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/build_system/cmake_files/RezRepository.cmake` & `rez-3.1.1/src/rezplugins/build_system/cmake_files/RezRepository.cmake`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/build_system/cmake_files/Utils.cmake` & `rez-3.1.1/src/rezplugins/build_system/cmake_files/Utils.cmake`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/build_system/custom.py` & `rez-3.1.1/src/rezplugins/build_system/custom.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/build_system/make.py` & `rez-3.1.1/src/rezplugins/build_system/make.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/build_system/rezconfig.py` & `rez-3.1.1/src/rezplugins/build_system/rezconfig.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/build_system/template_files/Doxyfile` & `rez-3.1.1/src/rezplugins/build_system/template_files/Doxyfile`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/package_repository/filesystem.py` & `rez-3.1.1/src/rezplugins/package_repository/filesystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -463,15 +463,15 @@
                 - python-2.5
             '1.1+':
                 requires:
                 - python-2.6
     """
     schema_dict = {"file_lock_timeout": int,
                    "file_lock_dir": Or(None, str),
-                   "file_lock_type": Or("default", "link", "mkdir"),
+                   "file_lock_type": Or("default", "link", "mkdir", "symlink"),
                    "package_filenames": [str]}
 
     building_prefix = ".building"
     ignore_prefix = ".ignore"
 
     package_file_mode = (
         None if os.name == "nt" else
@@ -969,14 +969,16 @@
 
         if _settings.file_lock_type == 'default':
             from rez.vendor.lockfile import LockFile
         elif _settings.file_lock_type == 'mkdir':
             from rez.vendor.lockfile.mkdirlockfile import MkdirLockFile as LockFile
         elif _settings.file_lock_type == 'link':
             from rez.vendor.lockfile.linklockfile import LinkLockFile as LockFile
+        elif _settings.file_lock_type == 'symlink':
+            from rez.vendor.lockfile.symlinklockfile import SymlinkLockFile as LockFile
 
         path = self.location
 
         if self.file_lock_dir:
             path = os.path.join(path, self.file_lock_dir)
 
         if not os.path.exists(path):
```

### Comparing `rez-3.1.0/src/rezplugins/package_repository/memory.py` & `rez-3.1.1/src/rezplugins/package_repository/memory.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/package_repository/rezconfig` & `rez-3.1.1/src/rezplugins/package_repository/rezconfig.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,48 @@
-filesystem:
+# SPDX-License-Identifier: Apache-2.0
+# Copyright Contributors to the Rez Project
+
+
+filesystem = {
     # The mechanism used to create the lockfile. If set to 'default', this will
-    # use hardlinks if the 'os.link' method is present, otherwise mkdir is used.
-    # It can also be explicitly set to use only 'hardlink', or only 'mkdir'.
-    # Valid options are 'default', 'mkdir', or 'hardlink'
-    file_lock_type: default
+    # use hardlinks (link) if the 'os.link' method is present, otherwise mkdir is used.
+    # Valid options are 'default', 'mkdir', 'link', or 'symlink'
+    "file_lock_type": "default",
 
     # The timeout to use when creating file locks. This is done when a variant is
     # installed into an existing package, to prevent multiple file writes at
     # once (which could result in a variant install getting lost). The timeout
     # value is in seconds. A value of zero indicates no timeout.
-    file_lock_timeout: 10
+    "file_lock_timeout": 10,
 
     # The relative directory, under the repository location, where file locks
     # are created. You might need to use this option when file permissions are
     # locked down so that only certain users can release certain packages. In
     # this scenario, package releases may fail because a user with limited
     # permissions will fail to create the lockfile in the repository root. By
     # providing a subdirectory, you can open up the permissions on this
     # directory only. If null, lockfiles are left created in the root.
     #
     # Note: The directory can have any name, but we suggest '.lock' as the
     # standard convention.
-    file_lock_dir:
+    "file_lock_dir": None,
 
     # If True, verify that a potential package directory contains a package.py /
     # package.yaml file before treating it as a package. There *shouldn't* be
     # non-packages in these directories, and the solver is faster if this value
     # is False, because a lot of file stats are avoided.
-    check_package_definition_files: false
+    "check_package_definition_files": False,
 
     # A list of filenames that are expected to contain Rez definitions.
     # The list will be checked in top to bottom order, and the first filename
     # that contains a valid package definition will be used. You might need to
     # use this option if the name 'package.[py/yaml]' is being used by a different
     # packaging system.
     #
     # Please note: The first filename in this list is used as the installed /
     # released package filename, regardless of the definition filename present
     # in the source.
     #
-    package_filenames:
-    - 'package'
+    "package_filenames": [
+        "package"
+    ]
+}
```

### Comparing `rez-3.1.0/src/rezplugins/release_hook/amqp.py` & `rez-3.1.1/src/rezplugins/release_hook/amqp.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/release_hook/command.py` & `rez-3.1.1/src/rezplugins/release_hook/command.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/release_hook/emailer.py` & `rez-3.1.1/src/rezplugins/release_hook/emailer.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/release_vcs/git.py` & `rez-3.1.1/src/rezplugins/release_vcs/git.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/release_vcs/hg.py` & `rez-3.1.1/src/rezplugins/release_vcs/hg.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/release_vcs/stub.py` & `rez-3.1.1/src/rezplugins/release_vcs/stub.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/release_vcs/svn.py` & `rez-3.1.1/src/rezplugins/release_vcs/svn.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/shell/_utils/powershell_base.py` & `rez-3.1.1/src/rezplugins/shell/_utils/powershell_base.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/shell/_utils/windows.py` & `rez-3.1.1/src/rezplugins/shell/_utils/windows.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/shell/bash.py` & `rez-3.1.1/src/rezplugins/shell/bash.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/shell/cmd.py` & `rez-3.1.1/src/rezplugins/shell/cmd.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/shell/csh.py` & `rez-3.1.1/src/rezplugins/shell/csh.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/shell/gitbash.py` & `rez-3.1.1/src/rezplugins/shell/gitbash.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/shell/pwsh.py` & `rez-3.1.1/src/rezplugins/shell/pwsh.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/shell/sh.py` & `rez-3.1.1/src/rezplugins/shell/sh.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/shell/tcsh.py` & `rez-3.1.1/src/rezplugins/shell/tcsh.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/src/rezplugins/shell/zsh.py` & `rez-3.1.1/src/rezplugins/shell/zsh.py`

 * *Files identical despite different names*

### Comparing `rez-3.1.0/tests/test.py` & `rez-3.1.1/tests/test.py`

 * *Files identical despite different names*


# Comparing `tmp/libfcrypto-python-20240115.tar.gz` & `tmp/libfcrypto-python-20240414.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libfcrypto-python-20240115.tar", last modified: Mon Jan 15 04:25:43 2024, max compression
+gzip compressed data, was "libfcrypto-python-20240414.tar", last modified: Sun Apr 14 10:13:32 2024, max compression
```

## Comparing `libfcrypto-python-20240115.tar` & `libfcrypto-python-20240414.tar`

### file list

```diff
@@ -1,227 +1,230 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:43.000000 libfcrypto-20240115/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1974 2024-01-15 04:23:28.000000 libfcrypto-20240115/libfcrypto.spec
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-01-15 04:20:15.000000 libfcrypto-20240115/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-01-15 04:23:21.000000 libfcrypto-20240115/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:20:15.000000 libfcrypto-20240115/NEWS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:43.000000 libfcrypto-20240115/pyfcrypto/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8158 2024-01-15 04:20:15.000000 libfcrypto-20240115/pyfcrypto/pyfcrypto_blowfish_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8071 2024-01-15 04:20:15.000000 libfcrypto-20240115/pyfcrypto/pyfcrypto_serpent_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-01-15 04:20:15.000000 libfcrypto-20240115/pyfcrypto/pyfcrypto_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2044 2024-01-15 04:20:15.000000 libfcrypto-20240115/pyfcrypto/pyfcrypto_crypt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1899 2024-01-15 04:20:15.000000 libfcrypto-20240115/pyfcrypto/pyfcrypto_rc4_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7751 2024-01-15 04:22:04.000000 libfcrypto-20240115/pyfcrypto/pyfcrypto.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      932 2024-01-14 11:10:31.000000 libfcrypto-20240115/pyfcrypto/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7795 2024-01-15 04:20:15.000000 libfcrypto-20240115/pyfcrypto/pyfcrypto_rc4_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1921 2024-01-15 04:20:15.000000 libfcrypto-20240115/pyfcrypto/pyfcrypto_des3_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1987 2024-01-15 04:20:15.000000 libfcrypto-20240115/pyfcrypto/pyfcrypto_serpent_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5592 2024-01-15 04:20:15.000000 libfcrypto-20240115/pyfcrypto/pyfcrypto_crypt_modes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9586 2024-01-15 04:20:15.000000 libfcrypto-20240115/pyfcrypto/pyfcrypto_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1558 2024-01-15 04:20:15.000000 libfcrypto-20240115/pyfcrypto/pyfcrypto_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      989 2024-01-15 04:20:15.000000 libfcrypto-20240115/pyfcrypto/pyfcrypto_libfcrypto.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-15 04:20:15.000000 libfcrypto-20240115/pyfcrypto/pyfcrypto_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1331 2024-01-15 04:20:15.000000 libfcrypto-20240115/pyfcrypto/pyfcrypto.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-15 04:20:15.000000 libfcrypto-20240115/pyfcrypto/pyfcrypto_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2009 2024-01-15 04:20:15.000000 libfcrypto-20240115/pyfcrypto/pyfcrypto_blowfish_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27507 2024-01-15 04:20:15.000000 libfcrypto-20240115/pyfcrypto/pyfcrypto_crypt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1668 2024-01-15 04:20:15.000000 libfcrypto-20240115/pyfcrypto/pyfcrypto_crypt_modes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37155 2024-01-15 04:23:22.000000 libfcrypto-20240115/pyfcrypto/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7866 2024-01-15 04:20:15.000000 libfcrypto-20240115/pyfcrypto/pyfcrypto_des3_context.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-01-15 04:23:22.000000 libfcrypto-20240115/depcomp
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2024-01-15 04:20:15.000000 libfcrypto-20240115/libfcrypto.spec.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:42.000000 libfcrypto-20240115/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:04:04.000000 libfcrypto-20240115/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:04:04.000000 libfcrypto-20240115/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:04:04.000000 libfcrypto-20240115/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:04:04.000000 libfcrypto-20240115/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:04:04.000000 libfcrypto-20240115/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:04:04.000000 libfcrypto-20240115/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-01-15 04:23:19.000000 libfcrypto-20240115/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-01-15 04:23:19.000000 libfcrypto-20240115/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:04:04.000000 libfcrypto-20240115/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-01-15 04:23:19.000000 libfcrypto-20240115/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:04:04.000000 libfcrypto-20240115/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:04:04.000000 libfcrypto-20240115/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:04:04.000000 libfcrypto-20240115/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-01-15 04:23:19.000000 libfcrypto-20240115/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:04:04.000000 libfcrypto-20240115/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:04:04.000000 libfcrypto-20240115/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-01-15 04:23:19.000000 libfcrypto-20240115/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:04:04.000000 libfcrypto-20240115/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:04:04.000000 libfcrypto-20240115/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:04:04.000000 libfcrypto-20240115/m4/types.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:42.000000 libfcrypto-20240115/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10314 2024-01-15 04:20:15.000000 libfcrypto-20240115/include/libfcrypto.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      479 2024-01-15 04:20:15.000000 libfcrypto-20240115/include/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:42.000000 libfcrypto-20240115/include/libfcrypto/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1836 2024-01-15 04:20:15.000000 libfcrypto-20240115/include/libfcrypto/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1834 2024-01-15 04:23:28.000000 libfcrypto-20240115/include/libfcrypto/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5106 2024-01-15 04:20:15.000000 libfcrypto-20240115/include/libfcrypto/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4975 2024-01-15 04:23:28.000000 libfcrypto-20240115/include/libfcrypto/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1248 2024-01-15 04:20:15.000000 libfcrypto-20240115/include/libfcrypto/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6894 2024-01-15 04:20:15.000000 libfcrypto-20240115/include/libfcrypto/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-01-15 04:20:15.000000 libfcrypto-20240115/include/libfcrypto/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1248 2024-01-15 04:23:28.000000 libfcrypto-20240115/include/libfcrypto/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21005 2024-01-15 04:23:22.000000 libfcrypto-20240115/include/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10314 2024-01-15 04:23:28.000000 libfcrypto-20240115/include/libfcrypto.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      268 2024-01-15 04:20:15.000000 libfcrypto-20240115/libfcrypto.pc.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:42.000000 libfcrypto-20240115/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-01-15 04:20:15.000000 libfcrypto-20240115/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-01-15 04:20:15.000000 libfcrypto-20240115/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-01-15 04:20:15.000000 libfcrypto-20240115/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-01-15 04:20:15.000000 libfcrypto-20240115/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-01-15 04:20:15.000000 libfcrypto-20240115/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-01-15 04:20:15.000000 libfcrypto-20240115/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-01-15 04:20:15.000000 libfcrypto-20240115/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-01-15 04:20:15.000000 libfcrypto-20240115/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-01-15 04:20:15.000000 libfcrypto-20240115/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7376 2024-01-15 04:23:28.000000 libfcrypto-20240115/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9229 2024-01-15 04:23:21.000000 libfcrypto-20240115/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9799 2024-01-15 04:23:03.000000 libfcrypto-20240115/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-01-15 04:20:15.000000 libfcrypto-20240115/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-01-15 04:20:15.000000 libfcrypto-20240115/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-01-15 04:20:15.000000 libfcrypto-20240115/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17999 2024-01-15 04:23:21.000000 libfcrypto-20240115/common/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1419 2023-12-03 09:03:56.000000 libfcrypto-20240115/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:03:56.000000 libfcrypto-20240115/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-01-15 04:23:21.000000 libfcrypto-20240115/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:42.000000 libfcrypto-20240115/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1030 2024-01-15 04:20:15.000000 libfcrypto-20240115/dpkg/copyright
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-01-15 04:20:15.000000 libfcrypto-20240115/dpkg/libfcrypto.install
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:42.000000 libfcrypto-20240115/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-01-15 04:20:15.000000 libfcrypto-20240115/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-01-15 04:20:15.000000 libfcrypto-20240115/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      721 2024-01-15 04:20:15.000000 libfcrypto-20240115/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-01-15 04:20:15.000000 libfcrypto-20240115/dpkg/libfcrypto-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      123 2024-01-15 04:20:15.000000 libfcrypto-20240115/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-01-15 04:20:15.000000 libfcrypto-20240115/dpkg/libfcrypto-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      142 2024-01-15 04:23:28.000000 libfcrypto-20240115/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-01-15 04:20:15.000000 libfcrypto-20240115/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      488 2024-01-15 04:23:28.000000 libfcrypto-20240115/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-01-15 04:20:15.000000 libfcrypto-20240115/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)   838518 2024-01-15 04:23:21.000000 libfcrypto-20240115/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-01-15 04:23:21.000000 libfcrypto-20240115/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-01-15 04:23:21.000000 libfcrypto-20240115/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:43.000000 libfcrypto-20240115/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:43.000000 libfcrypto-20240115/msvscpp/fcrypto_test_rc4_context/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4917 2024-01-15 04:20:17.000000 libfcrypto-20240115/msvscpp/fcrypto_test_rc4_context/fcrypto_test_rc4_context.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:43.000000 libfcrypto-20240115/msvscpp/pyfcrypto/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6032 2024-01-15 04:20:17.000000 libfcrypto-20240115/msvscpp/pyfcrypto/pyfcrypto.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      595 2024-01-15 04:20:17.000000 libfcrypto-20240115/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:43.000000 libfcrypto-20240115/msvscpp/fcrypto_test_serpent_context/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4929 2024-01-15 04:20:17.000000 libfcrypto-20240115/msvscpp/fcrypto_test_serpent_context/fcrypto_test_serpent_context.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:43.000000 libfcrypto-20240115/msvscpp/fcrypto_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4647 2024-01-15 04:20:17.000000 libfcrypto-20240115/msvscpp/fcrypto_test_error/fcrypto_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:43.000000 libfcrypto-20240115/msvscpp/fcrypto_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-01-15 04:20:17.000000 libfcrypto-20240115/msvscpp/fcrypto_test_support/fcrypto_test_support.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6622 2024-01-15 04:20:17.000000 libfcrypto-20240115/msvscpp/libfcrypto.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:43.000000 libfcrypto-20240115/msvscpp/libfcrypto/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5877 2024-01-15 04:20:17.000000 libfcrypto-20240115/msvscpp/libfcrypto/libfcrypto.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15562 2024-01-15 04:23:22.000000 libfcrypto-20240115/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:43.000000 libfcrypto-20240115/msvscpp/fcrypto_test_des3_context/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4920 2024-01-15 04:20:17.000000 libfcrypto-20240115/msvscpp/fcrypto_test_des3_context/fcrypto_test_des3_context.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:43.000000 libfcrypto-20240115/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-01-15 04:20:17.000000 libfcrypto-20240115/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:43.000000 libfcrypto-20240115/msvscpp/fcrypto_test_blowfish_context/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4932 2024-01-15 04:20:17.000000 libfcrypto-20240115/msvscpp/fcrypto_test_blowfish_context/fcrypto_test_blowfish_context.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       94 2024-01-15 04:20:15.000000 libfcrypto-20240115/AUTHORS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      286 2024-01-15 04:20:15.000000 libfcrypto-20240115/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-01-15 04:23:21.000000 libfcrypto-20240115/INSTALL
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-01-15 04:20:15.000000 libfcrypto-20240115/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      489 2024-01-15 04:20:15.000000 libfcrypto-20240115/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-01-15 04:23:21.000000 libfcrypto-20240115/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-01-15 04:20:15.000000 libfcrypto-20240115/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      773 2024-01-15 04:20:15.000000 libfcrypto-20240115/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:03:56.000000 libfcrypto-20240115/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:43.000000 libfcrypto-20240115/libfcrypto/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3331 2024-01-15 04:20:15.000000 libfcrypto-20240115/libfcrypto/libfcrypto_blowfish_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-01-15 04:20:15.000000 libfcrypto-20240115/libfcrypto/libfcrypto_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42088 2024-01-15 04:20:15.000000 libfcrypto-20240115/libfcrypto/libfcrypto_blowfish_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1827 2024-01-15 04:20:15.000000 libfcrypto-20240115/libfcrypto/libfcrypto.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1902 2024-01-15 04:20:15.000000 libfcrypto-20240115/libfcrypto/libfcrypto_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2103 2024-01-15 04:20:15.000000 libfcrypto-20240115/libfcrypto/libfcrypto_rc4_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2024-01-15 04:20:15.000000 libfcrypto-20240115/libfcrypto/libfcrypto_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2186 2024-01-15 04:20:15.000000 libfcrypto-20240115/libfcrypto/libfcrypto_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2184 2024-01-15 04:23:28.000000 libfcrypto-20240115/libfcrypto/libfcrypto_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9130 2024-01-15 04:20:15.000000 libfcrypto-20240115/libfcrypto/libfcrypto_rc4_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-01-14 07:04:21.000000 libfcrypto-20240115/libfcrypto/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1078 2024-01-15 04:20:15.000000 libfcrypto-20240115/libfcrypto/libfcrypto.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3115 2024-01-15 04:20:15.000000 libfcrypto-20240115/libfcrypto/libfcrypto_serpent_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    75716 2024-01-15 04:20:15.000000 libfcrypto-20240115/libfcrypto/libfcrypto_serpent_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32055 2024-01-15 04:20:15.000000 libfcrypto-20240115/libfcrypto/libfcrypto_des3_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2891 2024-01-15 04:20:15.000000 libfcrypto-20240115/libfcrypto/libfcrypto_des3_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2938 2024-01-15 04:20:15.000000 libfcrypto-20240115/libfcrypto/libfcrypto_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2024-01-15 04:20:15.000000 libfcrypto-20240115/libfcrypto/libfcrypto_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1841 2024-01-15 04:20:15.000000 libfcrypto-20240115/libfcrypto/libfcrypto_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-01-15 04:20:15.000000 libfcrypto-20240115/libfcrypto/libfcrypto_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26113 2024-01-15 04:23:22.000000 libfcrypto-20240115/libfcrypto/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-01-15 04:20:15.000000 libfcrypto-20240115/libfcrypto/libfcrypto_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1076 2024-01-15 04:23:28.000000 libfcrypto-20240115/libfcrypto/libfcrypto.rc
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-01-15 04:23:22.000000 libfcrypto-20240115/test-driver
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      419 2024-01-14 16:30:12.000000 libfcrypto-20240115/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:43.000000 libfcrypto-20240115/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      132 2023-12-03 09:04:04.000000 libfcrypto-20240115/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18209 2024-01-15 04:23:22.000000 libfcrypto-20240115/manuals/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4826 2024-01-15 04:22:04.000000 libfcrypto-20240115/manuals/libfcrypto.3
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:43.000000 libfcrypto-20240115/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-01-15 04:20:15.000000 libfcrypto-20240115/tests/fcrypto_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4794 2024-01-15 04:20:15.000000 libfcrypto-20240115/tests/fcrypto_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1584 2024-01-15 04:22:04.000000 libfcrypto-20240115/tests/pyfcrypto_test_rc4_context.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20956 2024-01-15 04:22:04.000000 libfcrypto-20240115/tests/fcrypto_test_serpent_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-01-15 04:20:15.000000 libfcrypto-20240115/tests/pyfcrypto_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8644 2024-01-15 04:20:15.000000 libfcrypto-20240115/tests/fcrypto_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34555 2024-01-15 04:22:04.000000 libfcrypto-20240115/tests/fcrypto_test_blowfish_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2568 2024-01-15 04:22:04.000000 libfcrypto-20240115/tests/pyfcrypto_test_blowfish_context.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2451 2024-01-15 04:20:15.000000 libfcrypto-20240115/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1724 2024-01-15 04:20:15.000000 libfcrypto-20240115/tests/fcrypto_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18454 2024-01-15 04:22:04.000000 libfcrypto-20240115/tests/fcrypto_test_des3_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1596 2024-01-15 04:22:04.000000 libfcrypto-20240115/tests/pyfcrypto_test_des3_context.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49563 2024-01-15 04:22:04.000000 libfcrypto-20240115/tests/fcrypto_test_rc4_context.c
--rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-01-15 04:20:15.000000 libfcrypto-20240115/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3882 2024-01-15 04:22:04.000000 libfcrypto-20240115/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3219 2024-01-15 04:20:15.000000 libfcrypto-20240115/tests/fcrypto_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-01-15 04:22:04.000000 libfcrypto-20240115/tests/pyfcrypto_test_serpent_context.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-01-15 04:20:15.000000 libfcrypto-20240115/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-01-15 04:20:15.000000 libfcrypto-20240115/tests/fcrypto_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41903 2024-01-15 04:23:22.000000 libfcrypto-20240115/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2110 2024-01-15 04:20:15.000000 libfcrypto-20240115/tests/fcrypto_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      997 2024-01-15 04:20:15.000000 libfcrypto-20240115/tests/fcrypto_test_libfcrypto.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4118 2024-01-15 04:20:15.000000 libfcrypto-20240115/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:43.000000 libfcrypto-20240115/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      982 2024-01-15 04:20:15.000000 libfcrypto-20240115/ossfuzz/ossfuzz_libfcrypto.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1677 2024-01-15 04:20:15.000000 libfcrypto-20240115/ossfuzz/crypt_rc4_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1922 2024-01-15 04:20:15.000000 libfcrypto-20240115/ossfuzz/crypt_serpent_cbc_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1751 2024-01-15 04:20:15.000000 libfcrypto-20240115/ossfuzz/crypt_serpent_ecb_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1684 2024-01-14 11:33:35.000000 libfcrypto-20240115/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1681 2024-01-15 04:20:15.000000 libfcrypto-20240115/ossfuzz/crypt_blowfish_ecb_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29224 2024-01-15 04:23:22.000000 libfcrypto-20240115/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-01-15 04:23:19.000000 libfcrypto-20240115/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:43.000000 libfcrypto-20240115/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:04:04.000000 libfcrypto-20240115/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:04:04.000000 libfcrypto-20240115/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:04:04.000000 libfcrypto-20240115/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:04:04.000000 libfcrypto-20240115/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:04:04.000000 libfcrypto-20240115/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:04:04.000000 libfcrypto-20240115/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:04:04.000000 libfcrypto-20240115/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:04:04.000000 libfcrypto-20240115/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:04:04.000000 libfcrypto-20240115/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1856 2024-01-15 04:23:27.000000 libfcrypto-20240115/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:04:04.000000 libfcrypto-20240115/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:04:04.000000 libfcrypto-20240115/po/Rules-quot
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33230 2024-01-15 04:23:21.000000 libfcrypto-20240115/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-15 04:25:42.000000 libfcrypto-20240115/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-01-15 04:23:16.000000 libfcrypto-20240115/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-01-15 04:23:16.000000 libfcrypto-20240115/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-01-15 04:23:16.000000 libfcrypto-20240115/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-01-15 04:23:16.000000 libfcrypto-20240115/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-01-15 04:23:16.000000 libfcrypto-20240115/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-01-15 04:23:16.000000 libfcrypto-20240115/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-01-15 04:23:16.000000 libfcrypto-20240115/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-01-15 04:23:16.000000 libfcrypto-20240115/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-01-15 04:23:16.000000 libfcrypto-20240115/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-01-15 04:23:16.000000 libfcrypto-20240115/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-15 04:23:16.000000 libfcrypto-20240115/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22391 2024-01-15 04:23:22.000000 libfcrypto-20240115/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56383 2024-01-15 04:23:20.000000 libfcrypto-20240115/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3548 2024-01-15 04:20:15.000000 libfcrypto-20240115/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      420 2024-01-15 04:25:43.532132 libfcrypto-20240115/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:32.000000 libfcrypto-20240414/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1974 2024-04-14 10:08:49.000000 libfcrypto-20240414/libfcrypto.spec
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-04-14 09:51:41.000000 libfcrypto-20240414/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-04-14 10:08:35.000000 libfcrypto-20240414/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 09:51:41.000000 libfcrypto-20240414/NEWS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:31.000000 libfcrypto-20240414/pyfcrypto/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8158 2024-04-14 09:51:44.000000 libfcrypto-20240414/pyfcrypto/pyfcrypto_blowfish_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8071 2024-04-14 09:51:44.000000 libfcrypto-20240414/pyfcrypto/pyfcrypto_serpent_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-04-14 09:51:44.000000 libfcrypto-20240414/pyfcrypto/pyfcrypto_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2044 2024-04-14 09:51:44.000000 libfcrypto-20240414/pyfcrypto/pyfcrypto_crypt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1899 2024-04-14 09:51:44.000000 libfcrypto-20240414/pyfcrypto/pyfcrypto_rc4_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7751 2024-04-14 09:56:55.000000 libfcrypto-20240414/pyfcrypto/pyfcrypto.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      928 2024-04-14 09:53:09.000000 libfcrypto-20240414/pyfcrypto/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7795 2024-04-14 09:51:44.000000 libfcrypto-20240414/pyfcrypto/pyfcrypto_rc4_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1921 2024-04-14 09:51:44.000000 libfcrypto-20240414/pyfcrypto/pyfcrypto_des3_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1987 2024-04-14 09:51:44.000000 libfcrypto-20240414/pyfcrypto/pyfcrypto_serpent_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5592 2024-04-14 09:51:44.000000 libfcrypto-20240414/pyfcrypto/pyfcrypto_crypt_modes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9586 2024-04-14 09:51:44.000000 libfcrypto-20240414/pyfcrypto/pyfcrypto_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1558 2024-04-14 09:51:44.000000 libfcrypto-20240414/pyfcrypto/pyfcrypto_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      989 2024-04-14 09:51:44.000000 libfcrypto-20240414/pyfcrypto/pyfcrypto_libfcrypto.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-14 09:51:44.000000 libfcrypto-20240414/pyfcrypto/pyfcrypto_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1331 2024-04-14 09:51:44.000000 libfcrypto-20240414/pyfcrypto/pyfcrypto.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-14 09:51:44.000000 libfcrypto-20240414/pyfcrypto/pyfcrypto_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2009 2024-04-14 09:51:44.000000 libfcrypto-20240414/pyfcrypto/pyfcrypto_blowfish_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27507 2024-04-14 09:51:44.000000 libfcrypto-20240414/pyfcrypto/pyfcrypto_crypt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1668 2024-04-14 09:51:44.000000 libfcrypto-20240414/pyfcrypto/pyfcrypto_crypt_modes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37639 2024-04-14 10:08:35.000000 libfcrypto-20240414/pyfcrypto/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7866 2024-04-14 09:51:44.000000 libfcrypto-20240414/pyfcrypto/pyfcrypto_des3_context.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-04-14 10:08:35.000000 libfcrypto-20240414/depcomp
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2024-04-14 09:51:41.000000 libfcrypto-20240414/libfcrypto.spec.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:30.000000 libfcrypto-20240414/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:04:04.000000 libfcrypto-20240414/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:04:04.000000 libfcrypto-20240414/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:04:04.000000 libfcrypto-20240414/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:04:04.000000 libfcrypto-20240414/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:04:04.000000 libfcrypto-20240414/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-03-30 04:38:22.000000 libfcrypto-20240414/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-04-14 10:08:32.000000 libfcrypto-20240414/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-04-14 10:08:32.000000 libfcrypto-20240414/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:04:04.000000 libfcrypto-20240414/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-04-14 10:08:32.000000 libfcrypto-20240414/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:04:04.000000 libfcrypto-20240414/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-04-14 09:51:44.000000 libfcrypto-20240414/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:04:04.000000 libfcrypto-20240414/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-04-14 10:08:32.000000 libfcrypto-20240414/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:04:04.000000 libfcrypto-20240414/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:04:04.000000 libfcrypto-20240414/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-04-14 10:08:32.000000 libfcrypto-20240414/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:04:04.000000 libfcrypto-20240414/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:04:04.000000 libfcrypto-20240414/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:04:04.000000 libfcrypto-20240414/m4/types.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:31.000000 libfcrypto-20240414/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10314 2024-04-14 09:51:43.000000 libfcrypto-20240414/include/libfcrypto.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      430 2024-04-14 09:52:08.000000 libfcrypto-20240414/include/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:31.000000 libfcrypto-20240414/include/libfcrypto/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1836 2024-04-14 09:51:43.000000 libfcrypto-20240414/include/libfcrypto/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1834 2024-04-14 10:08:49.000000 libfcrypto-20240414/include/libfcrypto/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5106 2024-04-14 09:51:43.000000 libfcrypto-20240414/include/libfcrypto/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4975 2024-04-14 10:08:49.000000 libfcrypto-20240414/include/libfcrypto/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1248 2024-04-14 09:51:43.000000 libfcrypto-20240414/include/libfcrypto/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6894 2024-04-14 09:51:43.000000 libfcrypto-20240414/include/libfcrypto/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-14 09:51:43.000000 libfcrypto-20240414/include/libfcrypto/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1248 2024-04-14 10:08:49.000000 libfcrypto-20240414/include/libfcrypto/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20985 2024-04-14 10:08:35.000000 libfcrypto-20240414/include/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10314 2024-04-14 10:08:49.000000 libfcrypto-20240414/include/libfcrypto.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      268 2024-04-14 09:51:41.000000 libfcrypto-20240414/libfcrypto.pc.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:31.000000 libfcrypto-20240414/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-14 09:51:42.000000 libfcrypto-20240414/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-04-14 09:51:42.000000 libfcrypto-20240414/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-04-14 09:51:42.000000 libfcrypto-20240414/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-04-14 09:51:42.000000 libfcrypto-20240414/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-14 09:51:42.000000 libfcrypto-20240414/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-14 09:51:42.000000 libfcrypto-20240414/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-04-14 09:51:43.000000 libfcrypto-20240414/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      356 2024-04-14 09:52:08.000000 libfcrypto-20240414/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-14 09:51:43.000000 libfcrypto-20240414/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7376 2024-04-14 10:08:49.000000 libfcrypto-20240414/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9229 2024-04-14 10:08:35.000000 libfcrypto-20240414/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9799 2024-04-14 10:08:00.000000 libfcrypto-20240414/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-04-14 09:51:43.000000 libfcrypto-20240414/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-04-14 09:51:42.000000 libfcrypto-20240414/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-04-14 09:51:42.000000 libfcrypto-20240414/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-04-14 10:08:35.000000 libfcrypto-20240414/common/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1227 2024-04-14 09:52:55.000000 libfcrypto-20240414/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:03:56.000000 libfcrypto-20240414/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-04-14 10:08:35.000000 libfcrypto-20240414/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:30.000000 libfcrypto-20240414/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1030 2024-04-14 09:51:44.000000 libfcrypto-20240414/dpkg/copyright
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-04-14 09:51:41.000000 libfcrypto-20240414/dpkg/libfcrypto.install
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:30.000000 libfcrypto-20240414/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-04-14 09:51:41.000000 libfcrypto-20240414/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-04-14 09:51:41.000000 libfcrypto-20240414/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      721 2024-04-14 09:51:41.000000 libfcrypto-20240414/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-04-14 09:51:41.000000 libfcrypto-20240414/dpkg/libfcrypto-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      123 2024-04-14 09:51:41.000000 libfcrypto-20240414/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-04-14 09:51:41.000000 libfcrypto-20240414/dpkg/libfcrypto-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      142 2024-04-14 10:08:49.000000 libfcrypto-20240414/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-04-14 09:51:41.000000 libfcrypto-20240414/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      488 2024-04-14 10:08:49.000000 libfcrypto-20240414/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-04-14 09:51:41.000000 libfcrypto-20240414/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)   838636 2024-04-14 10:08:34.000000 libfcrypto-20240414/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-04-14 10:08:35.000000 libfcrypto-20240414/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-04-14 10:08:35.000000 libfcrypto-20240414/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:32.000000 libfcrypto-20240414/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:32.000000 libfcrypto-20240414/msvscpp/fcrypto_test_rc4_context/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4917 2024-04-14 09:51:46.000000 libfcrypto-20240414/msvscpp/fcrypto_test_rc4_context/fcrypto_test_rc4_context.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:32.000000 libfcrypto-20240414/msvscpp/pyfcrypto/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6032 2024-04-14 09:51:46.000000 libfcrypto-20240414/msvscpp/pyfcrypto/pyfcrypto.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      566 2024-04-14 09:53:26.000000 libfcrypto-20240414/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:32.000000 libfcrypto-20240414/msvscpp/fcrypto_test_serpent_context/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4929 2024-04-14 09:51:46.000000 libfcrypto-20240414/msvscpp/fcrypto_test_serpent_context/fcrypto_test_serpent_context.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:32.000000 libfcrypto-20240414/msvscpp/fcrypto_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4647 2024-04-14 09:51:46.000000 libfcrypto-20240414/msvscpp/fcrypto_test_error/fcrypto_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:32.000000 libfcrypto-20240414/msvscpp/fcrypto_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-04-14 09:51:46.000000 libfcrypto-20240414/msvscpp/fcrypto_test_support/fcrypto_test_support.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6622 2024-04-14 09:51:46.000000 libfcrypto-20240414/msvscpp/libfcrypto.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:32.000000 libfcrypto-20240414/msvscpp/libfcrypto/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5877 2024-04-14 09:51:46.000000 libfcrypto-20240414/msvscpp/libfcrypto/libfcrypto.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15562 2024-04-14 10:08:35.000000 libfcrypto-20240414/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:32.000000 libfcrypto-20240414/msvscpp/fcrypto_test_des3_context/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4920 2024-04-14 09:51:46.000000 libfcrypto-20240414/msvscpp/fcrypto_test_des3_context/fcrypto_test_des3_context.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:32.000000 libfcrypto-20240414/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-04-14 09:51:46.000000 libfcrypto-20240414/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:32.000000 libfcrypto-20240414/msvscpp/fcrypto_test_blowfish_context/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4932 2024-04-14 09:51:46.000000 libfcrypto-20240414/msvscpp/fcrypto_test_blowfish_context/fcrypto_test_blowfish_context.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       94 2024-04-14 09:51:42.000000 libfcrypto-20240414/AUTHORS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      286 2024-04-14 09:51:41.000000 libfcrypto-20240414/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-04-14 10:08:35.000000 libfcrypto-20240414/INSTALL
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-14 09:51:41.000000 libfcrypto-20240414/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      489 2024-04-14 09:51:41.000000 libfcrypto-20240414/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-04-14 10:08:35.000000 libfcrypto-20240414/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-04-14 09:51:41.000000 libfcrypto-20240414/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      773 2024-04-14 09:52:05.000000 libfcrypto-20240414/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:03:56.000000 libfcrypto-20240414/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:31.000000 libfcrypto-20240414/libfcrypto/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3331 2024-04-14 09:51:43.000000 libfcrypto-20240414/libfcrypto/libfcrypto_blowfish_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-14 09:51:43.000000 libfcrypto-20240414/libfcrypto/libfcrypto_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42088 2024-04-14 09:51:43.000000 libfcrypto-20240414/libfcrypto/libfcrypto_blowfish_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1827 2024-04-14 09:51:43.000000 libfcrypto-20240414/libfcrypto/libfcrypto.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1902 2024-04-14 09:51:43.000000 libfcrypto-20240414/libfcrypto/libfcrypto_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2103 2024-04-14 09:51:43.000000 libfcrypto-20240414/libfcrypto/libfcrypto_rc4_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2024-04-14 09:51:43.000000 libfcrypto-20240414/libfcrypto/libfcrypto_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2186 2024-04-14 09:51:43.000000 libfcrypto-20240414/libfcrypto/libfcrypto_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2184 2024-04-14 10:08:49.000000 libfcrypto-20240414/libfcrypto/libfcrypto_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9130 2024-04-14 09:51:43.000000 libfcrypto-20240414/libfcrypto/libfcrypto_rc4_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1130 2024-04-14 09:55:17.000000 libfcrypto-20240414/libfcrypto/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1078 2024-04-14 09:51:43.000000 libfcrypto-20240414/libfcrypto/libfcrypto.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3115 2024-04-14 09:51:43.000000 libfcrypto-20240414/libfcrypto/libfcrypto_serpent_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    75716 2024-04-14 09:51:43.000000 libfcrypto-20240414/libfcrypto/libfcrypto_serpent_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32055 2024-04-14 09:51:43.000000 libfcrypto-20240414/libfcrypto/libfcrypto_des3_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2891 2024-04-14 09:51:43.000000 libfcrypto-20240414/libfcrypto/libfcrypto_des3_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2938 2024-04-14 09:51:43.000000 libfcrypto-20240414/libfcrypto/libfcrypto_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2024-04-14 09:51:43.000000 libfcrypto-20240414/libfcrypto/libfcrypto_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1841 2024-04-14 09:51:43.000000 libfcrypto-20240414/libfcrypto/libfcrypto_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-04-14 09:51:43.000000 libfcrypto-20240414/libfcrypto/libfcrypto_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26446 2024-04-14 10:08:35.000000 libfcrypto-20240414/libfcrypto/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-14 09:51:43.000000 libfcrypto-20240414/libfcrypto/libfcrypto_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1076 2024-04-14 10:08:49.000000 libfcrypto-20240414/libfcrypto/libfcrypto.rc
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-04-14 10:08:35.000000 libfcrypto-20240414/test-driver
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      419 2024-01-14 16:30:12.000000 libfcrypto-20240414/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:32.000000 libfcrypto-20240414/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      103 2024-04-14 09:53:36.000000 libfcrypto-20240414/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18209 2024-04-14 10:08:35.000000 libfcrypto-20240414/manuals/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4826 2024-04-14 09:55:42.000000 libfcrypto-20240414/manuals/libfcrypto.3
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:32.000000 libfcrypto-20240414/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-14 09:51:44.000000 libfcrypto-20240414/tests/fcrypto_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4794 2024-04-14 09:51:44.000000 libfcrypto-20240414/tests/fcrypto_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1584 2024-04-14 09:57:02.000000 libfcrypto-20240414/tests/pyfcrypto_test_rc4_context.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20956 2024-04-14 09:52:05.000000 libfcrypto-20240414/tests/fcrypto_test_serpent_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-14 09:51:44.000000 libfcrypto-20240414/tests/pyfcrypto_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8644 2024-04-14 09:51:44.000000 libfcrypto-20240414/tests/fcrypto_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44027 2024-04-14 09:52:05.000000 libfcrypto-20240414/tests/fcrypto_test_blowfish_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2568 2024-04-14 09:57:02.000000 libfcrypto-20240414/tests/pyfcrypto_test_blowfish_context.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2447 2024-04-14 09:55:35.000000 libfcrypto-20240414/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1724 2024-04-14 09:51:44.000000 libfcrypto-20240414/tests/fcrypto_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18454 2024-04-14 09:52:05.000000 libfcrypto-20240414/tests/fcrypto_test_des3_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1596 2024-04-14 09:57:02.000000 libfcrypto-20240414/tests/pyfcrypto_test_des3_context.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49563 2024-04-14 09:52:05.000000 libfcrypto-20240414/tests/fcrypto_test_rc4_context.c
+-rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-14 09:51:44.000000 libfcrypto-20240414/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4105 2024-04-14 09:58:24.000000 libfcrypto-20240414/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3219 2024-04-14 09:51:44.000000 libfcrypto-20240414/tests/fcrypto_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-04-14 09:57:02.000000 libfcrypto-20240414/tests/pyfcrypto_test_serpent_context.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-04-14 09:51:44.000000 libfcrypto-20240414/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-14 09:51:44.000000 libfcrypto-20240414/tests/fcrypto_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42260 2024-04-14 10:08:35.000000 libfcrypto-20240414/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2110 2024-04-14 09:51:44.000000 libfcrypto-20240414/tests/fcrypto_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      997 2024-04-14 09:51:44.000000 libfcrypto-20240414/tests/fcrypto_test_libfcrypto.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4087 2024-04-14 09:51:44.000000 libfcrypto-20240414/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:32.000000 libfcrypto-20240414/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1677 2024-04-14 09:51:43.000000 libfcrypto-20240414/ossfuzz/crypt_des3_ecb_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      982 2024-04-14 09:51:43.000000 libfcrypto-20240414/ossfuzz/ossfuzz_libfcrypto.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1677 2024-04-14 09:51:43.000000 libfcrypto-20240414/ossfuzz/crypt_rc4_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1922 2024-04-14 09:51:43.000000 libfcrypto-20240414/ossfuzz/crypt_serpent_cbc_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1750 2024-04-14 09:51:43.000000 libfcrypto-20240414/ossfuzz/crypt_serpent_ecb_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1815 2024-04-14 09:51:43.000000 libfcrypto-20240414/ossfuzz/crypt_des3_cbc_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2790 2024-04-14 09:53:48.000000 libfcrypto-20240414/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1681 2024-04-14 09:51:43.000000 libfcrypto-20240414/ossfuzz/crypt_blowfish_ecb_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1819 2024-04-14 09:51:43.000000 libfcrypto-20240414/ossfuzz/crypt_blowfish_cbc_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34310 2024-04-14 10:08:35.000000 libfcrypto-20240414/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-04-14 10:08:32.000000 libfcrypto-20240414/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:32.000000 libfcrypto-20240414/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:04:04.000000 libfcrypto-20240414/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:04:04.000000 libfcrypto-20240414/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:04:04.000000 libfcrypto-20240414/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:04:04.000000 libfcrypto-20240414/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:04:04.000000 libfcrypto-20240414/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:04:04.000000 libfcrypto-20240414/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:04:04.000000 libfcrypto-20240414/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:04:04.000000 libfcrypto-20240414/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:04:04.000000 libfcrypto-20240414/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1856 2024-04-14 10:08:49.000000 libfcrypto-20240414/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:04:04.000000 libfcrypto-20240414/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:04:04.000000 libfcrypto-20240414/po/Rules-quot
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33112 2024-04-14 10:08:35.000000 libfcrypto-20240414/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-14 10:13:31.000000 libfcrypto-20240414/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-04-14 10:08:28.000000 libfcrypto-20240414/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-04-14 10:08:28.000000 libfcrypto-20240414/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-14 10:08:28.000000 libfcrypto-20240414/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-04-14 10:08:28.000000 libfcrypto-20240414/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-14 10:08:28.000000 libfcrypto-20240414/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-14 10:08:28.000000 libfcrypto-20240414/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-04-14 10:08:28.000000 libfcrypto-20240414/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-04-14 10:08:28.000000 libfcrypto-20240414/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-04-14 10:08:28.000000 libfcrypto-20240414/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-14 10:08:28.000000 libfcrypto-20240414/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-14 10:08:28.000000 libfcrypto-20240414/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22540 2024-04-14 10:08:35.000000 libfcrypto-20240414/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56383 2024-04-14 10:08:34.000000 libfcrypto-20240414/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3548 2024-04-14 09:51:41.000000 libfcrypto-20240414/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      420 2024-04-14 10:13:32.724274 libfcrypto-20240414/PKG-INFO
```

### Comparing `libfcrypto-20240115/libfcrypto.spec` & `libfcrypto-20240414/libfcrypto.spec`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libfcrypto
-Version: 20240115
+Version: 20240414
 Release: 1
 Summary: Library to support encryption formats
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libfcrypto
  
@@ -76,10 +76,10 @@
 %files -n libfcrypto-python3
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_libdir}/python3*/site-packages/*.a
 %{_libdir}/python3*/site-packages/*.so
 
 %changelog
-* Mon Jan 15 2024 Joachim Metz <joachim.metz@gmail.com> 20240115-1
+* Sun Apr 14 2024 Joachim Metz <joachim.metz@gmail.com> 20240414-1
 - Auto-generated
```

### Comparing `libfcrypto-20240115/COPYING` & `libfcrypto-20240414/COPYING`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/install-sh` & `libfcrypto-20240414/install-sh`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/pyfcrypto/pyfcrypto_blowfish_context.c` & `libfcrypto-20240414/pyfcrypto/pyfcrypto_blowfish_context.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/pyfcrypto/pyfcrypto_serpent_context.c` & `libfcrypto-20240414/pyfcrypto/pyfcrypto_serpent_context.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/pyfcrypto/pyfcrypto_python.h` & `libfcrypto-20240414/pyfcrypto/pyfcrypto_python.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/pyfcrypto/pyfcrypto_crypt.h` & `libfcrypto-20240414/pyfcrypto/pyfcrypto_crypt.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/pyfcrypto/pyfcrypto_rc4_context.h` & `libfcrypto-20240414/pyfcrypto/pyfcrypto_rc4_context.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/pyfcrypto/pyfcrypto.c` & `libfcrypto-20240414/pyfcrypto/pyfcrypto.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/pyfcrypto/Makefile.am` & `libfcrypto-20240414/pyfcrypto/Makefile.am`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_PYTHON
 AM_CFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBFCRYPTO_DLL_IMPORT@
 
 pyexec_LTLIBRARIES = pyfcrypto.la
 
 pyfcrypto_la_SOURCES = \
 	pyfcrypto.c pyfcrypto.h \
@@ -26,13 +26,11 @@
 	../libfcrypto/libfcrypto.la
 
 pyfcrypto_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pyfcrypto_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libfcrypto-20240115/pyfcrypto/pyfcrypto_rc4_context.c` & `libfcrypto-20240414/pyfcrypto/pyfcrypto_rc4_context.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/pyfcrypto/pyfcrypto_des3_context.h` & `libfcrypto-20240414/pyfcrypto/pyfcrypto_des3_context.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/pyfcrypto/pyfcrypto_serpent_context.h` & `libfcrypto-20240414/pyfcrypto/pyfcrypto_serpent_context.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/pyfcrypto/pyfcrypto_crypt_modes.c` & `libfcrypto-20240414/pyfcrypto/pyfcrypto_crypt_modes.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/pyfcrypto/pyfcrypto_error.c` & `libfcrypto-20240414/pyfcrypto/pyfcrypto_error.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/pyfcrypto/pyfcrypto_error.h` & `libfcrypto-20240414/pyfcrypto/pyfcrypto_error.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/pyfcrypto/pyfcrypto_libfcrypto.h` & `libfcrypto-20240414/pyfcrypto/pyfcrypto_libfcrypto.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/pyfcrypto/pyfcrypto_libcerror.h` & `libfcrypto-20240414/pyfcrypto/pyfcrypto_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/pyfcrypto/pyfcrypto.h` & `libfcrypto-20240414/pyfcrypto/pyfcrypto.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/pyfcrypto/pyfcrypto_unused.h` & `libfcrypto-20240414/pyfcrypto/pyfcrypto_unused.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/pyfcrypto/pyfcrypto_blowfish_context.h` & `libfcrypto-20240414/pyfcrypto/pyfcrypto_blowfish_context.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/pyfcrypto/pyfcrypto_crypt.c` & `libfcrypto-20240414/pyfcrypto/pyfcrypto_crypt.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/pyfcrypto/pyfcrypto_crypt_modes.h` & `libfcrypto-20240414/pyfcrypto/pyfcrypto_crypt_modes.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/pyfcrypto/Makefile.in` & `libfcrypto-20240414/pyfcrypto/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -417,16 +417,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_PYTHON_TRUE@AM_CFLAGS = \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/include \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/common \
+@HAVE_PYTHON_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_PYTHON_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBFCRYPTO_DLL_IMPORT@
 
 @HAVE_PYTHON_TRUE@pyexec_LTLIBRARIES = pyfcrypto.la
 @HAVE_PYTHON_TRUE@pyfcrypto_la_SOURCES = \
 @HAVE_PYTHON_TRUE@	pyfcrypto.c pyfcrypto.h \
 @HAVE_PYTHON_TRUE@	pyfcrypto_blowfish_context.c pyfcrypto_blowfish_context.h \
@@ -443,15 +443,16 @@
 
 @HAVE_PYTHON_TRUE@pyfcrypto_la_LIBADD = \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_PYTHON_TRUE@	../libfcrypto/libfcrypto.la
 
 @HAVE_PYTHON_TRUE@pyfcrypto_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pyfcrypto_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -741,24 +742,34 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-pyexecLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/pyfcrypto_la-pyfcrypto.Plo
+	-rm -f ./$(DEPDIR)/pyfcrypto_la-pyfcrypto_blowfish_context.Plo
+	-rm -f ./$(DEPDIR)/pyfcrypto_la-pyfcrypto_crypt.Plo
+	-rm -f ./$(DEPDIR)/pyfcrypto_la-pyfcrypto_crypt_modes.Plo
+	-rm -f ./$(DEPDIR)/pyfcrypto_la-pyfcrypto_des3_context.Plo
+	-rm -f ./$(DEPDIR)/pyfcrypto_la-pyfcrypto_error.Plo
+	-rm -f ./$(DEPDIR)/pyfcrypto_la-pyfcrypto_rc4_context.Plo
+	-rm -f ./$(DEPDIR)/pyfcrypto_la-pyfcrypto_serpent_context.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -850,13 +861,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-pyexecLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfcrypto-20240115/pyfcrypto/pyfcrypto_des3_context.c` & `libfcrypto-20240414/pyfcrypto/pyfcrypto_des3_context.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/depcomp` & `libfcrypto-20240414/depcomp`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libfcrypto.spec.in` & `libfcrypto-20240414/libfcrypto.spec.in`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/m4/tests.m4` & `libfcrypto-20240414/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/m4/lib-prefix.m4` & `libfcrypto-20240414/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/m4/progtest.m4` & `libfcrypto-20240414/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/m4/gettext.m4` & `libfcrypto-20240414/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/m4/lib-ld.m4` & `libfcrypto-20240414/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/m4/common.m4` & `libfcrypto-20240414/m4/common.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for common headers and functions
 dnl
-dnl Version: 20181117
+dnl Version: 20240308
 
 dnl Function to test if a certain feature was disabled
 AC_DEFUN([AX_COMMON_ARG_DISABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
@@ -22,15 +22,15 @@
 dnl Function to test if a certain feature was enabled
 AC_DEFUN([AX_COMMON_ARG_ENABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
       [--enable-$1],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_enable_$2=$enableval],
     [ac_cv_enable_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to enable $3],
       [ac_cv_enable_$2],
       [ac_cv_enable_$2=$4])dnl
@@ -39,15 +39,15 @@
 dnl Function to test if the location of a certain feature was provided
 AC_DEFUN([AX_COMMON_ARG_WITH],
 [
   AC_ARG_WITH(
     [$1],
     [AS_HELP_STRING(
       [--with-$1[[=$5]]],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_with_$2=$withval],
     [ac_cv_with_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to use $3],
       [ac_cv_with_$2],
       [ac_cv_with_$2=$4])dnl
```

### Comparing `libfcrypto-20240115/m4/ltversion.m4` & `libfcrypto-20240414/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/m4/ltsugar.m4` & `libfcrypto-20240414/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/m4/host-cpu-c-abi.m4` & `libfcrypto-20240414/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/m4/libtool.m4` & `libfcrypto-20240414/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/m4/po.m4` & `libfcrypto-20240414/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/m4/libcerror.m4` & `libfcrypto-20240414/m4/libcerror.m4`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
     [ac_cv_libcerror=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcerror which returns "yes" and --with-libcerror= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect],
+      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcerror"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcerror],
           [1])
@@ -95,16 +97,17 @@
           cerror,
           libcerror_system_set_error,
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -162,15 +165,15 @@
       [test "x$ac_cv_func_strerror" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: strerror_r and strerror],
         [1])
       ])
     ])
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
   ])
 
 dnl Function to detect how to enable libcerror
 AC_DEFUN([AX_LIBCERROR_CHECK_ENABLE],
```

### Comparing `libfcrypto-20240115/m4/intlmacosx.m4` & `libfcrypto-20240414/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/m4/lt~obsolete.m4` & `libfcrypto-20240414/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/m4/lib-link.m4` & `libfcrypto-20240414/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/m4/iconv.m4` & `libfcrypto-20240414/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/m4/ltoptions.m4` & `libfcrypto-20240414/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/m4/nls.m4` & `libfcrypto-20240414/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/m4/python.m4` & `libfcrypto-20240414/m4/python.m4`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/m4/types.m4` & `libfcrypto-20240414/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/include/libfcrypto.h.in` & `libfcrypto-20240414/include/libfcrypto.h.in`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/include/libfcrypto/definitions.h.in` & `libfcrypto-20240414/include/libfcrypto/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/include/libfcrypto/definitions.h` & `libfcrypto-20240414/include/libfcrypto/definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBFCRYPTO_DEFINITIONS_H )
 #define _LIBFCRYPTO_DEFINITIONS_H
 
 #include <libfcrypto/types.h>
 
-#define LIBFCRYPTO_VERSION			20240115
+#define LIBFCRYPTO_VERSION			20240414
 
 /* The version string
  */
-#define LIBFCRYPTO_VERSION_STRING		"20240115"
+#define LIBFCRYPTO_VERSION_STRING		"20240414"
 
 /* The crypt modes
  */
 enum LIBFCRYPTO_CRYPT_MODES
 {
 	LIBFCRYPTO_CRYPT_MODE_DECRYPT		= 0,
 	LIBFCRYPTO_CRYPT_MODE_ENCRYPT		= 1
```

### Comparing `libfcrypto-20240115/include/libfcrypto/types.h.in` & `libfcrypto-20240414/include/libfcrypto/types.h.in`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/include/libfcrypto/types.h` & `libfcrypto-20240414/include/libfcrypto/types.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/include/libfcrypto/features.h.in` & `libfcrypto-20240414/include/libfcrypto/features.h.in`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/include/libfcrypto/error.h` & `libfcrypto-20240414/include/libfcrypto/error.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/include/libfcrypto/extern.h` & `libfcrypto-20240414/include/libfcrypto/extern.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/include/libfcrypto/features.h` & `libfcrypto-20240414/include/libfcrypto/features.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/include/Makefile.in` & `libfcrypto-20240414/include/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -376,15 +376,20 @@
 
 EXTRA_DIST = \
 	libfcrypto.h.in \
 	libfcrypto/definitions.h.in \
 	libfcrypto/features.h.in \
 	libfcrypto/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfcrypto.h \
+	libfcrypto/definitions.h \
+	libfcrypto/features.h \
+	libfcrypto/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -581,23 +586,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -679,17 +686,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libfcrypto.h
-	-rm -f libfcrypto/definitions.h
-	-rm -f libfcrypto/features.h
-	-rm -f libfcrypto/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfcrypto-20240115/include/libfcrypto.h` & `libfcrypto-20240414/include/libfcrypto.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/common/config_borlandc.h` & `libfcrypto-20240414/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/common/file_stream.h` & `libfcrypto-20240414/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/common/memory.h` & `libfcrypto-20240414/common/memory.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/common/byte_stream.h` & `libfcrypto-20240414/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/common/common.h` & `libfcrypto-20240414/common/common.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/common/config_winapi.h` & `libfcrypto-20240414/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/common/system_string.h` & `libfcrypto-20240414/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/common/types.h.in` & `libfcrypto-20240414/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/common/types.h` & `libfcrypto-20240414/common/types.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/common/config.h.in` & `libfcrypto-20240414/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/common/config.h` & `libfcrypto-20240414/common/config.h`

 * *Files 4% similar despite different names*

```diff
@@ -283,24 +283,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libfcrypto"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libfcrypto 20240115"
+#define PACKAGE_STRING "libfcrypto 20240414"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libfcrypto"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240115"
+#define PACKAGE_VERSION "20240414"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -318,15 +318,15 @@
    backward compatibility; new code need not use it. */
 #define STDC_HEADERS 1
 
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Version number of package */
-#define VERSION "20240115"
+#define VERSION "20240414"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libfcrypto-20240115/common/wide_string.h` & `libfcrypto-20240414/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/common/narrow_string.h` & `libfcrypto-20240414/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/common/config_msc.h` & `libfcrypto-20240414/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/common/Makefile.in` & `libfcrypto-20240414/common/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -330,15 +330,17 @@
 sharedstatedir = @sharedstatedir@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
-AM_CPPFLAGS = -I$(top_srcdir)/include
+AM_CPPFLAGS = \
+	-I../include -I../include -I$(top_srcdir)/include
+
 EXTRA_DIST = \
 	byte_stream.h \
 	common.h \
 	config.h \
 	config_borlandc.h \
 	config_msc.h \
 	config_winapi.h \
@@ -346,15 +348,18 @@
 	memory.h \
 	narrow_string.h \
 	system_string.h \
 	types.h \
 	types.h.in \
 	wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	config.h \
+	types.h \
+	Makefile \
 	Makefile.in
 
 all: config.h
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -522,23 +527,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-hdr distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -618,15 +625,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f config.h
-	-rm -f types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfcrypto-20240115/Makefile.am` & `libfcrypto-20240414/Makefile.am`

 * *Files 27% similar despite different names*

```diff
@@ -44,16 +44,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libfcrypto.pc \
+	libfcrypto.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libfcrypto.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -63,19 +70,7 @@
 
 library:
 	(cd $(srcdir)/common && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcerror && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfcrypto && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libfcrypto.pc
-	-rm -f libfcrypto.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libfcrypto-20240115/config.guess` & `libfcrypto-20240414/config.guess`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/dpkg/copyright` & `libfcrypto-20240414/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/dpkg/control` & `libfcrypto-20240414/dpkg/control`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/dpkg/rules` & `libfcrypto-20240414/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/COPYING.LESSER` & `libfcrypto-20240414/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/configure` & `libfcrypto-20240414/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libfcrypto 20240115.
+# Generated by GNU Autoconf 2.71 for libfcrypto 20240414.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libfcrypto'
 PACKAGE_TARNAME='libfcrypto'
-PACKAGE_VERSION='20240115'
-PACKAGE_STRING='libfcrypto 20240115'
+PACKAGE_VERSION='20240414'
+PACKAGE_STRING='libfcrypto 20240414'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libfcrypto.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1445,15 +1445,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libfcrypto 20240115 to adapt to many kinds of systems.
+\`configure' configures libfcrypto 20240414 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1516,15 +1516,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libfcrypto 20240115:";;
+     short | recursive ) echo "Configuration of libfcrypto 20240414:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1658,15 +1658,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libfcrypto configure 20240115
+libfcrypto configure 20240414
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2379,15 +2379,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libfcrypto $as_me 20240115, which was
+It was created by libfcrypto $as_me 20240414, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -3868,15 +3868,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libfcrypto'
- VERSION='20240115'
+ VERSION='20240414'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23347,15 +23347,15 @@
 printf "%s\n" "$ac_cv_with_libcerror" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno
 then :
   ac_cv_libcerror=no
 else $as_nop
   ac_cv_libcerror=check
-        if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect
+                if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   if test -d "$ac_cv_with_libcerror"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -23846,15 +23846,16 @@
 fi
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes
+
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -23996,15 +23997,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -25198,15 +25199,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libfcrypto $as_me 20240115, which was
+This file was extended by libfcrypto $as_me 20240414, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -25266,15 +25267,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libfcrypto config.status 20240115
+libfcrypto config.status 20240414
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libfcrypto-20240115/compile` & `libfcrypto-20240414/compile`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/missing` & `libfcrypto-20240414/missing`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/msvscpp/fcrypto_test_rc4_context/fcrypto_test_rc4_context.vcproj` & `libfcrypto-20240414/msvscpp/fcrypto_test_rc4_context/fcrypto_test_rc4_context.vcproj`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/msvscpp/pyfcrypto/pyfcrypto.vcproj` & `libfcrypto-20240414/msvscpp/pyfcrypto/pyfcrypto.vcproj`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/msvscpp/Makefile.am` & `libfcrypto-20240414/msvscpp/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -9,13 +9,11 @@
 	libfcrypto/libfcrypto.vcproj \
 	pyfcrypto/pyfcrypto.vcproj \
 	libfcrypto.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libfcrypto-20240115/msvscpp/fcrypto_test_serpent_context/fcrypto_test_serpent_context.vcproj` & `libfcrypto-20240414/msvscpp/fcrypto_test_serpent_context/fcrypto_test_serpent_context.vcproj`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/msvscpp/fcrypto_test_error/fcrypto_test_error.vcproj` & `libfcrypto-20240414/msvscpp/fcrypto_test_error/fcrypto_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/msvscpp/fcrypto_test_support/fcrypto_test_support.vcproj` & `libfcrypto-20240414/msvscpp/fcrypto_test_support/fcrypto_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/msvscpp/libfcrypto.sln` & `libfcrypto-20240414/msvscpp/libfcrypto.sln`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/msvscpp/libfcrypto/libfcrypto.vcproj` & `libfcrypto-20240414/msvscpp/libfcrypto/libfcrypto.vcproj`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/msvscpp/Makefile.in` & `libfcrypto-20240414/msvscpp/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -327,15 +327,16 @@
 	libfcrypto/libfcrypto.vcproj \
 	pyfcrypto/pyfcrypto.vcproj \
 	libfcrypto.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -439,23 +440,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -534,13 +537,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfcrypto-20240115/msvscpp/fcrypto_test_des3_context/fcrypto_test_des3_context.vcproj` & `libfcrypto-20240414/msvscpp/fcrypto_test_des3_context/fcrypto_test_des3_context.vcproj`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/msvscpp/libcerror/libcerror.vcproj` & `libfcrypto-20240414/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/msvscpp/fcrypto_test_blowfish_context/fcrypto_test_blowfish_context.vcproj` & `libfcrypto-20240414/msvscpp/fcrypto_test_blowfish_context/fcrypto_test_blowfish_context.vcproj`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/INSTALL` & `libfcrypto-20240414/INSTALL`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/config.sub` & `libfcrypto-20240414/config.sub`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/setup.py` & `libfcrypto-20240414/setup.py`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/acinclude.m4` & `libfcrypto-20240414/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/config.rpath` & `libfcrypto-20240414/config.rpath`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libfcrypto/libfcrypto_blowfish_context.h` & `libfcrypto-20240414/libfcrypto/libfcrypto_blowfish_context.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libfcrypto/libfcrypto_extern.h` & `libfcrypto-20240414/libfcrypto/libfcrypto_extern.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libfcrypto/libfcrypto_blowfish_context.c` & `libfcrypto-20240414/libfcrypto/libfcrypto_blowfish_context.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libfcrypto/libfcrypto.c` & `libfcrypto-20240414/libfcrypto/libfcrypto.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libfcrypto/libfcrypto_types.h` & `libfcrypto-20240414/libfcrypto/libfcrypto_types.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libfcrypto/libfcrypto_rc4_context.h` & `libfcrypto-20240414/libfcrypto/libfcrypto_rc4_context.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libfcrypto/libfcrypto_support.c` & `libfcrypto-20240414/libfcrypto/libfcrypto_support.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libfcrypto/libfcrypto_definitions.h.in` & `libfcrypto-20240414/libfcrypto/libfcrypto_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libfcrypto/libfcrypto_definitions.h` & `libfcrypto-20240414/libfcrypto/libfcrypto_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfcrypto/definitions.h> are copied here
  * for local use of libfcrypto
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFCRYPTO_VERSION			20240115
+#define LIBFCRYPTO_VERSION			20240414
 
 /* The version string
  */
-#define LIBFCRYPTO_VERSION_STRING		"20240115"
+#define LIBFCRYPTO_VERSION_STRING		"20240414"
 
 /* The crypt modes
  */
 enum LIBFCRYPTO_CRYPT_MODES
 {
 	LIBFCRYPTO_CRYPT_MODE_DECRYPT		= 0,
 	LIBFCRYPTO_CRYPT_MODE_ENCRYPT		= 1
```

### Comparing `libfcrypto-20240115/libfcrypto/libfcrypto_rc4_context.c` & `libfcrypto-20240414/libfcrypto/libfcrypto_rc4_context.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libfcrypto/Makefile.am` & `libfcrypto-20240414/libfcrypto/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBFCRYPTO_DLL_EXPORT@
 
 lib_LTLIBRARIES = libfcrypto.la
 
 libfcrypto_la_SOURCES = \
 	libfcrypto.c \
@@ -26,21 +26,19 @@
 libfcrypto_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libfcrypto_definitions.h.in \
 	libfcrypto.rc \
 	libfcrypto.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfcrypto_definitions.h \
+	libfcrypto.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libfcrypto_definitions.h
-	-rm -f libfcrypto.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcrypto ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcrypto_la_SOURCES)
```

### Comparing `libfcrypto-20240115/libfcrypto/libfcrypto.rc.in` & `libfcrypto-20240414/libfcrypto/libfcrypto.rc.in`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libfcrypto/libfcrypto_serpent_context.h` & `libfcrypto-20240414/libfcrypto/libfcrypto_serpent_context.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libfcrypto/libfcrypto_serpent_context.c` & `libfcrypto-20240414/libfcrypto/libfcrypto_serpent_context.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libfcrypto/libfcrypto_des3_context.c` & `libfcrypto-20240414/libfcrypto/libfcrypto_des3_context.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libfcrypto/libfcrypto_des3_context.h` & `libfcrypto-20240414/libfcrypto/libfcrypto_des3_context.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libfcrypto/libfcrypto_error.c` & `libfcrypto-20240414/libfcrypto/libfcrypto_error.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libfcrypto/libfcrypto_support.h` & `libfcrypto-20240414/libfcrypto/libfcrypto_support.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libfcrypto/libfcrypto_error.h` & `libfcrypto-20240414/libfcrypto/libfcrypto_error.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libfcrypto/libfcrypto_libcerror.h` & `libfcrypto-20240414/libfcrypto/libfcrypto_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libfcrypto/Makefile.in` & `libfcrypto-20240414/libfcrypto/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -402,16 +402,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBFCRYPTO_DLL_EXPORT@
 
 lib_LTLIBRARIES = libfcrypto.la
 libfcrypto_la_SOURCES = \
 	libfcrypto.c \
 	libfcrypto_blowfish_context.c libfcrypto_blowfish_context.h \
@@ -431,15 +431,18 @@
 
 libfcrypto_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libfcrypto_definitions.h.in \
 	libfcrypto.rc \
 	libfcrypto.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfcrypto_definitions.h \
+	libfcrypto.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -676,24 +679,33 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libLTLIBRARIES clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfcrypto.Plo
+	-rm -f ./$(DEPDIR)/libfcrypto_blowfish_context.Plo
+	-rm -f ./$(DEPDIR)/libfcrypto_des3_context.Plo
+	-rm -f ./$(DEPDIR)/libfcrypto_error.Plo
+	-rm -f ./$(DEPDIR)/libfcrypto_rc4_context.Plo
+	-rm -f ./$(DEPDIR)/libfcrypto_serpent_context.Plo
+	-rm -f ./$(DEPDIR)/libfcrypto_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -783,19 +795,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libfcrypto_definitions.h
-	-rm -f libfcrypto.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcrypto ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcrypto_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfcrypto-20240115/libfcrypto/libfcrypto_unused.h` & `libfcrypto-20240414/libfcrypto/libfcrypto_unused.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libfcrypto/libfcrypto.rc` & `libfcrypto-20240414/libfcrypto/libfcrypto.rc`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to support encryption formats\0"
-      VALUE "FileVersion",		"20240115" "\0"
+      VALUE "FileVersion",		"20240414" "\0"
       VALUE "InternalName",		"libfcrypto.dll\0"
       VALUE "LegalCopyright",		"(C) 2017-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libfcrypto.dll\0"
       VALUE "ProductName",		"libfcrypto\0"
-      VALUE "ProductVersion",		"20240115" "\0"
+      VALUE "ProductVersion",		"20240414" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libfcrypto/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libfcrypto-20240115/test-driver` & `libfcrypto-20240414/test-driver`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/manuals/Makefile.in` & `libfcrypto-20240414/manuals/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -349,15 +349,16 @@
 top_srcdir = @top_srcdir@
 man_MANS = \
 	libfcrypto.3
 
 EXTRA_DIST = \
 	libfcrypto.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -507,23 +508,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -604,13 +607,10 @@
 	mostlyclean mostlyclean-generic mostlyclean-libtool pdf pdf-am \
 	ps ps-am sources-am sources-local splint-am splint-local \
 	tags-am uninstall uninstall-am uninstall-man uninstall-man3
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfcrypto-20240115/manuals/libfcrypto.3` & `libfcrypto-20240414/manuals/libfcrypto.3`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/tests/fcrypto_test_libcerror.h` & `libfcrypto-20240414/tests/fcrypto_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/tests/fcrypto_test_memory.c` & `libfcrypto-20240414/tests/fcrypto_test_memory.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/tests/pyfcrypto_test_rc4_context.py` & `libfcrypto-20240414/tests/pyfcrypto_test_rc4_context.py`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/tests/fcrypto_test_serpent_context.c` & `libfcrypto-20240414/tests/fcrypto_test_serpent_context.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/tests/pyfcrypto_test_support.py` & `libfcrypto-20240414/tests/pyfcrypto_test_support.py`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/tests/fcrypto_test_macros.h` & `libfcrypto-20240414/tests/fcrypto_test_macros.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/tests/fcrypto_test_blowfish_context.c` & `libfcrypto-20240414/tests/fcrypto_test_blowfish_context.c`

 * *Files 12% similar despite different names*

```diff
@@ -32,14 +32,138 @@
 #include "fcrypto_test_libfcrypto.h"
 #include "fcrypto_test_macros.h"
 #include "fcrypto_test_memory.h"
 #include "fcrypto_test_unused.h"
 
 #include "../libfcrypto/libfcrypto_blowfish_context.h"
 
+typedef struct fcrypto_test_blowfish_test_vector fcrypto_test_blowfish_test_vector_t;
+
+struct fcrypto_test_blowfish_test_vector
+{
+        /* The key
+         */
+        uint8_t key[ 8 ];
+
+        /* The unencrypted data
+         */
+        uint8_t unencrypted_data[ 8 ];
+
+        /* The encrypted data
+         */
+        uint8_t encrypted_data[ 8 ];
+};
+
+#define FCRYPTO_TEST_BLOWFISH_NUMBER_OF_TEST_VECTORS	34
+
+fcrypto_test_blowfish_test_vector_t fcrypto_test_blowfish_test_vectors[ FCRYPTO_TEST_BLOWFISH_NUMBER_OF_TEST_VECTORS ] = {
+	{ { 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00 },
+	  { 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00 },
+	  { 0x4e, 0xf9, 0x97, 0x45, 0x61, 0x98, 0xdd, 0x78 } },
+	{ { 0xff, 0xff, 0xff, 0xff, 0xff, 0xff, 0xff, 0xff },
+	  { 0xff, 0xff, 0xff, 0xff, 0xff, 0xff, 0xff, 0xff },
+	  { 0x51, 0x86, 0x6f, 0xd5, 0xb8, 0x5e, 0xcb, 0x8a } },
+	{ { 0x30, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00 },
+	  { 0x10, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x01 },
+	  { 0x7d, 0x85, 0x6f, 0x9a, 0x61, 0x30, 0x63, 0xf2 } },
+	{ { 0x11, 0x11, 0x11, 0x11, 0x11, 0x11, 0x11, 0x11 },
+	  { 0x11, 0x11, 0x11, 0x11, 0x11, 0x11, 0x11, 0x11 },
+	  { 0x24, 0x66, 0xdd, 0x87, 0x8b, 0x96, 0x3c, 0x9d } },
+	{ { 0x01, 0x23, 0x45, 0x67, 0x89, 0xab, 0xcd, 0xef },
+	  { 0x11, 0x11, 0x11, 0x11, 0x11, 0x11, 0x11, 0x11 },
+	  { 0x61, 0xf9, 0xc3, 0x80, 0x22, 0x81, 0xb0, 0x96 } },
+	{ { 0x11, 0x11, 0x11, 0x11, 0x11, 0x11, 0x11, 0x11 },
+	  { 0x01, 0x23, 0x45, 0x67, 0x89, 0xab, 0xcd, 0xef },
+	  { 0x7d, 0x0c, 0xc6, 0x30, 0xaf, 0xda, 0x1e, 0xc7 } },
+	{ { 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00 },
+	  { 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00 },
+	  { 0x4e, 0xf9, 0x97, 0x45, 0x61, 0x98, 0xdd, 0x78 } },
+	{ { 0xfe, 0xdc, 0xba, 0x98, 0x76, 0x54, 0x32, 0x10 },
+	  { 0x01, 0x23, 0x45, 0x67, 0x89, 0xab, 0xcd, 0xef },
+	  { 0x0a, 0xce, 0xab, 0x0f, 0xc6, 0xa0, 0xa2, 0x8d } },
+	{ { 0x7c, 0xa1, 0x10, 0x45, 0x4a, 0x1a, 0x6e, 0x57 },
+	  { 0x01, 0xa1, 0xd6, 0xd0, 0x39, 0x77, 0x67, 0x42 },
+	  { 0x59, 0xc6, 0x82, 0x45, 0xeb, 0x05, 0x28, 0x2b } },
+	{ { 0x01, 0x31, 0xd9, 0x61, 0x9d, 0xc1, 0x37, 0x6e },
+	  { 0x5c, 0xd5, 0x4c, 0xa8, 0x3d, 0xef, 0x57, 0xda },
+	  { 0xb1, 0xb8, 0xcc, 0x0b, 0x25, 0x0f, 0x09, 0xa0 } },
+	{ { 0x07, 0xa1, 0x13, 0x3e, 0x4a, 0x0b, 0x26, 0x86 },
+	  { 0x02, 0x48, 0xd4, 0x38, 0x06, 0xf6, 0x71, 0x72 },
+	  { 0x17, 0x30, 0xe5, 0x77, 0x8b, 0xea, 0x1d, 0xa4 } },
+	{ { 0x38, 0x49, 0x67, 0x4c, 0x26, 0x02, 0x31, 0x9e },
+	  { 0x51, 0x45, 0x4b, 0x58, 0x2d, 0xdf, 0x44, 0x0a },
+	  { 0xa2, 0x5e, 0x78, 0x56, 0xcf, 0x26, 0x51, 0xeb } },
+	{ { 0x04, 0xb9, 0x15, 0xba, 0x43, 0xfe, 0xb5, 0xb6 },
+	  { 0x42, 0xfd, 0x44, 0x30, 0x59, 0x57, 0x7f, 0xa2 },
+	  { 0x35, 0x38, 0x82, 0xb1, 0x09, 0xce, 0x8f, 0x1a } },
+	{ { 0x01, 0x13, 0xb9, 0x70, 0xfd, 0x34, 0xf2, 0xce },
+	  { 0x05, 0x9b, 0x5e, 0x08, 0x51, 0xcf, 0x14, 0x3a },
+	  { 0x48, 0xf4, 0xd0, 0x88, 0x4c, 0x37, 0x99, 0x18 } },
+	{ { 0x01, 0x70, 0xf1, 0x75, 0x46, 0x8f, 0xb5, 0xe6 },
+	  { 0x07, 0x56, 0xd8, 0xe0, 0x77, 0x47, 0x61, 0xd2 },
+	  { 0x43, 0x21, 0x93, 0xb7, 0x89, 0x51, 0xfc, 0x98 } },
+	{ { 0x43, 0x29, 0x7f, 0xad, 0x38, 0xe3, 0x73, 0xfe },
+	  { 0x76, 0x25, 0x14, 0xb8, 0x29, 0xbf, 0x48, 0x6a },
+	  { 0x13, 0xf0, 0x41, 0x54, 0xd6, 0x9d, 0x1a, 0xe5 } },
+	{ { 0x07, 0xa7, 0x13, 0x70, 0x45, 0xda, 0x2a, 0x16 },
+	  { 0x3b, 0xdd, 0x11, 0x90, 0x49, 0x37, 0x28, 0x02 },
+	  { 0x2e, 0xed, 0xda, 0x93, 0xff, 0xd3, 0x9c, 0x79 } },
+	{ { 0x04, 0x68, 0x91, 0x04, 0xc2, 0xfd, 0x3b, 0x2f },
+	  { 0x26, 0x95, 0x5f, 0x68, 0x35, 0xaf, 0x60, 0x9a },
+	  { 0xd8, 0x87, 0xe0, 0x39, 0x3c, 0x2d, 0xa6, 0xe3 } },
+	{ { 0x37, 0xd0, 0x6b, 0xb5, 0x16, 0xcb, 0x75, 0x46 },
+	  { 0x16, 0x4d, 0x5e, 0x40, 0x4f, 0x27, 0x52, 0x32 },
+	  { 0x5f, 0x99, 0xd0, 0x4f, 0x5b, 0x16, 0x39, 0x69 } },
+	{ { 0x1f, 0x08, 0x26, 0x0d, 0x1a, 0xc2, 0x46, 0x5e },
+	  { 0x6b, 0x05, 0x6e, 0x18, 0x75, 0x9f, 0x5c, 0xca },
+	  { 0x4a, 0x05, 0x7a, 0x3b, 0x24, 0xd3, 0x97, 0x7b } },
+	{ { 0x58, 0x40, 0x23, 0x64, 0x1a, 0xba, 0x61, 0x76 },
+	  { 0x00, 0x4b, 0xd6, 0xef, 0x09, 0x17, 0x60, 0x62 },
+	  { 0x45, 0x20, 0x31, 0xc1, 0xe4, 0xfa, 0xda, 0x8e } },
+	{ { 0x02, 0x58, 0x16, 0x16, 0x46, 0x29, 0xb0, 0x07 },
+	  { 0x48, 0x0d, 0x39, 0x00, 0x6e, 0xe7, 0x62, 0xf2 },
+	  { 0x75, 0x55, 0xae, 0x39, 0xf5, 0x9b, 0x87, 0xbd } },
+	{ { 0x49, 0x79, 0x3e, 0xbc, 0x79, 0xb3, 0x25, 0x8f },
+	  { 0x43, 0x75, 0x40, 0xc8, 0x69, 0x8f, 0x3c, 0xfa },
+	  { 0x53, 0xc5, 0x5f, 0x9c, 0xb4, 0x9f, 0xc0, 0x19 } },
+	{ { 0x4f, 0xb0, 0x5e, 0x15, 0x15, 0xab, 0x73, 0xa7 },
+	  { 0x07, 0x2d, 0x43, 0xa0, 0x77, 0x07, 0x52, 0x92 },
+	  { 0x7a, 0x8e, 0x7b, 0xfa, 0x93, 0x7e, 0x89, 0xa3 } },
+	{ { 0x49, 0xe9, 0x5d, 0x6d, 0x4c, 0xa2, 0x29, 0xbf },
+	  { 0x02, 0xfe, 0x55, 0x77, 0x81, 0x17, 0xf1, 0x2a },
+	  { 0xcf, 0x9c, 0x5d, 0x7a, 0x49, 0x86, 0xad, 0xb5 } },
+	{ { 0x01, 0x83, 0x10, 0xdc, 0x40, 0x9b, 0x26, 0xd6 },
+	  { 0x1d, 0x9d, 0x5c, 0x50, 0x18, 0xf7, 0x28, 0xc2 },
+	  { 0xd1, 0xab, 0xb2, 0x90, 0x65, 0x8b, 0xc7, 0x78 } },
+	{ { 0x1c, 0x58, 0x7f, 0x1c, 0x13, 0x92, 0x4f, 0xef },
+	  { 0x30, 0x55, 0x32, 0x28, 0x6d, 0x6f, 0x29, 0x5a },
+	  { 0x55, 0xcb, 0x37, 0x74, 0xd1, 0x3e, 0xf2, 0x01 } },
+	{ { 0x01, 0x01, 0x01, 0x01, 0x01, 0x01, 0x01, 0x01 },
+	  { 0x01, 0x23, 0x45, 0x67, 0x89, 0xab, 0xcd, 0xef },
+	  { 0xfa, 0x34, 0xec, 0x48, 0x47, 0xb2, 0x68, 0xb2 } },
+	{ { 0x1f, 0x1f, 0x1f, 0x1f, 0x0e, 0x0e, 0x0e, 0x0e },
+	  { 0x01, 0x23, 0x45, 0x67, 0x89, 0xab, 0xcd, 0xef },
+	  { 0xa7, 0x90, 0x79, 0x51, 0x08, 0xea, 0x3c, 0xae } },
+	{ { 0xe0, 0xfe, 0xe0, 0xfe, 0xf1, 0xfe, 0xf1, 0xfe },
+	  { 0x01, 0x23, 0x45, 0x67, 0x89, 0xab, 0xcd, 0xef },
+	  { 0xc3, 0x9e, 0x07, 0x2d, 0x9f, 0xac, 0x63, 0x1d } },
+	{ { 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00 },
+	  { 0xff, 0xff, 0xff, 0xff, 0xff, 0xff, 0xff, 0xff },
+	  { 0x01, 0x49, 0x33, 0xe0, 0xcd, 0xaf, 0xf6, 0xe4 } },
+	{ { 0xff, 0xff, 0xff, 0xff, 0xff, 0xff, 0xff, 0xff },
+	  { 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00 },
+	  { 0xf2, 0x1e, 0x9a, 0x77, 0xb7, 0x1c, 0x49, 0xbc } },
+	{ { 0x01, 0x23, 0x45, 0x67, 0x89, 0xab, 0xcd, 0xef },
+	  { 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00 },
+	  { 0x24, 0x59, 0x46, 0x88, 0x57, 0x54, 0x36, 0x9a } },
+	{ { 0xfe, 0xdc, 0xba, 0x98, 0x76, 0x54, 0x32, 0x10 },
+	  { 0xff, 0xff, 0xff, 0xff, 0xff, 0xff, 0xff, 0xff },
+	  { 0x6b, 0x5c, 0x5a, 0x9c, 0x5d, 0x9e, 0x0a, 0x5a } }
+};
+
 /* Tests the libfcrypto_blowfish_context_initialize function
  * Returns 1 if successful or 0 if not
  */
 int fcrypto_test_blowfish_context_initialize(
      void )
 {
 	libcerror_error_t *error                        = NULL;
@@ -1715,14 +1839,175 @@
 		libfcrypto_blowfish_context_free(
 		 &blowfish_context,
 		 NULL );
 	}
 	return( 0 );
 }
 
+/* Tests the libfcrypto_blowfish_crypt function with a test vector
+ * Returns 1 if successful or 0 if not
+ */
+int fcrypto_test_blowfish_crypt_with_test_vector(
+     fcrypto_test_blowfish_test_vector_t *test_vector )
+{
+	uint8_t output_data[ 8 ];
+
+	libcerror_error_t *error                        = NULL;
+	libfcrypto_blowfish_context_t *blowfish_context = NULL;
+	int result                                      = 0;
+
+	FCRYPTO_TEST_ASSERT_IS_NOT_NULL(
+	 "test_vector",
+	 test_vector );
+
+	result = libfcrypto_blowfish_context_initialize(
+	          &blowfish_context,
+	          &error );
+
+	FCRYPTO_TEST_ASSERT_EQUAL_INT(
+	 "result",
+	 result,
+	 1 );
+
+	FCRYPTO_TEST_ASSERT_IS_NOT_NULL(
+	 "blowfish_context",
+	 blowfish_context );
+
+	FCRYPTO_TEST_ASSERT_IS_NULL(
+	 "error",
+	 error );
+
+	result = libfcrypto_blowfish_context_set_key(
+	          blowfish_context,
+	          test_vector->key,
+	          64,
+	          &error );
+
+	FCRYPTO_TEST_ASSERT_EQUAL_INT(
+	 "result",
+	 result,
+	 1 );
+
+	FCRYPTO_TEST_ASSERT_IS_NULL(
+	 "error",
+	 error );
+
+	result = libfcrypto_blowfish_crypt_ecb(
+	          blowfish_context,
+	          LIBFCRYPTO_BLOWFISH_CRYPT_MODE_DECRYPT,
+	          test_vector->encrypted_data,
+	          8,
+	          output_data,
+	          8,
+	          &error );
+
+	FCRYPTO_TEST_ASSERT_EQUAL_INT(
+	 "result",
+	 result,
+	 1 );
+
+	FCRYPTO_TEST_ASSERT_IS_NULL(
+	 "error",
+	 error );
+
+	result = memory_compare(
+	          output_data,
+	          test_vector->unencrypted_data,
+	          8 );
+
+	FCRYPTO_TEST_ASSERT_EQUAL_INT(
+	 "result",
+	 result,
+	 0 );
+
+	result = libfcrypto_blowfish_crypt_ecb(
+	          blowfish_context,
+	          LIBFCRYPTO_BLOWFISH_CRYPT_MODE_ENCRYPT,
+	          test_vector->unencrypted_data,
+	          8,
+	          output_data,
+	          8,
+	          &error );
+
+	FCRYPTO_TEST_ASSERT_EQUAL_INT(
+	 "result",
+	 result,
+	 1 );
+
+	FCRYPTO_TEST_ASSERT_IS_NULL(
+	 "error",
+	 error );
+
+	result = memory_compare(
+	          output_data,
+	          test_vector->encrypted_data,
+	          8 );
+
+	FCRYPTO_TEST_ASSERT_EQUAL_INT(
+	 "result",
+	 result,
+	 0 );
+
+	result = libfcrypto_blowfish_context_free(
+	          &blowfish_context,
+	          &error );
+
+	FCRYPTO_TEST_ASSERT_EQUAL_INT(
+	 "result",
+	 result,
+	 1 );
+
+	FCRYPTO_TEST_ASSERT_IS_NULL(
+	 "blowfish_context",
+	 blowfish_context );
+
+	FCRYPTO_TEST_ASSERT_IS_NULL(
+	 "error",
+	 error );
+
+	return( 1 );
+
+on_error:
+	if( error != NULL )
+	{
+		libcerror_error_free(
+		 &error );
+	}
+	if( blowfish_context != NULL )
+	{
+		libfcrypto_blowfish_context_free(
+		 &blowfish_context,
+		 NULL );
+	}
+	return( 0 );
+}
+
+/* Tests the libfcrypto_blowfish_crypt function with test vectors
+ * See: https://www.schneier.com/wp-content/uploads/2015/12/vectors-2.txt
+ * Returns 1 if successful or 0 if not
+ */
+int fcrypto_test_blowfish_crypt_with_test_vectors(
+     void )
+{
+	int result      = 0;
+	int test_vector = 0;
+
+	while( test_vector < FCRYPTO_TEST_BLOWFISH_NUMBER_OF_TEST_VECTORS )
+	{
+		result = fcrypto_test_blowfish_crypt_with_test_vector(
+		          &( fcrypto_test_blowfish_test_vectors[ test_vector++ ] ) );
+
+		if( result == 0 )
+		{
+			break;
+		}
+	}
+	return( result );
+}
+
 /* The main program
  */
 #if defined( HAVE_WIDE_SYSTEM_CHARACTER )
 int wmain(
      int argc FCRYPTO_TEST_ATTRIBUTE_UNUSED,
      wchar_t * const argv[] FCRYPTO_TEST_ATTRIBUTE_UNUSED )
 #else
@@ -1770,13 +2055,17 @@
 	 "libfcrypto_blowfish_crypt_cbc",
 	 fcrypto_test_blowfish_crypt_cbc );
 
 	FCRYPTO_TEST_RUN(
 	 "libfcrypto_blowfish_crypt_ecb",
 	 fcrypto_test_blowfish_crypt_ecb );
 
+	FCRYPTO_TEST_RUN(
+	 "libfcrypto_blowfish_crypt_with_test_vectors",
+	 fcrypto_test_blowfish_crypt_with_test_vectors );
+
 	return( EXIT_SUCCESS );
 
 on_error:
 	return( EXIT_FAILURE );
 }
```

### Comparing `libfcrypto-20240115/tests/pyfcrypto_test_blowfish_context.py` & `libfcrypto-20240414/tests/pyfcrypto_test_blowfish_context.py`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/tests/Makefile.am` & `libfcrypto-20240414/tests/Makefile.am`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBFCRYPTO_DLL_IMPORT@
 
 if HAVE_PYTHON_TESTS
 TESTS_PYFCRYPTO = \
 	test_python_module.sh
 endif
@@ -97,13 +97,11 @@
 	fcrypto_test_macros.h \
 	fcrypto_test_support.c \
 	fcrypto_test_unused.h
 
 fcrypto_test_support_LDADD = \
 	../libfcrypto/libfcrypto.la
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libfcrypto-20240115/tests/fcrypto_test_memory.h` & `libfcrypto-20240414/tests/fcrypto_test_memory.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/tests/fcrypto_test_des3_context.c` & `libfcrypto-20240414/tests/fcrypto_test_des3_context.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/tests/pyfcrypto_test_des3_context.py` & `libfcrypto-20240414/tests/pyfcrypto_test_des3_context.py`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/tests/fcrypto_test_rc4_context.c` & `libfcrypto-20240414/tests/fcrypto_test_rc4_context.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/tests/test_python_module.sh` & `libfcrypto-20240414/tests/test_python_module.sh`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
+EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="blowfish_context des3_context rc4_context serpent_context support";
 TEST_FUNCTIONS_WITH_INPUT="";
 OPTION_SETS=();
 
 TEST_TOOL_DIRECTORY=".";
@@ -120,20 +121,17 @@
 }
 
 if test -n "${SKIP_PYTHON_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
@@ -143,15 +141,19 @@
 RESULT=${EXIT_IGNORE};
 
 for TEST_FUNCTION in ${TEST_FUNCTIONS};
 do
 	test_python_function "${TEST_FUNCTION}";
 	RESULT=$?;
 
-	if test ${RESULT} -ne ${EXIT_SUCCESS};
+	if test ${RESULT} -eq ${EXIT_NO_TESTS_RAN};
+	then
+		RESULT=${EXIT_IGNORE};
+	fi
+	if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 	then
 		break;
 	fi
 done
 
 if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 then
@@ -164,16 +166,19 @@
 	then
 		test_python_function_with_input "${TEST_FUNCTION}";
 		RESULT=$?;
 	else
 		test_python_function "${TEST_FUNCTION}";
 		RESULT=$?;
 	fi
-
-	if test ${RESULT} -ne ${EXIT_SUCCESS};
+	if test ${RESULT} -eq ${EXIT_NO_TESTS_RAN};
+	then
+		RESULT=${EXIT_IGNORE};
+	fi
+	if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 	then
 		break;
 	fi
 done
 
 exit ${RESULT};
```

### Comparing `libfcrypto-20240115/tests/fcrypto_test_error.c` & `libfcrypto-20240414/tests/fcrypto_test_error.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/tests/pyfcrypto_test_serpent_context.py` & `libfcrypto-20240414/tests/pyfcrypto_test_serpent_context.py`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/tests/test_runner.sh` & `libfcrypto-20240414/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/tests/fcrypto_test_unused.h` & `libfcrypto-20240414/tests/fcrypto_test_unused.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/tests/Makefile.in` & `libfcrypto-20240414/tests/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -614,16 +614,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBFCRYPTO_DLL_IMPORT@
 
 @HAVE_PYTHON_TESTS_TRUE@TESTS_PYFCRYPTO = \
 @HAVE_PYTHON_TESTS_TRUE@	test_python_module.sh
 
 TESTS = \
@@ -706,15 +706,16 @@
 	fcrypto_test_macros.h \
 	fcrypto_test_support.c \
 	fcrypto_test_unused.h
 
 fcrypto_test_support_LDADD = \
 	../libfcrypto/libfcrypto.la
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .log .o .obj .test .test$(EXEEXT) .trs
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1114,24 +1115,33 @@
 	-test -z "$(TEST_SUITE_LOG)" || rm -f $(TEST_SUITE_LOG)
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/fcrypto_test_blowfish_context.Po
+	-rm -f ./$(DEPDIR)/fcrypto_test_des3_context.Po
+	-rm -f ./$(DEPDIR)/fcrypto_test_error.Po
+	-rm -f ./$(DEPDIR)/fcrypto_test_memory.Po
+	-rm -f ./$(DEPDIR)/fcrypto_test_rc4_context.Po
+	-rm -f ./$(DEPDIR)/fcrypto_test_serpent_context.Po
+	-rm -f ./$(DEPDIR)/fcrypto_test_support.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1221,13 +1231,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	recheck sources-am sources-local splint-am splint-local tags \
 	tags-am uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfcrypto-20240115/tests/fcrypto_test_support.c` & `libfcrypto-20240414/tests/fcrypto_test_support.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/tests/fcrypto_test_libfcrypto.h` & `libfcrypto-20240414/tests/fcrypto_test_libfcrypto.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/tests/test_library.sh` & `libfcrypto-20240414/tests/test_library.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests library functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 LIBRARY_TESTS="blowfish_context des3_context error rc4_context serpent_context support";
 LIBRARY_TESTS_WITH_INPUT="";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_LIBRARY_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libfcrypto-20240115/ossfuzz/ossfuzz_libfcrypto.h` & `libfcrypto-20240414/ossfuzz/ossfuzz_libfcrypto.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/ossfuzz/crypt_rc4_fuzzer.cc` & `libfcrypto-20240414/ossfuzz/crypt_rc4_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/ossfuzz/crypt_serpent_cbc_fuzzer.cc` & `libfcrypto-20240414/ossfuzz/crypt_serpent_cbc_fuzzer.cc`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,18 @@
 #include "ossfuzz_libfcrypto.h"
 
 int LLVMFuzzerTestOneInput(
      const uint8_t *data,
      size_t size )
 {
 	uint8_t encrypted_data[ 64 ];
+
 	uint8_t initialization_vector[ 16 ] = {
 		0x00, 0x01, 0x02, 0x03, 0x04, 0x05, 0x06, 0x07, 0x08, 0x09, 0x0a, 0x0b, 0x0c, 0x0d, 0x0e, 0x0f };
-	uint8_t key[ 16 ]  = {
+	uint8_t key[ 16 ] = {
 		0x00, 0x01, 0x02, 0x03, 0x04, 0x05, 0x06, 0x07, 0x08, 0x09, 0x0a, 0x0b, 0x0c, 0x0d, 0x0e, 0x0f };
 
 	libfcrypto_serpent_context_t *context = NULL;
 
 	if( libfcrypto_serpent_context_initialize(
 	     &context,
 	     NULL ) != 1 )
```

### Comparing `libfcrypto-20240115/ossfuzz/crypt_serpent_ecb_fuzzer.cc` & `libfcrypto-20240414/ossfuzz/crypt_serpent_ecb_fuzzer.cc`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 int LLVMFuzzerTestOneInput(
      const uint8_t *data,
      size_t size )
 {
 	uint8_t encrypted_data[ 64 ];
 
-	uint8_t key[ 16 ]  = {
+	uint8_t key[ 16 ] = {
 		0x00, 0x01, 0x02, 0x03, 0x04, 0x05, 0x06, 0x07, 0x08, 0x09, 0x0a, 0x0b, 0x0c, 0x0d, 0x0e, 0x0f };
 
 	libfcrypto_serpent_context_t *context = NULL;
 
 	if( libfcrypto_serpent_context_initialize(
 	     &context,
 	     NULL ) != 1 )
```

### Comparing `libfcrypto-20240115/ossfuzz/Makefile.am` & `libfcrypto-20240414/ossfuzz/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,53 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common
 
 bin_PROGRAMS = \
+	crypt_blowfish_cbc_fuzzer \
 	crypt_blowfish_ecb_fuzzer \
+	crypt_des3_cbc_fuzzer \
+	crypt_des3_ecb_fuzzer \
 	crypt_rc4_fuzzer \
 	crypt_serpent_cbc_fuzzer \
 	crypt_serpent_ecb_fuzzer
 
+crypt_blowfish_cbc_fuzzer_SOURCES = \
+	crypt_blowfish_cbc_fuzzer.cc \
+	ossfuzz_libfcrypto.h
+
+crypt_blowfish_cbc_fuzzer_LDADD = \
+	@LIB_FUZZING_ENGINE@ \
+	../libfcrypto/libfcrypto.la
+
 crypt_blowfish_ecb_fuzzer_SOURCES = \
 	crypt_blowfish_ecb_fuzzer.cc \
 	ossfuzz_libfcrypto.h
 
 crypt_blowfish_ecb_fuzzer_LDADD = \
 	@LIB_FUZZING_ENGINE@ \
 	../libfcrypto/libfcrypto.la
 
+crypt_des3_cbc_fuzzer_SOURCES = \
+	crypt_des3_cbc_fuzzer.cc \
+	ossfuzz_libfcrypto.h
+
+crypt_des3_cbc_fuzzer_LDADD = \
+	@LIB_FUZZING_ENGINE@ \
+	../libfcrypto/libfcrypto.la
+
+crypt_des3_ecb_fuzzer_SOURCES = \
+	crypt_des3_ecb_fuzzer.cc \
+	ossfuzz_libfcrypto.h
+
+crypt_des3_ecb_fuzzer_LDADD = \
+	@LIB_FUZZING_ENGINE@ \
+	../libfcrypto/libfcrypto.la
+
 crypt_rc4_fuzzer_SOURCES = \
 	crypt_rc4_fuzzer.cc \
 	ossfuzz_libfcrypto.h
 
 crypt_rc4_fuzzer_LDADD = \
 	@LIB_FUZZING_ENGINE@ \
 	../libfcrypto/libfcrypto.la
@@ -38,23 +65,27 @@
 	ossfuzz_libfcrypto.h
 
 crypt_serpent_ecb_fuzzer_LDADD = \
 	@LIB_FUZZING_ENGINE@ \
 	../libfcrypto/libfcrypto.la
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
+	@echo "Running splint on crypt_blowfish_cbc_fuzzer ..."
+	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(crypt_blowfish_cbc_fuzzer_SOURCES)
 	@echo "Running splint on crypt_blowfish_ecb_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(crypt_blowfish_ecb_fuzzer_SOURCES)
+	@echo "Running splint on crypt_des3_cbc_fuzzer ..."
+	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(crypt_des3_cbc_fuzzer_SOURCES)
+	@echo "Running splint on crypt_des3_ecb_fuzzer ..."
+	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(crypt_des3_ecb_fuzzer_SOURCES)
 	@echo "Running splint on crypt_rc4_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(crypt_rc4_fuzzer_SOURCES)
 	@echo "Running splint on crypt_serpent_cbc_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(crypt_serpent_cbc_fuzzer_SOURCES)
 	@echo "Running splint on crypt_serpent_ecb_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(crypt_serpent_ecb_fuzzer_SOURCES)
```

### Comparing `libfcrypto-20240115/ossfuzz/crypt_blowfish_ecb_fuzzer.cc` & `libfcrypto-20240414/ossfuzz/crypt_blowfish_ecb_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/ossfuzz/Makefile.in` & `libfcrypto-20240414/Makefile.in`

 * *Files 23% similar despite different names*

```diff
@@ -84,19 +84,15 @@
 PRE_INSTALL = :
 POST_INSTALL = :
 NORMAL_UNINSTALL = :
 PRE_UNINSTALL = :
 POST_UNINSTALL = :
 build_triplet = @build@
 host_triplet = @host@
-@HAVE_LIB_FUZZING_ENGINE_TRUE@bin_PROGRAMS = crypt_blowfish_ecb_fuzzer$(EXEEXT) \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	crypt_rc4_fuzzer$(EXEEXT) \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	crypt_serpent_cbc_fuzzer$(EXEEXT) \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	crypt_serpent_ecb_fuzzer$(EXEEXT)
-subdir = ossfuzz
+subdir = .
 ACLOCAL_M4 = $(top_srcdir)/aclocal.m4
 am__aclocal_m4_deps = $(top_srcdir)/m4/common.m4 \
 	$(top_srcdir)/m4/gettext.m4 $(top_srcdir)/m4/host-cpu-c-abi.m4 \
 	$(top_srcdir)/m4/iconv.m4 $(top_srcdir)/m4/intlmacosx.m4 \
 	$(top_srcdir)/m4/lib-ld.m4 $(top_srcdir)/m4/lib-link.m4 \
 	$(top_srcdir)/m4/lib-prefix.m4 $(top_srcdir)/m4/libcerror.m4 \
 	$(top_srcdir)/m4/libtool.m4 $(top_srcdir)/m4/ltoptions.m4 \
@@ -104,122 +100,88 @@
 	$(top_srcdir)/m4/lt~obsolete.m4 $(top_srcdir)/m4/nls.m4 \
 	$(top_srcdir)/m4/po.m4 $(top_srcdir)/m4/progtest.m4 \
 	$(top_srcdir)/m4/python.m4 $(top_srcdir)/m4/tests.m4 \
 	$(top_srcdir)/m4/types.m4 $(top_srcdir)/acinclude.m4 \
 	$(top_srcdir)/configure.ac
 am__configure_deps = $(am__aclocal_m4_deps) $(CONFIGURE_DEPENDENCIES) \
 	$(ACLOCAL_M4)
-DIST_COMMON = $(srcdir)/Makefile.am $(am__DIST_COMMON)
+DIST_COMMON = $(srcdir)/Makefile.am $(top_srcdir)/configure \
+	$(am__configure_deps) $(am__DIST_COMMON)
+am__CONFIG_DISTCLEAN_FILES = config.status config.cache config.log \
+ configure.lineno config.status.lineno
 mkinstalldirs = $(install_sh) -d
 CONFIG_HEADER = $(top_builddir)/common/config.h
-CONFIG_CLEAN_FILES =
+CONFIG_CLEAN_FILES = include/libfcrypto/definitions.h \
+	include/libfcrypto/features.h include/libfcrypto/types.h \
+	dpkg/changelog libfcrypto.pc libfcrypto.spec setup.cfg
 CONFIG_CLEAN_VPATH_FILES =
-am__installdirs = "$(DESTDIR)$(bindir)"
-PROGRAMS = $(bin_PROGRAMS)
-am__crypt_blowfish_ecb_fuzzer_SOURCES_DIST =  \
-	crypt_blowfish_ecb_fuzzer.cc ossfuzz_libfcrypto.h
-@HAVE_LIB_FUZZING_ENGINE_TRUE@am_crypt_blowfish_ecb_fuzzer_OBJECTS = crypt_blowfish_ecb_fuzzer.$(OBJEXT)
-crypt_blowfish_ecb_fuzzer_OBJECTS =  \
-	$(am_crypt_blowfish_ecb_fuzzer_OBJECTS)
-@HAVE_LIB_FUZZING_ENGINE_TRUE@crypt_blowfish_ecb_fuzzer_DEPENDENCIES =  \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	../libfcrypto/libfcrypto.la
-AM_V_lt = $(am__v_lt_@AM_V@)
-am__v_lt_ = $(am__v_lt_@AM_DEFAULT_V@)
-am__v_lt_0 = --silent
-am__v_lt_1 = 
-am__crypt_rc4_fuzzer_SOURCES_DIST = crypt_rc4_fuzzer.cc \
-	ossfuzz_libfcrypto.h
-@HAVE_LIB_FUZZING_ENGINE_TRUE@am_crypt_rc4_fuzzer_OBJECTS =  \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	crypt_rc4_fuzzer.$(OBJEXT)
-crypt_rc4_fuzzer_OBJECTS = $(am_crypt_rc4_fuzzer_OBJECTS)
-@HAVE_LIB_FUZZING_ENGINE_TRUE@crypt_rc4_fuzzer_DEPENDENCIES =  \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	../libfcrypto/libfcrypto.la
-am__crypt_serpent_cbc_fuzzer_SOURCES_DIST =  \
-	crypt_serpent_cbc_fuzzer.cc ossfuzz_libfcrypto.h
-@HAVE_LIB_FUZZING_ENGINE_TRUE@am_crypt_serpent_cbc_fuzzer_OBJECTS = crypt_serpent_cbc_fuzzer.$(OBJEXT)
-crypt_serpent_cbc_fuzzer_OBJECTS =  \
-	$(am_crypt_serpent_cbc_fuzzer_OBJECTS)
-@HAVE_LIB_FUZZING_ENGINE_TRUE@crypt_serpent_cbc_fuzzer_DEPENDENCIES =  \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	../libfcrypto/libfcrypto.la
-am__crypt_serpent_ecb_fuzzer_SOURCES_DIST =  \
-	crypt_serpent_ecb_fuzzer.cc ossfuzz_libfcrypto.h
-@HAVE_LIB_FUZZING_ENGINE_TRUE@am_crypt_serpent_ecb_fuzzer_OBJECTS = crypt_serpent_ecb_fuzzer.$(OBJEXT)
-crypt_serpent_ecb_fuzzer_OBJECTS =  \
-	$(am_crypt_serpent_ecb_fuzzer_OBJECTS)
-@HAVE_LIB_FUZZING_ENGINE_TRUE@crypt_serpent_ecb_fuzzer_DEPENDENCIES =  \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	../libfcrypto/libfcrypto.la
 AM_V_P = $(am__v_P_@AM_V@)
 am__v_P_ = $(am__v_P_@AM_DEFAULT_V@)
 am__v_P_0 = false
 am__v_P_1 = :
 AM_V_GEN = $(am__v_GEN_@AM_V@)
 am__v_GEN_ = $(am__v_GEN_@AM_DEFAULT_V@)
 am__v_GEN_0 = @echo "  GEN     " $@;
 am__v_GEN_1 = 
 AM_V_at = $(am__v_at_@AM_V@)
 am__v_at_ = $(am__v_at_@AM_DEFAULT_V@)
 am__v_at_0 = @
 am__v_at_1 = 
-DEFAULT_INCLUDES = -I.@am__isrc@ -I$(top_builddir)/common
-depcomp = $(SHELL) $(top_srcdir)/depcomp
-am__maybe_remake_depfiles = depfiles
-am__depfiles_remade = ./$(DEPDIR)/crypt_blowfish_ecb_fuzzer.Po \
-	./$(DEPDIR)/crypt_rc4_fuzzer.Po \
-	./$(DEPDIR)/crypt_serpent_cbc_fuzzer.Po \
-	./$(DEPDIR)/crypt_serpent_ecb_fuzzer.Po
-am__mv = mv -f
-CXXCOMPILE = $(CXX) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) \
-	$(AM_CPPFLAGS) $(CPPFLAGS) $(AM_CXXFLAGS) $(CXXFLAGS)
-LTCXXCOMPILE = $(LIBTOOL) $(AM_V_lt) --tag=CXX $(AM_LIBTOOLFLAGS) \
-	$(LIBTOOLFLAGS) --mode=compile $(CXX) $(DEFS) \
-	$(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(CPPFLAGS) \
-	$(AM_CXXFLAGS) $(CXXFLAGS)
-AM_V_CXX = $(am__v_CXX_@AM_V@)
-am__v_CXX_ = $(am__v_CXX_@AM_DEFAULT_V@)
-am__v_CXX_0 = @echo "  CXX     " $@;
-am__v_CXX_1 = 
-CXXLD = $(CXX)
-CXXLINK = $(LIBTOOL) $(AM_V_lt) --tag=CXX $(AM_LIBTOOLFLAGS) \
-	$(LIBTOOLFLAGS) --mode=link $(CXXLD) $(AM_CXXFLAGS) \
-	$(CXXFLAGS) $(AM_LDFLAGS) $(LDFLAGS) -o $@
-AM_V_CXXLD = $(am__v_CXXLD_@AM_V@)
-am__v_CXXLD_ = $(am__v_CXXLD_@AM_DEFAULT_V@)
-am__v_CXXLD_0 = @echo "  CXXLD   " $@;
-am__v_CXXLD_1 = 
-COMPILE = $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) \
-	$(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS)
-LTCOMPILE = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
-	$(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) \
-	$(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(CPPFLAGS) \
-	$(AM_CFLAGS) $(CFLAGS)
-AM_V_CC = $(am__v_CC_@AM_V@)
-am__v_CC_ = $(am__v_CC_@AM_DEFAULT_V@)
-am__v_CC_0 = @echo "  CC      " $@;
-am__v_CC_1 = 
-CCLD = $(CC)
-LINK = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
-	$(LIBTOOLFLAGS) --mode=link $(CCLD) $(AM_CFLAGS) $(CFLAGS) \
-	$(AM_LDFLAGS) $(LDFLAGS) -o $@
-AM_V_CCLD = $(am__v_CCLD_@AM_V@)
-am__v_CCLD_ = $(am__v_CCLD_@AM_DEFAULT_V@)
-am__v_CCLD_0 = @echo "  CCLD    " $@;
-am__v_CCLD_1 = 
-SOURCES = $(crypt_blowfish_ecb_fuzzer_SOURCES) \
-	$(crypt_rc4_fuzzer_SOURCES) \
-	$(crypt_serpent_cbc_fuzzer_SOURCES) \
-	$(crypt_serpent_ecb_fuzzer_SOURCES)
-DIST_SOURCES = $(am__crypt_blowfish_ecb_fuzzer_SOURCES_DIST) \
-	$(am__crypt_rc4_fuzzer_SOURCES_DIST) \
-	$(am__crypt_serpent_cbc_fuzzer_SOURCES_DIST) \
-	$(am__crypt_serpent_ecb_fuzzer_SOURCES_DIST)
+SOURCES =
+DIST_SOURCES =
+RECURSIVE_TARGETS = all-recursive check-recursive cscopelist-recursive \
+	ctags-recursive dvi-recursive html-recursive info-recursive \
+	install-data-recursive install-dvi-recursive \
+	install-exec-recursive install-html-recursive \
+	install-info-recursive install-pdf-recursive \
+	install-ps-recursive install-recursive installcheck-recursive \
+	installdirs-recursive pdf-recursive ps-recursive \
+	tags-recursive uninstall-recursive
 am__can_run_installinfo = \
   case $$AM_UPDATE_INFO_DIR in \
     n|no|NO) false;; \
     *) (install-info --version) >/dev/null 2>&1;; \
   esac
+am__vpath_adj_setup = srcdirstrip=`echo "$(srcdir)" | sed 's|.|.|g'`;
+am__vpath_adj = case $$p in \
+    $(srcdir)/*) f=`echo "$$p" | sed "s|^$$srcdirstrip/||"`;; \
+    *) f=$$p;; \
+  esac;
+am__strip_dir = f=`echo $$p | sed -e 's|^.*/||'`;
+am__install_max = 40
+am__nobase_strip_setup = \
+  srcdirstrip=`echo "$(srcdir)" | sed 's/[].[^$$\\*|]/\\\\&/g'`
+am__nobase_strip = \
+  for p in $$list; do echo "$$p"; done | sed -e "s|$$srcdirstrip/||"
+am__nobase_list = $(am__nobase_strip_setup); \
+  for p in $$list; do echo "$$p $$p"; done | \
+  sed "s| $$srcdirstrip/| |;"' / .*\//!s/ .*/ ./; s,\( .*\)/[^/]*$$,\1,' | \
+  $(AWK) 'BEGIN { files["."] = "" } { files[$$2] = files[$$2] " " $$1; \
+    if (++n[$$2] == $(am__install_max)) \
+      { print $$2, files[$$2]; n[$$2] = 0; files[$$2] = "" } } \
+    END { for (dir in files) print dir, files[dir] }'
+am__base_list = \
+  sed '$$!N;$$!N;$$!N;$$!N;$$!N;$$!N;$$!N;s/\n/ /g' | \
+  sed '$$!N;$$!N;$$!N;$$!N;s/\n/ /g'
+am__uninstall_files_from_dir = { \
+  test -z "$$files" \
+    || { test ! -d "$$dir" && test ! -f "$$dir" && test ! -r "$$dir"; } \
+    || { echo " ( cd '$$dir' && rm -f" $$files ")"; \
+         $(am__cd) "$$dir" && rm -f $$files; }; \
+  }
+am__installdirs = "$(DESTDIR)$(pkgconfigdir)"
+DATA = $(pkgconfig_DATA)
+RECURSIVE_CLEAN_TARGETS = mostlyclean-recursive clean-recursive	\
+  distclean-recursive maintainer-clean-recursive
+am__recursive_targets = \
+  $(RECURSIVE_TARGETS) \
+  $(RECURSIVE_CLEAN_TARGETS) \
+  $(am__extra_recursive_targets)
+AM_RECURSIVE_TARGETS = $(am__recursive_targets:-recursive=) TAGS CTAGS \
+	cscope distdir distdir-am dist dist-all distcheck
 am__extra_recursive_targets = sources-recursive splint-recursive
 am__tagged_files = $(HEADERS) $(SOURCES) $(TAGS_FILES) $(LISP)
 # Read a list of newline-separated strings from the standard input,
 # and print each of them once, without duplicates.  Input order is
 # *not* preserved.
 am__uniquify_input = $(AWK) '\
   BEGIN { nonempty = 0; } \
@@ -230,16 +192,68 @@
 # e.g., the same source file might be shared among _SOURCES variables
 # for different programs/libraries.
 am__define_uniq_tagged_files = \
   list='$(am__tagged_files)'; \
   unique=`for i in $$list; do \
     if test -f "$$i"; then echo $$i; else echo $(srcdir)/$$i; fi; \
   done | $(am__uniquify_input)`
-am__DIST_COMMON = $(srcdir)/Makefile.in $(top_srcdir)/depcomp
+DIST_SUBDIRS = $(SUBDIRS)
+am__DIST_COMMON = $(srcdir)/Makefile.in $(srcdir)/libfcrypto.pc.in \
+	$(srcdir)/libfcrypto.spec.in $(srcdir)/setup.cfg.in \
+	$(top_srcdir)/dpkg/changelog.in \
+	$(top_srcdir)/include/libfcrypto/definitions.h.in \
+	$(top_srcdir)/include/libfcrypto/features.h.in \
+	$(top_srcdir)/include/libfcrypto/types.h.in ABOUT-NLS AUTHORS \
+	COPYING COPYING.LESSER ChangeLog INSTALL NEWS README compile \
+	config.guess config.rpath config.sub install-sh ltmain.sh \
+	missing
 DISTFILES = $(DIST_COMMON) $(DIST_SOURCES) $(TEXINFOS) $(EXTRA_DIST)
+distdir = $(PACKAGE)-$(VERSION)
+top_distdir = $(distdir)
+am__remove_distdir = \
+  if test -d "$(distdir)"; then \
+    find "$(distdir)" -type d ! -perm -200 -exec chmod u+w {} ';' \
+      && rm -rf "$(distdir)" \
+      || { sleep 5 && rm -rf "$(distdir)"; }; \
+  else :; fi
+am__post_remove_distdir = $(am__remove_distdir)
+am__relativize = \
+  dir0=`pwd`; \
+  sed_first='s,^\([^/]*\)/.*$$,\1,'; \
+  sed_rest='s,^[^/]*/*,,'; \
+  sed_last='s,^.*/\([^/]*\)$$,\1,'; \
+  sed_butlast='s,/*[^/]*$$,,'; \
+  while test -n "$$dir1"; do \
+    first=`echo "$$dir1" | sed -e "$$sed_first"`; \
+    if test "$$first" != "."; then \
+      if test "$$first" = ".."; then \
+        dir2=`echo "$$dir0" | sed -e "$$sed_last"`/"$$dir2"; \
+        dir0=`echo "$$dir0" | sed -e "$$sed_butlast"`; \
+      else \
+        first2=`echo "$$dir2" | sed -e "$$sed_first"`; \
+        if test "$$first2" = "$$first"; then \
+          dir2=`echo "$$dir2" | sed -e "$$sed_rest"`; \
+        else \
+          dir2="../$$dir2"; \
+        fi; \
+        dir0="$$dir0"/"$$first"; \
+      fi; \
+    fi; \
+    dir1=`echo "$$dir1" | sed -e "$$sed_rest"`; \
+  done; \
+  reldir="$$dir2"
+DIST_ARCHIVES = $(distdir).tar.gz
+GZIP_ENV = --best
+DIST_TARGETS = dist-gzip
+# Exists only to be overridden by the user if desired.
+AM_DISTCHECK_DVI_TARGET = dvi
+distuninstallcheck_listfiles = find . -type f -print
+am__distuninstallcheck_listfiles = $(distuninstallcheck_listfiles) \
+  | sed 's|^\./|$(prefix)/|' | grep -v '$(infodir)/dir$$'
+distcleancheck_listfiles = find . -type f -print
 ACLOCAL = @ACLOCAL@
 AMTAR = @AMTAR@
 AM_DEFAULT_VERBOSITY = @AM_DEFAULT_VERBOSITY@
 AR = @AR@
 AS = @AS@
 AUTOCONF = @AUTOCONF@
 AUTOHEADER = @AUTOHEADER@
@@ -417,232 +431,247 @@
 sharedstatedir = @sharedstatedir@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
-@HAVE_LIB_FUZZING_ENGINE_TRUE@AM_CPPFLAGS = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/common
-
-@HAVE_LIB_FUZZING_ENGINE_TRUE@crypt_blowfish_ecb_fuzzer_SOURCES = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	crypt_blowfish_ecb_fuzzer.cc \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	ossfuzz_libfcrypto.h
-
-@HAVE_LIB_FUZZING_ENGINE_TRUE@crypt_blowfish_ecb_fuzzer_LDADD = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIB_FUZZING_ENGINE@ \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	../libfcrypto/libfcrypto.la
-
-@HAVE_LIB_FUZZING_ENGINE_TRUE@crypt_rc4_fuzzer_SOURCES = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	crypt_rc4_fuzzer.cc \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	ossfuzz_libfcrypto.h
-
-@HAVE_LIB_FUZZING_ENGINE_TRUE@crypt_rc4_fuzzer_LDADD = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIB_FUZZING_ENGINE@ \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	../libfcrypto/libfcrypto.la
-
-@HAVE_LIB_FUZZING_ENGINE_TRUE@crypt_serpent_cbc_fuzzer_SOURCES = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	crypt_serpent_cbc_fuzzer.cc \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	ossfuzz_libfcrypto.h
-
-@HAVE_LIB_FUZZING_ENGINE_TRUE@crypt_serpent_cbc_fuzzer_LDADD = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIB_FUZZING_ENGINE@ \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	../libfcrypto/libfcrypto.la
-
-@HAVE_LIB_FUZZING_ENGINE_TRUE@crypt_serpent_ecb_fuzzer_SOURCES = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	crypt_serpent_ecb_fuzzer.cc \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	ossfuzz_libfcrypto.h
-
-@HAVE_LIB_FUZZING_ENGINE_TRUE@crypt_serpent_ecb_fuzzer_LDADD = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIB_FUZZING_ENGINE@ \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	../libfcrypto/libfcrypto.la
+ACLOCAL_AMFLAGS = -I m4
+SUBDIRS = \
+	include \
+	common \
+	libcerror \
+	libfcrypto \
+	pyfcrypto \
+	po \
+	manuals \
+	tests \
+	ossfuzz \
+	msvscpp
+
+DPKG_FILES = \
+	dpkg/changelog \
+	dpkg/changelog.in \
+	dpkg/compat \
+	dpkg/control \
+	dpkg/copyright \
+	dpkg/rules \
+	dpkg/libfcrypto-dev.install \
+	dpkg/libfcrypto.install \
+	dpkg/libfcrypto-python3.install \
+	dpkg/source/format
+
+GETTEXT_FILES = \
+	config.rpath \
+	po/Makevars.in
+
+PKGCONFIG_FILES = \
+	libfcrypto.pc.in
+
+SETUP_PY_FILES = \
+	pyproject.toml \
+	setup.cfg \
+	setup.cfg.in \
+	setup.py
+
+SPEC_FILES = \
+	libfcrypto.spec \
+	libfcrypto.spec.in
+
+EXTRA_DIST = \
+	$(DPKG_FILES) \
+	$(GETTEXT_FILES) \
+	$(PKGCONFIG_FILES) \
+	$(SETUP_PY_FILES) \
+	$(SPEC_FILES)
+
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libfcrypto.pc \
+	libfcrypto.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
+
+pkgconfigdir = $(libdir)/pkgconfig
+pkgconfig_DATA = \
+	libfcrypto.pc
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
-
-all: all-am
+all: all-recursive
 
 .SUFFIXES:
-.SUFFIXES: .cc .lo .o .obj
+am--refresh: Makefile
+	@:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
 	  case '$(am__configure_deps)' in \
 	    *$$dep*) \
-	      ( cd $(top_builddir) && $(MAKE) $(AM_MAKEFLAGS) am--refresh ) \
-	        && { if test -f $@; then exit 0; else break; fi; }; \
+	      echo ' cd $(srcdir) && $(AUTOMAKE) --gnu'; \
+	      $(am__cd) $(srcdir) && $(AUTOMAKE) --gnu \
+		&& exit 0; \
 	      exit 1;; \
 	  esac; \
 	done; \
-	echo ' cd $(top_srcdir) && $(AUTOMAKE) --gnu ossfuzz/Makefile'; \
+	echo ' cd $(top_srcdir) && $(AUTOMAKE) --gnu Makefile'; \
 	$(am__cd) $(top_srcdir) && \
-	  $(AUTOMAKE) --gnu ossfuzz/Makefile
+	  $(AUTOMAKE) --gnu Makefile
 Makefile: $(srcdir)/Makefile.in $(top_builddir)/config.status
 	@case '$?' in \
 	  *config.status*) \
-	    cd $(top_builddir) && $(MAKE) $(AM_MAKEFLAGS) am--refresh;; \
+	    echo ' $(SHELL) ./config.status'; \
+	    $(SHELL) ./config.status;; \
 	  *) \
-	    echo ' cd $(top_builddir) && $(SHELL) ./config.status $(subdir)/$@ $(am__maybe_remake_depfiles)'; \
-	    cd $(top_builddir) && $(SHELL) ./config.status $(subdir)/$@ $(am__maybe_remake_depfiles);; \
+	    echo ' cd $(top_builddir) && $(SHELL) ./config.status $@ $(am__maybe_remake_depfiles)'; \
+	    cd $(top_builddir) && $(SHELL) ./config.status $@ $(am__maybe_remake_depfiles);; \
 	esac;
 
 $(top_builddir)/config.status: $(top_srcdir)/configure $(CONFIG_STATUS_DEPENDENCIES)
-	cd $(top_builddir) && $(MAKE) $(AM_MAKEFLAGS) am--refresh
+	$(SHELL) ./config.status --recheck
 
 $(top_srcdir)/configure:  $(am__configure_deps)
-	cd $(top_builddir) && $(MAKE) $(AM_MAKEFLAGS) am--refresh
+	$(am__cd) $(srcdir) && $(AUTOCONF)
 $(ACLOCAL_M4):  $(am__aclocal_m4_deps)
-	cd $(top_builddir) && $(MAKE) $(AM_MAKEFLAGS) am--refresh
+	$(am__cd) $(srcdir) && $(ACLOCAL) $(ACLOCAL_AMFLAGS)
 $(am__aclocal_m4_deps):
-install-binPROGRAMS: $(bin_PROGRAMS)
-	@$(NORMAL_INSTALL)
-	@list='$(bin_PROGRAMS)'; test -n "$(bindir)" || list=; \
-	if test -n "$$list"; then \
-	  echo " $(MKDIR_P) '$(DESTDIR)$(bindir)'"; \
-	  $(MKDIR_P) "$(DESTDIR)$(bindir)" || exit 1; \
-	fi; \
-	for p in $$list; do echo "$$p $$p"; done | \
-	sed 's/$(EXEEXT)$$//' | \
-	while read p p1; do if test -f $$p \
-	 || test -f $$p1 \
-	  ; then echo "$$p"; echo "$$p"; else :; fi; \
-	done | \
-	sed -e 'p;s,.*/,,;n;h' \
-	    -e 's|.*|.|' \
-	    -e 'p;x;s,.*/,,;s/$(EXEEXT)$$//;$(transform);s/$$/$(EXEEXT)/' | \
-	sed 'N;N;N;s,\n, ,g' | \
-	$(AWK) 'BEGIN { files["."] = ""; dirs["."] = 1 } \
-	  { d=$$3; if (dirs[d] != 1) { print "d", d; dirs[d] = 1 } \
-	    if ($$2 == $$4) files[d] = files[d] " " $$1; \
-	    else { print "f", $$3 "/" $$4, $$1; } } \
-	  END { for (d in files) print "f", d, files[d] }' | \
-	while read type dir files; do \
-	    if test "$$dir" = .; then dir=; else dir=/$$dir; fi; \
-	    test -z "$$files" || { \
-	    echo " $(INSTALL_PROGRAM_ENV) $(LIBTOOL) $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=install $(INSTALL_PROGRAM) $$files '$(DESTDIR)$(bindir)$$dir'"; \
-	    $(INSTALL_PROGRAM_ENV) $(LIBTOOL) $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=install $(INSTALL_PROGRAM) $$files "$(DESTDIR)$(bindir)$$dir" || exit $$?; \
-	    } \
-	; done
-
-uninstall-binPROGRAMS:
-	@$(NORMAL_UNINSTALL)
-	@list='$(bin_PROGRAMS)'; test -n "$(bindir)" || list=; \
-	files=`for p in $$list; do echo "$$p"; done | \
-	  sed -e 'h;s,^.*/,,;s/$(EXEEXT)$$//;$(transform)' \
-	      -e 's/$$/$(EXEEXT)/' \
-	`; \
-	test -n "$$list" || exit 0; \
-	echo " ( cd '$(DESTDIR)$(bindir)' && rm -f" $$files ")"; \
-	cd "$(DESTDIR)$(bindir)" && rm -f $$files
-
-clean-binPROGRAMS:
-	@list='$(bin_PROGRAMS)'; test -n "$$list" || exit 0; \
-	echo " rm -f" $$list; \
-	rm -f $$list || exit $$?; \
-	test -n "$(EXEEXT)" || exit 0; \
-	list=`for p in $$list; do echo "$$p"; done | sed 's/$(EXEEXT)$$//'`; \
-	echo " rm -f" $$list; \
-	rm -f $$list
-
-crypt_blowfish_ecb_fuzzer$(EXEEXT): $(crypt_blowfish_ecb_fuzzer_OBJECTS) $(crypt_blowfish_ecb_fuzzer_DEPENDENCIES) $(EXTRA_crypt_blowfish_ecb_fuzzer_DEPENDENCIES) 
-	@rm -f crypt_blowfish_ecb_fuzzer$(EXEEXT)
-	$(AM_V_CXXLD)$(CXXLINK) $(crypt_blowfish_ecb_fuzzer_OBJECTS) $(crypt_blowfish_ecb_fuzzer_LDADD) $(LIBS)
-
-crypt_rc4_fuzzer$(EXEEXT): $(crypt_rc4_fuzzer_OBJECTS) $(crypt_rc4_fuzzer_DEPENDENCIES) $(EXTRA_crypt_rc4_fuzzer_DEPENDENCIES) 
-	@rm -f crypt_rc4_fuzzer$(EXEEXT)
-	$(AM_V_CXXLD)$(CXXLINK) $(crypt_rc4_fuzzer_OBJECTS) $(crypt_rc4_fuzzer_LDADD) $(LIBS)
-
-crypt_serpent_cbc_fuzzer$(EXEEXT): $(crypt_serpent_cbc_fuzzer_OBJECTS) $(crypt_serpent_cbc_fuzzer_DEPENDENCIES) $(EXTRA_crypt_serpent_cbc_fuzzer_DEPENDENCIES) 
-	@rm -f crypt_serpent_cbc_fuzzer$(EXEEXT)
-	$(AM_V_CXXLD)$(CXXLINK) $(crypt_serpent_cbc_fuzzer_OBJECTS) $(crypt_serpent_cbc_fuzzer_LDADD) $(LIBS)
-
-crypt_serpent_ecb_fuzzer$(EXEEXT): $(crypt_serpent_ecb_fuzzer_OBJECTS) $(crypt_serpent_ecb_fuzzer_DEPENDENCIES) $(EXTRA_crypt_serpent_ecb_fuzzer_DEPENDENCIES) 
-	@rm -f crypt_serpent_ecb_fuzzer$(EXEEXT)
-	$(AM_V_CXXLD)$(CXXLINK) $(crypt_serpent_ecb_fuzzer_OBJECTS) $(crypt_serpent_ecb_fuzzer_LDADD) $(LIBS)
-
-mostlyclean-compile:
-	-rm -f *.$(OBJEXT)
-
-distclean-compile:
-	-rm -f *.tab.c
-
-@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/crypt_blowfish_ecb_fuzzer.Po@am__quote@ # am--include-marker
-@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/crypt_rc4_fuzzer.Po@am__quote@ # am--include-marker
-@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/crypt_serpent_cbc_fuzzer.Po@am__quote@ # am--include-marker
-@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/crypt_serpent_ecb_fuzzer.Po@am__quote@ # am--include-marker
-
-$(am__depfiles_remade):
-	@$(MKDIR_P) $(@D)
-	@echo '# dummy' >$@-t && $(am__mv) $@-t $@
-
-am--depfiles: $(am__depfiles_remade)
-
-.cc.o:
-@am__fastdepCXX_TRUE@	$(AM_V_CXX)$(CXXCOMPILE) -MT $@ -MD -MP -MF $(DEPDIR)/$*.Tpo -c -o $@ $<
-@am__fastdepCXX_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/$*.Tpo $(DEPDIR)/$*.Po
-@AMDEP_TRUE@@am__fastdepCXX_FALSE@	$(AM_V_CXX)source='$<' object='$@' libtool=no @AMDEPBACKSLASH@
-@AMDEP_TRUE@@am__fastdepCXX_FALSE@	DEPDIR=$(DEPDIR) $(CXXDEPMODE) $(depcomp) @AMDEPBACKSLASH@
-@am__fastdepCXX_FALSE@	$(AM_V_CXX@am__nodep@)$(CXXCOMPILE) -c -o $@ $<
-
-.cc.obj:
-@am__fastdepCXX_TRUE@	$(AM_V_CXX)$(CXXCOMPILE) -MT $@ -MD -MP -MF $(DEPDIR)/$*.Tpo -c -o $@ `$(CYGPATH_W) '$<'`
-@am__fastdepCXX_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/$*.Tpo $(DEPDIR)/$*.Po
-@AMDEP_TRUE@@am__fastdepCXX_FALSE@	$(AM_V_CXX)source='$<' object='$@' libtool=no @AMDEPBACKSLASH@
-@AMDEP_TRUE@@am__fastdepCXX_FALSE@	DEPDIR=$(DEPDIR) $(CXXDEPMODE) $(depcomp) @AMDEPBACKSLASH@
-@am__fastdepCXX_FALSE@	$(AM_V_CXX@am__nodep@)$(CXXCOMPILE) -c -o $@ `$(CYGPATH_W) '$<'`
-
-.cc.lo:
-@am__fastdepCXX_TRUE@	$(AM_V_CXX)$(LTCXXCOMPILE) -MT $@ -MD -MP -MF $(DEPDIR)/$*.Tpo -c -o $@ $<
-@am__fastdepCXX_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/$*.Tpo $(DEPDIR)/$*.Plo
-@AMDEP_TRUE@@am__fastdepCXX_FALSE@	$(AM_V_CXX)source='$<' object='$@' libtool=yes @AMDEPBACKSLASH@
-@AMDEP_TRUE@@am__fastdepCXX_FALSE@	DEPDIR=$(DEPDIR) $(CXXDEPMODE) $(depcomp) @AMDEPBACKSLASH@
-@am__fastdepCXX_FALSE@	$(AM_V_CXX@am__nodep@)$(LTCXXCOMPILE) -c -o $@ $<
+include/libfcrypto/definitions.h: $(top_builddir)/config.status $(top_srcdir)/include/libfcrypto/definitions.h.in
+	cd $(top_builddir) && $(SHELL) ./config.status $@
+include/libfcrypto/features.h: $(top_builddir)/config.status $(top_srcdir)/include/libfcrypto/features.h.in
+	cd $(top_builddir) && $(SHELL) ./config.status $@
+include/libfcrypto/types.h: $(top_builddir)/config.status $(top_srcdir)/include/libfcrypto/types.h.in
+	cd $(top_builddir) && $(SHELL) ./config.status $@
+dpkg/changelog: $(top_builddir)/config.status $(top_srcdir)/dpkg/changelog.in
+	cd $(top_builddir) && $(SHELL) ./config.status $@
+libfcrypto.pc: $(top_builddir)/config.status $(srcdir)/libfcrypto.pc.in
+	cd $(top_builddir) && $(SHELL) ./config.status $@
+libfcrypto.spec: $(top_builddir)/config.status $(srcdir)/libfcrypto.spec.in
+	cd $(top_builddir) && $(SHELL) ./config.status $@
+setup.cfg: $(top_builddir)/config.status $(srcdir)/setup.cfg.in
+	cd $(top_builddir) && $(SHELL) ./config.status $@
 
 mostlyclean-libtool:
 	-rm -f *.lo
 
 clean-libtool:
 	-rm -rf .libs _libs
+
+distclean-libtool:
+	-rm -f libtool config.lt
+install-pkgconfigDATA: $(pkgconfig_DATA)
+	@$(NORMAL_INSTALL)
+	@list='$(pkgconfig_DATA)'; test -n "$(pkgconfigdir)" || list=; \
+	if test -n "$$list"; then \
+	  echo " $(MKDIR_P) '$(DESTDIR)$(pkgconfigdir)'"; \
+	  $(MKDIR_P) "$(DESTDIR)$(pkgconfigdir)" || exit 1; \
+	fi; \
+	for p in $$list; do \
+	  if test -f "$$p"; then d=; else d="$(srcdir)/"; fi; \
+	  echo "$$d$$p"; \
+	done | $(am__base_list) | \
+	while read files; do \
+	  echo " $(INSTALL_DATA) $$files '$(DESTDIR)$(pkgconfigdir)'"; \
+	  $(INSTALL_DATA) $$files "$(DESTDIR)$(pkgconfigdir)" || exit $$?; \
+	done
+
+uninstall-pkgconfigDATA:
+	@$(NORMAL_UNINSTALL)
+	@list='$(pkgconfig_DATA)'; test -n "$(pkgconfigdir)" || list=; \
+	files=`for p in $$list; do echo $$p; done | sed -e 's|^.*/||'`; \
+	dir='$(DESTDIR)$(pkgconfigdir)'; $(am__uninstall_files_from_dir)
+
+# This directory's subdirectories are mostly independent; you can cd
+# into them and run 'make' without going through this Makefile.
+# To change the values of 'make' variables: instead of editing Makefiles,
+# (1) if the variable is set in 'config.status', edit 'config.status'
+#     (which will cause the Makefiles to be regenerated when you run 'make');
+# (2) otherwise, pass the desired values on the 'make' command line.
+$(am__recursive_targets):
+	@fail=; \
+	if $(am__make_keepgoing); then \
+	  failcom='fail=yes'; \
+	else \
+	  failcom='exit 1'; \
+	fi; \
+	dot_seen=no; \
+	target=`echo $@ | sed s/-recursive//`; \
+	case "$@" in \
+	  distclean-* | maintainer-clean-*) list='$(DIST_SUBDIRS)' ;; \
+	  *) list='$(SUBDIRS)' ;; \
+	esac; \
+	for subdir in $$list; do \
+	  echo "Making $$target in $$subdir"; \
+	  if test "$$subdir" = "."; then \
+	    dot_seen=yes; \
+	    local_target="$$target-am"; \
+	  else \
+	    local_target="$$target"; \
+	  fi; \
+	  ($(am__cd) $$subdir && $(MAKE) $(AM_MAKEFLAGS) $$local_target) \
+	  || eval $$failcom; \
+	done; \
+	if test "$$dot_seen" = "no"; then \
+	  $(MAKE) $(AM_MAKEFLAGS) "$$target-am" || exit 1; \
+	fi; test -z "$$fail"
 sources-local: 
 splint-local: 
 
 ID: $(am__tagged_files)
 	$(am__define_uniq_tagged_files); mkid -fID $$unique
-tags: tags-am
+tags: tags-recursive
 TAGS: tags
 
 tags-am: $(TAGS_DEPENDENCIES) $(am__tagged_files)
 	set x; \
 	here=`pwd`; \
+	if ($(ETAGS) --etags-include --version) >/dev/null 2>&1; then \
+	  include_option=--etags-include; \
+	  empty_fix=.; \
+	else \
+	  include_option=--include; \
+	  empty_fix=; \
+	fi; \
+	list='$(SUBDIRS)'; for subdir in $$list; do \
+	  if test "$$subdir" = .; then :; else \
+	    test ! -f $$subdir/TAGS || \
+	      set "$$@" "$$include_option=$$here/$$subdir/TAGS"; \
+	  fi; \
+	done; \
 	$(am__define_uniq_tagged_files); \
 	shift; \
 	if test -z "$(ETAGS_ARGS)$$*$$unique"; then :; else \
 	  test -n "$$unique" || unique=$$empty_fix; \
 	  if test $$# -gt 0; then \
 	    $(ETAGS) $(ETAGSFLAGS) $(AM_ETAGSFLAGS) $(ETAGS_ARGS) \
 	      "$$@" $$unique; \
 	  else \
 	    $(ETAGS) $(ETAGSFLAGS) $(AM_ETAGSFLAGS) $(ETAGS_ARGS) \
 	      $$unique; \
 	  fi; \
 	fi
-ctags: ctags-am
+ctags: ctags-recursive
 
 CTAGS: ctags
 ctags-am: $(TAGS_DEPENDENCIES) $(am__tagged_files)
 	$(am__define_uniq_tagged_files); \
 	test -z "$(CTAGS_ARGS)$$unique" \
 	  || $(CTAGS) $(CTAGSFLAGS) $(AM_CTAGSFLAGS) $(CTAGS_ARGS) \
 	     $$unique
 
 GTAGS:
 	here=`$(am__cd) $(top_builddir) && pwd` \
 	  && $(am__cd) $(top_srcdir) \
 	  && gtags -i $(GTAGS_ARGS) "$$here"
-cscopelist: cscopelist-am
+cscope: cscope.files
+	test ! -s cscope.files \
+	  || $(CSCOPE) -b -q $(AM_CSCOPEFLAGS) $(CSCOPEFLAGS) -i cscope.files $(CSCOPE_ARGS)
+clean-cscope:
+	-rm -f cscope.files
+cscope.files: clean-cscope cscopelist
+cscopelist: cscopelist-recursive
 
 cscopelist-am: $(am__tagged_files)
 	list='$(am__tagged_files)'; \
 	case "$(srcdir)" in \
 	  [\\/]* | ?:[\\/]*) sdir="$(srcdir)" ;; \
 	  *) sdir=$(subdir)/$(srcdir) ;; \
 	esac; \
@@ -652,18 +681,21 @@
 	  else \
 	    echo "$$sdir/$$i"; \
 	  fi; \
 	done >> $(top_builddir)/cscope.files
 
 distclean-tags:
 	-rm -f TAGS ID GTAGS GRTAGS GSYMS GPATH tags
+	-rm -f cscope.out cscope.in.out cscope.po.out cscope.files
 distdir: $(BUILT_SOURCES)
 	$(MAKE) $(AM_MAKEFLAGS) distdir-am
 
 distdir-am: $(DISTFILES)
+	$(am__remove_distdir)
+	test -d "$(distdir)" || mkdir "$(distdir)"
 	@srcdirstrip=`echo "$(srcdir)" | sed 's/[].[^$$\\*]/\\\\&/g'`; \
 	topsrcdirstrip=`echo "$(top_srcdir)" | sed 's/[].[^$$\\*]/\\\\&/g'`; \
 	list='$(DISTFILES)'; \
 	  dist_files=`for file in $$list; do echo $$file; done | \
 	  sed -e "s|^$$srcdirstrip/||;t" \
 	      -e "s|^$$topsrcdirstrip/|$(top_builddir)/|;t"`; \
 	case $$dist_files in \
@@ -685,30 +717,193 @@
 	    cp -fpR $$d/$$file "$(distdir)$$dir" || exit 1; \
 	  else \
 	    test -f "$(distdir)/$$file" \
 	    || cp -p $$d/$$file "$(distdir)/$$file" \
 	    || exit 1; \
 	  fi; \
 	done
+	@list='$(DIST_SUBDIRS)'; for subdir in $$list; do \
+	  if test "$$subdir" = .; then :; else \
+	    $(am__make_dryrun) \
+	      || test -d "$(distdir)/$$subdir" \
+	      || $(MKDIR_P) "$(distdir)/$$subdir" \
+	      || exit 1; \
+	    dir1=$$subdir; dir2="$(distdir)/$$subdir"; \
+	    $(am__relativize); \
+	    new_distdir=$$reldir; \
+	    dir1=$$subdir; dir2="$(top_distdir)"; \
+	    $(am__relativize); \
+	    new_top_distdir=$$reldir; \
+	    echo " (cd $$subdir && $(MAKE) $(AM_MAKEFLAGS) top_distdir="$$new_top_distdir" distdir="$$new_distdir" \\"; \
+	    echo "     am__remove_distdir=: am__skip_length_check=: am__skip_mode_fix=: distdir)"; \
+	    ($(am__cd) $$subdir && \
+	      $(MAKE) $(AM_MAKEFLAGS) \
+	        top_distdir="$$new_top_distdir" \
+	        distdir="$$new_distdir" \
+		am__remove_distdir=: \
+		am__skip_length_check=: \
+		am__skip_mode_fix=: \
+	        distdir) \
+	      || exit 1; \
+	  fi; \
+	done
+	-test -n "$(am__skip_mode_fix)" \
+	|| find "$(distdir)" -type d ! -perm -755 \
+		-exec chmod u+rwx,go+rx {} \; -o \
+	  ! -type d ! -perm -444 -links 1 -exec chmod a+r {} \; -o \
+	  ! -type d ! -perm -400 -exec chmod a+r {} \; -o \
+	  ! -type d ! -perm -444 -exec $(install_sh) -c -m a+r {} {} \; \
+	|| chmod -R a+r "$(distdir)"
+dist-gzip: distdir
+	tardir=$(distdir) && $(am__tar) | eval GZIP= gzip $(GZIP_ENV) -c >$(distdir).tar.gz
+	$(am__post_remove_distdir)
+
+dist-bzip2: distdir
+	tardir=$(distdir) && $(am__tar) | BZIP2=$${BZIP2--9} bzip2 -c >$(distdir).tar.bz2
+	$(am__post_remove_distdir)
+
+dist-lzip: distdir
+	tardir=$(distdir) && $(am__tar) | lzip -c $${LZIP_OPT--9} >$(distdir).tar.lz
+	$(am__post_remove_distdir)
+
+dist-xz: distdir
+	tardir=$(distdir) && $(am__tar) | XZ_OPT=$${XZ_OPT--e} xz -c >$(distdir).tar.xz
+	$(am__post_remove_distdir)
+
+dist-zstd: distdir
+	tardir=$(distdir) && $(am__tar) | zstd -c $${ZSTD_CLEVEL-$${ZSTD_OPT--19}} >$(distdir).tar.zst
+	$(am__post_remove_distdir)
+
+dist-tarZ: distdir
+	@echo WARNING: "Support for distribution archives compressed with" \
+		       "legacy program 'compress' is deprecated." >&2
+	@echo WARNING: "It will be removed altogether in Automake 2.0" >&2
+	tardir=$(distdir) && $(am__tar) | compress -c >$(distdir).tar.Z
+	$(am__post_remove_distdir)
+
+dist-shar: distdir
+	@echo WARNING: "Support for shar distribution archives is" \
+	               "deprecated." >&2
+	@echo WARNING: "It will be removed altogether in Automake 2.0" >&2
+	shar $(distdir) | eval GZIP= gzip $(GZIP_ENV) -c >$(distdir).shar.gz
+	$(am__post_remove_distdir)
+
+dist-zip: distdir
+	-rm -f $(distdir).zip
+	zip -rq $(distdir).zip $(distdir)
+	$(am__post_remove_distdir)
+
+dist dist-all:
+	$(MAKE) $(AM_MAKEFLAGS) $(DIST_TARGETS) am__post_remove_distdir='@:'
+	$(am__post_remove_distdir)
+
+# This target untars the dist file and tries a VPATH configuration.  Then
+# it guarantees that the distribution is self-contained by making another
+# tarfile.
+distcheck: dist
+	case '$(DIST_ARCHIVES)' in \
+	*.tar.gz*) \
+	  eval GZIP= gzip $(GZIP_ENV) -dc $(distdir).tar.gz | $(am__untar) ;;\
+	*.tar.bz2*) \
+	  bzip2 -dc $(distdir).tar.bz2 | $(am__untar) ;;\
+	*.tar.lz*) \
+	  lzip -dc $(distdir).tar.lz | $(am__untar) ;;\
+	*.tar.xz*) \
+	  xz -dc $(distdir).tar.xz | $(am__untar) ;;\
+	*.tar.Z*) \
+	  uncompress -c $(distdir).tar.Z | $(am__untar) ;;\
+	*.shar.gz*) \
+	  eval GZIP= gzip $(GZIP_ENV) -dc $(distdir).shar.gz | unshar ;;\
+	*.zip*) \
+	  unzip $(distdir).zip ;;\
+	*.tar.zst*) \
+	  zstd -dc $(distdir).tar.zst | $(am__untar) ;;\
+	esac
+	chmod -R a-w $(distdir)
+	chmod u+w $(distdir)
+	mkdir $(distdir)/_build $(distdir)/_build/sub $(distdir)/_inst
+	chmod a-w $(distdir)
+	test -d $(distdir)/_build || exit 0; \
+	dc_install_base=`$(am__cd) $(distdir)/_inst && pwd | sed -e 's,^[^:\\/]:[\\/],/,'` \
+	  && dc_destdir="$${TMPDIR-/tmp}/am-dc-$$$$/" \
+	  && am__cwd=`pwd` \
+	  && $(am__cd) $(distdir)/_build/sub \
+	  && ../../configure \
+	    $(AM_DISTCHECK_CONFIGURE_FLAGS) \
+	    $(DISTCHECK_CONFIGURE_FLAGS) \
+	    --srcdir=../.. --prefix="$$dc_install_base" \
+	  && $(MAKE) $(AM_MAKEFLAGS) \
+	  && $(MAKE) $(AM_MAKEFLAGS) $(AM_DISTCHECK_DVI_TARGET) \
+	  && $(MAKE) $(AM_MAKEFLAGS) check \
+	  && $(MAKE) $(AM_MAKEFLAGS) install \
+	  && $(MAKE) $(AM_MAKEFLAGS) installcheck \
+	  && $(MAKE) $(AM_MAKEFLAGS) uninstall \
+	  && $(MAKE) $(AM_MAKEFLAGS) distuninstallcheck_dir="$$dc_install_base" \
+	        distuninstallcheck \
+	  && chmod -R a-w "$$dc_install_base" \
+	  && ({ \
+	       (cd ../.. && umask 077 && mkdir "$$dc_destdir") \
+	       && $(MAKE) $(AM_MAKEFLAGS) DESTDIR="$$dc_destdir" install \
+	       && $(MAKE) $(AM_MAKEFLAGS) DESTDIR="$$dc_destdir" uninstall \
+	       && $(MAKE) $(AM_MAKEFLAGS) DESTDIR="$$dc_destdir" \
+	            distuninstallcheck_dir="$$dc_destdir" distuninstallcheck; \
+	      } || { rm -rf "$$dc_destdir"; exit 1; }) \
+	  && rm -rf "$$dc_destdir" \
+	  && $(MAKE) $(AM_MAKEFLAGS) dist \
+	  && rm -rf $(DIST_ARCHIVES) \
+	  && $(MAKE) $(AM_MAKEFLAGS) distcleancheck \
+	  && cd "$$am__cwd" \
+	  || exit 1
+	$(am__post_remove_distdir)
+	@(echo "$(distdir) archives ready for distribution: "; \
+	  list='$(DIST_ARCHIVES)'; for i in $$list; do echo $$i; done) | \
+	  sed -e 1h -e 1s/./=/g -e 1p -e 1x -e '$$p' -e '$$x'
+distuninstallcheck:
+	@test -n '$(distuninstallcheck_dir)' || { \
+	  echo 'ERROR: trying to run $@ with an empty' \
+	       '$$(distuninstallcheck_dir)' >&2; \
+	  exit 1; \
+	}; \
+	$(am__cd) '$(distuninstallcheck_dir)' || { \
+	  echo 'ERROR: cannot chdir into $(distuninstallcheck_dir)' >&2; \
+	  exit 1; \
+	}; \
+	test `$(am__distuninstallcheck_listfiles) | wc -l` -eq 0 \
+	   || { echo "ERROR: files left after uninstall:" ; \
+	        if test -n "$(DESTDIR)"; then \
+	          echo "  (check DESTDIR support)"; \
+	        fi ; \
+	        $(distuninstallcheck_listfiles) ; \
+	        exit 1; } >&2
+distcleancheck: distclean
+	@if test '$(srcdir)' = . ; then \
+	  echo "ERROR: distcleancheck can only run from a VPATH build" ; \
+	  exit 1 ; \
+	fi
+	@test `$(distcleancheck_listfiles) | wc -l` -eq 0 \
+	  || { echo "ERROR: files left in build directory after distclean:" ; \
+	       $(distcleancheck_listfiles) ; \
+	       exit 1; } >&2
 check-am: all-am
-check: check-am
-all-am: Makefile $(PROGRAMS)
-installdirs:
-	for dir in "$(DESTDIR)$(bindir)"; do \
+check: check-recursive
+all-am: Makefile $(DATA)
+installdirs: installdirs-recursive
+installdirs-am:
+	for dir in "$(DESTDIR)$(pkgconfigdir)"; do \
 	  test -z "$$dir" || $(MKDIR_P) "$$dir"; \
 	done
-install: install-am
-install-exec: install-exec-am
-install-data: install-data-am
-uninstall: uninstall-am
+install: install-recursive
+install-exec: install-exec-recursive
+install-data: install-data-recursive
+uninstall: uninstall-recursive
 
 install-am: all-am
 	@$(MAKE) $(AM_MAKEFLAGS) install-exec-am install-data-am
 
-installcheck: installcheck-am
+installcheck: installcheck-recursive
 install-strip:
 	if test -z '$(STRIP)'; then \
 	  $(MAKE) $(AM_MAKEFLAGS) INSTALL_PROGRAM="$(INSTALL_STRIP_PROGRAM)" \
 	    install_sh_PROGRAM="$(INSTALL_STRIP_PROGRAM)" INSTALL_STRIP_FLAG=-s \
 	      install; \
 	else \
 	  $(MAKE) $(AM_MAKEFLAGS) INSTALL_PROGRAM="$(INSTALL_STRIP_PROGRAM)" \
@@ -718,126 +913,127 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
-clean: clean-am
+clean: clean-recursive
 
-clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
+clean-am: clean-generic clean-libtool mostlyclean-am
 
-distclean-am: clean-am distclean-compile distclean-generic \
+distclean: distclean-recursive
+	-rm -f $(am__CONFIG_DISTCLEAN_FILES)
+	-rm -f Makefile
+distclean-am: clean-am distclean-generic distclean-libtool \
 	distclean-tags
 
-dvi: dvi-am
+dvi: dvi-recursive
 
 dvi-am:
 
-html: html-am
+html: html-recursive
 
 html-am:
 
-info: info-am
+info: info-recursive
 
 info-am:
 
-install-data-am:
+install-data-am: install-pkgconfigDATA
 
-install-dvi: install-dvi-am
+install-dvi: install-dvi-recursive
 
 install-dvi-am:
 
-install-exec-am: install-binPROGRAMS
+install-exec-am:
 
-install-html: install-html-am
+install-html: install-html-recursive
 
 install-html-am:
 
-install-info: install-info-am
+install-info: install-info-recursive
 
 install-info-am:
 
 install-man:
 
-install-pdf: install-pdf-am
+install-pdf: install-pdf-recursive
 
 install-pdf-am:
 
-install-ps: install-ps-am
+install-ps: install-ps-recursive
 
 install-ps-am:
 
 installcheck-am:
 
-maintainer-clean: maintainer-clean-am
-		-rm -f ./$(DEPDIR)/crypt_blowfish_ecb_fuzzer.Po
-	-rm -f ./$(DEPDIR)/crypt_rc4_fuzzer.Po
-	-rm -f ./$(DEPDIR)/crypt_serpent_cbc_fuzzer.Po
-	-rm -f ./$(DEPDIR)/crypt_serpent_ecb_fuzzer.Po
+maintainer-clean: maintainer-clean-recursive
+	-rm -f $(am__CONFIG_DISTCLEAN_FILES)
+	-rm -rf $(top_srcdir)/autom4te.cache
 	-rm -f Makefile
 maintainer-clean-am: distclean-am maintainer-clean-generic
 
-mostlyclean: mostlyclean-am
+mostlyclean: mostlyclean-recursive
 
-mostlyclean-am: mostlyclean-compile mostlyclean-generic \
-	mostlyclean-libtool
+mostlyclean-am: mostlyclean-generic mostlyclean-libtool
 
-pdf: pdf-am
+pdf: pdf-recursive
 
 pdf-am:
 
-ps: ps-am
+ps: ps-recursive
 
 ps-am:
 
-sources: sources-am
+sources: sources-recursive
 
 sources-am: sources-local
 
-splint: splint-am
+splint: splint-recursive
 
 splint-am: splint-local
 
-uninstall-am: uninstall-binPROGRAMS
+uninstall-am: uninstall-pkgconfigDATA
 
-.MAKE: install-am install-strip
+.MAKE: $(am__recursive_targets) install-am install-strip
 
-.PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
-	clean-binPROGRAMS clean-generic clean-libtool cscopelist-am \
-	ctags ctags-am distclean distclean-compile distclean-generic \
-	distclean-libtool distclean-tags distdir dvi dvi-am html \
-	html-am info info-am install install-am install-binPROGRAMS \
-	install-data install-data-am install-dvi install-dvi-am \
-	install-exec install-exec-am install-html install-html-am \
-	install-info install-info-am install-man install-pdf \
-	install-pdf-am install-ps install-ps-am install-strip \
-	installcheck installcheck-am installdirs maintainer-clean \
-	maintainer-clean-generic mostlyclean mostlyclean-compile \
+.PHONY: $(am__recursive_targets) CTAGS GTAGS TAGS all all-am \
+	am--refresh check check-am clean clean-cscope clean-generic \
+	clean-libtool cscope cscopelist-am ctags ctags-am dist \
+	dist-all dist-bzip2 dist-gzip dist-lzip dist-shar dist-tarZ \
+	dist-xz dist-zip dist-zstd distcheck distclean \
+	distclean-generic distclean-libtool distclean-tags \
+	distcleancheck distdir distuninstallcheck dvi dvi-am html \
+	html-am info info-am install install-am install-data \
+	install-data-am install-dvi install-dvi-am install-exec \
+	install-exec-am install-html install-html-am install-info \
+	install-info-am install-man install-pdf install-pdf-am \
+	install-pkgconfigDATA install-ps install-ps-am install-strip \
+	installcheck installcheck-am installdirs installdirs-am \
+	maintainer-clean maintainer-clean-generic mostlyclean \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
-	uninstall uninstall-am uninstall-binPROGRAMS
+	uninstall uninstall-am uninstall-pkgconfigDATA
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
+libtool: @LIBTOOL_DEPS@
+	cd $(srcdir) && $(SHELL) ./config.status --recheck
+
+lib: library
 
-splint-local:
-	@echo "Running splint on crypt_blowfish_ecb_fuzzer ..."
-	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(crypt_blowfish_ecb_fuzzer_SOURCES)
-	@echo "Running splint on crypt_rc4_fuzzer ..."
-	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(crypt_rc4_fuzzer_SOURCES)
-	@echo "Running splint on crypt_serpent_cbc_fuzzer ..."
-	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(crypt_serpent_cbc_fuzzer_SOURCES)
-	@echo "Running splint on crypt_serpent_ecb_fuzzer ..."
-	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(crypt_serpent_ecb_fuzzer_SOURCES)
+library:
+	(cd $(srcdir)/common && $(MAKE) $(AM_MAKEFLAGS))
+	(cd $(srcdir)/libcerror && $(MAKE) $(AM_MAKEFLAGS))
+	(cd $(srcdir)/libfcrypto && $(MAKE) $(AM_MAKEFLAGS))
+	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfcrypto-20240115/ltmain.sh` & `libfcrypto-20240414/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/po/remove-potcdate.sin` & `libfcrypto-20240414/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/po/Makefile.in.in` & `libfcrypto-20240414/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/po/en@quot.header` & `libfcrypto-20240414/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/po/en@boldquot.header` & `libfcrypto-20240414/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/po/insert-header.sin` & `libfcrypto-20240414/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/po/Makevars` & `libfcrypto-20240414/po/Makevars`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/po/Makevars.in` & `libfcrypto-20240414/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/po/Rules-quot` & `libfcrypto-20240414/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libcerror/libcerror_system.c` & `libfcrypto-20240414/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libcerror/libcerror_error.c` & `libfcrypto-20240414/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libcerror/libcerror_extern.h` & `libfcrypto-20240414/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libcerror/Makefile.am` & `libfcrypto-20240414/libcerror/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 if HAVE_LOCAL_LIBCERROR
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common 
 
 noinst_LTLIBRARIES = libcerror.la
 
 libcerror_la_SOURCES = \
 	libcerror_definitions.h \
 	libcerror_extern.h \
 	libcerror_error.c libcerror_error.h \
 	libcerror_support.c libcerror_support.h \
 	libcerror_system.c libcerror_system.h \
 	libcerror_types.h \
 	libcerror_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
```

### Comparing `libfcrypto-20240115/libcerror/libcerror_types.h` & `libfcrypto-20240414/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libcerror/libcerror_support.h` & `libfcrypto-20240414/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libcerror/libcerror_error.h` & `libfcrypto-20240414/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libcerror/libcerror_system.h` & `libfcrypto-20240414/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libcerror/libcerror_definitions.h` & `libfcrypto-20240414/libcerror/libcerror_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcerror/definitions.h>
 
 /* The definitions in <libcerror/definitions.h> are copied here
  * for local use of libcerror
  */
 #else
 
-#define LIBCERROR_VERSION				20240101
+#define LIBCERROR_VERSION				20240413
 
 /* The libcerror version string
  */
-#define LIBCERROR_VERSION_STRING			"20240101"
+#define LIBCERROR_VERSION_STRING			"20240413"
 
 /* The error domains
  */
 enum LIBCERROR_ERROR_DOMAINS
 {
 	LIBCERROR_ERROR_DOMAIN_ARGUMENTS		= (int) 'a',
 	LIBCERROR_ERROR_DOMAIN_CONVERSION		= (int) 'c',
```

### Comparing `libfcrypto-20240115/libcerror/libcerror_support.c` & `libfcrypto-20240414/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libcerror/libcerror_unused.h` & `libfcrypto-20240414/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/libcerror/Makefile.in` & `libfcrypto-20240414/libcerror/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -371,28 +371,29 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCERROR_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/common 
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../common -I$(top_srcdir)/common 
 
 @HAVE_LOCAL_LIBCERROR_TRUE@noinst_LTLIBRARIES = libcerror.la
 @HAVE_LOCAL_LIBCERROR_TRUE@libcerror_la_SOURCES = \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_definitions.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_extern.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_error.c libcerror_error.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_support.c libcerror_support.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_system.c libcerror_system.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_types.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -594,24 +595,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcerror_error.Plo
+	-rm -f ./$(DEPDIR)/libcerror_support.Plo
+	-rm -f ./$(DEPDIR)/libcerror_system.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -697,17 +703,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfcrypto-20240115/aclocal.m4` & `libfcrypto-20240414/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libfcrypto-20240115/configure.ac` & `libfcrypto-20240414/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libfcrypto],
- [20240115],
+ [20240414],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libfcrypto.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```


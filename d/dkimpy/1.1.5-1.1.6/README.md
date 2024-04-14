# Comparing `tmp/dkimpy-1.1.5.tar.gz` & `tmp/dkimpy-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkimpy-1.1.5.tar", last modified: Fri Jul 28 16:02:28 2023, max compression
+gzip compressed data, was "dkimpy-1.1.6.tar", last modified: Sun Apr 14 19:32:18 2024, max compression
```

## Comparing `dkimpy-1.1.5.tar` & `dkimpy-1.1.6.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-07-28 16:02:28.864313 dkimpy-1.1.5/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    14298 2023-07-28 15:57:20.000000 dkimpy-1.1.5/ChangeLog
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      979 2020-04-06 04:06:13.000000 dkimpy-1.1.5/LICENSE
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      200 2020-04-06 04:27:45.000000 dkimpy-1.1.5/MANIFEST.in
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    11065 2023-07-28 16:02:28.864313 dkimpy-1.1.5/PKG-INFO
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     8122 2023-07-28 15:59:27.000000 dkimpy-1.1.5/README.md
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-07-28 16:02:28.840312 dkimpy-1.1.5/dkim/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    57999 2023-05-12 05:08:45.000000 dkimpy-1.1.5/dkim/__init__.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      139 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/__main__.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     2570 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/arcsign.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1774 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/arcverify.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4300 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/asn1.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4829 2023-04-30 13:58:34.000000 dkimpy-1.1.5/dkim/asyncsupport.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4610 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/canonicalization.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     8173 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/crypto.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3628 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/dkimsign.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1951 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/dkimverify.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4737 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/dknewkey.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3315 2023-07-28 15:54:58.000000 dkimpy-1.1.5/dkim/dnsplug.py
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-07-28 16:02:28.848312 dkimpy-1.1.5/dkim/tests/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1769 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/tests/__init__.py
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-07-28 16:02:28.860313 dkimpy-1.1.5/dkim/tests/data/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:27:45.000000 dkimpy-1.1.5/dkim/tests/data/1024_testkey.key
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      212 2020-04-06 04:27:45.000000 dkimpy-1.1.5/dkim/tests/data/1024_testkey_wo_markers.pub.rsa.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:27:45.000000 dkimpy-1.1.5/dkim/tests/data/1024_testkey_wo_markers.pub.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1679 2020-04-06 04:27:45.000000 dkimpy-1.1.5/dkim/tests/data/2048_testkey.key
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1704 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/tests/data/2048_testkey_PKCS8.key
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      416 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/tests/data/2048_testkey_PKCS8.key.pub.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      384 2020-04-06 04:27:45.000000 dkimpy-1.1.5/dkim/tests/data/2048_testkey_wo_markers.pub.rsa.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      416 2020-04-06 04:27:45.000000 dkimpy-1.1.5/dkim/tests/data/2048_testkey_wo_markers.pub.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      251 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/badk.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/badversion.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       58 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/ed25519test.dns
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       45 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/ed25519test.key
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      346 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/ed25519test.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      588 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/ed25519test2.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       67 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/eximtest.dns
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4444 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/message.mbox
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      269 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/rfc6376.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1069 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/rfc6376.signed.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      708 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/rfc6376.signed.rsa.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      275 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/tests/data/rfc6376.w1258.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       45 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/rfc8032_7_1.key
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      346 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/test.message
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      778 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/tests/data/test.message.baddomain
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/test.private
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/test.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1104 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/test2.message
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/test2.private
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      233 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/test2.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/test_bad.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      219 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/test_extra.message
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      164 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/test_nofrom.message
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      250 2020-04-06 04:27:45.000000 dkimpy-1.1.5/dkim/tests/data/test_tlsrpt.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     5300 2020-04-06 04:27:45.000000 dkimpy-1.1.5/dkim/tests/test_arc.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     6045 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/test_canonicalization.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     6786 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/test_crypto.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    23644 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/tests/test_dkim.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    12866 2020-04-06 04:27:45.000000 dkimpy-1.1.5/dkim/tests/test_dkim_ed25519.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4476 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/tests/test_dkim_generate.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4923 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/tests/test_dkim_rsavariants.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    11980 2020-04-06 04:27:45.000000 dkimpy-1.1.5/dkim/tests/test_dkim_tlsrpt.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1557 2020-04-06 04:27:45.000000 dkimpy-1.1.5/dkim/tests/test_dnsplug.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3432 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/test_util.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     2501 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/util.py
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-07-28 16:02:28.860313 dkimpy-1.1.5/dkimpy.egg-info/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    11065 2023-07-28 16:02:28.000000 dkimpy-1.1.5/dkimpy.egg-info/PKG-INFO
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1986 2023-07-28 16:02:28.000000 dkimpy-1.1.5/dkimpy.egg-info/SOURCES.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)        1 2023-07-28 16:02:28.000000 dkimpy-1.1.5/dkimpy.egg-info/dependency_links.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      173 2023-07-28 16:02:28.000000 dkimpy-1.1.5/dkimpy.egg-info/entry_points.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)        1 2020-04-06 12:14:30.000000 dkimpy-1.1.5/dkimpy.egg-info/not-zip-safe
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       84 2023-07-28 16:02:28.000000 dkimpy-1.1.5/dkimpy.egg-info/requires.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)        5 2023-07-28 16:02:28.000000 dkimpy-1.1.5/dkimpy.egg-info/top_level.txt
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-07-28 16:02:28.864313 dkimpy-1.1.5/man/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4392 2020-04-06 04:06:13.000000 dkimpy-1.1.5/man/arcsign.1
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4152 2020-04-06 04:06:13.000000 dkimpy-1.1.5/man/arcverify.1
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4957 2020-04-06 04:06:13.000000 dkimpy-1.1.5/man/dkimsign.1
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4273 2023-04-30 14:18:48.000000 dkimpy-1.1.5/man/dkimverify.1
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4923 2020-04-06 04:06:13.000000 dkimpy-1.1.5/man/dknewkey.1
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       38 2023-07-28 16:02:28.864313 dkimpy-1.1.5/setup.cfg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3386 2023-07-28 15:59:47.000000 dkimpy-1.1.5/setup.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      268 2020-04-06 04:06:13.000000 dkimpy-1.1.5/test.py
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2024-04-14 19:32:18.070522 dkimpy-1.1.6/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    14489 2024-04-14 19:30:39.000000 dkimpy-1.1.6/ChangeLog
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      979 2020-04-06 04:06:13.000000 dkimpy-1.1.6/LICENSE
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      200 2020-04-06 04:27:45.000000 dkimpy-1.1.6/MANIFEST.in
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     9152 2024-04-14 19:32:18.070522 dkimpy-1.1.6/PKG-INFO
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     8122 2024-04-14 19:25:58.000000 dkimpy-1.1.6/README.md
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2024-04-14 19:32:18.066522 dkimpy-1.1.6/dkim/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    58000 2024-04-14 18:16:50.000000 dkimpy-1.1.6/dkim/__init__.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      139 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/__main__.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     2570 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/arcsign.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1774 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/arcverify.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4300 2023-04-30 14:18:48.000000 dkimpy-1.1.6/dkim/asn1.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4829 2023-04-30 13:58:34.000000 dkimpy-1.1.6/dkim/asyncsupport.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4610 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/canonicalization.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     8173 2023-04-30 14:18:48.000000 dkimpy-1.1.6/dkim/crypto.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3628 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/dkimsign.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1951 2023-04-30 14:18:48.000000 dkimpy-1.1.6/dkim/dkimverify.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4737 2023-04-30 14:18:48.000000 dkimpy-1.1.6/dkim/dknewkey.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3315 2023-07-28 15:54:58.000000 dkimpy-1.1.6/dkim/dnsplug.py
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2024-04-14 19:32:18.066522 dkimpy-1.1.6/dkim/tests/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1769 2023-04-30 14:18:48.000000 dkimpy-1.1.6/dkim/tests/__init__.py
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2024-04-14 19:32:18.070522 dkimpy-1.1.6/dkim/tests/data/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:27:45.000000 dkimpy-1.1.6/dkim/tests/data/1024_testkey.key
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      212 2020-04-06 04:27:45.000000 dkimpy-1.1.6/dkim/tests/data/1024_testkey_wo_markers.pub.rsa.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:27:45.000000 dkimpy-1.1.6/dkim/tests/data/1024_testkey_wo_markers.pub.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1679 2020-04-06 04:27:45.000000 dkimpy-1.1.6/dkim/tests/data/2048_testkey.key
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1704 2023-04-30 14:18:48.000000 dkimpy-1.1.6/dkim/tests/data/2048_testkey_PKCS8.key
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      416 2023-04-30 14:18:48.000000 dkimpy-1.1.6/dkim/tests/data/2048_testkey_PKCS8.key.pub.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      384 2020-04-06 04:27:45.000000 dkimpy-1.1.6/dkim/tests/data/2048_testkey_wo_markers.pub.rsa.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      416 2020-04-06 04:27:45.000000 dkimpy-1.1.6/dkim/tests/data/2048_testkey_wo_markers.pub.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      251 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/data/badk.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/data/badversion.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       58 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/data/ed25519test.dns
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       45 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/data/ed25519test.key
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      346 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/data/ed25519test.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      588 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/data/ed25519test2.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       67 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/data/eximtest.dns
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4444 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/data/message.mbox
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      269 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/data/rfc6376.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1069 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/data/rfc6376.signed.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      708 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/data/rfc6376.signed.rsa.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      275 2023-04-30 14:18:48.000000 dkimpy-1.1.6/dkim/tests/data/rfc6376.w1258.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       45 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/data/rfc8032_7_1.key
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      346 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/data/test.message
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      778 2023-04-30 14:18:48.000000 dkimpy-1.1.6/dkim/tests/data/test.message.baddomain
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/data/test.private
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/data/test.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1104 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/data/test2.message
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/data/test2.private
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      233 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/data/test2.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/data/test_bad.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      219 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/data/test_extra.message
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      164 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/data/test_nofrom.message
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      250 2020-04-06 04:27:45.000000 dkimpy-1.1.6/dkim/tests/data/test_tlsrpt.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     5300 2020-04-06 04:27:45.000000 dkimpy-1.1.6/dkim/tests/test_arc.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     6045 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/test_canonicalization.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     6786 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/test_crypto.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    23644 2023-04-30 14:18:48.000000 dkimpy-1.1.6/dkim/tests/test_dkim.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    12866 2020-04-06 04:27:45.000000 dkimpy-1.1.6/dkim/tests/test_dkim_ed25519.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4476 2023-04-30 14:18:48.000000 dkimpy-1.1.6/dkim/tests/test_dkim_generate.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4923 2023-04-30 14:18:48.000000 dkimpy-1.1.6/dkim/tests/test_dkim_rsavariants.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    11980 2020-04-06 04:27:45.000000 dkimpy-1.1.6/dkim/tests/test_dkim_tlsrpt.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1557 2020-04-06 04:27:45.000000 dkimpy-1.1.6/dkim/tests/test_dnsplug.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3432 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/tests/test_util.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     2501 2020-04-06 04:06:13.000000 dkimpy-1.1.6/dkim/util.py
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2024-04-14 19:32:18.070522 dkimpy-1.1.6/dkimpy.egg-info/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     9152 2024-04-14 19:32:17.000000 dkimpy-1.1.6/dkimpy.egg-info/PKG-INFO
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1986 2024-04-14 19:32:18.000000 dkimpy-1.1.6/dkimpy.egg-info/SOURCES.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)        1 2024-04-14 19:32:17.000000 dkimpy-1.1.6/dkimpy.egg-info/dependency_links.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      172 2024-04-14 19:32:17.000000 dkimpy-1.1.6/dkimpy.egg-info/entry_points.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)        1 2020-04-06 12:14:30.000000 dkimpy-1.1.6/dkimpy.egg-info/not-zip-safe
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       84 2024-04-14 19:32:17.000000 dkimpy-1.1.6/dkimpy.egg-info/requires.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)        5 2024-04-14 19:32:17.000000 dkimpy-1.1.6/dkimpy.egg-info/top_level.txt
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2024-04-14 19:32:18.070522 dkimpy-1.1.6/man/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4392 2020-04-06 04:06:13.000000 dkimpy-1.1.6/man/arcsign.1
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4152 2020-04-06 04:06:13.000000 dkimpy-1.1.6/man/arcverify.1
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4957 2020-04-06 04:06:13.000000 dkimpy-1.1.6/man/dkimsign.1
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4273 2023-04-30 14:18:48.000000 dkimpy-1.1.6/man/dkimverify.1
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4923 2020-04-06 04:06:13.000000 dkimpy-1.1.6/man/dknewkey.1
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       38 2024-04-14 19:32:18.074522 dkimpy-1.1.6/setup.cfg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3386 2024-04-14 19:27:00.000000 dkimpy-1.1.6/setup.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      268 2020-04-06 04:06:13.000000 dkimpy-1.1.6/test.py
```

### Comparing `dkimpy-1.1.5/ChangeLog` & `dkimpy-1.1.6/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2024-04-14 Version 1.1.6
+   - Use raw byte string for regex; fixes SyntaxWarning in Python 3.12 due to
+     invalid escape sequence (LP: #2049518)  - Thanks to Simon Chopin for the
+     fix
+
 2023-07-28 Version 1.1.5
    - Use dns.resolver.resolve instead of dns.resolver.query due to deprecation
      (LP: 2028783) - Thanks to Pedro Vicente for the report and the fix
 
 2023-05-12 Version 1.1.4
    - Treat dns.resolver.NoNameservers like NXDOMAIN (not an error) (Thanks to
      David for the patch and the report)
```

### Comparing `dkimpy-1.1.5/LICENSE` & `dkimpy-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/PKG-INFO` & `dkimpy-1.1.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,255 +1,15 @@
 Metadata-Version: 2.1
 Name: dkimpy
-Version: 1.1.5
+Version: 1.1.6
 Summary: DKIM (DomainKeys Identified Mail), ARC (Authenticated Receive Chain), and TLSRPT (TLS Report) email signing and verification
 Home-page: https://launchpad.net/dkimpy
 Author: Scott Kitterman
 Author-email: scott@kitterman.com
 License: BSD-like
-Description: dkimpy - DKIM (DomainKeys Identified Mail)
-        https://launchpad.net/dkimpy/
-        
-        Friendly fork of:
-        http://hewgill.com/pydkim/
-        
-        # INTRODUCTION
-        
-        dkimpy is a library that implements DKIM (DomainKeys Identified Mail) email
-        signing and verification.  Basic DKIM requirements are defined in RFC 6376:
-        
-        https://tools.ietf.org/html/rfc6376
-        
-        # VERSION
-        
-        This is dkimpy 1.1.5.
-        
-        # REQUIREMENTS
-        
-        Dependencies will be automatically included for normal DKIM usage.  The
-        extras_requires feature 'ed25519' will add the dependencies needed for signing
-        and verifying using the new DCRUP ed25519-sha256 algorithm.  The
-        extras_requires feature 'ARC' will add the extra dependencies needed for ARC.
-        Similarly, extras_requires feature 'asyncio' will add the extra dependencies
-        needed for asyncio.
-        
-         - Python 3.x >= 3.5.  Recent versions have not been on python3 < 3.4, but
-           may still work on earlier python3 versions.
-         - dnspython or py3dns. dnspython is preferred if both are present and
-           installed to satisfy the DNS module requirement if neither are installed.
-         - authres.  Needed for ARC.
-         - PyNaCl.  Needed for use of ed25519 capability.
-         - aiodns.  Needed for asycnio (Requires python3.5 or later)
-        
-        # INSTALLATION
-        
-        This package includes a scripts and man pages.  For those to be installed when
-        installing using setup.py, the following incantation is required because
-        setuptools developers decided not being able to do this by default is a
-        feature:
-        
-        ```python3 setup.py install --single-version-externally-managed --record=/dev/null```
-        
-        # DOCUMENTATION
-        
-        An online version of the package documentation for the most recent release can
-        be found at:
-        
-        https://pymilter.org/pydkim/
-        
-        # TESTING
-        
-        To run dkimpy's test suite:
-        
-        ```PYTHONPATH=. python3 dkim```
-        
-        or
-        
-        ```python3 test.py```
-        
-        or
-        
-        ```PYTHONPATH=. python3 -m unittest dkim.tests.test_suite```
-        
-        
-        Alternatively, if you have testrepository installed:
-        
-        ```testr init```
-        
-        ```testr run```
-        
-        You should install all optional dependencies required for the test suite, e.g.
-        by creating a virtualenv and using:
-        
-        ```pip install -e '.[testing]'```
-        
-        The included ARC tests are very limited.  The primary testing method for ARC
-        is using the ARC test suite: https://github.com/ValiMail/arc_test_suite
-        
-        As of 0.6.0, all tests pass for both python2.7 and python3. The test suite
-         ships with test runners for dkimpy.  After downloading the test suite, you
-         can run the signing and validation tests like this:
-        
-        ```python3 ./testarc.py sign runners/arcsigntest.py```
-        ```python3 ./testarc.py validate runners/arcverifytest.py```
-        
-        As ov version 1.1.0, python2.7 is no longer supported.
-        
-        # USAGE
-        
-        The dkimpy library offers one module called dkim. The sign() function takes an
-        RFC822 formatted message, along with some signing options, and returns a
-        DKIM-Signature header line that can be prepended to the message. The verify()
-        function takes an RFC822 formatted message, and returns True or False depending
-        on whether the signature verifies correctly.  There is also a DKIM class which
-        can be used to perform these functions in a more modern way.
-        
-        In version 0.9.0, the default set of header fields that are oversigned was
-        changed from 'from', 'subject', 'date' to 'from' to reduce fragility of
-        signatures.  To restore the previous behavior, you can add them back after
-        instantiating your DKIM class using the add_frozen function as shown in the
-        following example:
-        
-        ```python
-        >>> dkim = DKIM()
-        >>> dkim.add_frozen((b'date',b'subject'))
-        >>> [text(x) for x in sorted(dkim.frozen_sign)]
-        ['date', 'from', 'subject']
-        ```
-        
-        ## DKIM RSA MODERNIZATION (RFC 8301)
-        
-        RFC8301 updated DKIM requirements in two ways:
-        
-        1.  It set the minimum valid RSA key size to 1024 bits.
-        2.  It removed use of rsa-sha1.
-        
-        As of version 0.7, the dkimpy defaults largely support these requirements.
-        
-        It is possible to override the minimum key size to a lower value, but this is
-        strongly discouraged.  As of 2018, keys much smaller than the minimum are not
-        difficult to factor.
-        
-        The code for rsa-sha1 signing and verification is retained, but not used for
-        signing by default.  Future releases will raise warnings and then errors when
-        verifying rsa-sha1 signatures.  There are still some significant users of
-        rsa-sha1 signatures, so operationally it's premature to disable verification
-        of rsa-sha1.
-        
-        ## ED25519 (RFC 8463) SUPPORT
-        
-        As of version 0.7, experimental signing and verifying of DKIM Ed25519
-        signatures is supported as described in draft-ietf-dcrup-dkim-crypto:
-        
-        https://datatracker.ietf.org/doc/draft-ietf-dcrup-dkim-crypto/
-        
-        The RFC that documents ed25519 DKIM signatures, RFC 8463, has been released
-        and dkimpy 0.7 and later are aligned to its requirements.  As of 0.8, ed25519
-        need not be considered experimental.  The dkimpy implementation has
-        successfully interoperated with three other implementations and the technical
-        parameters for ed25519-sha256 are defined and stable.
-        
-        To install from pypi with the required optional depenencies, use the ed25519
-        option:
-        
-        ```pip install -e '.[ed25519]'```
-        
-        ## DKIM SCRIPTS
-        
-        Three helper programs are also supplied: dknewkey, dkimsign and
-        dkimverify
-        
-        dknewkey is s script that produces private and public key pairs suitable
-        for use with DKIM.  Note that the private key file format used for ed25519 is
-        not standardized (there is no standard) and is unique to dkimpy.  Creation of
-        keys should be done in a secure environment.  If an unauthorized entity gains
-        access to current private keys they can generate signed email that will pass
-        DKIM checkes and will be difficult to repudiate.
-        
-        dkimsign is a filter that reads an RFC822 message on standard input, and
-        writes the same message on standard output with a DKIM-Signature line
-        prepended. The signing options are specified on the command line:
-        
-        dkimsign selector domain privatekeyfile [identity]
-        
-        The identity is optional and defaults to "@domain".
-        
-        dkimverify reads an RFC822 message on standard input, and returns with exit
-        code 0 if the signature verifies successfully. Otherwise, it returns with exit
-        code 1. 
-        
-        ## ARC (Authenticated Receive Chain)
-        
-        As of version 0.6.0, dkimpy provides experimental support for ARC (Authenticated
-        Received Chain).  See RFC 8617 for the current version of ARC:
-        
-        https://tools.ietf.org/html/rfc8617
-        
-        In addition to arcsign and arcverify, the dkim module now provides
-        arc_sign and arc_verify functions as well as an ARC class.
-        
-        If an invalid authentication results header field is included in the set for
-        ARC, it is ignored and no error is raised.
-        
-        Both DKIM ed25519 and ARC are now considered stable (no longer experimantal).
-        
-        ## ASYNC SUPPORT
-        
-        As of version 1.0, an alternative to dkim.verify for use in an async
-        environment is provied.  It requires aiodns, https://pypi.org/project/aiodns/.
-        Here is a simple example of dkim.verify_async usage:
-        
-        ```python
-        >>> sys.stdin = sys.stdin.detach()
-        >>>
-        >>> async def main():
-        >>>     res = await dkim.verify_async(message)
-        >>>     return res
-        >>>
-        >>> if __name__ == "__main__":
-        >>>     res = asyncio.run(main())
-        ```
-        
-        This feature requires python3.5 or newer.
-        
-        If aiodns is available, the async functions will be used.  To avoide async
-        when aiodns is availale, set dkim.USE_ASYNC = False.
-        
-        ## TLSRPT (TLS Report)
-        
-        As of version 1.0, the RFC 8460 tlsrpt service type is supported:
-        
-        https://tools.ietf.org/html/rfc8460
-        
-        A non-tlsrpt signed with a key record with s=tlsrpt won't verify.  Since the
-        service type (s=) is optional in the DKIM public key record, it is not
-        required by RFC 8460.  When checking for a tlsrpt signature, set the tlsrpt=
-        flag when verifying the signature:
-        
-        ```python
-        >>> res = dkim.verify(smessage, tlsrpt='strict')
-        ```
-        
-        If tlsrpt='strict', only public key records with s=tlsrpt will be considered
-        valid.  If set to tlsrpt=True, the service type is not required, but other
-        RFC 8460 requirements are applied.
-        
-        # LIMITATIONS
-        
-        Dkimpy will correctly sign/verify messages with ASCII or UTF-8 content.
-        Messages that contain other types of content will not verify correctly.  It
-        does not yet implement RFC 8616, Email Authentication for Internationalized
-        Mail.
-        
-        # FEEDBACK
-        
-        Bug reports may be submitted to the bug tracker for the dkimpy project on
-        launchpad.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: Developers
 Classifier: License :: DFSG approved
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -258,7 +18,247 @@
 Classifier: Topic :: Internet :: Name Service (DNS)
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: ARC
 Provides-Extra: asyncio
 Provides-Extra: ed25519
 Provides-Extra: testing
+License-File: LICENSE
+
+dkimpy - DKIM (DomainKeys Identified Mail)
+https://launchpad.net/dkimpy/
+
+Friendly fork of:
+http://hewgill.com/pydkim/
+
+# INTRODUCTION
+
+dkimpy is a library that implements DKIM (DomainKeys Identified Mail) email
+signing and verification.  Basic DKIM requirements are defined in RFC 6376:
+
+https://tools.ietf.org/html/rfc6376
+
+# VERSION
+
+This is dkimpy 1.1.6.
+
+# REQUIREMENTS
+
+Dependencies will be automatically included for normal DKIM usage.  The
+extras_requires feature 'ed25519' will add the dependencies needed for signing
+and verifying using the new DCRUP ed25519-sha256 algorithm.  The
+extras_requires feature 'ARC' will add the extra dependencies needed for ARC.
+Similarly, extras_requires feature 'asyncio' will add the extra dependencies
+needed for asyncio.
+
+ - Python 3.x >= 3.5.  Recent versions have not been on python3 < 3.4, but
+   may still work on earlier python3 versions.
+ - dnspython or py3dns. dnspython is preferred if both are present and
+   installed to satisfy the DNS module requirement if neither are installed.
+ - authres.  Needed for ARC.
+ - PyNaCl.  Needed for use of ed25519 capability.
+ - aiodns.  Needed for asycnio (Requires python3.5 or later)
+
+# INSTALLATION
+
+This package includes a scripts and man pages.  For those to be installed when
+installing using setup.py, the following incantation is required because
+setuptools developers decided not being able to do this by default is a
+feature:
+
+```python3 setup.py install --single-version-externally-managed --record=/dev/null```
+
+# DOCUMENTATION
+
+An online version of the package documentation for the most recent release can
+be found at:
+
+https://pymilter.org/pydkim/
+
+# TESTING
+
+To run dkimpy's test suite:
+
+```PYTHONPATH=. python3 dkim```
+
+or
+
+```python3 test.py```
+
+or
+
+```PYTHONPATH=. python3 -m unittest dkim.tests.test_suite```
+
+
+Alternatively, if you have testrepository installed:
+
+```testr init```
+
+```testr run```
+
+You should install all optional dependencies required for the test suite, e.g.
+by creating a virtualenv and using:
+
+```pip install -e '.[testing]'```
+
+The included ARC tests are very limited.  The primary testing method for ARC
+is using the ARC test suite: https://github.com/ValiMail/arc_test_suite
+
+As of 0.6.0, all tests pass for both python2.7 and python3. The test suite
+ ships with test runners for dkimpy.  After downloading the test suite, you
+ can run the signing and validation tests like this:
+
+```python3 ./testarc.py sign runners/arcsigntest.py```
+```python3 ./testarc.py validate runners/arcverifytest.py```
+
+As ov version 1.1.0, python2.7 is no longer supported.
+
+# USAGE
+
+The dkimpy library offers one module called dkim. The sign() function takes an
+RFC822 formatted message, along with some signing options, and returns a
+DKIM-Signature header line that can be prepended to the message. The verify()
+function takes an RFC822 formatted message, and returns True or False depending
+on whether the signature verifies correctly.  There is also a DKIM class which
+can be used to perform these functions in a more modern way.
+
+In version 0.9.0, the default set of header fields that are oversigned was
+changed from 'from', 'subject', 'date' to 'from' to reduce fragility of
+signatures.  To restore the previous behavior, you can add them back after
+instantiating your DKIM class using the add_frozen function as shown in the
+following example:
+
+```python
+>>> dkim = DKIM()
+>>> dkim.add_frozen((b'date',b'subject'))
+>>> [text(x) for x in sorted(dkim.frozen_sign)]
+['date', 'from', 'subject']
+```
+
+## DKIM RSA MODERNIZATION (RFC 8301)
+
+RFC8301 updated DKIM requirements in two ways:
+
+1.  It set the minimum valid RSA key size to 1024 bits.
+2.  It removed use of rsa-sha1.
+
+As of version 0.7, the dkimpy defaults largely support these requirements.
+
+It is possible to override the minimum key size to a lower value, but this is
+strongly discouraged.  As of 2018, keys much smaller than the minimum are not
+difficult to factor.
+
+The code for rsa-sha1 signing and verification is retained, but not used for
+signing by default.  Future releases will raise warnings and then errors when
+verifying rsa-sha1 signatures.  There are still some significant users of
+rsa-sha1 signatures, so operationally it's premature to disable verification
+of rsa-sha1.
+
+## ED25519 (RFC 8463) SUPPORT
+
+As of version 0.7, experimental signing and verifying of DKIM Ed25519
+signatures is supported as described in draft-ietf-dcrup-dkim-crypto:
+
+https://datatracker.ietf.org/doc/draft-ietf-dcrup-dkim-crypto/
+
+The RFC that documents ed25519 DKIM signatures, RFC 8463, has been released
+and dkimpy 0.7 and later are aligned to its requirements.  As of 0.8, ed25519
+need not be considered experimental.  The dkimpy implementation has
+successfully interoperated with three other implementations and the technical
+parameters for ed25519-sha256 are defined and stable.
+
+To install from pypi with the required optional depenencies, use the ed25519
+option:
+
+```pip install -e '.[ed25519]'```
+
+## DKIM SCRIPTS
+
+Three helper programs are also supplied: dknewkey, dkimsign and
+dkimverify
+
+dknewkey is s script that produces private and public key pairs suitable
+for use with DKIM.  Note that the private key file format used for ed25519 is
+not standardized (there is no standard) and is unique to dkimpy.  Creation of
+keys should be done in a secure environment.  If an unauthorized entity gains
+access to current private keys they can generate signed email that will pass
+DKIM checkes and will be difficult to repudiate.
+
+dkimsign is a filter that reads an RFC822 message on standard input, and
+writes the same message on standard output with a DKIM-Signature line
+prepended. The signing options are specified on the command line:
+
+dkimsign selector domain privatekeyfile [identity]
+
+The identity is optional and defaults to "@domain".
+
+dkimverify reads an RFC822 message on standard input, and returns with exit
+code 0 if the signature verifies successfully. Otherwise, it returns with exit
+code 1. 
+
+## ARC (Authenticated Receive Chain)
+
+As of version 0.6.0, dkimpy provides experimental support for ARC (Authenticated
+Received Chain).  See RFC 8617 for the current version of ARC:
+
+https://tools.ietf.org/html/rfc8617
+
+In addition to arcsign and arcverify, the dkim module now provides
+arc_sign and arc_verify functions as well as an ARC class.
+
+If an invalid authentication results header field is included in the set for
+ARC, it is ignored and no error is raised.
+
+Both DKIM ed25519 and ARC are now considered stable (no longer experimantal).
+
+## ASYNC SUPPORT
+
+As of version 1.0, an alternative to dkim.verify for use in an async
+environment is provied.  It requires aiodns, https://pypi.org/project/aiodns/.
+Here is a simple example of dkim.verify_async usage:
+
+```python
+>>> sys.stdin = sys.stdin.detach()
+>>>
+>>> async def main():
+>>>     res = await dkim.verify_async(message)
+>>>     return res
+>>>
+>>> if __name__ == "__main__":
+>>>     res = asyncio.run(main())
+```
+
+This feature requires python3.5 or newer.
+
+If aiodns is available, the async functions will be used.  To avoide async
+when aiodns is availale, set dkim.USE_ASYNC = False.
+
+## TLSRPT (TLS Report)
+
+As of version 1.0, the RFC 8460 tlsrpt service type is supported:
+
+https://tools.ietf.org/html/rfc8460
+
+A non-tlsrpt signed with a key record with s=tlsrpt won't verify.  Since the
+service type (s=) is optional in the DKIM public key record, it is not
+required by RFC 8460.  When checking for a tlsrpt signature, set the tlsrpt=
+flag when verifying the signature:
+
+```python
+>>> res = dkim.verify(smessage, tlsrpt='strict')
+```
+
+If tlsrpt='strict', only public key records with s=tlsrpt will be considered
+valid.  If set to tlsrpt=True, the service type is not required, but other
+RFC 8460 requirements are applied.
+
+# LIMITATIONS
+
+Dkimpy will correctly sign/verify messages with ASCII or UTF-8 content.
+Messages that contain other types of content will not verify correctly.  It
+does not yet implement RFC 8616, Email Authentication for Internationalized
+Mail.
+
+# FEEDBACK
+
+Bug reports may be submitted to the bug tracker for the dkimpy project on
+launchpad.
```

### Comparing `dkimpy-1.1.5/README.md` & `dkimpy-1.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 dkimpy is a library that implements DKIM (DomainKeys Identified Mail) email
 signing and verification.  Basic DKIM requirements are defined in RFC 6376:
 
 https://tools.ietf.org/html/rfc6376
 
 # VERSION
 
-This is dkimpy 1.1.5.
+This is dkimpy 1.1.6.
 
 # REQUIREMENTS
 
 Dependencies will be automatically included for normal DKIM usage.  The
 extras_requires feature 'ed25519' will add the dependencies needed for signing
 and verifying using the new DCRUP ed25519-sha256 algorithm.  The
 extras_requires feature 'ARC' will add the extra dependencies needed for ARC.
```

### Comparing `dkimpy-1.1.5/dkim/__init__.py` & `dkimpy-1.1.6/dkim/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,15 +298,15 @@
     if b'cv' in sig and sig[b'cv'] not in (CV_Pass, CV_Fail, CV_None):
         raise ValidationError("cv= value is not valid (%s)" % sig[b'cv'])
 
     # Limit domain validation to ASCII domains because too hard
     try:
         str(sig[b'd'], 'ascii')
         # No specials, which is close enough
-        if re.findall(b"[\(\)<>\[\]:;@\\,]", sig[b'd']):
+        if re.findall(rb"[\(\)<>\[\]:;@\\,]", sig[b'd']):
             raise ValidationError("d= value is not valid (%s)" % sig[b'd'])
     except UnicodeDecodeError as e:
         # Not an ASCII domain
         pass
 
     # Nasty hack to support both str and bytes... check for both the
     # character and integer values.
```

### Comparing `dkimpy-1.1.5/dkim/arcsign.py` & `dkimpy-1.1.6/dkim/arcsign.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/arcverify.py` & `dkimpy-1.1.6/dkim/arcverify.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/asn1.py` & `dkimpy-1.1.6/dkim/asn1.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/asyncsupport.py` & `dkimpy-1.1.6/dkim/asyncsupport.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/canonicalization.py` & `dkimpy-1.1.6/dkim/canonicalization.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/crypto.py` & `dkimpy-1.1.6/dkim/crypto.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/dkimsign.py` & `dkimpy-1.1.6/dkim/dkimsign.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/dkimverify.py` & `dkimpy-1.1.6/dkim/dkimverify.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/dknewkey.py` & `dkimpy-1.1.6/dkim/dknewkey.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/dnsplug.py` & `dkimpy-1.1.6/dkim/dnsplug.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/tests/__init__.py` & `dkimpy-1.1.6/dkim/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/tests/data/1024_testkey.key` & `dkimpy-1.1.6/dkim/tests/data/1024_testkey.key`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/tests/data/2048_testkey.key` & `dkimpy-1.1.6/dkim/tests/data/2048_testkey.key`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/tests/data/2048_testkey_PKCS8.key` & `dkimpy-1.1.6/dkim/tests/data/2048_testkey_PKCS8.key`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/tests/data/ed25519test2.msg` & `dkimpy-1.1.6/dkim/tests/data/ed25519test2.msg`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/tests/data/message.mbox` & `dkimpy-1.1.6/dkim/tests/data/message.mbox`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/tests/data/rfc6376.signed.msg` & `dkimpy-1.1.6/dkim/tests/data/rfc6376.signed.msg`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/tests/data/rfc6376.signed.rsa.msg` & `dkimpy-1.1.6/dkim/tests/data/rfc6376.signed.rsa.msg`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/tests/data/test.message.baddomain` & `dkimpy-1.1.6/dkim/tests/data/test.message.baddomain`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/tests/data/test.private` & `dkimpy-1.1.6/dkim/tests/data/test.private`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/tests/data/test2.message` & `dkimpy-1.1.6/dkim/tests/data/test2.message`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/tests/data/test2.private` & `dkimpy-1.1.6/dkim/tests/data/test2.private`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/tests/test_arc.py` & `dkimpy-1.1.6/dkim/tests/test_arc.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/tests/test_canonicalization.py` & `dkimpy-1.1.6/dkim/tests/test_canonicalization.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/tests/test_crypto.py` & `dkimpy-1.1.6/dkim/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/tests/test_dkim.py` & `dkimpy-1.1.6/dkim/tests/test_dkim.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/tests/test_dkim_ed25519.py` & `dkimpy-1.1.6/dkim/tests/test_dkim_ed25519.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/tests/test_dkim_generate.py` & `dkimpy-1.1.6/dkim/tests/test_dkim_generate.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/tests/test_dkim_rsavariants.py` & `dkimpy-1.1.6/dkim/tests/test_dkim_rsavariants.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/tests/test_dkim_tlsrpt.py` & `dkimpy-1.1.6/dkim/tests/test_dkim_tlsrpt.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/tests/test_dnsplug.py` & `dkimpy-1.1.6/dkim/tests/test_dnsplug.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/tests/test_util.py` & `dkimpy-1.1.6/dkim/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkim/util.py` & `dkimpy-1.1.6/dkim/util.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/dkimpy.egg-info/PKG-INFO` & `dkimpy-1.1.6/dkimpy.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,255 +1,15 @@
 Metadata-Version: 2.1
 Name: dkimpy
-Version: 1.1.5
+Version: 1.1.6
 Summary: DKIM (DomainKeys Identified Mail), ARC (Authenticated Receive Chain), and TLSRPT (TLS Report) email signing and verification
 Home-page: https://launchpad.net/dkimpy
 Author: Scott Kitterman
 Author-email: scott@kitterman.com
 License: BSD-like
-Description: dkimpy - DKIM (DomainKeys Identified Mail)
-        https://launchpad.net/dkimpy/
-        
-        Friendly fork of:
-        http://hewgill.com/pydkim/
-        
-        # INTRODUCTION
-        
-        dkimpy is a library that implements DKIM (DomainKeys Identified Mail) email
-        signing and verification.  Basic DKIM requirements are defined in RFC 6376:
-        
-        https://tools.ietf.org/html/rfc6376
-        
-        # VERSION
-        
-        This is dkimpy 1.1.5.
-        
-        # REQUIREMENTS
-        
-        Dependencies will be automatically included for normal DKIM usage.  The
-        extras_requires feature 'ed25519' will add the dependencies needed for signing
-        and verifying using the new DCRUP ed25519-sha256 algorithm.  The
-        extras_requires feature 'ARC' will add the extra dependencies needed for ARC.
-        Similarly, extras_requires feature 'asyncio' will add the extra dependencies
-        needed for asyncio.
-        
-         - Python 3.x >= 3.5.  Recent versions have not been on python3 < 3.4, but
-           may still work on earlier python3 versions.
-         - dnspython or py3dns. dnspython is preferred if both are present and
-           installed to satisfy the DNS module requirement if neither are installed.
-         - authres.  Needed for ARC.
-         - PyNaCl.  Needed for use of ed25519 capability.
-         - aiodns.  Needed for asycnio (Requires python3.5 or later)
-        
-        # INSTALLATION
-        
-        This package includes a scripts and man pages.  For those to be installed when
-        installing using setup.py, the following incantation is required because
-        setuptools developers decided not being able to do this by default is a
-        feature:
-        
-        ```python3 setup.py install --single-version-externally-managed --record=/dev/null```
-        
-        # DOCUMENTATION
-        
-        An online version of the package documentation for the most recent release can
-        be found at:
-        
-        https://pymilter.org/pydkim/
-        
-        # TESTING
-        
-        To run dkimpy's test suite:
-        
-        ```PYTHONPATH=. python3 dkim```
-        
-        or
-        
-        ```python3 test.py```
-        
-        or
-        
-        ```PYTHONPATH=. python3 -m unittest dkim.tests.test_suite```
-        
-        
-        Alternatively, if you have testrepository installed:
-        
-        ```testr init```
-        
-        ```testr run```
-        
-        You should install all optional dependencies required for the test suite, e.g.
-        by creating a virtualenv and using:
-        
-        ```pip install -e '.[testing]'```
-        
-        The included ARC tests are very limited.  The primary testing method for ARC
-        is using the ARC test suite: https://github.com/ValiMail/arc_test_suite
-        
-        As of 0.6.0, all tests pass for both python2.7 and python3. The test suite
-         ships with test runners for dkimpy.  After downloading the test suite, you
-         can run the signing and validation tests like this:
-        
-        ```python3 ./testarc.py sign runners/arcsigntest.py```
-        ```python3 ./testarc.py validate runners/arcverifytest.py```
-        
-        As ov version 1.1.0, python2.7 is no longer supported.
-        
-        # USAGE
-        
-        The dkimpy library offers one module called dkim. The sign() function takes an
-        RFC822 formatted message, along with some signing options, and returns a
-        DKIM-Signature header line that can be prepended to the message. The verify()
-        function takes an RFC822 formatted message, and returns True or False depending
-        on whether the signature verifies correctly.  There is also a DKIM class which
-        can be used to perform these functions in a more modern way.
-        
-        In version 0.9.0, the default set of header fields that are oversigned was
-        changed from 'from', 'subject', 'date' to 'from' to reduce fragility of
-        signatures.  To restore the previous behavior, you can add them back after
-        instantiating your DKIM class using the add_frozen function as shown in the
-        following example:
-        
-        ```python
-        >>> dkim = DKIM()
-        >>> dkim.add_frozen((b'date',b'subject'))
-        >>> [text(x) for x in sorted(dkim.frozen_sign)]
-        ['date', 'from', 'subject']
-        ```
-        
-        ## DKIM RSA MODERNIZATION (RFC 8301)
-        
-        RFC8301 updated DKIM requirements in two ways:
-        
-        1.  It set the minimum valid RSA key size to 1024 bits.
-        2.  It removed use of rsa-sha1.
-        
-        As of version 0.7, the dkimpy defaults largely support these requirements.
-        
-        It is possible to override the minimum key size to a lower value, but this is
-        strongly discouraged.  As of 2018, keys much smaller than the minimum are not
-        difficult to factor.
-        
-        The code for rsa-sha1 signing and verification is retained, but not used for
-        signing by default.  Future releases will raise warnings and then errors when
-        verifying rsa-sha1 signatures.  There are still some significant users of
-        rsa-sha1 signatures, so operationally it's premature to disable verification
-        of rsa-sha1.
-        
-        ## ED25519 (RFC 8463) SUPPORT
-        
-        As of version 0.7, experimental signing and verifying of DKIM Ed25519
-        signatures is supported as described in draft-ietf-dcrup-dkim-crypto:
-        
-        https://datatracker.ietf.org/doc/draft-ietf-dcrup-dkim-crypto/
-        
-        The RFC that documents ed25519 DKIM signatures, RFC 8463, has been released
-        and dkimpy 0.7 and later are aligned to its requirements.  As of 0.8, ed25519
-        need not be considered experimental.  The dkimpy implementation has
-        successfully interoperated with three other implementations and the technical
-        parameters for ed25519-sha256 are defined and stable.
-        
-        To install from pypi with the required optional depenencies, use the ed25519
-        option:
-        
-        ```pip install -e '.[ed25519]'```
-        
-        ## DKIM SCRIPTS
-        
-        Three helper programs are also supplied: dknewkey, dkimsign and
-        dkimverify
-        
-        dknewkey is s script that produces private and public key pairs suitable
-        for use with DKIM.  Note that the private key file format used for ed25519 is
-        not standardized (there is no standard) and is unique to dkimpy.  Creation of
-        keys should be done in a secure environment.  If an unauthorized entity gains
-        access to current private keys they can generate signed email that will pass
-        DKIM checkes and will be difficult to repudiate.
-        
-        dkimsign is a filter that reads an RFC822 message on standard input, and
-        writes the same message on standard output with a DKIM-Signature line
-        prepended. The signing options are specified on the command line:
-        
-        dkimsign selector domain privatekeyfile [identity]
-        
-        The identity is optional and defaults to "@domain".
-        
-        dkimverify reads an RFC822 message on standard input, and returns with exit
-        code 0 if the signature verifies successfully. Otherwise, it returns with exit
-        code 1. 
-        
-        ## ARC (Authenticated Receive Chain)
-        
-        As of version 0.6.0, dkimpy provides experimental support for ARC (Authenticated
-        Received Chain).  See RFC 8617 for the current version of ARC:
-        
-        https://tools.ietf.org/html/rfc8617
-        
-        In addition to arcsign and arcverify, the dkim module now provides
-        arc_sign and arc_verify functions as well as an ARC class.
-        
-        If an invalid authentication results header field is included in the set for
-        ARC, it is ignored and no error is raised.
-        
-        Both DKIM ed25519 and ARC are now considered stable (no longer experimantal).
-        
-        ## ASYNC SUPPORT
-        
-        As of version 1.0, an alternative to dkim.verify for use in an async
-        environment is provied.  It requires aiodns, https://pypi.org/project/aiodns/.
-        Here is a simple example of dkim.verify_async usage:
-        
-        ```python
-        >>> sys.stdin = sys.stdin.detach()
-        >>>
-        >>> async def main():
-        >>>     res = await dkim.verify_async(message)
-        >>>     return res
-        >>>
-        >>> if __name__ == "__main__":
-        >>>     res = asyncio.run(main())
-        ```
-        
-        This feature requires python3.5 or newer.
-        
-        If aiodns is available, the async functions will be used.  To avoide async
-        when aiodns is availale, set dkim.USE_ASYNC = False.
-        
-        ## TLSRPT (TLS Report)
-        
-        As of version 1.0, the RFC 8460 tlsrpt service type is supported:
-        
-        https://tools.ietf.org/html/rfc8460
-        
-        A non-tlsrpt signed with a key record with s=tlsrpt won't verify.  Since the
-        service type (s=) is optional in the DKIM public key record, it is not
-        required by RFC 8460.  When checking for a tlsrpt signature, set the tlsrpt=
-        flag when verifying the signature:
-        
-        ```python
-        >>> res = dkim.verify(smessage, tlsrpt='strict')
-        ```
-        
-        If tlsrpt='strict', only public key records with s=tlsrpt will be considered
-        valid.  If set to tlsrpt=True, the service type is not required, but other
-        RFC 8460 requirements are applied.
-        
-        # LIMITATIONS
-        
-        Dkimpy will correctly sign/verify messages with ASCII or UTF-8 content.
-        Messages that contain other types of content will not verify correctly.  It
-        does not yet implement RFC 8616, Email Authentication for Internationalized
-        Mail.
-        
-        # FEEDBACK
-        
-        Bug reports may be submitted to the bug tracker for the dkimpy project on
-        launchpad.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: Developers
 Classifier: License :: DFSG approved
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -258,7 +18,247 @@
 Classifier: Topic :: Internet :: Name Service (DNS)
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: ARC
 Provides-Extra: asyncio
 Provides-Extra: ed25519
 Provides-Extra: testing
+License-File: LICENSE
+
+dkimpy - DKIM (DomainKeys Identified Mail)
+https://launchpad.net/dkimpy/
+
+Friendly fork of:
+http://hewgill.com/pydkim/
+
+# INTRODUCTION
+
+dkimpy is a library that implements DKIM (DomainKeys Identified Mail) email
+signing and verification.  Basic DKIM requirements are defined in RFC 6376:
+
+https://tools.ietf.org/html/rfc6376
+
+# VERSION
+
+This is dkimpy 1.1.6.
+
+# REQUIREMENTS
+
+Dependencies will be automatically included for normal DKIM usage.  The
+extras_requires feature 'ed25519' will add the dependencies needed for signing
+and verifying using the new DCRUP ed25519-sha256 algorithm.  The
+extras_requires feature 'ARC' will add the extra dependencies needed for ARC.
+Similarly, extras_requires feature 'asyncio' will add the extra dependencies
+needed for asyncio.
+
+ - Python 3.x >= 3.5.  Recent versions have not been on python3 < 3.4, but
+   may still work on earlier python3 versions.
+ - dnspython or py3dns. dnspython is preferred if both are present and
+   installed to satisfy the DNS module requirement if neither are installed.
+ - authres.  Needed for ARC.
+ - PyNaCl.  Needed for use of ed25519 capability.
+ - aiodns.  Needed for asycnio (Requires python3.5 or later)
+
+# INSTALLATION
+
+This package includes a scripts and man pages.  For those to be installed when
+installing using setup.py, the following incantation is required because
+setuptools developers decided not being able to do this by default is a
+feature:
+
+```python3 setup.py install --single-version-externally-managed --record=/dev/null```
+
+# DOCUMENTATION
+
+An online version of the package documentation for the most recent release can
+be found at:
+
+https://pymilter.org/pydkim/
+
+# TESTING
+
+To run dkimpy's test suite:
+
+```PYTHONPATH=. python3 dkim```
+
+or
+
+```python3 test.py```
+
+or
+
+```PYTHONPATH=. python3 -m unittest dkim.tests.test_suite```
+
+
+Alternatively, if you have testrepository installed:
+
+```testr init```
+
+```testr run```
+
+You should install all optional dependencies required for the test suite, e.g.
+by creating a virtualenv and using:
+
+```pip install -e '.[testing]'```
+
+The included ARC tests are very limited.  The primary testing method for ARC
+is using the ARC test suite: https://github.com/ValiMail/arc_test_suite
+
+As of 0.6.0, all tests pass for both python2.7 and python3. The test suite
+ ships with test runners for dkimpy.  After downloading the test suite, you
+ can run the signing and validation tests like this:
+
+```python3 ./testarc.py sign runners/arcsigntest.py```
+```python3 ./testarc.py validate runners/arcverifytest.py```
+
+As ov version 1.1.0, python2.7 is no longer supported.
+
+# USAGE
+
+The dkimpy library offers one module called dkim. The sign() function takes an
+RFC822 formatted message, along with some signing options, and returns a
+DKIM-Signature header line that can be prepended to the message. The verify()
+function takes an RFC822 formatted message, and returns True or False depending
+on whether the signature verifies correctly.  There is also a DKIM class which
+can be used to perform these functions in a more modern way.
+
+In version 0.9.0, the default set of header fields that are oversigned was
+changed from 'from', 'subject', 'date' to 'from' to reduce fragility of
+signatures.  To restore the previous behavior, you can add them back after
+instantiating your DKIM class using the add_frozen function as shown in the
+following example:
+
+```python
+>>> dkim = DKIM()
+>>> dkim.add_frozen((b'date',b'subject'))
+>>> [text(x) for x in sorted(dkim.frozen_sign)]
+['date', 'from', 'subject']
+```
+
+## DKIM RSA MODERNIZATION (RFC 8301)
+
+RFC8301 updated DKIM requirements in two ways:
+
+1.  It set the minimum valid RSA key size to 1024 bits.
+2.  It removed use of rsa-sha1.
+
+As of version 0.7, the dkimpy defaults largely support these requirements.
+
+It is possible to override the minimum key size to a lower value, but this is
+strongly discouraged.  As of 2018, keys much smaller than the minimum are not
+difficult to factor.
+
+The code for rsa-sha1 signing and verification is retained, but not used for
+signing by default.  Future releases will raise warnings and then errors when
+verifying rsa-sha1 signatures.  There are still some significant users of
+rsa-sha1 signatures, so operationally it's premature to disable verification
+of rsa-sha1.
+
+## ED25519 (RFC 8463) SUPPORT
+
+As of version 0.7, experimental signing and verifying of DKIM Ed25519
+signatures is supported as described in draft-ietf-dcrup-dkim-crypto:
+
+https://datatracker.ietf.org/doc/draft-ietf-dcrup-dkim-crypto/
+
+The RFC that documents ed25519 DKIM signatures, RFC 8463, has been released
+and dkimpy 0.7 and later are aligned to its requirements.  As of 0.8, ed25519
+need not be considered experimental.  The dkimpy implementation has
+successfully interoperated with three other implementations and the technical
+parameters for ed25519-sha256 are defined and stable.
+
+To install from pypi with the required optional depenencies, use the ed25519
+option:
+
+```pip install -e '.[ed25519]'```
+
+## DKIM SCRIPTS
+
+Three helper programs are also supplied: dknewkey, dkimsign and
+dkimverify
+
+dknewkey is s script that produces private and public key pairs suitable
+for use with DKIM.  Note that the private key file format used for ed25519 is
+not standardized (there is no standard) and is unique to dkimpy.  Creation of
+keys should be done in a secure environment.  If an unauthorized entity gains
+access to current private keys they can generate signed email that will pass
+DKIM checkes and will be difficult to repudiate.
+
+dkimsign is a filter that reads an RFC822 message on standard input, and
+writes the same message on standard output with a DKIM-Signature line
+prepended. The signing options are specified on the command line:
+
+dkimsign selector domain privatekeyfile [identity]
+
+The identity is optional and defaults to "@domain".
+
+dkimverify reads an RFC822 message on standard input, and returns with exit
+code 0 if the signature verifies successfully. Otherwise, it returns with exit
+code 1. 
+
+## ARC (Authenticated Receive Chain)
+
+As of version 0.6.0, dkimpy provides experimental support for ARC (Authenticated
+Received Chain).  See RFC 8617 for the current version of ARC:
+
+https://tools.ietf.org/html/rfc8617
+
+In addition to arcsign and arcverify, the dkim module now provides
+arc_sign and arc_verify functions as well as an ARC class.
+
+If an invalid authentication results header field is included in the set for
+ARC, it is ignored and no error is raised.
+
+Both DKIM ed25519 and ARC are now considered stable (no longer experimantal).
+
+## ASYNC SUPPORT
+
+As of version 1.0, an alternative to dkim.verify for use in an async
+environment is provied.  It requires aiodns, https://pypi.org/project/aiodns/.
+Here is a simple example of dkim.verify_async usage:
+
+```python
+>>> sys.stdin = sys.stdin.detach()
+>>>
+>>> async def main():
+>>>     res = await dkim.verify_async(message)
+>>>     return res
+>>>
+>>> if __name__ == "__main__":
+>>>     res = asyncio.run(main())
+```
+
+This feature requires python3.5 or newer.
+
+If aiodns is available, the async functions will be used.  To avoide async
+when aiodns is availale, set dkim.USE_ASYNC = False.
+
+## TLSRPT (TLS Report)
+
+As of version 1.0, the RFC 8460 tlsrpt service type is supported:
+
+https://tools.ietf.org/html/rfc8460
+
+A non-tlsrpt signed with a key record with s=tlsrpt won't verify.  Since the
+service type (s=) is optional in the DKIM public key record, it is not
+required by RFC 8460.  When checking for a tlsrpt signature, set the tlsrpt=
+flag when verifying the signature:
+
+```python
+>>> res = dkim.verify(smessage, tlsrpt='strict')
+```
+
+If tlsrpt='strict', only public key records with s=tlsrpt will be considered
+valid.  If set to tlsrpt=True, the service type is not required, but other
+RFC 8460 requirements are applied.
+
+# LIMITATIONS
+
+Dkimpy will correctly sign/verify messages with ASCII or UTF-8 content.
+Messages that contain other types of content will not verify correctly.  It
+does not yet implement RFC 8616, Email Authentication for Internationalized
+Mail.
+
+# FEEDBACK
+
+Bug reports may be submitted to the bug tracker for the dkimpy project on
+launchpad.
```

### Comparing `dkimpy-1.1.5/dkimpy.egg-info/SOURCES.txt` & `dkimpy-1.1.6/dkimpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/man/arcsign.1` & `dkimpy-1.1.6/man/arcsign.1`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/man/arcverify.1` & `dkimpy-1.1.6/man/arcverify.1`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/man/dkimsign.1` & `dkimpy-1.1.6/man/dkimsign.1`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/man/dkimverify.1` & `dkimpy-1.1.6/man/dkimverify.1`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/man/dknewkey.1` & `dkimpy-1.1.6/man/dknewkey.1`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.5/setup.py` & `dkimpy-1.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # This has been modified from the original software.
 # Copyright (c) 2011,2012,2018 Scott Kitterman <scott@kitterman.com>
 
 from setuptools import setup
 import os
 import sys
 
-version = "1.1.5"
+version = "1.1.6"
 
 kw = {}  # Work-around for lack of 'or' requires in setuptools.
 try:
     import DNS
     kw['install_requires'] = ['Py3DNS']
 except ImportError:  # If PyDNS is not installed, prefer dnspython
     kw['install_requires'] = ['dnspython>=2.0.0']
```


# Comparing `tmp/hashcat-5.1.0.post2.tar.gz` & `tmp/hashcat-5.1.0.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hashcat-5.1.0.post2.tar", last modified: Thu Jan 16 03:46:01 2020, max compression
+gzip compressed data, was "dist/hashcat-5.1.0.post3.tar", last modified: Fri Jan 17 23:47:13 2020, max compression
```

## Comparing `hashcat-5.1.0.post2.tar` & `hashcat-5.1.0.post3.tar`

### file list

```diff
@@ -1,1071 +1,1071 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/
--rw-rw-r--   0 user      (1000) user      (1000)      849 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)       38 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/setup.cfg
--rwxrwxr-x   0 user      (1000) user      (1000)     1452 2020-01-16 03:43:29.000000 hashcat-5.1.0.post2/setup.py
--rwxrwxr-x   0 user      (1000) user      (1000)      113 2020-01-16 03:43:56.000000 hashcat-5.1.0.post2/MANIFEST.in
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-01-16 03:43:29.000000 hashcat-5.1.0.post2/hashcat/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      533 2020-01-16 03:43:29.000000 hashcat-5.1.0.post2/hashcat/cli.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/
--rw-r--r--   0 user      (1000) user      (1000)   240526 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/hashcat.hcstat2
--rw-r--r--   0 user      (1000) user      (1000)   853504 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/hashcat64.exe
--rw-r--r--   0 user      (1000) user      (1000)       58 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/example500.cmd
--rw-r--r--   0 user      (1000) user      (1000)  1069601 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/example.dict
--rw-r--r--   0 user      (1000) user      (1000)       65 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/example400.cmd
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/masks/
--rw-r--r--   0 user      (1000) user      (1000)   443104 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/masks/rockyou-7-2592000.hcmask
--rw-r--r--   0 user      (1000) user      (1000)    42746 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/masks/rockyou-2-1800.hcmask
--rw-r--r--   0 user      (1000) user      (1000)    11004 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/masks/rockyou-1-60.hcmask
--rw-r--r--   0 user      (1000) user      (1000)   121300 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/masks/rockyou-4-43200.hcmask
--rw-r--r--   0 user      (1000) user      (1000)   444816 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/masks/8char-1l-1u-1d-1s-noncompliant.hcmask
--rw-r--r--   0 user      (1000) user      (1000)   734832 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/masks/8char-1l-1u-1d-1s-compliant.hcmask
--rw-r--r--   0 user      (1000) user      (1000)   171648 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/masks/rockyou-5-86400.hcmask
--rw-r--r--   0 user      (1000) user      (1000)   296002 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/masks/rockyou-6-864000.hcmask
--rw-r--r--   0 user      (1000) user      (1000)    58670 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/masks/rockyou-3-3600.hcmask
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/extra/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/extra/tab_completion/
--rwxr-xr-x   0 user      (1000) user      (1000)     2942 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/extra/tab_completion/install
--rw-r--r--   0 user      (1000) user      (1000)      105 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/extra/tab_completion/howto.txt
--rwxr-xr-x   0 user      (1000) user      (1000)    24446 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/extra/tab_completion/hashcat.sh
--rw-r--r--   0 user      (1000) user      (1000)       69 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/example0.cmd
--rw-r--r--   0 user      (1000) user      (1000)   867840 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/hashcat32.exe
--rwxr-xr-x   0 user      (1000) user      (1000)       58 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/example400.sh
--rwxr-xr-x   0 user      (1000) user      (1000)       52 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/example500.sh
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/docs/
--rw-r--r--   0 user      (1000) user      (1000)      258 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/docs/performance.txt
--rw-r--r--   0 user      (1000) user      (1000)     1106 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/docs/license.txt
--rw-r--r--   0 user      (1000) user      (1000)      191 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/docs/user_manuals.txt
--rw-r--r--   0 user      (1000) user      (1000)     2617 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/docs/team.txt
--rw-r--r--   0 user      (1000) user      (1000)     2081 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/docs/credits.txt
--rw-r--r--   0 user      (1000) user      (1000)     6950 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/docs/readme.txt
--rw-r--r--   0 user      (1000) user      (1000)    63603 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/docs/changes.txt
--rw-r--r--   0 user      (1000) user      (1000)     5004 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/docs/rules.txt
--rw-r--r--   0 user      (1000) user      (1000)      185 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/docs/status_codes.txt
--rw-r--r--   0 user      (1000) user      (1000)       50 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/docs/contact.txt
--rw-r--r--   0 user      (1000) user      (1000)     2249 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/docs/limits.txt
--rw-r--r--   0 user      (1000) user      (1000)   214302 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/example0.hash
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/layouts/
--rw-r--r--   0 user      (1000) user      (1000)      495 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/layouts/de.hckmap
--rw-r--r--   0 user      (1000) user      (1000)      475 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/layouts/us.hckmap
--rwxr-xr-x   0 user      (1000) user      (1000)  1000844 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/hashcat32.bin
--rwxr-xr-x   0 user      (1000) user      (1000)   854072 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/hashcat64.bin
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/English/
--rw-r--r--   0 user      (1000) user      (1000)        2 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/English/en_cp1252.hcchr
--rw-r--r--   0 user      (1000) user      (1000)        1 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/English/en_ISO-8859-1.hcchr
--rw-r--r--   0 user      (1000) user      (1000)        2 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/English/en_ISO-8859-15.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/GreekPolytonic/
--rw-r--r--   0 user      (1000) user      (1000)       70 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/GreekPolytonic/el_polytonic_cp1253.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       70 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/GreekPolytonic/el_polytonic_ISO-8859-7.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Bulgarian/
--rw-r--r--   0 user      (1000) user      (1000)       60 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Bulgarian/bg_KOI8-R.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       60 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Bulgarian/bg_ISO-8859-5.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       61 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Bulgarian/bg_cp1251.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Russian/
--rw-r--r--   0 user      (1000) user      (1000)       67 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Russian/ru_cp1251.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       66 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Russian/ru_KOI8-R.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       67 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Russian/ru_ISO-8859-5.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Greek/
--rw-r--r--   0 user      (1000) user      (1000)       50 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Greek/el_ISO-8859-7.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       50 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Greek/el_cp1253.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Slovak/
--rw-r--r--   0 user      (1000) user      (1000)       35 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Slovak/sk_cp1250.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       34 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Slovak/sk_ISO-8859-2.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Lithuanian/
--rw-r--r--   0 user      (1000) user      (1000)       19 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Lithuanian/lt_cp1257.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       18 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Lithuanian/lt_ISO-8859-13.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       18 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Lithuanian/lt_ISO-8859-4.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Spanish/
--rw-r--r--   0 user      (1000) user      (1000)       27 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Spanish/es_ISO-8859-15.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       26 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Spanish/es_ISO-8859-1.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       27 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Spanish/es_cp1252.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Portuguese/
--rw-r--r--   0 user      (1000) user      (1000)       27 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Portuguese/pt_cp1252.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       26 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Portuguese/pt_ISO-8859-1.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       27 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Portuguese/pt_ISO-8859-15.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Castilian/
--rw-r--r--   0 user      (1000) user      (1000)       17 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Castilian/es-ES_ISO-8859-15.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       17 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Castilian/es-ES_cp1252.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Castilian/es-ES_ISO-8859-1.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/French/
--rw-r--r--   0 user      (1000) user      (1000)       35 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/French/fr_ISO-8859-15.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       35 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/French/fr_cp1252.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       33 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/French/fr_ISO-8859-16.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       31 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/French/fr_ISO-8859-1.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/German/
--rw-r--r--   0 user      (1000) user      (1000)        7 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/German/de_ISO-8859-1.hcchr
--rw-r--r--   0 user      (1000) user      (1000)        8 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/German/de_cp1252.hcchr
--rw-r--r--   0 user      (1000) user      (1000)        8 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/German/de_ISO-8859-15.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Hungarian/
--rw-r--r--   0 user      (1000) user      (1000)       18 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Hungarian/hu_cp1250.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Catalan/
--rw-r--r--   0 user      (1000) user      (1000)       23 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Catalan/ca_ISO-8859-15.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       22 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Catalan/ca_ISO-8859-1.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       23 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Catalan/ca_cp1252.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Italian/
--rw-r--r--   0 user      (1000) user      (1000)       21 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Italian/it_ISO-8859-15.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       21 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Italian/it_cp1252.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       20 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Italian/it_ISO-8859-1.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Polish/
--rw-r--r--   0 user      (1000) user      (1000)       18 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Polish/pl_ISO-8859-2.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       18 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/standard/Polish/pl_cp1250.hcchr
--rwxr-xr-x   0 user      (1000) user      (1000)      256 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/DES_full.charset
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/combined/
--rw-r--r--   0 user      (1000) user      (1000)       85 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/combined/Russian.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       28 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/combined/Catalan.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       80 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/combined/Bulgarian.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       12 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/combined/German.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       32 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/combined/Spanish.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       72 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/combined/GreekPolytonic.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       47 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/combined/Slovak.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       35 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/combined/Portuguese.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       25 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/combined/Polish.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       33 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/combined/Lithuanian.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       45 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/combined/French.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       26 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/combined/Italian.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       72 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/combined/Greek.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       22 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/combined/Castilian.hcchr
--rw-r--r--   0 user      (1000) user      (1000)        3 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/combined/English.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/DES_special/
--rw-r--r--   0 user      (1000) user      (1000)       36 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/DES_special/DES_alpha.charset
--rw-r--r--   0 user      (1000) user      (1000)      100 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/DES_special/DES_numeral.charset
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/DES_special/multiple_nodes/
--rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_0.charset
--rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_C.charset
--rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_5.charset
--rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_B.charset
--rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_F.charset
--rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_8.charset
--rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_9.charset
--rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_7.charset
--rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_A.charset
--rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_3.charset
--rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_D.charset
--rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_E.charset
--rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_6.charset
--rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_1.charset
--rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_4.charset
--rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_2.charset
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Russian/
--rw-r--r--   0 user      (1000) user      (1000)       69 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Russian/ru_cp1251-special.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       68 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Russian/ru_ISO-8859-5-special.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Greek/
--rw-r--r--   0 user      (1000) user      (1000)       70 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Greek/el_cp1253-special.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       70 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Greek/el_ISO-8859-7-special.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Slovak/
--rw-r--r--   0 user      (1000) user      (1000)       38 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Slovak/sk_ISO-8859-2-special.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       39 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Slovak/sk_cp1250-special.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Spanish/
--rw-r--r--   0 user      (1000) user      (1000)       30 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Spanish/es_ISO-8859-1-special.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       31 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Spanish/es_cp1252-special.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       29 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Spanish/es_ISO-8859-15-special.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Portuguese/
--rw-r--r--   0 user      (1000) user      (1000)       33 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Portuguese/pt_ISO-8859-1-special.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       34 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Portuguese/pt_cp1252-special.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       32 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Portuguese/pt_ISO-8859-15-special.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Castilian/
--rw-r--r--   0 user      (1000) user      (1000)       21 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Castilian/es-ES_cp1252-special.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       20 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Castilian/es-ES_ISO-8859-1-special.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       19 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Castilian/es-ES_ISO-8859-15-special.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/French/
--rw-r--r--   0 user      (1000) user      (1000)       39 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/French/fr_ISO-8859-15-special.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       37 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/French/fr_ISO-8859-1-special.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       41 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/French/fr_cp1252-special.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       36 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/French/fr_ISO-8859-16-special.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/German/
--rw-r--r--   0 user      (1000) user      (1000)       11 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/German/de_ISO-8859-15-special.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       11 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/German/de_cp1252-special.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       10 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/German/de_ISO-8859-1-special.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Catalan/
--rw-r--r--   0 user      (1000) user      (1000)       25 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Catalan/ca_ISO-8859-15-special.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       26 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Catalan/ca_ISO-8859-1-special.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       27 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Catalan/ca_cp1252-special.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Italian/
--rw-r--r--   0 user      (1000) user      (1000)       25 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Italian/it_cp1252-special.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       24 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Italian/it_ISO-8859-15-special.hcchr
--rw-r--r--   0 user      (1000) user      (1000)       24 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Italian/it_ISO-8859-1-special.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Polish/
--rw-r--r--   0 user      (1000) user      (1000)       19 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/charsets/special/Polish/pl_cp1250-special.hcchr
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/
--rw-r--r--   0 user      (1000) user      (1000)   234289 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/d3ad0ne.rule
--rw-r--r--   0 user      (1000) user      (1000)     1536 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/oscommerce.rule
--rw-r--r--   0 user      (1000) user      (1000)     1774 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/specific.rule
--rw-r--r--   0 user      (1000) user      (1000)      690 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/toggles2.rule
--rw-r--r--   0 user      (1000) user      (1000)   887155 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/dive.rule
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/
--rw-r--r--   0 user      (1000) user      (1000)       40 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_d.rule
--rw-r--r--   0 user      (1000) user      (1000)       64 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_hl.rule
--rw-r--r--   0 user      (1000) user      (1000)      135 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_s_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      276 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_dus.rule
--rw-r--r--   0 user      (1000) user      (1000)      132 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_s.rule
--rw-r--r--   0 user      (1000) user      (1000)      144 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_ld.rule
--rw-r--r--   0 user      (1000) user      (1000)       64 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_hu.rule
--rw-r--r--   0 user      (1000) user      (1000)      251 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_ldu_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      279 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_lds_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      279 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_dus_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)       40 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_d.rule
--rw-r--r--   0 user      (1000) user      (1000)      211 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_lu_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      340 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_lus.rule
--rw-r--r--   0 user      (1000) user      (1000)      248 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_ldu.rule
--rw-r--r--   0 user      (1000) user      (1000)      340 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_lus.rule
--rw-r--r--   0 user      (1000) user      (1000)      236 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_ls.rule
--rw-r--r--   0 user      (1000) user      (1000)       67 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_hu_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)       67 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_hl_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)       64 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_hl.rule
--rw-r--r--   0 user      (1000) user      (1000)      104 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_l.rule
--rw-r--r--   0 user      (1000) user      (1000)      147 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_du_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)       67 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_hu_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      248 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_ldu.rule
--rw-r--r--   0 user      (1000) user      (1000)      104 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_u.rule
--rw-r--r--   0 user      (1000) user      (1000)       67 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_hl_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      107 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_l_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      343 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_lus_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      172 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_ds.rule
--rw-r--r--   0 user      (1000) user      (1000)       43 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_d_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      276 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_dus.rule
--rw-r--r--   0 user      (1000) user      (1000)      239 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_ls_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      135 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_s_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      144 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_du.rule
--rw-r--r--   0 user      (1000) user      (1000)      175 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_ds_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      107 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_u_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      276 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_lds.rule
--rw-r--r--   0 user      (1000) user      (1000)      383 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_ldus_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      104 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_u.rule
--rw-r--r--   0 user      (1000) user      (1000)      147 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_du_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      239 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_us_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      236 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_ls.rule
--rw-r--r--   0 user      (1000) user      (1000)      380 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_ldus.rule
--rw-r--r--   0 user      (1000) user      (1000)      211 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_lu_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      172 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_ds.rule
--rw-r--r--   0 user      (1000) user      (1000)       43 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_d_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      236 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_us.rule
--rw-r--r--   0 user      (1000) user      (1000)      239 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_us_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      343 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_lus_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      175 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_ds_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      380 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_ldus.rule
--rw-r--r--   0 user      (1000) user      (1000)      239 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_ls_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      383 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_ldus_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      276 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_lds.rule
--rw-r--r--   0 user      (1000) user      (1000)      107 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_u_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      144 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_du.rule
--rw-r--r--   0 user      (1000) user      (1000)      147 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_ld_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      208 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_lu.rule
--rw-r--r--   0 user      (1000) user      (1000)      279 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_dus_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      132 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_s.rule
--rw-r--r--   0 user      (1000) user      (1000)       64 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_hu.rule
--rw-r--r--   0 user      (1000) user      (1000)      208 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_lu.rule
--rw-r--r--   0 user      (1000) user      (1000)      279 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_lds_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      251 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_ldu_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      104 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_l.rule
--rw-r--r--   0 user      (1000) user      (1000)      236 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_us.rule
--rw-r--r--   0 user      (1000) user      (1000)      147 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/prepend_ld_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)      144 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_ld.rule
--rw-r--r--   0 user      (1000) user      (1000)      107 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/hybrid/append_l_passthrough.rule
--rw-r--r--   0 user      (1000) user      (1000)     4330 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/toggles3.rule
--rw-r--r--   0 user      (1000) user      (1000)    36041 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/T0XlC-insert_top_100_passwords_1_G.rule
--rw-r--r--   0 user      (1000) user      (1000)    42026 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/InsidePro-HashManager.rule
--rw-r--r--   0 user      (1000) user      (1000)      692 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/combinator.rule
--rw-r--r--   0 user      (1000) user      (1000)    92801 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/generated.rule
--rw-r--r--   0 user      (1000) user      (1000)     1035 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/best64.rule
--rw-r--r--   0 user      (1000) user      (1000)    38901 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/T0XlC.rule
--rw-r--r--   0 user      (1000) user      (1000)   324926 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/Incisive-leetspeak.rule
--rw-r--r--   0 user      (1000) user      (1000)    68087 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/T0XlC-insert_00-99_1950-2050_toprules_0_F.rule
--rw-r--r--   0 user      (1000) user      (1000)   116137 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/T0XlCv1.rule
--rw-r--r--   0 user      (1000) user      (1000)    22732 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/InsidePro-PasswordsPro.rule
--rw-r--r--   0 user      (1000) user      (1000)       60 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/toggles1.rule
--rw-r--r--   0 user      (1000) user      (1000)     2510 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/T0XlC-insert_space_and_special_0_F.rule
--rw-r--r--   0 user      (1000) user      (1000)    58419 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/unix-ninja-leetspeak.rule
--rw-r--r--   0 user      (1000) user      (1000)      327 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/leetspeak.rule
--rw-r--r--   0 user      (1000) user      (1000)   331161 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/rockyou-30000.rule
--rw-r--r--   0 user      (1000) user      (1000)   548542 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/generated2.rule
--rw-r--r--   0 user      (1000) user      (1000)    54016 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/toggles5.rule
--rw-r--r--   0 user      (1000) user      (1000)    17980 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/rules/toggles4.rule
--rw-r--r--   0 user      (1000) user      (1000)       35 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/example500.hash
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/
--rw-r--r--   0 user      (1000) user      (1000)    11093 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10100_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2681 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00060_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     6714 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16800-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    13351 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06212-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    14153 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07701_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    13499 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01760_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2347 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00020_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    16374 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07500_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    19150 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18200_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    78718 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_streebog256.cl
--rw-r--r--   0 user      (1000) user      (1000)     2648 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00130_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2367 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01440_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    14595 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00060_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3559 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06100_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    19034 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13100_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     9299 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01450_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    15773 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13752-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    35675 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03100_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    13612 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_veracrypt_xts.cl
--rw-r--r--   0 user      (1000) user      (1000)    27876 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01440_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    16891 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07500_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     8436 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13600-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     8515 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12700-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    22846 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13800_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     7854 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06400-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    15749 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08400_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     5428 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18100_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    11251 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05400_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    42757 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_md4.cl
--rw-r--r--   0 user      (1000) user      (1000)    13254 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14400_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    21795 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08100_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    32084 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04900_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    15991 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17700_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    10960 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13900_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2691 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04900_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2363 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00040_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     6208 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09820_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    24229 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01420_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2478 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00000_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    20099 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00040_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    19783 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05300_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    22137 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09700_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3007 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00110_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2632 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03800_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    14736 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10800_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    16718 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01740_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     7673 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14611-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     4652 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11200_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    20434 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06300-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    23912 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08400_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     7915 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15400_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    30310 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04400_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    14736 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01700_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    18133 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17800_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    78894 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_streebog512.cl
--rw-r--r--   0 user      (1000) user      (1000)     8966 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14700-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     6729 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04010_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    11695 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00060_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     9573 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06500-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2750 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01730_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    18467 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07801_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    17608 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02400_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     8852 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01000_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    32090 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03910_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    59884 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_sha1.cl
--rw-r--r--   0 user      (1000) user      (1000)    32010 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02710_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    14834 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06213-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3019 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00150_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3635 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01750_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    22338 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13900_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    21849 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00140_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3526 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00060_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     5020 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11750_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    27968 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00140_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    17941 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07801_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     4486 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_vendor.cl
--rw-r--r--   0 user      (1000) user      (1000)     2076 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00000_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    36231 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04010_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    22834 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01500_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     7827 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14641-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    18133 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17900_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    10610 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06800-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2843 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01420_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    17344 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13900_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    19879 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16300-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    10592 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05300_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    10330 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11100_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2689 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07300_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    21031 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08000_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    17504 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01730_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    18984 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01760_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    26846 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04010_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     4625 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05600_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     7324 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04010_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    30566 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01420_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3634 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05400_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2406 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01420_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    18083 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_truecrypt_xts.cl
--rw-r--r--   0 user      (1000) user      (1000)    26553 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08700_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    18045 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14400_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3966 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11800_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     6054 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06100_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    20969 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01400_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     4592 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11760_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2734 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15000_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2755 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01730_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2788 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11000_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3261 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07300_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    58619 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04520_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    68008 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_ripemd160.cl
--rw-r--r--   0 user      (1000) user      (1000)    10511 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14900_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     4602 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05600_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    19822 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02410_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     7957 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16400_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    22191 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08000_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2348 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_rp_optimized.h
--rw-r--r--   0 user      (1000) user      (1000)    27257 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02501-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    23138 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00200_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)      558 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/amp_a3.cl
--rw-r--r--   0 user      (1000) user      (1000)    18645 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16100_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    10548 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10420_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2168 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05100_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    13951 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01730_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2789 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16513_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    13513 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10400_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2345 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13800_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     5100 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11760_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     6687 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11400_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2095 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09900_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    17947 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07800_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    24621 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14000_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     8945 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00150_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    11437 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09810_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    14999 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09810_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     7714 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03910_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2109 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00900_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    24120 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16400_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3555 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01450_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    23690 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_cipher_serpent.cl
--rw-r--r--   0 user      (1000) user      (1000)     6656 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04310_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    23691 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04900_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    18091 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00010_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3966 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11700_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     6776 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04700_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     6691 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04310_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    41623 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13500_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3698 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_truecrypt_crc32.cl
--rw-r--r--   0 user      (1000) user      (1000)     7654 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10900-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     9163 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09710_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     4394 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05300_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2654 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01410_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2380 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00120_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     7350 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01600-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    10949 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15400_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     5754 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10410_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    20341 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06231-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     8337 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16600_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    17776 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04800_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    29494 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08500_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     8919 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12600_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    33493 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15300-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    11809 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01800-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    18931 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13771-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    14534 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00010_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    40785 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04500_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    14012 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07500_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     8335 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14623-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    10810 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09710_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    21913 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00120_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    36930 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00300_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2675 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01430_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3041 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01100_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    11817 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02400_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3185 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01760_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    23557 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01600-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3093 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01710_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2135 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01400_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2146 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01400_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     8304 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11500_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    16023 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18000_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    14193 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07700_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3620 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11800_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    26064 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00130_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    99253 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03000_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    55888 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11200_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    14739 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_constants.h
--rw-r--r--   0 user      (1000) user      (1000)     8303 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16400_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     6663 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14643-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)      746 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/amp_a0.cl
--rw-r--r--   0 user      (1000) user      (1000)    18720 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09700_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    29524 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04700_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     8894 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09810_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    13012 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00150_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3874 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05300_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    37721 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04110_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    16971 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10400_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     6894 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04500_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    11911 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11500_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    14194 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05100_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2789 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16512_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    25646 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03710_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2394 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07300_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    13736 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10420_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2505 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01400_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2486 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01720_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    12251 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15600-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2170 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13300_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    25853 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13800_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     9085 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00600_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3089 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00300_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    25687 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01300_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    13159 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13751-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    10974 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08400_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3359 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16513_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     8941 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12900-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    10634 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00000_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     4141 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11850_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    16924 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01750_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     9587 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00160_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    27662 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01420_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3868 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_scalar.cl
--rw-r--r--   0 user      (1000) user      (1000)    33137 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02610_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    17166 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05100_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    30918 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13300_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    21805 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13772-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     6035 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13500_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2109 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00100_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2804 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/markov_le.cl
--rw-r--r--   0 user      (1000) user      (1000)     6003 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06700-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    26941 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14000_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    12328 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09800_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2109 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00000_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    37818 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02500-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3181 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16801-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    47322 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13500_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    10214 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16200-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     5265 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08300_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    10014 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14632-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2478 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00900_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    13071 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01720_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    14754 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00030_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2749 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_rp.h
--rw-r--r--   0 user      (1000) user      (1000)     3602 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00400-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    18123 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08700_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    46831 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_sha224.cl
--rw-r--r--   0 user      (1000) user      (1000)    12326 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17300_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    25640 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11100_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2201 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05100_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    30841 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00100_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    23231 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11000_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    24870 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16000_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     7164 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06300-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    19032 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09900_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2226 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01700_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2810 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04800_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    20762 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01300_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    13366 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01450_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    25346 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00120_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3354 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04800_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     9702 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07500_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2378 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08100_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    25848 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00110_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    11484 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16400_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2724 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00160_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    29217 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09900_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     4592 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11860_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     4639 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11200_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    14675 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00050_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    28870 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11000_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3037 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01450_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    24231 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01300_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    28618 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16000_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    63431 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11700_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     8190 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02810_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    10873 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05100_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    66336 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04520_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2676 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01450_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     6937 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_luks_essiv.cl
--rw-r--r--   0 user      (1000) user      (1000)     3025 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00130_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2725 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16511_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    16243 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08300_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     9272 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16100_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    12358 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17400_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    15979 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06221-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    11558 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18200_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3066 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00060_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3450 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07000_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    15426 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01460_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    41399 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02810_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     9665 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06100_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     9941 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01460_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    10313 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13900_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     4227 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15100-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    12358 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17500_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    30215 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04010_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    10051 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08200-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    70518 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11700_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3893 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12200-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     7749 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02810_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    33779 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04400_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    18516 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01720_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     7749 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03910_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    13875 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13900_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     7472 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03710_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3918 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06100_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     7376 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04520_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     7913 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16600_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    24355 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03800_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    18787 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05600_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    21840 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00100_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    28404 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14100_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    76805 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_sha384.cl
--rw-r--r--   0 user      (1000) user      (1000)     2939 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15500_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2487 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00100_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)  2106344 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_common.cl
--rw-r--r--   0 user      (1000) user      (1000)     2420 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16511_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    29726 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09000-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     8335 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14622-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     5037 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13200-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    44558 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13500_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2723 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01710_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    30566 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01440_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)   107619 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14000_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    77481 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_sha512.cl
--rw-r--r--   0 user      (1000) user      (1000)    96744 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_luks_serpent.cl
--rw-r--r--   0 user      (1000) user      (1000)    21599 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07000_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    11183 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07701_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     6509 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14612-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2335 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01420_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    24050 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03200-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     9811 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10800_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     4501 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05400_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    21650 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08700_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    25540 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08100_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)   123006 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_luks_aes.cl
--rw-r--r--   0 user      (1000) user      (1000)     7868 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11600-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    17026 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01100_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2658 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00150_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2215 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01700_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     9377 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07100-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3705 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01760_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     4141 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11750_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     1001 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/amp_a1.cl
--rw-r--r--   0 user      (1000) user      (1000)    18534 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02410_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    15436 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02400_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    18135 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17600_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    11725 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10410_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3110 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00300_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     8054 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15400_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    17148 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01760_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2746 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01460_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2788 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00020_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    20766 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06223-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    22619 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09900_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    11603 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00050_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    13924 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15700-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     4829 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08300_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    32896 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16600_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    26381 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08500_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    12314 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14400_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     5787 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18100_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2422 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01440_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2617 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00050_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     8440 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14900_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3468 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01100_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    23826 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04310_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    18135 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17400_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     8260 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11300-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    11275 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12300-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    28002 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08100_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    18101 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17300_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    14730 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07801_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    63414 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11800_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2988 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00050_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2588 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00030_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    35638 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05500_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     7326 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04500_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2734 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01710_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    44752 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16600_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    13628 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07701_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2396 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00140_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2415 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01720_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    15282 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05400_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    10326 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10400_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)      260 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02000_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    11807 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08600_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    45206 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_md5.cl
--rw-r--r--   0 user      (1000) user      (1000)     4938 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05600_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     9581 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08600_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    40686 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06900_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    53621 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_cipher_aes.cl
--rw-r--r--   0 user      (1000) user      (1000)    19987 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00900_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    15152 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00150_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)      841 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_comp_multi.cl
--rw-r--r--   0 user      (1000) user      (1000)     2804 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00040_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     4498 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11750_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     6781 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04400_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    12097 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00900_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    24071 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05600_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     9294 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_cipher_kuznyechik.cl
--rw-r--r--   0 user      (1000) user      (1000)     8736 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09400-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2505 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01300_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     7574 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11400_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    23826 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02610_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    11936 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_cipher_camellia.cl
--rw-r--r--   0 user      (1000) user      (1000)     8742 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11100_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    10913 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06211-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    23720 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13773-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    18133 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18000_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    12358 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18000_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    19498 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15000_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    24447 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01440_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    16023 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17600_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    16499 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01730_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    12358 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17600_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     9811 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01700_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    15991 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17300_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     5453 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00200_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     9337 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12600_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3561 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05300_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    18840 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01750_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     7714 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02810_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    18851 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06222-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3319 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15500_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    11216 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18200_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3891 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07000_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2291 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08100_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)      611 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_truecrypt_keyfile.cl
--rw-r--r--   0 user      (1000) user      (1000)    41319 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16600_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    30492 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05800-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    13590 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01460_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    24200 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16100_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)   125526 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01500_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    10327 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08400_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    18516 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01740_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     7773 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07400-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    24762 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15500_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2125 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01000_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    25894 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01400_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    11245 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18200_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2974 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00010_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    17493 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00040_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3537 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00150_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2260 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00020_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    18445 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13300_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    27025 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14100_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    27175 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14400_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     9673 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07500_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     7904 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04520_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    41399 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03910_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    10161 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12800-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    13289 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01740_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2108 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01000_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    16504 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01720_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    10617 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07300_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    29840 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03100_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2766 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04900_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    42234 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06900_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2813 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00120_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     9049 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09820_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    20559 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01100_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2897 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04800_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    32090 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02810_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     7007 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03710_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3047 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01430_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    19218 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08400_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    22170 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16100_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    37738 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05500_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    24890 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05500_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    11706 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09710_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     6357 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04700_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     6509 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14613-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     7213 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04400_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2492 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16512_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    18473 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07800_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    28446 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01410_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    35475 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02810_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)      260 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02000_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    26764 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11000_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     9397 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16100_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    29244 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07400-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    14073 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00000_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     7126 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02610_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    13668 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07700_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2472 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09900_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3121 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01460_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    50061 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_luks_af.cl
--rw-r--r--   0 user      (1000) user      (1000)    21914 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13300_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    11139 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13100_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    19835 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_rp.cl
--rw-r--r--   0 user      (1000) user      (1000)    18154 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09800_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3339 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04900_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    15354 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05600_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    18018 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08000_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     4221 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11860_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2670 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01430_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    19987 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01000_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2305 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00120_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2260 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11000_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3093 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15000_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    66933 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11800_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    12962 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08600_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    18133 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17500_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    19707 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18200_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    16880 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07300_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     7645 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06000_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    28662 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01430_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    20648 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09100-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    46094 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00300_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2942 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15500_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2135 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01300_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2613 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00110_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    27657 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01410_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     7112 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04110_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    25917 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12400-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     6232 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02100-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)   106043 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_whirlpool.cl
--rw-r--r--   0 user      (1000) user      (1000)     2569 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10800_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    29181 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11100_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     7869 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06600-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    22511 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00130_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    10428 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09600-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     6616 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11400_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2556 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00010_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    25156 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07000_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    16499 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01710_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    25278 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00140_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    20794 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15000_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     9257 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00600_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     4493 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00400-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3359 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16512_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    37917 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04400_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    29774 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04110_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    15072 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00160_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    11178 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14631-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    19559 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03800_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     5020 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11850_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    22604 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00500-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    24635 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00010_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     5529 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13500_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    29917 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09700_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    16023 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17500_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    34799 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11100_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2154 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06000_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     9499 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14621-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3375 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07000_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     7784 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04110_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2907 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01720_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    22955 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06232-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    18371 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00100_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    12326 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17700_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    27743 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03000_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3511 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00300_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     7936 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16600_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    12151 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14400_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    25340 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05500_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    24614 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06233-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     4498 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11850_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    66950 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11700_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)      909 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_comp_multi_bs.cl
--rw-r--r--   0 user      (1000) user      (1000)     2645 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00130_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)   124964 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_simd.cl
--rw-r--r--   0 user      (1000) user      (1000)    33461 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00300_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    19079 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15900-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2632 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00110_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    29654 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14100_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    11223 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07700_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    16023 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17400_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    28557 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08500_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    12112 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09720_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    11507 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09820_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2337 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00140_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    37316 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04500_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     6802 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04400_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    11452 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13100_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2151 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13300_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    33269 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04110_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    62218 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04520_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    48474 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_types.cl
--rw-r--r--   0 user      (1000) user      (1000)    27968 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00120_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     8966 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00060_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    27232 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04900_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3101 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01750_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)      259 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_luks_xts.cl
--rw-r--r--   0 user      (1000) user      (1000)     2163 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06000_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    53738 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11200_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    21513 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10700-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     7361 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10420_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    14511 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16400_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    35475 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03910_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)      260 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02000_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     7139 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04110_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     5600 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13500_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    12385 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01000_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     8192 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03910_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    19593 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13100_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    16023 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17800_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    20062 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05400_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     7126 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04310_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    27255 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01500_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    23322 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03000_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3625 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01460_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2569 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01700_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    14648 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07300_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    37701 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04700_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2880 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10300-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    12358 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17800_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     6691 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02610_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    14953 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09720_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2128 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00100_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    33761 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10700-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2605 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00030_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3284 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03800_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    13236 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00160_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    32594 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00130_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    13679 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11500_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2589 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00010_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    27211 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02610_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    32594 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00110_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     8058 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13000-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     7389 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04520_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    30232 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07000_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3022 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01100_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3462 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00050_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3603 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00160_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    18323 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09720_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    21657 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14400_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2719 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03800_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     9731 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10410_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    13731 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01710_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    14985 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02410_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    41319 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02710_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2826 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01760_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    35395 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02710_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    43327 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12600_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    19871 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04800_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     5100 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11860_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    22291 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00110_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    12690 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08300_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2643 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01410_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    47489 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12600_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     6681 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07900-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    27211 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04310_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    32845 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04700_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    10686 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01800-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    17288 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01710_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2925 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01740_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3321 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05200-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    13280 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10800_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    16958 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13400-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2756 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01750_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3620 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11700_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2347 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11000_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2529 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13300_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    10314 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08400_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3611 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11700_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     9739 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06000_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    27657 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01430_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2532 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06000_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    14819 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06100_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    25109 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01430_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    10579 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07500_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     8712 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00900_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    13840 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00020_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3560 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06100_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     4354 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00500-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    15241 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12500-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     8119 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16900-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    15644 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_functions.cl
--rw-r--r--   0 user      (1000) user      (1000)    11234 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18300-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    14064 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00040_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    18101 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17700_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3611 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11800_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    17279 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00020_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    16023 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17900_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     9282 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08900-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    35043 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03710_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     8000 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00050_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    16018 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03800_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    33137 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04310_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2502 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01740_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2816 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/markov_be.cl
--rw-r--r--   0 user      (1000) user      (1000)     3953 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05400_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2831 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00140_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2352 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13800_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     8940 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12600_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2447 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01740_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    44921 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04500_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2990 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00030_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     6322 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04700_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    16734 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13100_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     6318 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10100_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     4221 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11760_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    32542 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15500_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    28629 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05800-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2811 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08100_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     6136 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11200_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    13312 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04800_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    50285 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11200_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    20099 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00020_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     6663 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14642-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     6915 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04500_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     6704 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04010_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     8769 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11100_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2492 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16513_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    15169 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09800_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     7964 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16400_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2226 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10800_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    15506 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01450_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    23140 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00000_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3007 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13800_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    37738 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06900_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     3111 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01730_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    12857 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01750_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     6972 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03710_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    80687 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_rp_optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    14736 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07800_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    18307 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00030_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     4140 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06000_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    16387 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14800-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2564 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05100_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)      315 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_comp_single.cl
--rw-r--r--   0 user      (1000) user      (1000)    46892 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_sha256.cl
--rw-r--r--   0 user      (1000) user      (1000)     2146 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01300_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    14159 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05300_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    24661 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00030_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2076 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00900_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     5274 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11900-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3029 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01410_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2058 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09900_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     9849 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10100_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    10300 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13900_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    16848 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18200_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    10014 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14633-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)   100718 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_luks_twofish.cl
--rw-r--r--   0 user      (1000) user      (1000)    15941 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15000_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    24873 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05500_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     3287 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16511_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    24707 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01100_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     9842 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10500-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    12661 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00600_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    39874 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12600_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    13280 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01700_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    24889 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01410_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     6307 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18100_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     8982 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00200_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2861 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01440_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     6908 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14900_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     7094 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09500-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2215 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10800_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    24438 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01400_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     4832 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08300_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    29463 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13800_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    11534 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08800-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    21209 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15500_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    70501 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11800_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    11110 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13100_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    28349 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_cipher_twofish.cl
--rw-r--r--   0 user      (1000) user      (1000)     3099 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00160_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     9834 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16100_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    12358 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17900_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    24209 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16000_a0-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    17432 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13753-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    33399 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03100_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)      264 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_comp_single_bs.cl
--rw-r--r--   0 user      (1000) user      (1000)     5884 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12000-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    32223 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05500_a0-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     2723 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15000_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2292 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00040_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    17131 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08300_a3-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)    29031 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03710_a1-optimized.cl
--rw-r--r--   0 user      (1000) user      (1000)     6656 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02610_a1-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)     2494 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01000_a3-pure.cl
--rw-r--r--   0 user      (1000) user      (1000)    28242 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/hashcat.hctune
--rw-r--r--   0 user      (1000) user      (1000)       35 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/example400.hash
--rwxr-xr-x   0 user      (1000) user      (1000)       63 2018-12-02 11:01:37.000000 hashcat-5.1.0.post2/hashcat/hashcat/example0.sh
--rw-rw-r--   0 user      (1000) user      (1000)        8 2020-01-16 03:45:58.000000 hashcat-5.1.0.post2/version
--rw-rw-r--   0 user      (1000) user      (1000)      300 2020-01-16 03:43:29.000000 hashcat-5.1.0.post2/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      849 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)        8 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)      150 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)    46063 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)       46 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2020-01-16 03:46:01.000000 hashcat-5.1.0.post2/hashcat.egg-info/dependency_links.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/
+-rw-rw-r--   0 user      (1000) user      (1000)      849 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/setup.cfg
+-rwxrwxr-x   0 user      (1000) user      (1000)     1452 2020-01-17 23:40:32.000000 hashcat-5.1.0.post3/setup.py
+-rwxrwxr-x   0 user      (1000) user      (1000)      113 2020-01-17 23:40:32.000000 hashcat-5.1.0.post3/MANIFEST.in
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-01-17 23:40:32.000000 hashcat-5.1.0.post3/hashcat/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      858 2020-01-17 23:41:46.000000 hashcat-5.1.0.post3/hashcat/cli.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/
+-rw-r--r--   0 user      (1000) user      (1000)   240526 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/hashcat.hcstat2
+-rw-r--r--   0 user      (1000) user      (1000)   853504 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/hashcat64.exe
+-rw-r--r--   0 user      (1000) user      (1000)       58 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/example500.cmd
+-rw-r--r--   0 user      (1000) user      (1000)  1069601 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/example.dict
+-rw-r--r--   0 user      (1000) user      (1000)       65 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/example400.cmd
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/masks/
+-rw-r--r--   0 user      (1000) user      (1000)   443104 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/masks/rockyou-7-2592000.hcmask
+-rw-r--r--   0 user      (1000) user      (1000)    42746 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/masks/rockyou-2-1800.hcmask
+-rw-r--r--   0 user      (1000) user      (1000)    11004 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/masks/rockyou-1-60.hcmask
+-rw-r--r--   0 user      (1000) user      (1000)   121300 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/masks/rockyou-4-43200.hcmask
+-rw-r--r--   0 user      (1000) user      (1000)   444816 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/masks/8char-1l-1u-1d-1s-noncompliant.hcmask
+-rw-r--r--   0 user      (1000) user      (1000)   734832 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/masks/8char-1l-1u-1d-1s-compliant.hcmask
+-rw-r--r--   0 user      (1000) user      (1000)   171648 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/masks/rockyou-5-86400.hcmask
+-rw-r--r--   0 user      (1000) user      (1000)   296002 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/masks/rockyou-6-864000.hcmask
+-rw-r--r--   0 user      (1000) user      (1000)    58670 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/masks/rockyou-3-3600.hcmask
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/extra/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/extra/tab_completion/
+-rwxr-xr-x   0 user      (1000) user      (1000)     2942 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/extra/tab_completion/install
+-rw-r--r--   0 user      (1000) user      (1000)      105 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/extra/tab_completion/howto.txt
+-rwxr-xr-x   0 user      (1000) user      (1000)    24446 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/extra/tab_completion/hashcat.sh
+-rw-r--r--   0 user      (1000) user      (1000)       69 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/example0.cmd
+-rw-r--r--   0 user      (1000) user      (1000)   867840 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/hashcat32.exe
+-rwxr-xr-x   0 user      (1000) user      (1000)       58 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/example400.sh
+-rwxr-xr-x   0 user      (1000) user      (1000)       52 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/example500.sh
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/docs/
+-rw-r--r--   0 user      (1000) user      (1000)      258 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/docs/performance.txt
+-rw-r--r--   0 user      (1000) user      (1000)     1106 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/docs/license.txt
+-rw-r--r--   0 user      (1000) user      (1000)      191 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/docs/user_manuals.txt
+-rw-r--r--   0 user      (1000) user      (1000)     2617 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/docs/team.txt
+-rw-r--r--   0 user      (1000) user      (1000)     2081 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/docs/credits.txt
+-rw-r--r--   0 user      (1000) user      (1000)     6950 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/docs/readme.txt
+-rw-r--r--   0 user      (1000) user      (1000)    63603 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/docs/changes.txt
+-rw-r--r--   0 user      (1000) user      (1000)     5004 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/docs/rules.txt
+-rw-r--r--   0 user      (1000) user      (1000)      185 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/docs/status_codes.txt
+-rw-r--r--   0 user      (1000) user      (1000)       50 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/docs/contact.txt
+-rw-r--r--   0 user      (1000) user      (1000)     2249 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/docs/limits.txt
+-rw-r--r--   0 user      (1000) user      (1000)   214302 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/example0.hash
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/layouts/
+-rw-r--r--   0 user      (1000) user      (1000)      495 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/layouts/de.hckmap
+-rw-r--r--   0 user      (1000) user      (1000)      475 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/layouts/us.hckmap
+-rwxr-xr-x   0 user      (1000) user      (1000)  1000844 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/hashcat32.bin
+-rwxr-xr-x   0 user      (1000) user      (1000)   854072 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/hashcat64.bin
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/English/
+-rw-r--r--   0 user      (1000) user      (1000)        2 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/English/en_cp1252.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)        1 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/English/en_ISO-8859-1.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)        2 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/English/en_ISO-8859-15.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/GreekPolytonic/
+-rw-r--r--   0 user      (1000) user      (1000)       70 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/GreekPolytonic/el_polytonic_cp1253.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       70 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/GreekPolytonic/el_polytonic_ISO-8859-7.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Bulgarian/
+-rw-r--r--   0 user      (1000) user      (1000)       60 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Bulgarian/bg_KOI8-R.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       60 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Bulgarian/bg_ISO-8859-5.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       61 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Bulgarian/bg_cp1251.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Russian/
+-rw-r--r--   0 user      (1000) user      (1000)       67 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Russian/ru_cp1251.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       66 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Russian/ru_KOI8-R.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       67 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Russian/ru_ISO-8859-5.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Greek/
+-rw-r--r--   0 user      (1000) user      (1000)       50 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Greek/el_ISO-8859-7.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       50 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Greek/el_cp1253.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Slovak/
+-rw-r--r--   0 user      (1000) user      (1000)       35 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Slovak/sk_cp1250.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       34 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Slovak/sk_ISO-8859-2.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Lithuanian/
+-rw-r--r--   0 user      (1000) user      (1000)       19 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Lithuanian/lt_cp1257.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       18 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Lithuanian/lt_ISO-8859-13.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       18 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Lithuanian/lt_ISO-8859-4.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Spanish/
+-rw-r--r--   0 user      (1000) user      (1000)       27 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Spanish/es_ISO-8859-15.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       26 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Spanish/es_ISO-8859-1.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       27 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Spanish/es_cp1252.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Portuguese/
+-rw-r--r--   0 user      (1000) user      (1000)       27 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Portuguese/pt_cp1252.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       26 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Portuguese/pt_ISO-8859-1.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       27 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Portuguese/pt_ISO-8859-15.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Castilian/
+-rw-r--r--   0 user      (1000) user      (1000)       17 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Castilian/es-ES_ISO-8859-15.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       17 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Castilian/es-ES_cp1252.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Castilian/es-ES_ISO-8859-1.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/French/
+-rw-r--r--   0 user      (1000) user      (1000)       35 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/French/fr_ISO-8859-15.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       35 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/French/fr_cp1252.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       33 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/French/fr_ISO-8859-16.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       31 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/French/fr_ISO-8859-1.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/German/
+-rw-r--r--   0 user      (1000) user      (1000)        7 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/German/de_ISO-8859-1.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)        8 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/German/de_cp1252.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)        8 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/German/de_ISO-8859-15.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Hungarian/
+-rw-r--r--   0 user      (1000) user      (1000)       18 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Hungarian/hu_cp1250.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Catalan/
+-rw-r--r--   0 user      (1000) user      (1000)       23 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Catalan/ca_ISO-8859-15.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       22 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Catalan/ca_ISO-8859-1.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       23 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Catalan/ca_cp1252.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Italian/
+-rw-r--r--   0 user      (1000) user      (1000)       21 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Italian/it_ISO-8859-15.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       21 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Italian/it_cp1252.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       20 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Italian/it_ISO-8859-1.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Polish/
+-rw-r--r--   0 user      (1000) user      (1000)       18 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Polish/pl_ISO-8859-2.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       18 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/standard/Polish/pl_cp1250.hcchr
+-rwxr-xr-x   0 user      (1000) user      (1000)      256 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/DES_full.charset
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/combined/
+-rw-r--r--   0 user      (1000) user      (1000)       85 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/combined/Russian.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       28 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/combined/Catalan.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       80 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/combined/Bulgarian.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       12 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/combined/German.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       32 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/combined/Spanish.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       72 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/combined/GreekPolytonic.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       47 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/combined/Slovak.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       35 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/combined/Portuguese.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       25 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/combined/Polish.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       33 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/combined/Lithuanian.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       45 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/combined/French.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       26 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/combined/Italian.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       72 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/combined/Greek.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       22 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/combined/Castilian.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)        3 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/combined/English.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/DES_special/
+-rw-r--r--   0 user      (1000) user      (1000)       36 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/DES_special/DES_alpha.charset
+-rw-r--r--   0 user      (1000) user      (1000)      100 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/DES_special/DES_numeral.charset
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/DES_special/multiple_nodes/
+-rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_0.charset
+-rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_C.charset
+-rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_5.charset
+-rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_B.charset
+-rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_F.charset
+-rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_8.charset
+-rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_9.charset
+-rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_7.charset
+-rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_A.charset
+-rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_3.charset
+-rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_D.charset
+-rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_E.charset
+-rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_6.charset
+-rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_1.charset
+-rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_4.charset
+-rw-r--r--   0 user      (1000) user      (1000)       16 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/DES_special/multiple_nodes/DES_portion_2.charset
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Russian/
+-rw-r--r--   0 user      (1000) user      (1000)       69 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Russian/ru_cp1251-special.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       68 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Russian/ru_ISO-8859-5-special.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Greek/
+-rw-r--r--   0 user      (1000) user      (1000)       70 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Greek/el_cp1253-special.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       70 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Greek/el_ISO-8859-7-special.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Slovak/
+-rw-r--r--   0 user      (1000) user      (1000)       38 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Slovak/sk_ISO-8859-2-special.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       39 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Slovak/sk_cp1250-special.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Spanish/
+-rw-r--r--   0 user      (1000) user      (1000)       30 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Spanish/es_ISO-8859-1-special.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       31 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Spanish/es_cp1252-special.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       29 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Spanish/es_ISO-8859-15-special.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Portuguese/
+-rw-r--r--   0 user      (1000) user      (1000)       33 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Portuguese/pt_ISO-8859-1-special.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       34 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Portuguese/pt_cp1252-special.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       32 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Portuguese/pt_ISO-8859-15-special.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Castilian/
+-rw-r--r--   0 user      (1000) user      (1000)       21 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Castilian/es-ES_cp1252-special.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       20 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Castilian/es-ES_ISO-8859-1-special.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       19 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Castilian/es-ES_ISO-8859-15-special.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/French/
+-rw-r--r--   0 user      (1000) user      (1000)       39 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/French/fr_ISO-8859-15-special.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       37 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/French/fr_ISO-8859-1-special.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       41 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/French/fr_cp1252-special.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       36 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/French/fr_ISO-8859-16-special.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/German/
+-rw-r--r--   0 user      (1000) user      (1000)       11 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/German/de_ISO-8859-15-special.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       11 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/German/de_cp1252-special.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       10 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/German/de_ISO-8859-1-special.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Catalan/
+-rw-r--r--   0 user      (1000) user      (1000)       25 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Catalan/ca_ISO-8859-15-special.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       26 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Catalan/ca_ISO-8859-1-special.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       27 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Catalan/ca_cp1252-special.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Italian/
+-rw-r--r--   0 user      (1000) user      (1000)       25 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Italian/it_cp1252-special.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       24 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Italian/it_ISO-8859-15-special.hcchr
+-rw-r--r--   0 user      (1000) user      (1000)       24 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Italian/it_ISO-8859-1-special.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Polish/
+-rw-r--r--   0 user      (1000) user      (1000)       19 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/charsets/special/Polish/pl_cp1250-special.hcchr
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/
+-rw-r--r--   0 user      (1000) user      (1000)   234289 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/d3ad0ne.rule
+-rw-r--r--   0 user      (1000) user      (1000)     1536 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/oscommerce.rule
+-rw-r--r--   0 user      (1000) user      (1000)     1774 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/specific.rule
+-rw-r--r--   0 user      (1000) user      (1000)      690 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/toggles2.rule
+-rw-r--r--   0 user      (1000) user      (1000)   887155 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/dive.rule
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/
+-rw-r--r--   0 user      (1000) user      (1000)       40 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_d.rule
+-rw-r--r--   0 user      (1000) user      (1000)       64 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_hl.rule
+-rw-r--r--   0 user      (1000) user      (1000)      135 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_s_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      276 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_dus.rule
+-rw-r--r--   0 user      (1000) user      (1000)      132 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_s.rule
+-rw-r--r--   0 user      (1000) user      (1000)      144 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_ld.rule
+-rw-r--r--   0 user      (1000) user      (1000)       64 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_hu.rule
+-rw-r--r--   0 user      (1000) user      (1000)      251 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_ldu_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      279 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_lds_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      279 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_dus_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)       40 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_d.rule
+-rw-r--r--   0 user      (1000) user      (1000)      211 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_lu_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      340 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_lus.rule
+-rw-r--r--   0 user      (1000) user      (1000)      248 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_ldu.rule
+-rw-r--r--   0 user      (1000) user      (1000)      340 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_lus.rule
+-rw-r--r--   0 user      (1000) user      (1000)      236 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_ls.rule
+-rw-r--r--   0 user      (1000) user      (1000)       67 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_hu_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)       67 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_hl_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)       64 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_hl.rule
+-rw-r--r--   0 user      (1000) user      (1000)      104 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_l.rule
+-rw-r--r--   0 user      (1000) user      (1000)      147 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_du_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)       67 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_hu_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      248 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_ldu.rule
+-rw-r--r--   0 user      (1000) user      (1000)      104 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_u.rule
+-rw-r--r--   0 user      (1000) user      (1000)       67 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_hl_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      107 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_l_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      343 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_lus_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      172 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_ds.rule
+-rw-r--r--   0 user      (1000) user      (1000)       43 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_d_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      276 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_dus.rule
+-rw-r--r--   0 user      (1000) user      (1000)      239 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_ls_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      135 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_s_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      144 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_du.rule
+-rw-r--r--   0 user      (1000) user      (1000)      175 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_ds_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      107 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_u_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      276 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_lds.rule
+-rw-r--r--   0 user      (1000) user      (1000)      383 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_ldus_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      104 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_u.rule
+-rw-r--r--   0 user      (1000) user      (1000)      147 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_du_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      239 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_us_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      236 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_ls.rule
+-rw-r--r--   0 user      (1000) user      (1000)      380 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_ldus.rule
+-rw-r--r--   0 user      (1000) user      (1000)      211 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_lu_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      172 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_ds.rule
+-rw-r--r--   0 user      (1000) user      (1000)       43 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_d_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      236 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_us.rule
+-rw-r--r--   0 user      (1000) user      (1000)      239 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_us_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      343 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_lus_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      175 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_ds_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      380 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_ldus.rule
+-rw-r--r--   0 user      (1000) user      (1000)      239 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_ls_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      383 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_ldus_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      276 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_lds.rule
+-rw-r--r--   0 user      (1000) user      (1000)      107 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_u_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      144 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_du.rule
+-rw-r--r--   0 user      (1000) user      (1000)      147 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_ld_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      208 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_lu.rule
+-rw-r--r--   0 user      (1000) user      (1000)      279 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_dus_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      132 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_s.rule
+-rw-r--r--   0 user      (1000) user      (1000)       64 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_hu.rule
+-rw-r--r--   0 user      (1000) user      (1000)      208 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_lu.rule
+-rw-r--r--   0 user      (1000) user      (1000)      279 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_lds_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      251 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_ldu_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      104 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_l.rule
+-rw-r--r--   0 user      (1000) user      (1000)      236 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_us.rule
+-rw-r--r--   0 user      (1000) user      (1000)      147 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/prepend_ld_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)      144 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_ld.rule
+-rw-r--r--   0 user      (1000) user      (1000)      107 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/hybrid/append_l_passthrough.rule
+-rw-r--r--   0 user      (1000) user      (1000)     4330 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/toggles3.rule
+-rw-r--r--   0 user      (1000) user      (1000)    36041 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/T0XlC-insert_top_100_passwords_1_G.rule
+-rw-r--r--   0 user      (1000) user      (1000)    42026 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/InsidePro-HashManager.rule
+-rw-r--r--   0 user      (1000) user      (1000)      692 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/combinator.rule
+-rw-r--r--   0 user      (1000) user      (1000)    92801 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/generated.rule
+-rw-r--r--   0 user      (1000) user      (1000)     1035 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/best64.rule
+-rw-r--r--   0 user      (1000) user      (1000)    38901 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/T0XlC.rule
+-rw-r--r--   0 user      (1000) user      (1000)   324926 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/Incisive-leetspeak.rule
+-rw-r--r--   0 user      (1000) user      (1000)    68087 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/T0XlC-insert_00-99_1950-2050_toprules_0_F.rule
+-rw-r--r--   0 user      (1000) user      (1000)   116137 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/T0XlCv1.rule
+-rw-r--r--   0 user      (1000) user      (1000)    22732 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/InsidePro-PasswordsPro.rule
+-rw-r--r--   0 user      (1000) user      (1000)       60 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/toggles1.rule
+-rw-r--r--   0 user      (1000) user      (1000)     2510 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/T0XlC-insert_space_and_special_0_F.rule
+-rw-r--r--   0 user      (1000) user      (1000)    58419 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/unix-ninja-leetspeak.rule
+-rw-r--r--   0 user      (1000) user      (1000)      327 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/leetspeak.rule
+-rw-r--r--   0 user      (1000) user      (1000)   331161 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/rockyou-30000.rule
+-rw-r--r--   0 user      (1000) user      (1000)   548542 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/generated2.rule
+-rw-r--r--   0 user      (1000) user      (1000)    54016 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/toggles5.rule
+-rw-r--r--   0 user      (1000) user      (1000)    17980 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/rules/toggles4.rule
+-rw-r--r--   0 user      (1000) user      (1000)       35 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/example500.hash
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/
+-rw-r--r--   0 user      (1000) user      (1000)    11093 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10100_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2681 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00060_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6714 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16800-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13351 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06212-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14153 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07701_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13499 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01760_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2347 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00020_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    16374 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07500_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    19150 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18200_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    78718 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_streebog256.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2648 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00130_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2367 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01440_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14595 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00060_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3559 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06100_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    19034 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13100_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9299 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01450_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    15773 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13752-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    35675 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03100_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13612 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_veracrypt_xts.cl
+-rw-r--r--   0 user      (1000) user      (1000)    27876 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01440_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    16891 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07500_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8436 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13600-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8515 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12700-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    22846 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13800_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7854 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06400-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    15749 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08400_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     5428 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18100_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11251 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05400_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    42757 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_md4.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13254 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14400_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    21795 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08100_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    32084 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04900_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    15991 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17700_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10960 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13900_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2691 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04900_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2363 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00040_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6208 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09820_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    24229 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01420_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2478 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00000_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    20099 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00040_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    19783 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05300_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    22137 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09700_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3007 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00110_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2632 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03800_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14736 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10800_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    16718 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01740_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7673 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14611-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     4652 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11200_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    20434 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06300-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    23912 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08400_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7915 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15400_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    30310 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04400_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14736 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01700_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18133 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17800_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    78894 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_streebog512.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8966 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14700-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6729 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04010_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11695 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00060_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9573 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06500-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2750 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01730_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18467 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07801_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    17608 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02400_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8852 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01000_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    32090 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03910_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    59884 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_sha1.cl
+-rw-r--r--   0 user      (1000) user      (1000)    32010 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02710_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14834 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06213-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3019 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00150_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3635 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01750_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    22338 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13900_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    21849 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00140_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3526 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00060_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     5020 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11750_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    27968 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00140_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    17941 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07801_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     4486 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_vendor.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2076 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00000_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    36231 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04010_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    22834 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01500_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7827 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14641-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18133 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17900_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10610 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06800-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2843 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01420_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    17344 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13900_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    19879 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16300-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10592 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05300_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10330 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11100_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2689 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07300_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    21031 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08000_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    17504 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01730_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18984 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01760_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    26846 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04010_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     4625 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05600_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7324 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04010_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    30566 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01420_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3634 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05400_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2406 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01420_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18083 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_truecrypt_xts.cl
+-rw-r--r--   0 user      (1000) user      (1000)    26553 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08700_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18045 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14400_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3966 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11800_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6054 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06100_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    20969 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01400_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     4592 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11760_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2734 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15000_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2755 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01730_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2788 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11000_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3261 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07300_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    58619 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04520_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    68008 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_ripemd160.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10511 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14900_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     4602 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05600_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    19822 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02410_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7957 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16400_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    22191 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08000_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2348 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_rp_optimized.h
+-rw-r--r--   0 user      (1000) user      (1000)    27257 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02501-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    23138 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00200_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)      558 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/amp_a3.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18645 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16100_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10548 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10420_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2168 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05100_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13951 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01730_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2789 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16513_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13513 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10400_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2345 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13800_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     5100 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11760_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6687 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11400_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2095 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09900_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    17947 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07800_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    24621 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14000_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8945 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00150_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11437 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09810_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14999 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09810_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7714 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03910_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2109 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00900_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    24120 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16400_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3555 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01450_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    23690 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_cipher_serpent.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6656 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04310_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    23691 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04900_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18091 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00010_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3966 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11700_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6776 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04700_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6691 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04310_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    41623 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13500_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3698 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_truecrypt_crc32.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7654 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10900-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9163 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09710_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     4394 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05300_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2654 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01410_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2380 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00120_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7350 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01600-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10949 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15400_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     5754 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10410_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    20341 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06231-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8337 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16600_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    17776 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04800_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    29494 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08500_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8919 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12600_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    33493 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15300-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11809 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01800-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18931 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13771-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14534 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00010_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    40785 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04500_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14012 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07500_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8335 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14623-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10810 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09710_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    21913 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00120_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    36930 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00300_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2675 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01430_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3041 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01100_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11817 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02400_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3185 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01760_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    23557 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01600-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3093 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01710_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2135 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01400_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2146 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01400_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8304 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11500_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    16023 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18000_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14193 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07700_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3620 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11800_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    26064 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00130_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    99253 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03000_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    55888 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11200_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14739 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_constants.h
+-rw-r--r--   0 user      (1000) user      (1000)     8303 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16400_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6663 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14643-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)      746 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/amp_a0.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18720 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09700_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    29524 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04700_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8894 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09810_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13012 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00150_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3874 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05300_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    37721 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04110_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    16971 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10400_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6894 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04500_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11911 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11500_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14194 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05100_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2789 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16512_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    25646 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03710_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2394 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07300_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13736 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10420_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2505 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01400_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2486 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01720_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    12251 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15600-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2170 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13300_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    25853 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13800_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9085 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00600_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3089 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00300_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    25687 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01300_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13159 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13751-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10974 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08400_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3359 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16513_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8941 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12900-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10634 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00000_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     4141 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11850_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    16924 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01750_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9587 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00160_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    27662 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01420_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3868 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_scalar.cl
+-rw-r--r--   0 user      (1000) user      (1000)    33137 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02610_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    17166 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05100_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    30918 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13300_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    21805 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13772-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6035 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13500_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2109 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00100_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2804 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/markov_le.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6003 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06700-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    26941 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14000_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    12328 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09800_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2109 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00000_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    37818 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02500-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3181 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16801-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    47322 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13500_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10214 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16200-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     5265 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08300_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10014 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14632-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2478 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00900_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13071 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01720_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14754 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00030_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2749 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_rp.h
+-rw-r--r--   0 user      (1000) user      (1000)     3602 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00400-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18123 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08700_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    46831 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_sha224.cl
+-rw-r--r--   0 user      (1000) user      (1000)    12326 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17300_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    25640 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11100_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2201 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05100_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    30841 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00100_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    23231 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11000_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    24870 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16000_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7164 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06300-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    19032 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09900_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2226 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01700_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2810 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04800_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    20762 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01300_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13366 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01450_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    25346 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00120_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3354 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04800_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9702 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07500_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2378 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08100_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    25848 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00110_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11484 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16400_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2724 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00160_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    29217 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09900_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     4592 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11860_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     4639 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11200_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14675 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00050_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    28870 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11000_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3037 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01450_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    24231 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01300_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    28618 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16000_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    63431 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11700_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8190 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02810_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10873 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05100_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    66336 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04520_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2676 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01450_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6937 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_luks_essiv.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3025 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00130_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2725 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16511_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    16243 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08300_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9272 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16100_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    12358 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17400_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    15979 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06221-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11558 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18200_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3066 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00060_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3450 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07000_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    15426 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01460_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    41399 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02810_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9665 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06100_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9941 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01460_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10313 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13900_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     4227 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15100-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    12358 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17500_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    30215 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04010_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10051 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08200-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    70518 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11700_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3893 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12200-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7749 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02810_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    33779 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04400_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18516 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01720_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7749 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03910_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13875 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13900_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7472 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03710_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3918 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06100_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7376 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04520_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7913 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16600_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    24355 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03800_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18787 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05600_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    21840 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00100_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    28404 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14100_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    76805 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_sha384.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2939 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15500_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2487 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00100_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)  2106344 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_common.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2420 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16511_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    29726 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09000-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8335 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14622-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     5037 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13200-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    44558 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13500_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2723 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01710_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    30566 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01440_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)   107619 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14000_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    77481 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_sha512.cl
+-rw-r--r--   0 user      (1000) user      (1000)    96744 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_luks_serpent.cl
+-rw-r--r--   0 user      (1000) user      (1000)    21599 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07000_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11183 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07701_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6509 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14612-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2335 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01420_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    24050 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03200-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9811 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10800_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     4501 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05400_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    21650 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08700_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    25540 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08100_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)   123006 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_luks_aes.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7868 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11600-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    17026 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01100_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2658 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00150_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2215 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01700_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9377 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07100-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3705 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01760_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     4141 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11750_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     1001 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/amp_a1.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18534 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02410_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    15436 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02400_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18135 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17600_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11725 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10410_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3110 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00300_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8054 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15400_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    17148 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01760_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2746 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01460_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2788 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00020_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    20766 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06223-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    22619 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09900_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11603 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00050_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13924 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15700-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     4829 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08300_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    32896 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16600_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    26381 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08500_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    12314 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14400_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     5787 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18100_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2422 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01440_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2617 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00050_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8440 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14900_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3468 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01100_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    23826 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04310_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18135 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17400_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8260 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11300-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11275 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12300-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    28002 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08100_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18101 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17300_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14730 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07801_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    63414 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11800_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2988 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00050_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2588 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00030_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    35638 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05500_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7326 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04500_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2734 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01710_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    44752 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16600_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13628 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07701_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2396 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00140_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2415 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01720_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    15282 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05400_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10326 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10400_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)      260 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02000_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11807 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08600_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    45206 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_md5.cl
+-rw-r--r--   0 user      (1000) user      (1000)     4938 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05600_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9581 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08600_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    40686 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06900_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    53621 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_cipher_aes.cl
+-rw-r--r--   0 user      (1000) user      (1000)    19987 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00900_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    15152 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00150_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)      841 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_comp_multi.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2804 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00040_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     4498 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11750_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6781 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04400_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    12097 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00900_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    24071 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05600_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9294 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_cipher_kuznyechik.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8736 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09400-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2505 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01300_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7574 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11400_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    23826 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02610_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11936 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_cipher_camellia.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8742 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11100_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10913 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06211-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    23720 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13773-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18133 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18000_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    12358 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18000_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    19498 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15000_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    24447 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01440_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    16023 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17600_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    16499 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01730_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    12358 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17600_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9811 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01700_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    15991 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17300_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     5453 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00200_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9337 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12600_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3561 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05300_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18840 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01750_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7714 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02810_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18851 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06222-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3319 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15500_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11216 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18200_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3891 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07000_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2291 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08100_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)      611 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_truecrypt_keyfile.cl
+-rw-r--r--   0 user      (1000) user      (1000)    41319 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16600_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    30492 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05800-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13590 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01460_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    24200 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16100_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)   125526 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01500_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10327 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08400_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18516 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01740_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7773 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07400-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    24762 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15500_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2125 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01000_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    25894 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01400_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11245 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18200_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2974 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00010_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    17493 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00040_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3537 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00150_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2260 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00020_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18445 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13300_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    27025 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14100_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    27175 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14400_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9673 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07500_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7904 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04520_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    41399 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03910_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10161 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12800-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13289 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01740_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2108 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01000_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    16504 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01720_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10617 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07300_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    29840 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03100_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2766 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04900_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    42234 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06900_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2813 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00120_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9049 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09820_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    20559 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01100_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2897 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04800_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    32090 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02810_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7007 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03710_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3047 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01430_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    19218 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08400_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    22170 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16100_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    37738 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05500_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    24890 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05500_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11706 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09710_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6357 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04700_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6509 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14613-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7213 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04400_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2492 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16512_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18473 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07800_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    28446 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01410_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    35475 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02810_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)      260 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02000_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    26764 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11000_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9397 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16100_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    29244 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07400-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14073 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00000_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7126 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02610_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13668 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07700_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2472 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09900_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3121 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01460_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    50061 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_luks_af.cl
+-rw-r--r--   0 user      (1000) user      (1000)    21914 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13300_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11139 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13100_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    19835 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_rp.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18154 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09800_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3339 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04900_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    15354 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05600_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18018 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08000_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     4221 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11860_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2670 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01430_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    19987 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01000_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2305 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00120_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2260 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11000_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3093 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15000_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    66933 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11800_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    12962 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08600_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18133 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17500_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    19707 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18200_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    16880 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07300_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7645 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06000_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    28662 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01430_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    20648 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09100-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    46094 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00300_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2942 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15500_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2135 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01300_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2613 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00110_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    27657 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01410_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7112 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04110_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    25917 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12400-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6232 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02100-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)   106043 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_whirlpool.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2569 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10800_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    29181 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11100_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7869 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06600-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    22511 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00130_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10428 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09600-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6616 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11400_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2556 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00010_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    25156 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07000_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    16499 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01710_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    25278 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00140_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    20794 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15000_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9257 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00600_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     4493 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00400-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3359 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16512_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    37917 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04400_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    29774 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04110_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    15072 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00160_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11178 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14631-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    19559 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03800_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     5020 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11850_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    22604 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00500-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    24635 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00010_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     5529 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13500_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    29917 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09700_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    16023 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17500_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    34799 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11100_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2154 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06000_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9499 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14621-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3375 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07000_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7784 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04110_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2907 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01720_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    22955 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06232-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18371 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00100_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    12326 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17700_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    27743 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03000_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3511 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00300_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7936 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16600_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    12151 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14400_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    25340 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05500_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    24614 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06233-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     4498 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11850_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    66950 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11700_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)      909 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_comp_multi_bs.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2645 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00130_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)   124964 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_simd.cl
+-rw-r--r--   0 user      (1000) user      (1000)    33461 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00300_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    19079 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15900-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2632 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00110_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    29654 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14100_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11223 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07700_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    16023 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17400_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    28557 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08500_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    12112 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09720_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11507 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09820_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2337 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00140_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    37316 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04500_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6802 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04400_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11452 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13100_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2151 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13300_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    33269 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04110_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    62218 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04520_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    48474 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_types.cl
+-rw-r--r--   0 user      (1000) user      (1000)    27968 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00120_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8966 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00060_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    27232 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04900_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3101 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01750_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)      259 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_luks_xts.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2163 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06000_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    53738 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11200_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    21513 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10700-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7361 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10420_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14511 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16400_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    35475 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03910_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)      260 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02000_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7139 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04110_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     5600 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13500_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    12385 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01000_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8192 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03910_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    19593 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13100_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    16023 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17800_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    20062 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05400_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7126 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04310_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    27255 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01500_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    23322 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03000_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3625 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01460_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2569 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01700_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14648 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07300_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    37701 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04700_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2880 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10300-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    12358 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17800_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6691 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02610_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14953 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09720_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2128 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00100_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    33761 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10700-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2605 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00030_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3284 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03800_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13236 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00160_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    32594 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00130_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13679 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11500_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2589 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00010_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    27211 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02610_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    32594 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00110_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8058 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13000-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7389 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04520_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    30232 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07000_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3022 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01100_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3462 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00050_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3603 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00160_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18323 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09720_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    21657 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14400_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2719 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03800_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9731 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10410_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13731 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01710_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14985 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02410_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    41319 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02710_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2826 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01760_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    35395 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02710_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    43327 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12600_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    19871 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04800_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     5100 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11860_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    22291 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00110_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    12690 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08300_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2643 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01410_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    47489 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12600_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6681 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07900-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    27211 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04310_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    32845 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04700_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10686 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01800-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    17288 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01710_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2925 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01740_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3321 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05200-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13280 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10800_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    16958 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13400-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2756 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01750_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3620 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11700_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2347 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11000_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2529 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13300_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10314 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08400_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3611 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11700_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9739 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06000_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    27657 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01430_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2532 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06000_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14819 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06100_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    25109 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01430_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10579 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07500_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8712 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00900_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13840 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00020_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3560 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06100_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     4354 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00500-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    15241 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12500-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8119 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16900-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    15644 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_functions.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11234 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18300-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14064 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00040_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18101 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17700_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3611 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11800_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    17279 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00020_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    16023 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17900_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9282 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08900-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    35043 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03710_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8000 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00050_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    16018 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03800_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    33137 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04310_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2502 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01740_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2816 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/markov_be.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3953 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05400_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2831 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00140_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2352 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13800_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8940 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12600_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2447 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01740_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    44921 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04500_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2990 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00030_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6322 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04700_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    16734 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13100_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6318 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10100_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     4221 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11760_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    32542 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15500_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    28629 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05800-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2811 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08100_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6136 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11200_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13312 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04800_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    50285 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11200_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    20099 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00020_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6663 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14642-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6915 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04500_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6704 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04010_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8769 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11100_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2492 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16513_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    15169 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09800_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7964 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16400_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2226 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10800_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    15506 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01450_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    23140 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00000_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3007 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13800_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    37738 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06900_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3111 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01730_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    12857 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01750_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6972 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03710_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    80687 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_rp_optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14736 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07800_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    18307 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00030_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     4140 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06000_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    16387 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14800-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2564 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05100_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)      315 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_comp_single.cl
+-rw-r--r--   0 user      (1000) user      (1000)    46892 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_sha256.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2146 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01300_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    14159 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05300_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    24661 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00030_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2076 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00900_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     5274 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11900-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3029 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01410_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2058 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09900_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9849 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10100_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10300 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13900_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    16848 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18200_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    10014 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14633-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)   100718 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_luks_twofish.cl
+-rw-r--r--   0 user      (1000) user      (1000)    15941 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15000_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    24873 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05500_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3287 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16511_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    24707 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01100_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9842 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10500-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    12661 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00600_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    39874 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12600_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    13280 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01700_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    24889 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01410_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6307 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18100_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     8982 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00200_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2861 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01440_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6908 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14900_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     7094 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09500-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2215 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10800_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    24438 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01400_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     4832 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08300_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    29463 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13800_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11534 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08800-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    21209 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15500_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    70501 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11800_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    11110 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13100_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    28349 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_cipher_twofish.cl
+-rw-r--r--   0 user      (1000) user      (1000)     3099 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00160_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     9834 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16100_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    12358 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17900_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    24209 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16000_a0-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    17432 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13753-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    33399 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03100_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)      264 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_comp_single_bs.cl
+-rw-r--r--   0 user      (1000) user      (1000)     5884 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12000-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    32223 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05500_a0-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2723 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15000_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2292 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00040_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    17131 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08300_a3-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)    29031 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03710_a1-optimized.cl
+-rw-r--r--   0 user      (1000) user      (1000)     6656 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02610_a1-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)     2494 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01000_a3-pure.cl
+-rw-r--r--   0 user      (1000) user      (1000)    28242 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/hashcat.hctune
+-rw-r--r--   0 user      (1000) user      (1000)       35 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/example400.hash
+-rwxr-xr-x   0 user      (1000) user      (1000)       63 2018-12-02 11:01:37.000000 hashcat-5.1.0.post3/hashcat/hashcat/example0.sh
+-rw-rw-r--   0 user      (1000) user      (1000)        8 2020-01-17 23:43:48.000000 hashcat-5.1.0.post3/version
+-rw-rw-r--   0 user      (1000) user      (1000)      300 2020-01-17 23:40:32.000000 hashcat-5.1.0.post3/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      849 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)        8 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      150 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)    46063 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       46 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2020-01-17 23:47:13.000000 hashcat-5.1.0.post3/hashcat.egg-info/dependency_links.txt
```

### Comparing `hashcat-5.1.0.post2/PKG-INFO` & `hashcat-5.1.0.post3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashcat
-Version: 5.1.0.post2
+Version: 5.1.0.post3
 Summary: Python pip installer for hashcat
 Home-page: https://github.com/bannsec/hashcat
 Author: Michael Bann
 Author-email: self@bannsecurity.com
 License: MIT
 Description: # Overview
         Little wrapper around hashcat so it can be installed via pip. Attempts to also correctly determine which binary you should run and adds `hashcat` to your path.
```

### Comparing `hashcat-5.1.0.post2/setup.py` & `hashcat-5.1.0.post3/setup.py`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/hashcat.hcstat2` & `hashcat-5.1.0.post3/hashcat/hashcat/hashcat.hcstat2`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/hashcat64.exe` & `hashcat-5.1.0.post3/hashcat/hashcat/hashcat64.exe`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/example.dict` & `hashcat-5.1.0.post3/hashcat/hashcat/example.dict`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/masks/rockyou-7-2592000.hcmask` & `hashcat-5.1.0.post3/hashcat/hashcat/masks/rockyou-7-2592000.hcmask`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/masks/rockyou-2-1800.hcmask` & `hashcat-5.1.0.post3/hashcat/hashcat/masks/rockyou-2-1800.hcmask`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/masks/rockyou-1-60.hcmask` & `hashcat-5.1.0.post3/hashcat/hashcat/masks/rockyou-1-60.hcmask`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/masks/rockyou-4-43200.hcmask` & `hashcat-5.1.0.post3/hashcat/hashcat/masks/rockyou-4-43200.hcmask`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/masks/8char-1l-1u-1d-1s-noncompliant.hcmask` & `hashcat-5.1.0.post3/hashcat/hashcat/masks/8char-1l-1u-1d-1s-noncompliant.hcmask`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/masks/8char-1l-1u-1d-1s-compliant.hcmask` & `hashcat-5.1.0.post3/hashcat/hashcat/masks/8char-1l-1u-1d-1s-compliant.hcmask`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/masks/rockyou-5-86400.hcmask` & `hashcat-5.1.0.post3/hashcat/hashcat/masks/rockyou-5-86400.hcmask`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/masks/rockyou-6-864000.hcmask` & `hashcat-5.1.0.post3/hashcat/hashcat/masks/rockyou-6-864000.hcmask`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/masks/rockyou-3-3600.hcmask` & `hashcat-5.1.0.post3/hashcat/hashcat/masks/rockyou-3-3600.hcmask`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/extra/tab_completion/install` & `hashcat-5.1.0.post3/hashcat/hashcat/extra/tab_completion/install`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/extra/tab_completion/hashcat.sh` & `hashcat-5.1.0.post3/hashcat/hashcat/extra/tab_completion/hashcat.sh`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/hashcat32.exe` & `hashcat-5.1.0.post3/hashcat/hashcat/hashcat32.exe`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/docs/license.txt` & `hashcat-5.1.0.post3/hashcat/hashcat/docs/license.txt`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/docs/team.txt` & `hashcat-5.1.0.post3/hashcat/hashcat/docs/team.txt`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/docs/credits.txt` & `hashcat-5.1.0.post3/hashcat/hashcat/docs/credits.txt`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/docs/readme.txt` & `hashcat-5.1.0.post3/hashcat/hashcat/docs/readme.txt`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/docs/changes.txt` & `hashcat-5.1.0.post3/hashcat/hashcat/docs/changes.txt`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/docs/rules.txt` & `hashcat-5.1.0.post3/hashcat/hashcat/docs/rules.txt`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/docs/limits.txt` & `hashcat-5.1.0.post3/hashcat/hashcat/docs/limits.txt`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/example0.hash` & `hashcat-5.1.0.post3/hashcat/hashcat/example0.hash`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/hashcat32.bin` & `hashcat-5.1.0.post3/hashcat/hashcat/hashcat32.bin`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/hashcat64.bin` & `hashcat-5.1.0.post3/hashcat/hashcat/hashcat64.bin`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/rules/d3ad0ne.rule` & `hashcat-5.1.0.post3/hashcat/hashcat/rules/d3ad0ne.rule`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/rules/oscommerce.rule` & `hashcat-5.1.0.post3/hashcat/hashcat/rules/oscommerce.rule`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/rules/specific.rule` & `hashcat-5.1.0.post3/hashcat/hashcat/rules/specific.rule`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/rules/toggles2.rule` & `hashcat-5.1.0.post3/hashcat/hashcat/rules/toggles2.rule`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/rules/dive.rule` & `hashcat-5.1.0.post3/hashcat/hashcat/rules/dive.rule`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/rules/toggles3.rule` & `hashcat-5.1.0.post3/hashcat/hashcat/rules/toggles3.rule`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/rules/T0XlC-insert_top_100_passwords_1_G.rule` & `hashcat-5.1.0.post3/hashcat/hashcat/rules/T0XlC-insert_top_100_passwords_1_G.rule`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/rules/InsidePro-HashManager.rule` & `hashcat-5.1.0.post3/hashcat/hashcat/rules/InsidePro-HashManager.rule`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/rules/combinator.rule` & `hashcat-5.1.0.post3/hashcat/hashcat/rules/combinator.rule`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/rules/generated.rule` & `hashcat-5.1.0.post3/hashcat/hashcat/rules/generated.rule`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/rules/best64.rule` & `hashcat-5.1.0.post3/hashcat/hashcat/rules/best64.rule`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/rules/T0XlC.rule` & `hashcat-5.1.0.post3/hashcat/hashcat/rules/T0XlC.rule`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/rules/Incisive-leetspeak.rule` & `hashcat-5.1.0.post3/hashcat/hashcat/rules/Incisive-leetspeak.rule`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/rules/T0XlC-insert_00-99_1950-2050_toprules_0_F.rule` & `hashcat-5.1.0.post3/hashcat/hashcat/rules/T0XlC-insert_00-99_1950-2050_toprules_0_F.rule`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/rules/T0XlCv1.rule` & `hashcat-5.1.0.post3/hashcat/hashcat/rules/T0XlCv1.rule`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/rules/InsidePro-PasswordsPro.rule` & `hashcat-5.1.0.post3/hashcat/hashcat/rules/InsidePro-PasswordsPro.rule`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/rules/T0XlC-insert_space_and_special_0_F.rule` & `hashcat-5.1.0.post3/hashcat/hashcat/rules/T0XlC-insert_space_and_special_0_F.rule`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/rules/unix-ninja-leetspeak.rule` & `hashcat-5.1.0.post3/hashcat/hashcat/rules/unix-ninja-leetspeak.rule`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/rules/rockyou-30000.rule` & `hashcat-5.1.0.post3/hashcat/hashcat/rules/rockyou-30000.rule`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/rules/generated2.rule` & `hashcat-5.1.0.post3/hashcat/hashcat/rules/generated2.rule`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/rules/toggles5.rule` & `hashcat-5.1.0.post3/hashcat/hashcat/rules/toggles5.rule`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/rules/toggles4.rule` & `hashcat-5.1.0.post3/hashcat/hashcat/rules/toggles4.rule`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10100_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10100_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00060_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00060_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16800-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16800-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06212-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06212-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07701_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07701_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01760_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01760_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00020_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00020_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07500_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07500_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18200_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18200_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_streebog256.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_streebog256.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00130_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00130_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01440_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01440_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00060_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00060_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06100_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06100_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13100_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13100_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01450_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01450_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13752-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13752-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03100_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03100_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_veracrypt_xts.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_veracrypt_xts.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01440_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01440_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07500_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07500_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13600-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13600-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12700-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12700-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13800_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13800_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06400-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06400-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08400_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08400_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18100_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18100_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05400_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05400_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_md4.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_md4.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14400_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14400_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08100_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08100_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04900_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04900_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17700_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17700_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13900_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13900_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04900_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04900_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00040_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00040_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09820_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09820_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01420_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01420_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00000_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00000_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00040_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00040_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05300_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05300_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09700_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09700_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00110_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00110_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03800_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03800_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10800_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10800_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01740_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01740_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14611-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14611-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11200_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11200_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06300-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06300-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08400_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08400_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15400_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15400_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04400_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04400_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01700_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01700_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17800_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17800_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_streebog512.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_streebog512.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14700-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14700-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04010_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04010_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00060_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00060_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06500-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06500-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01730_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01730_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07801_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07801_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02400_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02400_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01000_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01000_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03910_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03910_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_sha1.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_sha1.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02710_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02710_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06213-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06213-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00150_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00150_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01750_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01750_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13900_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13900_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00140_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00140_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00060_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00060_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11750_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11750_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00140_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00140_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07801_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07801_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_vendor.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_vendor.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00000_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00000_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04010_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04010_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01500_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01500_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14641-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14641-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17900_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17900_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06800-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06800-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01420_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01420_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13900_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13900_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16300-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16300-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05300_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05300_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11100_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11100_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07300_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07300_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08000_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08000_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01730_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01730_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01760_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01760_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04010_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04010_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05600_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05600_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04010_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04010_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01420_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01420_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05400_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05400_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01420_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01420_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_truecrypt_xts.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_truecrypt_xts.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08700_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08700_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14400_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14400_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11800_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11800_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06100_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06100_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01400_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01400_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11760_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11760_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15000_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15000_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01730_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01730_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11000_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11000_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07300_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07300_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04520_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04520_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_ripemd160.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_ripemd160.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14900_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14900_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05600_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05600_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02410_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02410_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16400_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16400_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08000_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08000_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_rp_optimized.h` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_rp_optimized.h`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02501-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02501-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00200_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00200_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/amp_a3.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/amp_a3.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16100_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16100_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10420_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10420_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05100_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05100_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01730_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01730_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16513_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16513_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10400_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10400_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13800_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13800_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11760_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11760_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11400_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11400_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09900_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09900_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07800_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07800_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14000_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14000_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00150_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00150_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09810_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09810_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09810_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09810_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03910_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03910_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00900_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00900_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16400_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16400_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01450_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01450_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_cipher_serpent.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_cipher_serpent.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04310_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04310_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04900_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04900_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00010_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00010_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11700_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11700_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04700_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04700_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04310_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04310_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13500_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13500_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_truecrypt_crc32.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_truecrypt_crc32.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10900-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10900-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09710_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09710_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05300_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05300_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01410_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01410_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00120_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00120_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01600-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01600-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15400_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15400_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10410_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10410_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06231-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06231-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16600_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16600_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04800_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04800_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08500_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08500_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12600_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12600_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15300-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15300-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01800-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01800-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13771-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13771-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00010_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00010_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04500_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04500_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07500_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07500_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14623-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14623-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09710_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09710_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00120_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00120_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00300_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00300_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01430_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01430_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01100_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01100_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02400_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02400_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01760_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01760_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01600-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01600-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01710_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01710_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01400_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01400_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01400_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01400_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11500_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11500_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18000_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18000_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07700_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07700_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11800_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11800_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00130_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00130_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03000_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03000_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11200_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11200_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_constants.h` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_constants.h`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16400_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16400_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14643-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14643-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/amp_a0.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/amp_a0.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09700_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09700_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04700_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04700_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09810_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09810_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00150_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00150_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05300_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05300_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04110_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04110_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10400_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10400_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04500_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04500_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11500_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11500_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05100_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05100_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16512_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16512_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03710_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03710_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07300_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07300_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10420_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10420_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01400_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01400_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01720_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01720_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15600-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15600-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13300_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13300_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13800_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13800_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00600_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00600_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00300_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00300_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01300_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01300_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13751-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13751-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08400_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08400_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16513_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16513_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12900-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12900-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00000_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00000_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11850_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11850_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01750_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01750_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00160_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00160_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01420_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01420_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_scalar.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_scalar.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02610_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02610_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05100_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05100_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13300_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13300_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13772-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13772-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13500_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13500_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00100_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00100_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/markov_le.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/markov_le.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06700-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06700-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14000_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14000_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09800_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09800_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00000_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00000_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02500-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02500-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16801-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16801-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13500_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13500_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16200-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16200-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08300_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08300_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14632-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14632-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00900_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00900_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01720_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01720_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00030_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00030_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_rp.h` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_rp.h`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00400-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00400-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08700_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08700_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_sha224.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_sha224.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17300_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17300_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11100_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11100_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05100_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05100_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00100_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00100_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11000_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11000_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16000_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16000_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06300-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06300-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09900_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09900_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01700_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01700_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04800_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04800_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01300_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01300_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01450_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01450_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00120_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00120_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04800_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04800_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07500_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07500_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08100_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08100_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00110_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00110_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16400_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16400_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00160_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00160_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09900_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09900_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11860_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11860_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11200_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11200_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00050_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00050_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11000_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11000_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01450_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01450_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01300_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01300_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16000_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16000_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11700_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11700_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02810_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02810_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05100_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05100_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04520_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04520_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01450_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01450_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_luks_essiv.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_luks_essiv.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00130_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00130_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16511_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16511_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08300_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08300_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16100_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16100_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17400_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17400_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06221-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06221-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18200_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18200_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00060_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00060_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07000_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07000_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01460_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01460_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02810_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02810_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06100_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06100_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01460_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01460_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13900_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13900_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15100-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15100-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17500_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17500_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04010_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04010_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08200-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08200-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11700_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11700_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12200-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12200-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02810_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02810_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04400_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04400_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01720_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01720_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03910_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03910_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13900_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13900_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03710_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03710_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06100_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06100_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04520_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04520_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16600_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16600_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03800_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03800_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05600_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05600_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00100_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00100_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14100_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14100_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_sha384.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_sha384.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15500_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15500_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00100_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00100_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_common.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_common.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16511_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16511_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09000-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09000-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14622-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14622-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13200-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13200-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13500_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13500_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01710_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01710_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01440_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01440_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14000_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14000_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_sha512.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_sha512.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_luks_serpent.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_luks_serpent.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07000_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07000_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07701_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07701_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14612-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14612-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01420_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01420_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03200-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03200-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10800_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10800_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05400_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05400_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08700_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08700_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08100_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08100_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_luks_aes.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_luks_aes.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11600-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11600-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01100_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01100_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00150_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00150_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01700_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01700_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07100-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07100-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01760_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01760_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11750_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11750_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/amp_a1.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/amp_a1.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02410_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02410_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02400_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02400_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17600_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17600_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10410_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10410_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00300_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00300_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15400_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15400_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01760_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01760_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01460_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01460_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00020_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00020_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06223-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06223-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09900_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09900_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00050_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00050_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15700-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15700-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08300_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08300_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16600_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16600_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08500_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08500_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14400_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14400_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18100_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18100_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01440_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01440_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00050_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00050_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14900_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14900_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01100_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01100_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04310_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04310_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17400_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17400_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11300-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11300-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12300-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12300-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08100_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08100_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17300_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17300_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07801_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07801_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11800_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11800_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00050_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00050_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00030_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00030_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05500_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05500_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04500_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04500_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01710_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01710_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16600_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16600_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07701_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07701_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00140_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00140_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01720_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01720_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05400_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05400_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10400_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10400_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08600_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08600_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_md5.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_md5.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05600_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05600_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08600_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08600_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06900_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06900_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_cipher_aes.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_cipher_aes.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00900_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00900_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00150_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00150_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_comp_multi.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_comp_multi.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00040_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00040_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11750_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11750_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04400_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04400_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00900_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00900_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05600_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05600_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_cipher_kuznyechik.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_cipher_kuznyechik.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09400-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09400-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01300_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01300_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11400_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11400_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02610_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02610_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_cipher_camellia.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_cipher_camellia.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11100_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11100_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06211-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06211-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13773-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13773-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18000_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18000_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18000_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18000_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15000_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15000_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01440_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01440_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17600_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17600_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01730_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01730_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17600_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17600_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01700_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01700_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17300_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17300_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00200_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00200_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12600_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12600_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05300_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05300_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01750_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01750_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02810_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02810_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06222-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06222-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15500_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15500_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18200_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18200_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07000_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07000_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08100_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08100_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_truecrypt_keyfile.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_truecrypt_keyfile.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16600_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16600_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05800-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05800-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01460_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01460_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16100_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16100_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01500_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01500_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08400_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08400_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01740_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01740_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07400-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07400-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15500_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15500_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01000_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01000_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01400_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01400_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18200_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18200_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00010_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00010_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00040_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00040_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00150_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00150_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00020_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00020_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13300_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13300_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14100_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14100_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14400_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14400_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07500_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07500_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04520_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04520_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03910_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03910_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12800-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12800-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01740_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01740_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01000_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01000_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01720_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01720_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07300_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07300_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03100_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03100_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04900_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04900_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06900_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06900_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00120_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00120_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09820_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09820_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01100_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01100_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04800_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04800_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02810_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02810_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03710_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03710_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01430_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01430_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08400_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08400_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16100_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16100_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05500_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05500_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05500_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05500_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09710_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09710_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04700_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04700_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14613-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14613-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04400_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04400_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16512_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16512_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07800_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07800_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01410_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01410_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02810_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02810_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11000_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11000_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16100_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16100_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07400-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07400-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00000_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00000_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02610_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02610_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07700_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07700_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09900_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09900_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01460_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01460_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_luks_af.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_luks_af.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13300_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13300_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13100_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13100_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_rp.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_rp.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09800_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09800_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04900_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04900_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05600_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05600_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08000_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08000_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11860_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11860_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01430_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01430_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01000_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01000_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00120_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00120_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11000_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11000_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15000_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15000_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11800_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11800_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08600_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08600_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17500_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17500_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18200_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18200_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07300_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07300_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06000_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06000_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01430_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01430_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09100-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09100-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00300_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00300_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15500_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15500_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01300_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01300_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00110_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00110_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01410_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01410_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04110_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04110_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12400-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12400-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02100-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02100-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_whirlpool.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_whirlpool.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10800_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10800_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11100_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11100_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06600-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06600-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00130_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00130_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09600-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09600-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11400_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11400_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00010_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00010_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07000_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07000_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01710_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01710_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00140_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00140_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15000_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15000_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00600_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00600_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00400-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00400-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16512_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16512_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04400_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04400_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04110_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04110_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00160_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00160_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14631-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14631-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03800_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03800_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11850_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11850_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00500-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00500-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00010_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00010_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13500_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13500_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09700_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09700_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17500_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17500_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11100_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11100_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06000_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06000_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14621-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14621-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07000_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07000_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04110_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04110_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01720_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01720_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06232-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06232-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00100_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00100_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17700_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17700_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03000_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03000_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00300_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00300_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16600_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16600_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14400_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14400_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05500_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05500_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06233-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06233-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11850_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11850_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11700_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11700_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_comp_multi_bs.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_comp_multi_bs.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00130_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00130_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_simd.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_simd.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00300_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00300_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15900-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15900-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00110_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00110_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14100_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14100_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07700_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07700_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17400_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17400_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08500_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08500_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09720_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09720_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09820_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09820_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00140_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00140_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04500_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04500_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04400_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04400_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13100_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13100_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13300_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13300_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04110_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04110_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04520_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04520_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_types.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_types.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00120_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00120_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00060_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00060_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04900_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04900_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01750_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01750_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06000_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06000_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11200_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11200_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10700-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10700-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10420_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10420_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16400_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16400_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03910_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03910_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04110_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04110_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13500_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13500_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01000_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01000_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03910_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03910_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13100_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13100_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17800_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17800_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05400_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05400_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04310_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04310_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01500_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01500_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03000_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03000_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01460_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01460_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01700_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01700_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07300_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07300_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04700_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04700_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10300-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10300-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17800_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17800_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02610_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02610_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09720_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09720_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00100_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00100_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10700-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10700-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00030_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00030_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03800_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03800_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00160_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00160_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00130_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00130_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11500_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11500_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00010_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00010_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02610_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02610_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00110_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00110_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13000-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13000-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04520_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04520_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07000_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07000_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01100_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01100_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00050_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00050_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00160_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00160_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09720_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09720_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14400_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14400_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03800_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03800_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10410_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10410_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01710_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01710_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02410_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02410_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02710_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02710_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01760_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01760_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02710_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02710_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12600_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12600_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04800_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04800_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11860_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11860_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00110_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00110_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08300_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08300_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01410_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01410_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12600_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12600_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07900-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07900-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04310_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04310_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04700_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04700_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01800-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01800-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01710_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01710_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01740_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01740_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05200-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05200-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10800_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10800_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13400-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13400-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01750_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01750_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11700_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11700_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11000_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11000_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13300_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13300_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08400_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08400_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11700_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11700_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06000_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06000_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01430_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01430_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06000_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06000_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06100_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06100_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01430_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01430_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07500_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07500_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00900_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00900_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00020_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00020_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06100_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06100_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00500-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00500-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12500-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12500-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16900-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16900-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_functions.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_functions.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18300-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18300-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00040_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00040_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17700_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17700_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11800_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11800_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00020_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00020_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17900_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17900_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08900-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08900-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03710_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03710_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00050_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00050_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03800_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03800_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04310_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04310_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01740_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01740_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/markov_be.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/markov_be.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05400_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05400_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00140_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00140_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13800_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13800_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12600_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12600_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01740_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01740_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04500_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04500_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00030_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00030_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04700_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04700_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13100_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13100_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10100_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10100_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11760_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11760_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15500_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15500_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05800-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05800-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08100_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08100_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11200_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11200_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04800_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04800_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11200_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11200_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00020_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00020_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14642-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14642-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04500_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04500_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m04010_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m04010_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11100_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11100_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16513_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16513_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09800_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09800_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16400_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16400_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10800_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10800_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01450_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01450_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00000_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00000_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13800_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13800_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06900_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06900_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01730_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01730_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01750_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01750_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03710_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03710_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_rp_optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_rp_optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m07800_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m07800_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00030_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00030_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m06000_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m06000_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14800-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14800-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05100_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05100_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_hash_sha256.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_hash_sha256.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01300_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01300_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05300_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05300_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00030_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00030_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00900_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00900_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11900-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11900-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01410_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01410_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09900_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09900_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10100_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10100_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13900_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13900_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18200_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18200_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14633-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14633-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_luks_twofish.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_luks_twofish.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15000_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15000_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05500_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05500_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16511_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16511_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01100_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01100_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10500-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10500-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00600_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00600_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12600_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12600_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01700_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01700_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01410_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01410_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m18100_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m18100_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00200_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00200_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01440_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01440_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m14900_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m14900_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m09500-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m09500-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m10800_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m10800_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01400_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01400_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08300_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08300_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13800_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13800_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08800-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08800-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15500_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15500_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m11800_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m11800_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13100_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13100_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/inc_cipher_twofish.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/inc_cipher_twofish.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00160_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00160_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16100_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16100_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m17900_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m17900_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m16000_a0-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m16000_a0-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m13753-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m13753-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03100_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03100_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m12000-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m12000-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m05500_a0-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m05500_a0-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m15000_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m15000_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m00040_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m00040_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m08300_a3-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m08300_a3-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m03710_a1-optimized.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m03710_a1-optimized.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m02610_a1-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m02610_a1-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/OpenCL/m01000_a3-pure.cl` & `hashcat-5.1.0.post3/hashcat/hashcat/OpenCL/m01000_a3-pure.cl`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat/hashcat/hashcat.hctune` & `hashcat-5.1.0.post3/hashcat/hashcat/hashcat.hctune`

 * *Files identical despite different names*

### Comparing `hashcat-5.1.0.post2/hashcat.egg-info/PKG-INFO` & `hashcat-5.1.0.post3/hashcat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashcat
-Version: 5.1.0.post2
+Version: 5.1.0.post3
 Summary: Python pip installer for hashcat
 Home-page: https://github.com/bannsec/hashcat
 Author: Michael Bann
 Author-email: self@bannsecurity.com
 License: MIT
 Description: # Overview
         Little wrapper around hashcat so it can be installed via pip. Attempts to also correctly determine which binary you should run and adds `hashcat` to your path.
```

### Comparing `hashcat-5.1.0.post2/hashcat.egg-info/SOURCES.txt` & `hashcat-5.1.0.post3/hashcat.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/ontolocy-0.7.5.tar.gz` & `tmp/ontolocy-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontolocy-0.7.5.tar", last modified: Fri Apr  5 17:53:08 2024, max compression
+gzip compressed data, was "ontolocy-0.7.6.tar", last modified: Sat Apr 13 17:42:24 2024, max compression
```

## Comparing `ontolocy-0.7.5.tar` & `ontolocy-0.7.6.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:08.516383 ontolocy-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-05 17:53:03.000000 ontolocy-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-05 17:53:08.516383 ontolocy-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-05 17:53:03.000000 ontolocy-0.7.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-05 17:53:03.000000 ontolocy-0.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-05 17:53:03.000000 ontolocy-0.7.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-05 17:53:08.516383 ontolocy-0.7.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:08.504383 ontolocy-0.7.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:08.508383 ontolocy-0.7.5/src/ontolocy/
--rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/dataorigin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:08.516383 ontolocy-0.7.5/src/ontolocy/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/actortype.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/asn.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/banner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/campaign.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/capecpattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/cobaltstrikebeacon.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/cobaltstrikewatermark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/controlvalidationtest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/country.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/cpe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/cve.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/cwe.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/cyberharm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/dnsrecord.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/domainname.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/exploit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/intrusionset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/jarmhash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/listeningsocket.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/macaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/mitreattackcampaign.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/mitreattackdatacomponent.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/mitreattackdatasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/mitreattackgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/mitreattackmitigation.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/mitreattacksoftware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/mitreattacktactic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/mitreattacktechnique.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/networkservice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/organisation.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/port.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/sector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/threatactor.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/useraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/models/x509certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/relationship.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:08.516383 ontolocy-0.7.5/src/ontolocy/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/tools/ingester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:08.516383 ontolocy-0.7.5/src/ontolocy/tools/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/tools/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13416 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/tools/parsers/mitre_attack_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/tools/parsers/ontolocy_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-05 17:53:03.000000 ontolocy-0.7.5/src/ontolocy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:08.516383 ontolocy-0.7.5/src/ontolocy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-05 17:53:08.000000 ontolocy-0.7.5/src/ontolocy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-05 17:53:08.000000 ontolocy-0.7.5/src/ontolocy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:53:08.000000 ontolocy-0.7.5/src/ontolocy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 17:53:08.000000 ontolocy-0.7.5/src/ontolocy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-05 17:53:08.000000 ontolocy-0.7.5/src/ontolocy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 17:53:08.000000 ontolocy-0.7.5/src/ontolocy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:08.516383 ontolocy-0.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-05 17:53:03.000000 ontolocy-0.7.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-05 17:53:03.000000 ontolocy-0.7.5/tests/test_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:42:24.109370 ontolocy-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-13 17:42:17.000000 ontolocy-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-13 17:42:24.109370 ontolocy-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-13 17:42:17.000000 ontolocy-0.7.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-13 17:42:17.000000 ontolocy-0.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-13 17:42:17.000000 ontolocy-0.7.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-13 17:42:24.113370 ontolocy-0.7.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:42:24.097370 ontolocy-0.7.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:42:24.101370 ontolocy-0.7.6/src/ontolocy/
+-rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/dataorigin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:42:24.109370 ontolocy-0.7.6/src/ontolocy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/actortype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/asn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/banner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/campaign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/capecpattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/cobaltstrikebeacon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/cobaltstrikewatermark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/controlvalidationtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/country.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/cpe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/cve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/cwe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/cyberharm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/dnsrecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/domainname.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/exploit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/intrusionset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/jarmhash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/listeningsocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/macaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/mitreattackcampaign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/mitreattackdatacomponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/mitreattackdatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/mitreattackgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/mitreattackmitigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/mitreattacksoftware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/mitreattacktactic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/mitreattacktechnique.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/networkservice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/organisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/sector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/threatactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/useraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/models/x509certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/relationship.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:42:24.109370 ontolocy-0.7.6/src/ontolocy/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/tools/ingester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:42:24.109370 ontolocy-0.7.6/src/ontolocy/tools/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/tools/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13416 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/tools/parsers/mitre_attack_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/tools/parsers/ontolocy_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-13 17:42:17.000000 ontolocy-0.7.6/src/ontolocy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:42:24.109370 ontolocy-0.7.6/src/ontolocy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-13 17:42:24.000000 ontolocy-0.7.6/src/ontolocy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-13 17:42:24.000000 ontolocy-0.7.6/src/ontolocy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 17:42:24.000000 ontolocy-0.7.6/src/ontolocy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-13 17:42:24.000000 ontolocy-0.7.6/src/ontolocy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-13 17:42:24.000000 ontolocy-0.7.6/src/ontolocy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 17:42:24.000000 ontolocy-0.7.6/src/ontolocy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:42:24.109370 ontolocy-0.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-13 17:42:17.000000 ontolocy-0.7.6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-13 17:42:17.000000 ontolocy-0.7.6/tests/test_node.py
```

### Comparing `ontolocy-0.7.5/LICENSE` & `ontolocy-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/PKG-INFO` & `ontolocy-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontolocy
-Version: 0.7.5
+Version: 0.7.6
 Summary: A Python package for modeling cybersecurity data in a Neo4j graph database.
 Home-page: https://github.com/ontolocy/ontolocy-lib
 Author: Ontolocy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ontolocy-0.7.5/README.md` & `ontolocy-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/pyproject.toml` & `ontolocy-0.7.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/setup.cfg` & `ontolocy-0.7.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ontolocy
-version = 0.7.5
+version = 0.7.6
 author = Ontolocy
 description = A Python package for modeling cybersecurity data in a Neo4j graph database.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ontolocy/ontolocy-lib
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `ontolocy-0.7.5/src/ontolocy/__init__.py` & `ontolocy-0.7.6/src/ontolocy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,15 @@
     MitreAttackGroup,
     MitreAttackGroupUsesSoftware,
     MitreAttackGroupUsesTechnique,
 )
 from ontolocy.models.mitreattackmitigation import (
     MitreAttackMitigation,
     MitreAttackMitigationDefendsAgainstTechnique,
+    MitreAttackMitigationMapsToControl,
 )
 from ontolocy.models.mitreattacksoftware import (
     MitreAttackSoftware,
     MitreSoftwareUsesTechnique,
 )
 from ontolocy.models.mitreattacktactic import (
     MitreAttackTactic,
@@ -233,14 +234,15 @@
     "MitreCampaignAttributedTo",
     "MitreAttackDataComponent",
     "MitreAttackDataComponentDetectsTechnique",
     "MitreAttackDataSource",
     "MitreAttackDataSourceHasComponent",
     "MitreAttackMitigation",
     "MitreAttackMitigationDefendsAgainstTechnique",
+    "MitreAttackMitigationMapsToControl",
     "MitreAttackGroup",
     "MitreAttackGroupUsesSoftware",
     "MitreAttackGroupUsesTechnique",
     "NetworkService",
     "NetworkServiceRunsOnPort",
     "OpenPortHasJarmHash",
     "OpenPortPresentsBanner",
```

### Comparing `ontolocy-0.7.5/src/ontolocy/cli.py` & `ontolocy-0.7.6/src/ontolocy/cli.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/dataorigin.py` & `ontolocy-0.7.6/src/ontolocy/dataorigin.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/actortype.py` & `ontolocy-0.7.6/src/ontolocy/models/actortype.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/asn.py` & `ontolocy-0.7.6/src/ontolocy/models/asn.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/banner.py` & `ontolocy-0.7.6/src/ontolocy/models/banner.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/campaign.py` & `ontolocy-0.7.6/src/ontolocy/models/campaign.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/capecpattern.py` & `ontolocy-0.7.6/src/ontolocy/models/capecpattern.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/cobaltstrikebeacon.py` & `ontolocy-0.7.6/src/ontolocy/models/cobaltstrikebeacon.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/control.py` & `ontolocy-0.7.6/src/ontolocy/models/control.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/controlvalidationtest.py` & `ontolocy-0.7.6/src/ontolocy/models/controlvalidationtest.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/country.py` & `ontolocy-0.7.6/src/ontolocy/models/country.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/cpe.py` & `ontolocy-0.7.6/src/ontolocy/models/cpe.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/cve.py` & `ontolocy-0.7.6/src/ontolocy/models/cve.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/detection.py` & `ontolocy-0.7.6/src/ontolocy/models/detection.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/dnsrecord.py` & `ontolocy-0.7.6/src/ontolocy/models/dnsrecord.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/domainname.py` & `ontolocy-0.7.6/src/ontolocy/models/domainname.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/exploit.py` & `ontolocy-0.7.6/src/ontolocy/models/exploit.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/host.py` & `ontolocy-0.7.6/src/ontolocy/models/host.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/intrusionset.py` & `ontolocy-0.7.6/src/ontolocy/models/intrusionset.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/ip.py` & `ontolocy-0.7.6/src/ontolocy/models/ip.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/jarmhash.py` & `ontolocy-0.7.6/src/ontolocy/models/jarmhash.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/listeningsocket.py` & `ontolocy-0.7.6/src/ontolocy/models/listeningsocket.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/macaddress.py` & `ontolocy-0.7.6/src/ontolocy/models/macaddress.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/mitreattackcampaign.py` & `ontolocy-0.7.6/src/ontolocy/models/mitreattackcampaign.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/mitreattackdatacomponent.py` & `ontolocy-0.7.6/src/ontolocy/models/mitreattackdatacomponent.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/mitreattackdatasource.py` & `ontolocy-0.7.6/src/ontolocy/models/mitreattackdatasource.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/mitreattackgroup.py` & `ontolocy-0.7.6/src/ontolocy/models/mitreattackgroup.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/mitreattackmitigation.py` & `ontolocy-0.7.6/src/ontolocy/models/mitreattacksoftware.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from pydantic import HttpUrl
 
 from ..node import OntolocyNode
 from ..relationship import OntolocyRelationship
 from .mitreattacktechnique import MitreAttackTechnique
 
 
-class MitreAttackMitigation(OntolocyNode):
+class MitreAttackSoftware(OntolocyNode):
 
     __primaryproperty__: ClassVar[str] = "stix_id"
-    __primarylabel__: ClassVar[str] = "MitreAttackMitigation"
+    __primarylabel__: ClassVar[str] = "MitreAttackSoftware"
 
     stix_id: str
     stix_type: str
     stix_created: datetime
     stix_modified: datetime
     stix_spec_version: str = "2.1"
     stix_revoked: Optional[bool] = False
@@ -23,22 +23,20 @@
     attack_spec_version: str
     attack_version: str
     attack_id: str
     attack_deprecated: Optional[bool] = False
 
     ref_url: HttpUrl
     name: str
-    description: str
+    description: Optional[str] = None
 
 
 #
 # OUTGOING RELATIONSHIPS
 #
 
 
-class MitreAttackMitigationDefendsAgainstTechnique(OntolocyRelationship):
-    source: MitreAttackMitigation
+class MitreSoftwareUsesTechnique(OntolocyRelationship):
+    source: MitreAttackSoftware
     target: MitreAttackTechnique
 
-    __relationshiptype__: ClassVar[
-        str
-    ] = "MITRE_ATTACK_MITIGATION_DEFENDS_AGAINST_TECHNIQUE"
+    __relationshiptype__: ClassVar[str] = "MITRE_SOFTWARE_USES_TECHNIQUE"
```

### Comparing `ontolocy-0.7.5/src/ontolocy/models/mitreattacksoftware.py` & `ontolocy-0.7.6/src/ontolocy/models/mitreattackmitigation.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 from typing import ClassVar, Optional
 
 from pydantic import HttpUrl
 
 from ..node import OntolocyNode
 from ..relationship import OntolocyRelationship
 from .mitreattacktechnique import MitreAttackTechnique
+from .control import Control
 
 
-class MitreAttackSoftware(OntolocyNode):
+class MitreAttackMitigation(OntolocyNode):
 
     __primaryproperty__: ClassVar[str] = "stix_id"
-    __primarylabel__: ClassVar[str] = "MitreAttackSoftware"
+    __primarylabel__: ClassVar[str] = "MitreAttackMitigation"
 
     stix_id: str
     stix_type: str
     stix_created: datetime
     stix_modified: datetime
     stix_spec_version: str = "2.1"
     stix_revoked: Optional[bool] = False
@@ -23,20 +24,31 @@
     attack_spec_version: str
     attack_version: str
     attack_id: str
     attack_deprecated: Optional[bool] = False
 
     ref_url: HttpUrl
     name: str
-    description: Optional[str] = None
+    description: str
 
 
 #
 # OUTGOING RELATIONSHIPS
 #
 
 
-class MitreSoftwareUsesTechnique(OntolocyRelationship):
-    source: MitreAttackSoftware
+class MitreAttackMitigationDefendsAgainstTechnique(OntolocyRelationship):
+    source: MitreAttackMitigation
     target: MitreAttackTechnique
 
-    __relationshiptype__: ClassVar[str] = "MITRE_SOFTWARE_USES_TECHNIQUE"
+    __relationshiptype__: ClassVar[str] = (
+        "MITRE_ATTACK_MITIGATION_DEFENDS_AGAINST_TECHNIQUE"
+    )
+
+
+class MitreAttackMitigationMapsToControl(OntolocyRelationship):
+    source: MitreAttackMitigation
+    target: Control
+
+    __relationshiptype__: ClassVar[str] = (
+        "MITRE_ATTACK_MITIGATION_DEFENDS_AGAINST_TECHNIQUE"
+    )
```

### Comparing `ontolocy-0.7.5/src/ontolocy/models/mitreattacktactic.py` & `ontolocy-0.7.6/src/ontolocy/models/mitreattacktactic.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/mitreattacktechnique.py` & `ontolocy-0.7.6/src/ontolocy/models/mitreattacktechnique.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/networkservice.py` & `ontolocy-0.7.6/src/ontolocy/models/networkservice.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/organisation.py` & `ontolocy-0.7.6/src/ontolocy/models/organisation.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/port.py` & `ontolocy-0.7.6/src/ontolocy/models/port.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/report.py` & `ontolocy-0.7.6/src/ontolocy/models/report.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/sector.py` & `ontolocy-0.7.6/src/ontolocy/models/sector.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/threatactor.py` & `ontolocy-0.7.6/src/ontolocy/models/threatactor.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/useraccount.py` & `ontolocy-0.7.6/src/ontolocy/models/useraccount.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/models/x509certificate.py` & `ontolocy-0.7.6/src/ontolocy/models/x509certificate.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/node.py` & `ontolocy-0.7.6/src/ontolocy/node.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/relationship.py` & `ontolocy-0.7.6/src/ontolocy/relationship.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/tools/ingester.py` & `ontolocy-0.7.6/src/ontolocy/tools/ingester.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/tools/parsers/mitre_attack_parser.py` & `ontolocy-0.7.6/src/ontolocy/tools/parsers/mitre_attack_parser.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/tools/parsers/ontolocy_parser.py` & `ontolocy-0.7.6/src/ontolocy/tools/parsers/ontolocy_parser.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy/utils.py` & `ontolocy-0.7.6/src/ontolocy/utils.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/src/ontolocy.egg-info/PKG-INFO` & `ontolocy-0.7.6/src/ontolocy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontolocy
-Version: 0.7.5
+Version: 0.7.6
 Summary: A Python package for modeling cybersecurity data in a Neo4j graph database.
 Home-page: https://github.com/ontolocy/ontolocy-lib
 Author: Ontolocy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ontolocy-0.7.5/src/ontolocy.egg-info/SOURCES.txt` & `ontolocy-0.7.6/src/ontolocy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/tests/test_cli.py` & `ontolocy-0.7.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.7.5/tests/test_node.py` & `ontolocy-0.7.6/tests/test_node.py`

 * *Files identical despite different names*


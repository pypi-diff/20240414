# Comparing `tmp/keri-1.2.0.dev0.tar.gz` & `tmp/keri-1.2.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keri-1.2.0.dev0.tar", last modified: Sat Apr  6 18:11:53 2024, max compression
+gzip compressed data, was "keri-1.2.0.dev1.tar", last modified: Sat Apr 13 22:53:57 2024, max compression
```

## Comparing `keri-1.2.0.dev0.tar` & `keri-1.2.0.dev1.tar`

### file list

```diff
@@ -1,207 +1,210 @@
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.494755 keri-1.2.0.dev0/
--rw-r--r--   0 pfeairheller   (501) staff       (20)    11357 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/LICENSE
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1565 2024-04-06 18:11:53.494466 keri-1.2.0.dev0/PKG-INFO
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2457 2024-04-05 21:44:00.000000 keri-1.2.0.dev0/README.md
--rw-r--r--   0 pfeairheller   (501) staff       (20)       38 2024-04-06 18:11:53.494793 keri-1.2.0.dev0/setup.cfg
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4020 2024-04-06 18:09:23.000000 keri-1.2.0.dev0/setup.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.460777 keri-1.2.0.dev0/src/
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.463283 keri-1.2.0.dev0/src/keri/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       83 2024-04-06 18:09:23.000000 keri-1.2.0.dev0/src/keri/__init__.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.469911 keri-1.2.0.dev0/src/keri/app/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       58 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    37074 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/agenting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2780 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/apping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1648 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/challenging.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.470282 keri-1.2.0.dev0/src/keri/app/cli/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       62 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/__init__.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.473724 keri-1.2.0.dev0/src/keri/app/cli/commands/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/__init__.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.474225 keri-1.2.0.dev0/src/keri/app/cli/commands/challenge/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/challenge/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1529 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/challenge/generate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4353 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/challenge/respond.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5565 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/challenge/verify.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1847 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/clean.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.474444 keri-1.2.0.dev0/src/keri/app/cli/commands/contacts/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/contacts/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2662 2024-04-05 21:54:29.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/contacts/list.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.475146 keri-1.2.0.dev0/src/keri/app/cli/commands/delegate/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/delegate/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9342 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/delegate/confirm.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4076 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/delegate/request.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.475429 keri-1.2.0.dev0/src/keri/app/cli/commands/did/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/did/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3450 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/did/generate.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.475888 keri-1.2.0.dev0/src/keri/app/cli/commands/ends/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/ends/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4679 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/ends/add.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2873 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/ends/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2566 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/ends/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6291 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/escrow.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3774 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7156 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/incept.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5479 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/init.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3855 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/interact.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.477092 keri-1.2.0.dev0/src/keri/app/cli/commands/ipex/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/ipex/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6651 2024-04-05 21:44:00.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/ipex/admit.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      529 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/ipex/agree.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      470 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/ipex/apply.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6996 2024-04-05 21:44:00.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/ipex/grant.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9834 2024-04-05 21:44:00.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/ipex/join.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9870 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/ipex/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      564 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/ipex/offer.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5584 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/ipex/spurn.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3371 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/kevers.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1402 2023-11-27 19:46:40.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/list.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.477305 keri-1.2.0.dev0/src/keri/app/cli/commands/local/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/local/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9105 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/local/watch.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.477679 keri-1.2.0.dev0/src/keri/app/cli/commands/mailbox/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/mailbox/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4555 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/mailbox/debug.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2554 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/mailbox/update.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.478272 keri-1.2.0.dev0/src/keri/app/cli/commands/migrate/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/migrate/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1938 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/migrate/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1785 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/migrate/run.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1806 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/migrate/show.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6153 2024-04-05 21:44:00.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/migrate.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.480567 keri-1.2.0.dev0/src/keri/app/cli/commands/multisig/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/multisig/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3045 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/multisig/continue.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      735 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/multisig/demo.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6698 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/multisig/incept.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5619 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/multisig/interact.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    30790 2024-04-05 21:44:00.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/multisig/join.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5227 2024-04-05 21:44:00.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/multisig/notice.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10190 2024-04-05 21:44:00.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/multisig/rotate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9500 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/multisig/shell.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4891 2024-04-05 21:54:29.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/multisig/update.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      440 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/nonce.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.481118 keri-1.2.0.dev0/src/keri/app/cli/commands/oobi/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/oobi/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1975 2023-11-27 19:46:40.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/oobi/clean.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3120 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/oobi/generate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3716 2023-11-15 20:54:14.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/oobi/resolve.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.481577 keri-1.2.0.dev0/src/keri/app/cli/commands/passcode/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/passcode/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      662 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/passcode/generate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1521 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/passcode/remove.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2475 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/passcode/set.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3559 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/query.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2161 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/rename.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4044 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/rollback.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8450 2024-04-05 21:21:34.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/rotate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1051 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/saidify.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      528 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/salt.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2140 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/sign.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.481788 keri-1.2.0.dev0/src/keri/app/cli/commands/ssh/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/ssh/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3392 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/ssh/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2284 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/status.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      414 2024-04-05 21:44:00.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/time.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.482421 keri-1.2.0.dev0/src/keri/app/cli/commands/vc/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/vc/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10784 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/vc/create.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5966 2024-03-29 15:29:32.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/vc/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6251 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/vc/list.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.483001 keri-1.2.0.dev0/src/keri/app/cli/commands/vc/registry/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/vc/registry/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7267 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/vc/registry/incept.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1764 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/vc/registry/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3683 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/vc/registry/status.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7517 2024-04-05 21:44:00.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/vc/revoke.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2940 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/verify.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1251 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/version.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.483542 keri-1.2.0.dev0/src/keri/app/cli/commands/witness/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/witness/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3059 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/witness/demo.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4833 2024-04-05 21:21:50.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/witness/start.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3624 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/commands/witness/submit.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.484377 keri-1.2.0.dev0/src/keri/app/cli/common/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/common/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2877 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/common/config.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3887 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/cli/common/displaying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3357 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/cli/common/existing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1783 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/common/incepting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1208 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/common/rotating.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      415 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/cli/common/terming.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      728 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/cli/kli.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8151 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/configing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7632 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/connecting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10240 2024-04-05 21:20:43.000000 keri-1.2.0.dev0/src/keri/app/delegating.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    24676 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/directing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    18769 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/forwarding.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    26589 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/grouping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   124508 2024-04-05 21:21:01.000000 keri-1.2.0.dev0/src/keri/app/habbing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8557 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/httping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    41662 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/app/indirecting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    73666 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/keeping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/kiwiing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    13938 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/notifying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    23097 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/oobiing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4471 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/querying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8400 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/signaling.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5908 2024-04-05 21:44:00.000000 keri-1.2.0.dev0/src/keri/app/signing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1837 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/app/specing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9669 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/app/storing.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.487726 keri-1.2.0.dev0/src/keri/core/
--rw-r--r--   0 pfeairheller   (501) staff       (20)      465 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/core/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   233518 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/core/coring.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    37102 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/core/counting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   305955 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/core/eventing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    34157 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/core/indexing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    58447 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/core/parsing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    26305 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/core/routing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    12848 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/core/scheming.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    80505 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/core/serdering.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.489002 keri-1.2.0.dev0/src/keri/db/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       55 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/db/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   127626 2024-04-05 21:44:00.000000 keri-1.2.0.dev0/src/keri/db/basing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    77257 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/db/dbing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9316 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/db/escrowing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    30476 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/db/koming.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.489521 keri-1.2.0.dev0/src/keri/db/migrations/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/db/migrations/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2861 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/db/migrations/rekey_habs.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    59483 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/db/subing.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.490440 keri-1.2.0.dev0/src/keri/demo/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       59 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/demo/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2794 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/demo/demo_bob.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2811 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/demo/demo_eve.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      932 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/demo/demo_kev.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2836 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/demo/demo_sam.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    16437 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/demo/demoing.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.491025 keri-1.2.0.dev0/src/keri/end/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       73 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/end/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    24903 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/end/ending.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1322 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/end/priming.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.491275 keri-1.2.0.dev0/src/keri/help/
--rw-r--r--   0 pfeairheller   (501) staff       (20)      557 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/help/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    12490 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/help/helping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    27047 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/kering.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.491639 keri-1.2.0.dev0/src/keri/peer/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/peer/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    19472 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/peer/exchanging.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.492422 keri-1.2.0.dev0/src/keri/vc/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       56 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/vc/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10278 2024-04-05 21:44:00.000000 keri-1.2.0.dev0/src/keri/vc/protocoling.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2511 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/vc/proving.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3749 2024-03-12 23:12:35.000000 keri-1.2.0.dev0/src/keri/vc/walleting.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.493404 keri-1.2.0.dev0/src/keri/vdr/
--rw-r--r--   0 pfeairheller   (501) staff       (20)      120 2023-03-20 02:45:25.000000 keri-1.2.0.dev0/src/keri/vdr/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    34269 2024-04-04 13:35:27.000000 keri-1.2.0.dev0/src/keri/vdr/credentialing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    84597 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/vdr/eventing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    14381 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/vdr/verifying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    35856 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/src/keri/vdr/viring.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.494187 keri-1.2.0.dev0/src/keri.egg-info/
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1565 2024-04-06 18:11:53.000000 keri-1.2.0.dev0/src/keri.egg-info/PKG-INFO
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5817 2024-04-06 18:11:53.000000 keri-1.2.0.dev0/src/keri.egg-info/SOURCES.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2024-04-06 18:11:53.000000 keri-1.2.0.dev0/src/keri.egg-info/dependency_links.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)      181 2024-04-06 18:11:53.000000 keri-1.2.0.dev0/src/keri.egg-info/entry_points.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2023-03-20 03:44:29.000000 keri-1.2.0.dev0/src/keri.egg-info/not-zip-safe
--rw-r--r--   0 pfeairheller   (501) staff       (20)      300 2024-04-06 18:11:53.000000 keri-1.2.0.dev0/src/keri.egg-info/requires.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)        5 2024-04-06 18:11:53.000000 keri-1.2.0.dev0/src/keri.egg-info/top_level.txt
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 18:11:53.493768 keri-1.2.0.dev0/tests/
--rw-r--r--   0 pfeairheller   (501) staff       (20)    28418 2024-04-05 21:19:51.000000 keri-1.2.0.dev0/tests/test_kering.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.087839 keri-1.2.0.dev1/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    11357 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/LICENSE
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1594 2024-04-13 22:53:57.087558 keri-1.2.0.dev1/PKG-INFO
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2457 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/README.md
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       38 2024-04-13 22:53:57.087881 keri-1.2.0.dev1/setup.cfg
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4061 2024-04-13 22:43:05.000000 keri-1.2.0.dev1/setup.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.058806 keri-1.2.0.dev1/src/
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.061585 keri-1.2.0.dev1/src/keri/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       83 2024-04-13 22:43:05.000000 keri-1.2.0.dev1/src/keri/__init__.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.067066 keri-1.2.0.dev1/src/keri/app/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       58 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    37921 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/app/agenting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2780 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/apping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1648 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/challenging.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.067447 keri-1.2.0.dev1/src/keri/app/cli/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       62 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/__init__.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.070708 keri-1.2.0.dev1/src/keri/app/cli/commands/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/__init__.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.071277 keri-1.2.0.dev1/src/keri/app/cli/commands/challenge/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/challenge/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1529 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/challenge/generate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4353 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/challenge/respond.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5565 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/challenge/verify.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1847 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/clean.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.071517 keri-1.2.0.dev1/src/keri/app/cli/commands/contacts/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/contacts/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2662 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/contacts/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2074 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/decrypt.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.071877 keri-1.2.0.dev1/src/keri/app/cli/commands/delegate/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/delegate/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9425 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/delegate/confirm.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4076 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/delegate/request.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.072085 keri-1.2.0.dev1/src/keri/app/cli/commands/did/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/did/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3450 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/did/generate.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.072536 keri-1.2.0.dev1/src/keri/app/cli/commands/ends/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ends/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4679 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ends/add.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2873 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ends/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2566 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ends/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6291 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/escrow.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3744 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7156 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/incept.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5479 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/init.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4897 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/interact.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.073878 keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6651 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/admit.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      529 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/agree.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      470 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/apply.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6996 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/grant.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9834 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/join.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9870 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      564 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/offer.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5584 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/spurn.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3371 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/kevers.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1402 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/list.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.074169 keri-1.2.0.dev1/src/keri/app/cli/commands/local/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/local/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9105 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/local/watch.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.074531 keri-1.2.0.dev1/src/keri/app/cli/commands/mailbox/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/mailbox/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4555 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/mailbox/debug.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2554 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/mailbox/update.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.074988 keri-1.2.0.dev1/src/keri/app/cli/commands/migrate/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/migrate/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1938 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/migrate/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1785 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/migrate/run.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1806 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/migrate/show.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6153 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/migrate.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.076326 keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3045 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/continue.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      735 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/demo.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6698 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/incept.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5619 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/interact.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    30790 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/join.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5227 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/notice.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10190 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/rotate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9500 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/shell.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4891 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/update.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      440 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/nonce.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.076781 keri-1.2.0.dev1/src/keri/app/cli/commands/oobi/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/oobi/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1975 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/oobi/clean.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3120 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/oobi/generate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3716 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/oobi/resolve.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.077356 keri-1.2.0.dev1/src/keri/app/cli/commands/passcode/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/passcode/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      662 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/passcode/generate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1521 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/passcode/remove.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2549 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/passcode/set.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3559 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/query.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2161 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/rename.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4044 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/rollback.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8964 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/rotate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1051 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/saidify.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      519 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/salt.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2140 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/sign.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.077559 keri-1.2.0.dev1/src/keri/app/cli/commands/ssh/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ssh/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3392 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ssh/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2284 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/status.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      414 2024-04-05 21:44:00.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/time.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.078118 keri-1.2.0.dev1/src/keri/app/cli/commands/vc/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/vc/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10874 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/vc/create.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5966 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/vc/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6251 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/vc/list.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.078575 keri-1.2.0.dev1/src/keri/app/cli/commands/vc/registry/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/vc/registry/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7267 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/vc/registry/incept.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1764 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/vc/registry/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3683 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/vc/registry/status.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7517 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/vc/revoke.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2940 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/verify.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1251 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/version.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.079117 keri-1.2.0.dev1/src/keri/app/cli/commands/witness/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/witness/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4073 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/witness/authenticate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3047 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/witness/demo.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4836 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/witness/start.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4655 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/witness/submit.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.080134 keri-1.2.0.dev1/src/keri/app/cli/common/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/common/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2877 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/common/config.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3887 2024-04-12 20:57:42.000000 keri-1.2.0.dev1/src/keri/app/cli/common/displaying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3357 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/app/cli/common/existing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1783 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/cli/common/incepting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1208 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/common/rotating.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      415 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/common/terming.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      728 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/cli/kli.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8151 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/app/configing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7632 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/connecting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10242 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/app/delegating.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    24676 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/app/directing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    18769 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/app/forwarding.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    26643 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/app/grouping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   124687 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/app/habbing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8702 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/httping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    41665 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/app/indirecting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    73656 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/keeping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    13938 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/notifying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    23097 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/oobiing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4471 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/querying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8400 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/signaling.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5908 2024-04-05 21:44:00.000000 keri-1.2.0.dev1/src/keri/app/signing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1837 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/specing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9669 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/storing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.081882 keri-1.2.0.dev1/src/keri/core/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      566 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/core/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   202289 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/core/coring.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    37818 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/core/counting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   306732 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/core/eventing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    34157 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/core/indexing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    58295 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/core/parsing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    26820 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/core/routing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    12848 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/core/scheming.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    82877 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/core/serdering.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    35338 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/core/signing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    25640 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/core/structing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.083045 keri-1.2.0.dev1/src/keri/db/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       55 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/db/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   127663 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/db/basing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    77257 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/db/dbing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9359 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/db/escrowing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    30476 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/db/koming.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.083284 keri-1.2.0.dev1/src/keri/db/migrations/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/db/migrations/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2861 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/db/migrations/rekey_habs.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    59458 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/db/subing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.084187 keri-1.2.0.dev1/src/keri/demo/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       59 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/demo/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2790 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/demo/demo_bob.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2806 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/demo/demo_eve.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      932 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/demo/demo_kev.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2831 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/demo/demo_sam.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    16437 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/demo/demoing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.084778 keri-1.2.0.dev1/src/keri/end/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       73 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/end/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    24903 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/end/ending.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1322 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/end/priming.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.085027 keri-1.2.0.dev1/src/keri/help/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      619 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/help/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    12483 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/help/helping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    27047 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/kering.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.085241 keri-1.2.0.dev1/src/keri/peer/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/peer/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    19698 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/peer/exchanging.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.085875 keri-1.2.0.dev1/src/keri/vc/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       56 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/vc/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10278 2024-04-05 21:44:00.000000 keri-1.2.0.dev1/src/keri/vc/protocoling.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2528 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/vc/proving.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3749 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/vc/walleting.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.086749 keri-1.2.0.dev1/src/keri/vdr/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      120 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/vdr/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    34327 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/vdr/credentialing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    84668 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/vdr/eventing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    14424 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/vdr/verifying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    35856 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/vdr/viring.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.087292 keri-1.2.0.dev1/src/keri.egg-info/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1594 2024-04-13 22:53:57.000000 keri-1.2.0.dev1/src/keri.egg-info/PKG-INFO
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5932 2024-04-13 22:53:57.000000 keri-1.2.0.dev1/src/keri.egg-info/SOURCES.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2024-04-13 22:53:57.000000 keri-1.2.0.dev1/src/keri.egg-info/dependency_links.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      181 2024-04-13 22:53:57.000000 keri-1.2.0.dev1/src/keri.egg-info/entry_points.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2023-03-20 03:44:29.000000 keri-1.2.0.dev1/src/keri.egg-info/not-zip-safe
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      314 2024-04-13 22:53:57.000000 keri-1.2.0.dev1/src/keri.egg-info/requires.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        5 2024-04-13 22:53:57.000000 keri-1.2.0.dev1/src/keri.egg-info/top_level.txt
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.086879 keri-1.2.0.dev1/tests/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    28418 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/tests/test_kering.py
```

### Comparing `keri-1.2.0.dev0/LICENSE` & `keri-1.2.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/PKG-INFO` & `keri-1.2.0.dev1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keri
-Version: 1.2.0.dev0
+Version: 1.2.0.dev1
 Summary: Key Event Receipt Infrastructure
 Home-page: https://github.com/WebOfTrust/keripy
 Author: Samuel M. Smith
 Author-email: smith.samuel.m@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://keri.readthedocs.io/
 Project-URL: Changelog, https://keri.readthedocs.io/en/latest/changelog.html
@@ -35,9 +35,10 @@
 Requires-Dist: PyYaml>=6.0.1
 Requires-Dist: apispec>=6.6.0
 Requires-Dist: mnemonic>=0.21
 Requires-Dist: PrettyTable>=3.10.0
 Requires-Dist: http_sfv>=0.9.9
 Requires-Dist: cryptography>=42.0.5
 Requires-Dist: semver>=3.0.2
+Requires-Dist: qrcode>=7.4.2
 
 KERI Decentralized Key Management Infrastructure
```

### Comparing `keri-1.2.0.dev0/README.md` & `keri-1.2.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/setup.py` & `keri-1.2.0.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from glob import glob
 from os.path import basename
 from os.path import splitext
 
 from setuptools import find_packages, setup
 setup(
     name='keri',
-    version='1.2.0-dev0',  # also change in src/keri/__init__.py
+    version='1.2.0-dev1',  # also change in src/keri/__init__.py
     license='Apache Software License 2.0',
     description='Key Event Receipt Infrastructure',
     long_description="KERI Decentralized Key Management Infrastructure",
     author='Samuel M. Smith',
     author_email='smith.samuel.m@gmail.com',
     url='https://github.com/WebOfTrust/keripy',
     packages=find_packages('src'),
@@ -90,15 +90,16 @@
                         'hjson>=3.1.0',
                         'PyYaml>=6.0.1',
                         'apispec>=6.6.0',
                         'mnemonic>=0.21',
                         'PrettyTable>=3.10.0',
                         'http_sfv>=0.9.9',
                         'cryptography>=42.0.5',
-                        'semver>=3.0.2'
+                        'semver>=3.0.2',
+                        'qrcode>=7.4.2'
     ],
     extras_require={
     },
     tests_require=[
                     'coverage>=7.4.4',
                     'pytest>=8.1.1',
                     'pytest-shell>=0.3.2'
```

### Comparing `keri-1.2.0.dev0/src/keri/app/agenting.py` & `keri-1.2.0.dev1/src/keri/app/agenting.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,29 +35,31 @@
         self.clienter = httping.Clienter()
 
         doers = [self.clienter, doing.doify(self.witDo), doing.doify(self.gitDo)]
         self.hby = hby
 
         super(Receiptor, self).__init__(doers=doers)
 
-    def receipt(self, pre, sn=None):
+    def receipt(self, pre, sn=None, auths=None):
         """ Returns a generator for witness receipting
 
         The returns a generator that will submit the designated event to witnesses for receipts using
-        the synchronous witness API, the propogate the receipts to each of the other witnesses.
+        the synchronous witness API, then propogate the receipts to each of the other witnesses.
 
 
         Parameters:
             pre (str): qualified base64 identifier to gather receipts for
             sn: (Optiona[int]): sequence number of event to gather receipts for, latest is used if not provided
+            auths: (Options[dict]): map of witness AIDs to (time,auth) tuples for providing TOTP auth for witnessing
 
         Returns:
             list: identifiers of witnesses that returned receipts.
 
         """
+        auths = auths if auths is not None else dict()
         if pre not in self.hby.prefixes:
             raise kering.MissingEntryError(f"{pre} not a valid AID")
 
         hab = self.hby.habs[pre]
         sn = sn if sn is not None else hab.kever.sner.num
         wits = hab.kever.wits
 
@@ -82,30 +84,34 @@
                 doers.append(clientDoer)
                 self.extend([clientDoer])
             except (kering.MissingEntryError, gaierror) as e:
                 logger.error(f"unable to create http client for witness {wit}: {e}")
 
         rcts = dict()
         for wit, client in clients.items():
-            httping.streamCESRRequests(client=client, dest=wit, ims=bytearray(msg), path="/receipts")
+            headers = dict()
+            if wit in auths:
+                headers["Authorization"] = auths[wit]
+
+            httping.streamCESRRequests(client=client, dest=wit, ims=bytearray(msg), path="receipts", headers=headers)
             while not client.responses:
                 yield self.tock
 
             rep = client.respond()
             if rep.status == 200:
                 rct = bytearray(rep.body)
                 hab.psr.parseOne(bytearray(rct))
                 rserder = serdering.SerderKERI(raw=rct)
                 del rct[:rserder.size]
 
                 # pull off the count code
                 coring.Counter(qb64b=rct, strip=True)
                 rcts[wit] = rct
             else:
-                logger.error(f"invalid response {rep.status} from witnesses {wit}")
+                print(f"invalid response {rep.status} from witnesses {wit}")
 
         for wit in rcts:
             ewits = [w for w in rcts if w != wit]
             wigs = [sig for w, sig in rcts.items() if w != wit]
 
             msg = bytearray()
             if ser.ked['t'] in (coring.Ilks.icp, coring.Ilks.dip):  # introduce new witnesses
@@ -263,15 +269,15 @@
 
     Removes all Doers and exits as Done once all witnesses have been sent the entire
     receipt set.  Could be enhanced to have a `once` method that runs once and cleans up
     and an `all` method that runs and waits for more messages to receipt.
 
     """
 
-    def __init__(self, hby, msgs=None, cues=None, force=False, **kwa):
+    def __init__(self, hby, msgs=None, cues=None, force=False, auths=None, **kwa):
         """
         For the current event, gather the current set of witnesses, send the event,
         gather all receipts and send them to all other witnesses
 
         Parameters:
             hby (Habery): Habitat of the identifier to receipt witnesses
             msgs (Deck): incoming messages to publish to witnesses
@@ -279,14 +285,15 @@
             force (bool): True means to send witnesses all receipts even if we have a full compliment.
 
         """
         self.hby = hby
         self.force = force
         self.msgs = msgs if msgs is not None else decking.Deck()
         self.cues = cues if cues is not None else decking.Deck()
+        self.auths = auths if auths is not None else dict()
 
         super(WitnessReceiptor, self).__init__(doers=[doing.doify(self.receiptDo)], **kwa)
 
     def receiptDo(self, tymth=None, tock=0.0):
         """
         Returns doifiable Doist compatible generator method (doer dog)
 
@@ -322,15 +329,16 @@
                 msg = hab.makeOwnEvent(sn=sn)
                 ser = serdering.SerderKERI(raw=msg)
 
                 dgkey = dbing.dgKey(ser.preb, ser.saidb)
 
                 witers = []
                 for wit in wits:
-                    witer = messenger(hab, wit)
+                    auth = self.auths[wit] if wit in self.auths else None
+                    witer = messenger(hab, wit, auth=auth)
                     witers.append(witer)
                     self.extend([witer])
 
                 # Check to see if we already have all the receipts we need for this event
                 wigs = hab.db.getWigs(dgkey)
                 completed = len(wigs) == len(wits)
                 if len(wigs) != len(wits):  # We have all the receipts, skip
@@ -826,29 +834,30 @@
 
 class HTTPMessenger(doing.DoDoer):
     """
     Interacts with Recipients on HTTP and SSE for sending events and receiving receipts
 
     """
 
-    def __init__(self, hab, wit, url, msgs=None, sent=None, doers=None, **kwa):
+    def __init__(self, hab, wit, url, msgs=None, sent=None, doers=None, auth=None, **kwa):
         """
         For the current event, gather the current set of witnesses, send the event,
         gather all receipts and send them to all other witnesses
 
         Parameters:
             hab: Habitat of the identifier to populate witnesses
 
         """
         self.hab = hab
         self.wit = wit
         self.posted = 0
         self.msgs = msgs if msgs is not None else decking.Deck()
         self.sent = sent if sent is not None else decking.Deck()
         self.parser = None
+        self.auth = auth
         doers = doers if doers is not None else []
         doers.extend([doing.doify(self.msgDo), doing.doify(self.responseDo)])
 
         up = urlparse(url)
         if up.scheme != kering.Schemes.http and up.scheme != kering.Schemes.https:
             raise ValueError(f"invalid scheme {up.scheme} for HTTPMessenger")
 
@@ -871,15 +880,19 @@
         _ = (yield self.tock)
 
         while True:
             while not self.msgs:
                 yield self.tock
 
             msg = self.msgs.popleft()
-            self.posted += httping.streamCESRRequests(client=self.client, dest=self.wit, ims=msg)
+            headers = dict()
+            if self.auth is not None:
+                headers["Authorization"] = self.auth
+
+            self.posted += httping.streamCESRRequests(client=self.client, dest=self.wit, ims=msg, headers=headers)
             while self.client.requests:
                 yield self.tock
 
             yield self.tock
 
     def responseDo(self, tymth=None, tock=0.0):
         """
@@ -973,42 +986,44 @@
     if not kever.wits:
         return None
 
     mbx = random.choice(kever.wits)
     return mbx
 
 
-def messenger(hab, pre):
+def messenger(hab, pre, auth=None):
     """ Create a Messenger (tcp or http) based on available endpoints
 
     Parameters:
         hab (Habitat): Environment to use to look up witness URLs
         pre (str): qb64 identifier prefix of recipient to create a messanger for
+        auth (str): optional auth code to send with any request for messenger
 
     Returns:
         Optional(TcpWitnesser, HTTPMessenger): witnesser for ensuring full reciepts
     """
     urls = hab.fetchUrls(eid=pre)
-    return messengerFrom(hab, pre, urls)
+    return messengerFrom(hab, pre, urls, auth)
 
 
-def messengerFrom(hab, pre, urls):
+def messengerFrom(hab, pre, urls, auth=None):
     """ Create a Witnesser (tcp or http) based on provided endpoints
 
     Parameters:
         hab (Habitat): Environment to use to look up witness URLs
         pre (str): qb64 identifier prefix of recipient to create a messanger for
         urls (dict): map of schemes to urls of available endpoints
+        auth (str): optional auth code to send with any request for messenger
 
     Returns:
         Optional(TcpWitnesser, HTTPMessenger): witnesser for ensuring full reciepts
     """
     if kering.Schemes.http in urls or kering.Schemes.https in urls:
         url = urls[kering.Schemes.http] if kering.Schemes.http in urls else urls[kering.Schemes.https]
-        witer = HTTPMessenger(hab=hab, wit=pre, url=url)
+        witer = HTTPMessenger(hab=hab, wit=pre, url=url, auth=auth)
     elif kering.Schemes.tcp in urls:
         url = urls[kering.Schemes.tcp]
         witer = TCPMessenger(hab=hab, wit=pre, url=url)
     else:
         raise kering.ConfigurationError(f"unable to find a valid endpoint for witness {pre}")
 
     return witer
@@ -1053,15 +1068,15 @@
     """
     urls = hab.fetchUrls(eid=wit, scheme=kering.Schemes.http) or hab.fetchUrls(eid=wit, scheme=kering.Schemes.https)
     if not urls:
         raise kering.MissingEntryError(f"unable to query witness {wit}, no http endpoint")
 
     url = urls[kering.Schemes.http] if kering.Schemes.http in urls else urls[kering.Schemes.https]
     up = urlparse(url)
-    client = http.clienting.Client(scheme=up.scheme, hostname=up.hostname, port=up.port)
+    client = http.clienting.Client(scheme=up.scheme, hostname=up.hostname, port=up.port, path=up.path)
     clientDoer = http.clienting.ClientDoer(client=client)
 
     return client, clientDoer
 
 
 def schemes(db, eids):
     msgs = bytearray()
```

### Comparing `keri-1.2.0.dev0/src/keri/app/apping.py` & `keri-1.2.0.dev1/src/keri/app/apping.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/challenging.py` & `keri-1.2.0.dev1/src/keri/app/challenging.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/challenge/generate.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/challenge/generate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/challenge/respond.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/challenge/respond.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 parser = argparse.ArgumentParser(description='Respond to a list of challenge words by signing and sending an EXN '
                                              'response')
 parser.set_defaults(handler=lambda args: respond(args))
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', default=None)
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument('--words', '-d', help='JSON formatted array of words to sign, \'@\' allowed to load from a file',
                     action="store", required=True)
 parser.add_argument('--recipient', '-r', help='Contact alias of the AID to send the signed words to',
                     action="store", required=True)
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/challenge/verify.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/challenge/verify.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 parser.set_defaults(handler=lambda args: verify(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--alias', '-a', help='human readable alias for the identifier to whom the credential was issued',
                     default=None)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 
 parser.add_argument('--words', '-d', help='JSON formatted array of words to verfiy, \'@\' allowed to load from a file',
                     action="store", required=False)
 parser.add_argument('--generate', '-g', help="Generate words, print to stdout and wait for verification",
                     action="store_true")
 parser.add_argument('--strength', help='Cryptographic strength in bits.  Defaults to 128.  Only applies with '
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/clean.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/clean.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--temp', '-t', help='create a temporary keystore, used for testing', default=False)
 
 # Parameters for Manager creation
 # passcode => bran
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)
 
 
 class CleanDoer(doing.Doer):
 
     def __init__(self, args):
         self.args = args
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/contacts/list.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/contacts/list.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 parser = argparse.ArgumentParser(description='List existing contacts')
 parser.set_defaults(handler=lambda args: handler(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 
 
 def handler(args):
     kwa = dict(args=args)
     return [doing.doify(list, **kwa)]
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/delegate/confirm.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/delegate/confirm.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 
 from hio.base import doing
 
 from keri import help
 from keri.app import habbing, indirecting, agenting, grouping, forwarding, delegating, notifying
 from keri.app.cli.common import existing
 from keri.app.habbing import GroupHab
+from keri import core
 from keri.core import coring, serdering
 from keri.db import dbing
 from keri.peer import exchanging
 
 logger = help.ogler.getLogger()
 
 parser = argparse.ArgumentParser(description='Confirm success delegate event (icp or rot) and gather and '
                                              'propagate witness receipts.')
 parser.set_defaults(handler=lambda args: confirm(args))
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', required=True)
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument("--interact", "-i", help="anchor the delegation approval in an interaction event.  "
                                              "Default is to use a rotation event.", action="store_true")
 parser.add_argument("--auto", "-Y", help="auto approve any delegation request non-interactively", action="store_true")
 
 
 def confirm(args):
@@ -126,16 +127,16 @@
                         approve = yn in ('', 'y', 'Y')
 
                     if not approve:
                         continue
 
                     if isinstance(hab, GroupHab):
                         aids = hab.smids
-                        seqner = coring.Seqner(sn=eserder.sn)
-                        anchor = dict(i=eserder.ked["i"], s=seqner.snh, d=eserder.said)
+                        #seqner = coring.Seqner(sn=eserder.sn)
+                        anchor = dict(i=eserder.ked["i"], s=eserder.snh, d=eserder.said)
                         if self.interact:
                             msg = hab.interact(data=[anchor])
                         else:
                             print("Confirm does not support rotation for delegation approval with group multisig")
                             continue
 
                         serder = serdering.SerderKERI(raw=msg)
@@ -144,34 +145,34 @@
                         others.remove(hab.mhab.pre)
 
                         for recpt in others:  # send notification to other participants as a signalling mechanism
                             self.postman.send(src=hab.mhab.pre, dest=recpt, topic="multisig", serder=exn,
                                               attachment=atc)
 
                         prefixer = coring.Prefixer(qb64=hab.pre)
-                        seqner = coring.Seqner(sn=serder.sn)
+                        sner = core.Number(num=serder.sn, code=core.NumDex.Huge)  # maybe serder.sner instead so not Huge
                         saider = coring.Saider(qb64b=serder.saidb)
-                        self.counselor.start(ghab=hab, prefixer=prefixer, seqner=seqner, saider=saider)
+                        self.counselor.start(ghab=hab, prefixer=prefixer, seqner=sner, saider=saider)
 
                         while True:
-                            saider = self.hby.db.cgms.get(keys=(prefixer.qb64, seqner.qb64))
+                            saider = self.hby.db.cgms.get(keys=(prefixer.qb64, sner.qb64))
                             if saider is not None:
                                 break
 
                             yield self.tock
 
                         print(f"Delegate {eserder.pre} {typ} event committed.")
 
                         self.remove(self.toRemove)
                         return True
 
                     else:
                         cur = hab.kever.sner.num
-                        seqner = coring.Seqner(sn=eserder.sn)
-                        anchor = dict(i=eserder.ked["i"], s=seqner.snh, d=eserder.said)
+                        #seqner = coring.Seqner(sn=eserder.sn)
+                        anchor = dict(i=eserder.ked["i"], s=eserder.snh, d=eserder.said)
                         if self.interact:
                             hab.interact(data=[anchor])
                         else:
                             hab.rotate(data=[anchor])
 
                         witDoer = agenting.WitnessReceiptor(hby=self.hby)
                         self.extend(doers=[witDoer])
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/delegate/request.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/delegate/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 parser = argparse.ArgumentParser(description='Resend a delegation request message to a delegator that has not '
                                              'approved a previous delegation.')
 parser.set_defaults(handler=lambda args: request(args))
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', required=True)
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 
 def request(args):
     """
 
     Parameters:
         args(Namespace): parsed arguements namespace object
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/did/generate.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/did/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for which to generate a DID', default=None)
 parser.add_argument("--role", "-r", help="role of oobis to generate", required=False, default="witness")
 
 # Parameters for Manager access
 # passcode => bran
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)
 parser.add_argument('--url', '-u', help="generate a DID URL instead of a DID", action="store_true")
 
 
 def handler(args):
     """ command line method for generating oobies
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/ends/add.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/ends/add.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 parser = argparse.ArgumentParser(description='Add new endpoint role authorization.')
 parser.set_defaults(handler=lambda args: add_end(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', required=True)
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument("--role", "-r", help="KERI enpoint authorization role.",
                     required=True)
 parser.add_argument("--eid", "-e", help="qualified base64 of AID to authorize with new role for the AID identified "
                                         "by alias",
                     required=True)
 parser.add_argument("--time", help="timestamp for the end auth", required=False, default=None)
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/ends/export.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/ends/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 parser = argparse.ArgumentParser(description='Export end points')
 parser.set_defaults(handler=lambda args: export_ends(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 
 parser.add_argument("--aid", "-a", help="qualified base64 of AID to export rpy messages for all endpoints.",
                     required=True)
 
 
 def export_ends(args):
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/ends/list.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/ends/list.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 parser = argparse.ArgumentParser(description='Add new endpoint role authorization.')
 parser.set_defaults(handler=lambda args: add_end(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', required=True)
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument("--aid", help="qualified base64 of AID to export rpy messages for all endpoints.",
                     required=True)
 
 
 def add_end(args):
     """ Command line tool for adding endpoint role authorizations
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/escrow.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/escrow.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 parser = argparse.ArgumentParser(description='Initialize a prefix')
 parser.set_defaults(handler=lambda args: handler(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 
 parser.add_argument("--escrow", "-e", help="show values for one specific escrow", default=None)
 
 
 def handler(args):
     """ Command line escrow handler
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/export.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 from hio.base import doing
 
 from keri.app.cli.common import existing
 from keri.core import coring, serdering
 
 logger = help.ogler.getLogger()
 
-parser = argparse.ArgumentParser(description='List credentials and check mailboxes for any newly issued credentials')
+parser = argparse.ArgumentParser(description='Export key events in CESR stream format')
 parser.set_defaults(handler=lambda args: export(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--alias', '-a', help='human readable alias for the identifier to whom the credential was issued',
                     required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument("--files", help="export artifacts to individual files keyed off of AIDs or SAIDS, default is "
                                     "stdout", action="store_true")
 parser.add_argument("--ends", help="export service end points", action="store_true")
 
 
 def export(args):
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/incept.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/incept.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 parser.add_argument("--receipt-endpoint", help="Attempt to connect to witness receipt endpoint for witness receipts.",
                     dest="endpoint", action='store_true')
 parser.add_argument("--proxy", help="alias for delegation communication proxy", default="")
 
 parser.add_argument('--file', '-f', help='Filename to use to create the identifier', default="", required=False)
 
 # Authentication for keystore
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument('--aeid', help='qualified base64 of non-transferable identifier prefix for  authentication '
                                    'and encryption of secrets in keystore', default=None)
 incepting.addInceptingArgs(parser)
 
 
 @dataclass
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/init.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/init.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                     dest="configFile",
                     action='store',
                     default=None,
                     help="configuration filename override")
 
 # Parameters for Manager creation
 # passcode => bran
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)
 parser.add_argument('--nopasscode', help='create an unencrypted keystore', action='store_true')
 parser.add_argument('--aeid', '-a', help='qualified base64 of non-transferable identifier prefix for  authentication '
                                          'and encryption of secrets in keystore', default=None)
 parser.add_argument('--seed', '-e', help='qualified base64 private-signing key (seed) for the aeid from which the '
                                          'private decryption key may be derived', default=None)
 
@@ -82,15 +82,15 @@
         base = args.base
         temp = args.temp
         bran = args.bran
         configFile = args.configFile
         configDir = args.configDir
 
         if not args.nopasscode and not bran:
-            print("Creating encrypted keystore, please enter your 22 character passcode:")
+            print("Creating encrypted keystore, please enter your 21 character passcode:")
             while True:
                 bran = getpass.getpass("Passcode: ")
                 retry = getpass.getpass("Re-enter passcode: ")
 
                 if bran != retry:
                     print("Passcodes do not match, try again.")
                 else:
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/interact.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/query.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,115 +1,104 @@
 # -*- encoding: utf-8 -*-
 """
 keri.kli.commands module
 
 """
 import argparse
+import datetime
 import json
-from ordered_set import OrderedSet as oset
 
+from hio import help
 from hio.base import doing
+from hio.help import decking
 
-from keri import kering
-from ..common import existing
-from ... import habbing, agenting, indirecting
-
-parser = argparse.ArgumentParser(description='Create and publish an interaction event')
-parser.set_defaults(handler=lambda args: interact(args))
-parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
+from keri.app import indirecting, habbing, querying
+from keri.app.cli.common import displaying
+from keri.app.cli.common import existing
+from keri.help import helping
+
+logger = help.ogler.getLogger()
+
+parser = argparse.ArgumentParser(description='Request KEL from Witness')
+parser.set_defaults(handler=lambda args: query(args),
+                    transferable=True)
+parser.add_argument('--name', '-n', help='Human readable reference', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', required=True)
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
-                    dest="bran", default=None)  # passcode => bran
-parser.add_argument('--data', '-d', help='Anchor data, \'@\' allowed', default=None, action="store", required=False)
-
+parser.add_argument('--prefix', help='QB64 identifier to query', default="", required=True)
 
-def interact(args):
-    """
-    Performs a rotation of the identifier of the environment represented by the provided name parameter
+# Authentication for keystore
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
+                    dest="bran", default=None)  # passcode => bran
+parser.add_argument('--aeid', help='qualified base64 of non-transferable identifier prefix for  authentication '
+                                   'and encryption of secrets in keystore', default=None)
+parser.add_argument('--anchor', help='JSON file containing the anchor to search for', default=None, required=False)
 
-        args (parseargs):  Command line argument
 
-    """
+def query(args):
     name = args.name
-    alias = args.alias
-    base = args.base
-    bran = args.bran
-
-    if args.data is not None:
-        try:
-            if args.data.startswith("@"):
-                f = open(args.data[1:], "r")
-                data = json.load(f)
-            else:
-                data = json.loads(args.data)
-        except json.JSONDecodeError:
-            raise kering.ConfigurationError("data supplied must be value JSON to anchor in a seal")
-
-        if not isinstance(data, list):
-            data = [data]
-
-    else:
-        data = None
-
-    ixnDoer = InteractDoer(name=name, base=base, alias=alias, bran=bran, data=data)
-
-    return [ixnDoer]
-
-
-class InteractDoer(doing.DoDoer):
-    """
-    DoDoer that launches Doers needed to create an interaction event and publication of the event
-    to all appropriate witnesses
-    """
 
-    def __init__(self, name, base, bran, alias, data: list = None):
-        """
-        Returns DoDoer with all registered Doers needed to perform interaction event.
+    qryDoer = LaunchDoer(name=name, alias=args.alias, base=args.base, bran=args.bran, pre=args.prefix,
+                         anchor=args.anchor)
+    return [qryDoer]
 
-        Parameters:
-            name is human readable str of identifier
-            proto is tcp or http method for communicating with Witness
-            data is list of dicts of committed data such as seals
-       """
 
-        self.alias = alias
-        self.data = data
+class LaunchDoer(doing.DoDoer):
 
+    def __init__(self, name, alias, base, bran, pre, anchor, **kwa):
+        doers = []
         self.hby = existing.setupHby(name=name, base=base, bran=bran)
         self.hbyDoer = habbing.HaberyDoer(habery=self.hby)  # setup doer
-        self.mbx = indirecting.MailboxDirector(hby=self.hby, topics=['/receipt', "/replay", "/reply"])
-        doers = [self.hbyDoer, self.mbx, doing.doify(self.interactDo)]
+        hab = self.hby.habByName(alias)
 
-        super(InteractDoer, self).__init__(doers=doers)
+        self.hab = hab
+        self.logs = decking.Deck()
 
-    def interactDo(self, tymth, tock=0.0, **opts):
+        self.pre = pre
+        self.anchor = anchor
+        self.loaded = False
+
+        self.mbd = indirecting.MailboxDirector(hby=self.hby, topics=["/replay", "/receipt", "/reply"])
+        doers.extend([self.hbyDoer, self.mbd])
+
+        self.toRemove = list(doers)
+        doers.extend([doing.doify(self.queryDo)])
+        super(LaunchDoer, self).__init__(doers=doers, **kwa)
+
+    def queryDo(self, tymth, tock=0.0, **opts):
         """
         Returns:  doifiable Doist compatible generator method
         Usage:
             add result of doify on this method to doers list
         """
+        # enter context
         self.wind(tymth)
         self.tock = tock
         _ = (yield self.tock)
 
-        hab = self.hby.habByName(name=self.alias)
-        hab.interact(data=self.data)
+        end = helping.nowUTC() + datetime.timedelta(seconds=10)
+
+        if self.anchor is not None:
+            f = open(self.anchor)
+            anchor = json.load(f)
+            print(f"Checking for anchor {anchor}...")
+            doer = querying.AnchorQuerier(hby=self.hby, hab=self.hab, pre=self.pre, anchor=anchor)
+        else:
+            print(f"Checking for updates...")
+            doer = querying.QueryDoer(hby=self.hby, hab=self.hab, pre=self.pre, kvy=self.mbd.kvy)
+
+        self.extend([doer])
+
+        while helping.nowUTC() < end:
+            if doer.done:
+                break
+            yield 1.0
 
-        witDoer = agenting.WitnessReceiptor(hby=self.hby)
-        self.extend(doers=[witDoer])
+        self.remove([doer])
+        print("\n")
 
-        if hab.kever.wits:
-            witDoer.msgs.append(dict(pre=hab.pre))
-            while not witDoer.cues:
-                _ = yield self.tock
-
-        print(f'Prefix  {hab.pre}')
-        print(f'New Sequence No.  {hab.kever.sn}')
-        for idx, verfer in enumerate(hab.kever.verfers):
-            print(f'\tPublic key {idx+1}:  {verfer.qb64}')
+        displaying.printExternal(self.hby, self.pre)
 
-        toRemove = [self.hbyDoer, witDoer, self.mbx]
-        self.remove(toRemove)
+        self.remove(self.toRemove)
 
         return
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/ipex/admit.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/admit.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                                              'grant')
 parser.set_defaults(handler=lambda args: handler(args))
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--alias', '-a', help='human readable alias for the identifier to whom the credential was issued',
                     required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 
 parser.add_argument("--said", "-s", help="SAID of the exn grant message to admit", required=True)
 parser.add_argument("--message", "-m", help="optional human readable message to "
                                             "send to recipient", required=False, default="")
 parser.add_argument("--time", help="timestamp", required=False, default=None)
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/ipex/agree.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/agree.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/ipex/grant.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/grant.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                                              'credential issuance or presentation')
 parser.set_defaults(handler=lambda args: handler(args))
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--alias', '-a', help='human readable alias for the identifier to whom the credential was issued',
                     required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 
 parser.add_argument("--recipient", "-r", help="alias or qb64 identifier prefix of the self.recp of "
                                               "the credential", required=True)
 parser.add_argument("--said", "-s", help="SAID of the credential to grant", required=True)
 parser.add_argument("--message", "-m", help="optional human readable message to "
                                             "send to recipient", required=False, default="")
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/ipex/join.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/join.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 logger = help.ogler.getLogger()
 
 parser = argparse.ArgumentParser(description='Join group multisig ipex events')
 parser.set_defaults(handler=lambda args: join(args))
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument("--auto", "-Y", help="auto approve any delegation request non-interactively", action="store_true")
 
 
 def join(args):
     """  Wait for and provide interactive confirmation of group multisig inception, rotation or interaction events
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/ipex/list.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/list.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 parser.set_defaults(handler=lambda args: listNotes(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--alias', '-a', help='human readable alias for the identifier to whom the credential was issued',
                     default=None)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 
 parser.add_argument("--verbose", "-V", help="print full JSON of all credentials", action="store_true")
 parser.add_argument("--said", "-s", help="display only the SAID of found exn message, one per line.",
                     action="store_true")
 parser.add_argument("--type", "-t", help="message type to list, options are (apply, offer, agree, grant, submit)")
 parser.add_argument("--poll", "-P", help="Poll mailboxes for any IPEX messages", action="store_true")
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/ipex/offer.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/offer.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/ipex/spurn.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/spurn.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 parser = argparse.ArgumentParser(description='Reject an IPEX apply, offer, agree or grant message')
 parser.set_defaults(handler=lambda args: handler(args))
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--alias', '-a', help='human readable alias for the identifier to whom the credential was issued',
                     required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 
 parser.add_argument("--said", "-s", help="SAID of the exn IPEX message to spurn", required=True)
 parser.add_argument("--message", "-m", help="optional human readable message to "
                                             "send to recipient", required=False, default="")
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/kevers.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/kevers.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 parser = argparse.ArgumentParser(description='Initialize a prefix')
 parser.set_defaults(handler=lambda args: handler(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--prefix', help='qb64 identifier prefix to display', required=True)
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument("--poll", "-P", help="Poll mailboxes for any events", action="store_true")
 
 parser.add_argument("--verbose", "-V", help="print JSON of all current events", action="store_true")
 
 
 def handler(args):
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/list.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/list.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 parser = argparse.ArgumentParser(description='List existing identifiers')
 parser.set_defaults(handler=lambda args: list_identifiers(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 
 parser.add_argument("--verbose", "-V", help="print JSON of all current events", action="store_true")
 
 
 def list_identifiers(args):
     """ Command line list handler
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/local/watch.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/local/watch.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 parser.set_defaults(handler=lambda args: watch(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='Human readable reference', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 
 # Authentication for keystore
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument('--aeid', help='qualified base64 of non-transferable identifier prefix for  authentication '
                                    'and encryption of secrets in keystore', default=None)
 
 Stateage = namedtuple("Stateage", 'even ahead behind duplicitous')
 
 States = Stateage(even="even", ahead="ahead", behind="behind", duplicitous="duplicitous")
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/mailbox/debug.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/mailbox/debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 parser = argparse.ArgumentParser(description='Display mailbox status for an identifier and witness')
 parser.set_defaults(handler=lambda args: handler(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', default=None)
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument('--witness', '-w', help='The qualified b64 AID of the witness to poll', required=True)
 parser.add_argument("--verbose", "-V", help="print JSON of all current events", action="store_true")
 
 
 def handler(args):
     """
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/mailbox/update.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/mailbox/update.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 parser.add_argument("--config", "-c", help="directory override for configuration data")
 
 parser.add_argument("--witness", "-w", help="qualified b64 AID of witness to update", required=True)
 parser.add_argument("--topic", "-t", help="topic name to update", required=True)
 parser.add_argument("--index", "-i", help="new index for topic on witness", required=True)
 
 # Authentication for keystore
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument('--aeid', help='qualified base64 of non-transferable identifier prefix for  authentication '
                                    'and encryption of secrets in keystore', default=None)
 
 
 def handler(args):
     kwa = dict(args=args)
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/migrate/list.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/migrate/list.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--temp', '-t', help='create a temporary keystore, used for testing', default=False)
 
 # Parameters for Manager creation
 # passcode => bran
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)
 
 
 class ListDoer(doing.Doer):
 
     def __init__(self, args):
         self.args = args
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/migrate/run.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/migrate/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--temp', '-t', help='create a temporary keystore, used for testing', default=False)
 
 # Parameters for Manager creation
 # passcode => bran
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)
 
 
 class MigrateDoer(doing.Doer):
 
     def __init__(self, args):
         self.args = args
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/migrate/show.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/migrate/show.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                     required=False, default="")
 parser.add_argument('--temp', '-t', help='create a temporary keystore, used for testing', default=False)
 parser.add_argument('--migration', '-m', help='migration name', required=True)
 
 
 # Parameters for Manager creation
 # passcode => bran
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)
 
 
 class CleanDoer(doing.Doer):
 
     def __init__(self, args):
         self.args = args
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/migrate.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/migrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 parser = argparse.ArgumentParser(description='View status of a local AID')
 parser.set_defaults(handler=lambda args: handler(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument('--force', action="store_true", required=False,
                     help='True means perform migration without prompting the user')
 
 
 def handler(args):
     if not args.force:
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/multisig/continue.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/continue.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                                              'events.')
 parser.set_defaults(handler=lambda args: handler(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the local identifier prefix', required=True)
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 
 
 def handler(args):
     kever = ContinueDoer(name=args.name, base=args.base, bran=args.bran, alias=args.alias)
     return [kever]
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/multisig/demo.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/demo.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/multisig/incept.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/incept.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 parser = argparse.ArgumentParser(description='Initialize a group identifier prefix')
 parser.set_defaults(handler=lambda args: inceptMultisig(args))
 parser.add_argument('--name', '-n', help='Human readable environment reference for local identifier', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the local identifier prefix', required=True)
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument("--wait", "-w", help="number of seconds to wait for other multisig events, defaults to 10",
                     default=10)
 
 parser.add_argument('--group', '-g', help="Human readable environment reference for group identifier", required=True)
 parser.add_argument('--file', '-f', help='Filename to use to create the identifier', default="", required=True)
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/multisig/interact.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/interact.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 parser = argparse.ArgumentParser(description='Begin or join a rotation of a group identifier')
 parser.set_defaults(handler=lambda args: interactGroupIdentifier(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='Human readable reference', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the local identifier prefix', required=True)
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument('--data', '-d', help='Anchor data, \'@\' allowed', default=[], action="store", required=True)
 parser.add_argument("--aids", "-g", help="List of other participant qb64 identifiers to include in interaction event",
                     action="append", required=False, default=None)
 
 
 def interactGroupIdentifier(args):
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/multisig/join.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/join.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 logger = help.ogler.getLogger()
 
 parser = argparse.ArgumentParser(description='Join group multisig inception, rotation or interaction event.')
 parser.set_defaults(handler=lambda args: confirm(args))
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument("--auto", "-Y", help="auto approve any delegation request non-interactively", action="store_true")
 
 
 def confirm(args):
     """  Wait for and provide interactive confirmation of group multisig inception, rotation or interaction events
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/multisig/notice.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/notice.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', required=True)
 parser.add_argument("--config", "-c", help="directory override for configuration data")
 
 # Authentication for keystore
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument('--aeid', help='qualified base64 of non-transferable identifier prefix for  authentication '
                                    'and encryption of secrets in keystore', default=None)
 
 
 def handler(args):
     """
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/multisig/rotate.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/rotate.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 parser = argparse.ArgumentParser(description='Begin or join a rotation of a group identifier')
 parser.set_defaults(handler=lambda args: rotateGroupIdentifier(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='Human readable reference', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the local identifier prefix', required=True)
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument("--smids", "-s", help="List of other participant qb64 identifiers with signing authority in "
                                           "rotation event",
                     action="append", required=False, default=None)
 parser.add_argument("--rmids", help="List of other participant qb64 identifiers with rotation authority in rotation "
                                     "event",
                     action="append", required=False, default=None)
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/multisig/shell.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 parser = argparse.ArgumentParser(description='Initialize a prefix')
 parser.set_defaults(handler=lambda args: handler(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 
 parser.add_argument('--static-threshold', '-t', help='Specify this to switch to using one static number as the signing'
                                                      'threshold for the multisig group AID',
                     dest="static", action="store_true")  # passcode => bran
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/multisig/update.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/update.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 parser.add_argument('--name', '-n', help='Human readable reference', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', required=True)
 parser.add_argument('--witness', '-w', help='QB64 identifier of witness to query', default="", required=True)
 
 # Authentication for keystore
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument('--aeid', help='qualified base64 of non-transferable identifier prefix for  authentication '
                                    'and encryption of secrets in keystore', default=None)
 
 parser.add_argument('--sn', help="Serial number of the event expected on witness", default=0, required=True)
 parser.add_argument('--said', help="Said of the event expected on witness", default=None, required=True)
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/oobi/clean.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/oobi/clean.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 parser = argparse.ArgumentParser(description='Display OOBIs waiting for resolution and allow for clean up')
 parser.set_defaults(handler=lambda args: list_oobis(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 
 def list_oobis(args):
     """ Command line list handler
 
     """
     kwa = dict(args=args)
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/oobi/generate.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/oobi/generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', default=None)
 parser.add_argument("--role", "-r", help="role of oobis to generate", required=True)
 
 # Parameters for Manager access
 # passcode => bran
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)
 
 
 def handler(args):
     """ command line method for generating oobies
 
     Parameters:
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/oobi/resolve.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/oobi/resolve.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                     required=False, default=None)
 parser.add_argument('--force', action="store_true", required=False,
                     help='True means to resolve OOBI even if it has already been previously resolved')
 
 
 # Parameters for Manager access
 # passcode => bran
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)
 
 
 def resolve(args):
     """ command line method for resolving oobies
 
     Parameters:
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/passcode/generate.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/passcode/generate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/passcode/remove.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/passcode/remove.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 parser = argparse.ArgumentParser(description='Initialize a prefix')
 parser.set_defaults(handler=lambda args: remove(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--passcode', '-p', help='existing 22 character encryption passcode for keystore',
+parser.add_argument('--passcode', '-p', help='existing 21 character encryption passcode for keystore',
                     dest="bran", default=None)  # passcode => bran
 
 
 def handler(args):
     """ Command line passcode remove handler
 
     """
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/passcode/set.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/passcode/set.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,30 +3,36 @@
 keri.kli.common.passcode.set module
 
 """
 import argparse
 import getpass
 
 from hio import help
+
 from hio.base import doing
 
-from keri.app.cli.common import existing
-from keri.core import coring
 from keri.kering import ConfigurationError
 
-logger = help.ogler.getLogger()
+from keri import core
+from keri.core import coring
+
+from keri.app.cli.common import existing
+
+
+
+logger = help.ogler.getLogger()  # I think this should be keri.help not hio.help
 
 parser = argparse.ArgumentParser(description='Initialize a prefix')
 parser.set_defaults(handler=lambda args: set_passcode(args),
                     transferable=True)
-parser.add_argument("--new", help="new  22 character encryption passcode for keystore", required=False, default=None)
+parser.add_argument("--new", help="new  21 character encryption passcode for keystore", required=False, default=None)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--passcode', '-p', help='existing 22 character encryption passcode for keystore',
+parser.add_argument('--passcode', '-p', help='existing 21 character encryption passcode for keystore',
                     dest="bran", default=None)  # passcode => bran
 
 
 def handler(args):
     """ Command line status handler
 
     """
@@ -46,26 +52,26 @@
 
     newpasscode = args.new
 
     try:
         with existing.existingHby(name=name, base=base, bran=bran) as hby:
 
             if newpasscode is None:
-                print("Re-encrypting keystore, please enter the new 22 character passcode:")
+                print("Re-encrypting keystore, please enter the new 21 character passcode:")
                 while True:
                     newpasscode = getpass.getpass("New passcode: ")
                     retry = getpass.getpass("Re-enter new passcode: ")
 
                     if newpasscode != retry:
                         print("Passcodes do not match, try again.")
                     else:
                         break
 
             bran = coring.MtrDex.Salt_128 + newpasscode[:22]  # qb64 salt for seed
-            signer = coring.Salter(qb64=bran).signer(transferable=False,
+            signer = core.Salter(qb64=bran).signer(transferable=False,
                                                      temp=False)
             seed = signer.qb64
             aeid = signer.verfer.qb64
 
             hby.mgr.updateAeid(aeid, seed)
             print("Passcode reset and keystore re-encrypted.")
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/query.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/ssh/export.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,104 +1,87 @@
 # -*- encoding: utf-8 -*-
 """
+KERI
 keri.kli.commands module
 
 """
 import argparse
-import datetime
-import json
+import os
+import stat
+from pathlib import Path
 
+from cryptography.hazmat.primitives import serialization
+from cryptography.hazmat.primitives.asymmetric import ed25519
 from hio import help
 from hio.base import doing
-from hio.help import decking
 
-from keri.app import indirecting, habbing, querying
-from keri.app.cli.common import displaying
 from keri.app.cli.common import existing
-from keri.help import helping
+from keri.kering import ConfigurationError
 
 logger = help.ogler.getLogger()
 
-parser = argparse.ArgumentParser(description='Request KEL from Witness')
-parser.set_defaults(handler=lambda args: query(args),
+parser = argparse.ArgumentParser(description='Export keys of specified identifier for use with SSH')
+parser.set_defaults(handler=lambda args: handler(args),
                     transferable=True)
-parser.add_argument('--name', '-n', help='Human readable reference', required=True)
+parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', required=True)
-parser.add_argument('--prefix', help='QB64 identifier to query', default="", required=True)
-
-# Authentication for keystore
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', default=None)
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
-parser.add_argument('--aeid', help='qualified base64 of non-transferable identifier prefix for  authentication '
-                                   'and encryption of secrets in keystore', default=None)
-parser.add_argument('--anchor', help='JSON file containing the anchor to search for', default=None, required=False)
-
 
-def query(args):
-    name = args.name
+parser.add_argument("--private", help="export private key instead of public key", action="store_true")
+parser.add_argument("--username", help="override file name for the key to export", default=None)
 
-    qryDoer = LaunchDoer(name=name, alias=args.alias, base=args.base, bran=args.bran, pre=args.prefix,
-                         anchor=args.anchor)
-    return [qryDoer]
-
-
-class LaunchDoer(doing.DoDoer):
-
-    def __init__(self, name, alias, base, bran, pre, anchor, **kwa):
-        doers = []
-        self.hby = existing.setupHby(name=name, base=base, bran=bran)
-        self.hbyDoer = habbing.HaberyDoer(habery=self.hby)  # setup doer
-        hab = self.hby.habByName(alias)
-
-        self.hab = hab
-        self.logs = decking.Deck()
-
-        self.pre = pre
-        self.anchor = anchor
-        self.loaded = False
-
-        self.mbd = indirecting.MailboxDirector(hby=self.hby, topics=["/replay", "/receipt", "/reply"])
-        doers.extend([self.hbyDoer, self.mbd])
-
-        self.toRemove = list(doers)
-        doers.extend([doing.doify(self.queryDo)])
-        super(LaunchDoer, self).__init__(doers=doers, **kwa)
-
-    def queryDo(self, tymth, tock=0.0, **opts):
-        """
-        Returns:  doifiable Doist compatible generator method
-        Usage:
-            add result of doify on this method to doers list
-        """
-        # enter context
-        self.wind(tymth)
-        self.tock = tock
-        _ = (yield self.tock)
-
-        end = helping.nowUTC() + datetime.timedelta(seconds=10)
-
-        if self.anchor is not None:
-            f = open(self.anchor)
-            anchor = json.load(f)
-            print(f"Checking for anchor {anchor}...")
-            doer = querying.AnchorQuerier(hby=self.hby, hab=self.hab, pre=self.pre, anchor=anchor)
-        else:
-            print(f"Checking for updates...")
-            doer = querying.QueryDoer(hby=self.hby, hab=self.hab, pre=self.pre, kvy=self.mbd.kvy)
-
-        self.extend([doer])
-
-        while helping.nowUTC() < end:
-            if doer.done:
-                break
-            yield 1.0
 
-        self.remove([doer])
-        print("\n")
+def handler(args):
+    kwa = dict(args=args)
+    return [doing.doify(export, **kwa)]
 
-        displaying.printExternal(self.hby, self.pre)
 
-        self.remove(self.toRemove)
+def export(tymth, tock=0.0, **opts):
+    """ Command line status handler
 
-        return
+    """
+    _ = (yield tock)
+    args = opts["args"]
+    name = args.name
+    alias = args.alias
+    base = args.base
+    bran = args.bran
+    private = args.private
+    filename = args.username if args.username else alias
+    home = str(Path.home())
+
+    try:
+        with existing.existingHby(name=name, base=base, bran=bran) as hby:
+            if alias is None:
+                alias = existing.aliasInput(hby)
+
+            hab = hby.habByName(alias)
+            if private:
+                signer = hab.ks.pris.get(hab.kever.verfers[0].qb64,
+                                         decrypter=hab.mgr.decrypter)
+                sigkey = ed25519.Ed25519PrivateKey.from_private_bytes(signer.raw)
+                pem = sigkey.private_bytes(encoding=serialization.Encoding.PEM,
+                                           format=serialization.PrivateFormat.OpenSSH,
+                                           encryption_algorithm=serialization.NoEncryption())
+
+                f = open(os.path.join(home, ".ssh", filename), "w")
+                for line in pem.splitlines(keepends=True):
+                    f.write(line.decode("utf-8"))
+                f.close()
+                os.chmod(os.path.join(home, ".ssh", filename), stat.S_IRUSR | stat.S_IWUSR)
+
+            else:
+                verkey = ed25519.Ed25519PublicKey.from_public_bytes(hab.kever.verfers[0].raw)
+                pem = verkey.public_bytes(encoding=serialization.Encoding.OpenSSH,
+                                          format=serialization.PublicFormat.OpenSSH)
+
+                f = open(os.path.join(home, ".ssh", f"{filename}.pub"), "w")
+                for line in pem.splitlines(keepends=True):
+                    f.write(line.decode("utf-8"))
+
+
+    except ConfigurationError as e:
+        print(f"identifier prefix for {name} does not exist, incept must be run first", )
+        return -1
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/rename.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/rename.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 parser.set_defaults(handler=lambda args: handler(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the identifier prefix', required=True)
 parser.add_argument('new', help='new human readable alias for the identifier')
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 
 
 def handler(args):
     kwa = dict(args=args)
     return [doing.doify(rename, **kwa)]
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/rollback.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/rollback.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 parser = argparse.ArgumentParser(description='Revert an unpublished interaction event at the end of a local KEL')
 parser.set_defaults(handler=lambda args: handler(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', default=None)
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 
 
 def handler(args):
     kwa = dict(args=args)
     return [doing.doify(rollback, **kwa)]
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/rotate.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/rotate.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,29 +7,32 @@
 from dataclasses import dataclass
 
 from hio.base import doing
 
 from keri import kering
 from keri.app.cli.common import rotating, existing, config
 from keri.core import coring
+from keri.help import helping
 from ... import habbing, agenting, indirecting, delegating, forwarding
 
 parser = argparse.ArgumentParser(description='Rotate keys')
 parser.set_defaults(handler=lambda args: rotate(args))
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', required=True)
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument('--file', '-f', help='file path of config options (JSON) for rotation', default="", required=False)
 parser.add_argument('--next-count', '-C', help='Count of pre-rotated keys (signing keys after next rotation).',
                     default=None, type=int, required=False)
 parser.add_argument("--receipt-endpoint", help="Attempt to connect to witness receipt endpoint for witness receipts.",
                     dest="endpoint", action='store_true')
+parser.add_argument("--authenticate", '-z', help="Prompt the controller for authentication codes for each witness",
+                    action='store_true')
 parser.add_argument("--proxy", help="alias for delegation communication proxy", default="")
 
 rotating.addRotationArgs(parser)
 
 
 @dataclass
 class RotateOptions:
@@ -56,15 +59,15 @@
     """
     opts = mergeArgsWithFile(args)
     rotDoer = RotateDoer(name=args.name, base=args.base, alias=args.alias, endpoint=args.endpoint,
                          bran=args.bran, wits=opts.wits,
                          cuts=opts.witsCut, adds=opts.witsAdd,
                          isith=opts.isith, nsith=opts.nsith,
                          count=opts.ncount, toad=opts.toad,
-                         data=opts.data, proxy=args.proxy)
+                         data=opts.data, proxy=args.proxy, authenticate=args.authenticate)
 
     doers = [rotDoer]
 
     return doers
 
 
 def emptyOptions():
@@ -111,15 +114,15 @@
 class RotateDoer(doing.DoDoer):
     """
     DoDoer that launches Doers needed to perform a rotation and publication of the rotation event
     to all appropriate witnesses
     """
 
     def __init__(self, name, base, bran, alias, endpoint=False, isith=None, nsith=None, count=None,
-                 toad=None, wits=None, cuts=None, adds=None, data: list = None, proxy=None):
+                 toad=None, wits=None, cuts=None, adds=None, data: list = None, proxy=None, authenticate=False):
         """
         Returns DoDoer with all registered Doers needed to perform rotation.
 
         Parameters:
             name is human-readable str of identifier
             isith is current signing threshold as int or str hex or list of str weights
             nsith is next signing threshold as int or str hex or list of str weights
@@ -136,14 +139,15 @@
         self.isith = isith
         self.nsith = nsith
         self.count = count
         self.toad = toad
         self.data = data
         self.endpoint = endpoint
         self.proxy = proxy
+        self.authenticate = authenticate
 
         self.wits = wits if wits is not None else []
         self.cuts = cuts if cuts is not None else []
         self.adds = adds if adds is not None else []
 
         self.hby = existing.setupHby(name=name, base=base, bran=bran)
         self.hbyDoer = habbing.HaberyDoer(habery=self.hby)  # setup doer
@@ -183,29 +187,35 @@
                 for wit in self.adds:
                     yield from receiptor.catchup(hab.pre, wit)
 
         hab.rotate(isith=self.isith, nsith=self.nsith, ncount=self.count, toad=self.toad,
                    cuts=list(self.cuts), adds=list(self.adds),
                    data=self.data)
 
+        auths = {}
+        if self.authenticate:
+            for wit in hab.kever.wits:
+                code = input(f"Entire code for {wit}: ")
+                auths[wit] = f"{code}#{helping.nowIso8601()}"
+
         if hab.kever.delpre:
             self.swain.delegation(pre=hab.pre, sn=hab.kever.sn, proxy=self.hby.habByName(self.proxy))
             print("Waiting for delegation approval...")
             while not self.swain.complete(hab.kever.prefixer, coring.Seqner(sn=hab.kever.sn)):
                 yield self.tock
 
         elif hab.kever.wits:
             if self.endpoint:
-                yield from receiptor.receipt(hab.pre, sn=hab.kever.sn)
+                yield from receiptor.receipt(hab.pre, sn=hab.kever.sn, auths=auths)
             else:
                 for wit in self.adds:
                     self.mbx.addPoller(hab, witness=wit)
 
                 print("Waiting for witness receipts...")
-                witDoer = agenting.WitnessReceiptor(hby=self.hby)
+                witDoer = agenting.WitnessReceiptor(hby=self.hby, auths=auths)
                 self.extend(doers=[witDoer])
                 yield self.tock
 
                 witDoer.msgs.append(dict(pre=hab.pre))
                 while not witDoer.cues:
                     _ = yield self.tock
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/saidify.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/saidify.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/salt.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/salt.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 """
 import argparse
 
 import pysodium
 from hio.base import doing
 
-from keri.core import coring
+from keri import core
 
 parser = argparse.ArgumentParser(description='Print a new random passcode')
 parser.set_defaults(handler=lambda args: handler(args))
 
 
 def handler(_):
     return [doing.doify(passcode)]
 
 
 def passcode(tymth, tock=0.0):
     """ Command line version handler
     """
     _ = (yield tock)
 
-    print(coring.Salter(raw=pysodium.randombytes(pysodium.crypto_sign_SEEDBYTES)).qb64)
+    print(core.Salter(raw=pysodium.randombytes(pysodium.crypto_sign_SEEDBYTES)).qb64)
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/sign.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/sign.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 parser = argparse.ArgumentParser(description='Sign an arbitrary string')
 parser.set_defaults(handler=lambda args: handler(args))
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', required=True)
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument('--text', '-t', help='Text or file (starts with "@") to sign', required=True)
 
 
 def handler(args):
     """
     Sign arbitrary data
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/status.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 parser = argparse.ArgumentParser(description='View status of a local AID')
 parser.set_defaults(handler=lambda args: handler(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', default=None)
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 
 parser.add_argument("--verbose", "-V", help="print JSON of all current events", action="store_true")
 
 
 def handler(args):
     kwa = dict(args=args)
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/vc/create.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/vc/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import argparse
 import json
 
 from hio import help
 from hio.base import doing
 
 from keri import kering
+from keri import core
+from keri.core import coring, eventing, serdering
+
 from keri.app import indirecting, habbing, grouping, connecting, forwarding, signing, notifying
 from keri.app.cli.common import existing
-from keri.core import coring, eventing, serdering
 from keri.help import helping
 from keri.peer import exchanging
 from keri.vdr import credentialing, verifying
 
 logger = help.ogler.getLogger()
 
 parser = argparse.ArgumentParser(description='Initialize a prefix')
@@ -32,15 +34,15 @@
 parser.add_argument('--credential', help='Full credential, \'@\' allowed', default=None, action="store",
                     required=False)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', required=True)
 parser.add_argument("--private", help="flag to indicate if this credential needs privacy preserving features",
                     action="store_true")
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument("--time", help="timestamp for the credential creation", required=False, default=None)
 
 
 def issueCredential(args):
     name = args.name
     data = None
@@ -203,30 +205,31 @@
 
         registry = self.rgy.registryByName(self.registryName)
         hab = registry.hab
 
         dt = self.creder.attrib["dt"] if "dt" in self.creder.attrib else helping.nowIso8601()
         iserder = registry.issue(said=self.creder.said, dt=dt)
 
-        vcid = iserder.ked["i"]
-        rseq = coring.Seqner(snh=iserder.ked["s"])
-        rseal = eventing.SealEvent(vcid, rseq.snh, iserder.said)
+        #vcid = iserder.ked["i"]
+        #rseq = coring.Seqner(snh=iserder.ked["s"])
+        rseal = eventing.SealEvent(iserder.pre, iserder.snh, iserder.said)
         rseal = dict(i=rseal.i, s=rseal.s, d=rseal.d)
 
         if registry.estOnly:
             anc = hab.rotate(data=[rseal])
 
         else:
             anc = hab.interact(data=[rseal])
 
         aserder = serdering.SerderKERI(raw=anc)  # coring.Serder(raw=anc)
         self.credentialer.issue(self.creder, iserder)
         self.registrar.issue(self.creder, iserder, aserder)
 
-        acdc = signing.serialize(self.creder, coring.Prefixer(qb64=iserder.pre), coring.Seqner(sn=iserder.sn),
+        acdc = signing.serialize(self.creder, coring.Prefixer(qb64=iserder.pre),
+                                 core.Number(num=iserder.sn, code=core.NumDex.Huge),
                                  coring.Saider(qb64=iserder.said))
 
         if isinstance(self.hab, habbing.GroupHab):
             smids = self.hab.db.signingMembers(pre=self.hab.pre)
             smids.remove(self.hab.mhab.pre)
 
             for recp in smids:  # this goes to other participants only as a signaling mechanism
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/vc/export.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/vc/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 parser.set_defaults(handler=lambda args: export_credentials(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--alias', '-a', help='human readable alias for the identifier to whom the credential was issued',
                     required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 
 parser.add_argument("--said", "-s", help="SAID of the credential to export.", required=False, default=None)
 parser.add_argument("--tels", help="export the transaction event logs for the credential and any chained credentials",
                     action="store_true")
 parser.add_argument("--kels", help="export the key event logs for the issuer's of the credentials", action="store_true")
 parser.add_argument("--chains", help="export any chained credentials", action="store_true")
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/vc/list.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/vc/list.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 parser.set_defaults(handler=lambda args: list_credentials(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--alias', '-a', help='human readable alias for the identifier to whom the credential was issued',
                     default=None)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 
 parser.add_argument("--verbose", "-V", help="print full JSON of all credentials", action="store_true")
 parser.add_argument("--poll", "-P", help="Poll mailboxes for any issued credentials", action="store_true")
 parser.add_argument("--issued", "-i", help="Display credentials that this AID has issued.",
                     action="store_true")
 parser.add_argument("--said", "-s", help="Display only the SAID of found credentials, one per line.",
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/vc/registry/incept.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/vc/registry/incept.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                                       'appear multiple times', metavar="<prefix>", default=[], action="append",
                     required=False)
 parser.add_argument("--establishment-only", "-eo", help="Only allow establishment events for the anchoring events of "
                                                         "this registry", default=False, action="store")
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', required=True)
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument('--usage', '-u', help='For multisig issuers, a message to other participants about how this'
                                           ' registry is to be used',
                     default=None)
 
 
 def registryIncept(args):
@@ -70,15 +70,15 @@
     def __init__(self, name, base, alias, bran, registryName, usage, **kwa):
         """  Create RegistryIncepter to pass message and process cues
 
         Parameters:
             name (str): name of habery and shared db and file path
             base (str): optional if "" path component of shared db and files.
             alias(str): human readable name of identifier to use for registry inception
-            bran (str): Base64 22 char string that is used as base material for
+            bran (str): Base64 21 char string that is used as base material for
                         seed. bran allows alphanumeric passcodes generated by key managers
                         like 1password to be key store for seed.
             registryName(str): human readable name for newly created registry
 
         """
         self.name = name
         self.alias = alias
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/vc/registry/list.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/vc/registry/list.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 parser = argparse.ArgumentParser(description='List credential registry names and identifiers')
 parser.set_defaults(handler=lambda args: list_registries(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 
 parser.add_argument("--verbose", "-V", help="print JSON of all current events", action="store_true")
 
 
 def list_registries(args):
     """ Command line list credential registries handler
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/vc/registry/status.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/vc/registry/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 parser.set_defaults(handler=lambda args: registryStatus(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='Human readable reference', required=True)
 parser.add_argument('--registry-name', '-r', help='Human readable name for registry, defaults to name of Habitat',
                     default=None, required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument("--verbose", "-V", help="print JSON of all current events", action="store_true")
 
 
 def registryStatus(args):
     name = args.name
     bran = args.bran
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/vc/revoke.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/vc/revoke.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 parser.set_defaults(handler=lambda args: revokeCredential(args))
 parser.add_argument('--name', '-n', help='Human readable reference', required=True)
 parser.add_argument('--registry-name', '-r', help='Human readable name for registry, defaults to name of Habitat',
                     default=None)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', required=True)
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument('--said', help='is SAID vc content qb64')
 parser.add_argument('--send', help='alias of contact to send the revocation events to (can be repeated)',
                     required=False, action="append")
 parser.add_argument("--time", help="timestamp for the revocation", required=False, default=None)
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/verify.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/verify.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 parser = argparse.ArgumentParser(description='Verify signature(s) on arbitrary data')
 parser.set_defaults(handler=lambda args: handler(args))
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', required=True)
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 
 parser.add_argument("--prefix", help="Identifier prefix of the signer", required=True)
 parser.add_argument('--text', '-t', help='Original signed text or file (starts with "@")', required=True)
 parser.add_argument('--signature', '-s', default=[], help='list of signatures to verify (can appear multiple times)',
                     action="append", required=True)
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/version.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/version.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 parser = argparse.ArgumentParser(description='Print version of KLI')
 parser.set_defaults(handler=lambda args: handler(args))
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=False,
                     default=None)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 
 
 def handler(args):
     kwa = dict(args=args)
     return [doing.doify(version, **kwa)]
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/witness/demo.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/witness/demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,21 @@
 """
 
 import argparse
 import logging
 
 from hio.base import doing
 
-from keri.app import habbing, indirecting, configing
-from keri.core.coring import Salter
 from keri import help
 
+from keri.app import habbing, indirecting, configing
+
+from keri.core import Salter
+
+
 parser = argparse.ArgumentParser(description="Run a demo collection of witnesses")
 parser.set_defaults(handler=lambda args: demo(args))
 
 
 help.ogler.level = logging.INFO
 logger = help.ogler.getLogger()
 
@@ -53,15 +56,15 @@
     def __init__(self, wan, wil, wes, wit, wub, wyz):
         self.wan = wan
         self.wil = wil
         self.wes = wes
         self.wit = wit
         self.wub = wub
         self.wyz = wyz
-        
+
         super(InitDoer, self).__init__(doers=[doing.doify(self.initialize)])
 
     def initialize(self, tymth, tock=0.0):
         # enter context
         self.wind(tymth)
         self.tock = tock
         _ = (yield self.tock)
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/witness/start.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/witness/start.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 parser.add_argument('-n', '--name',
                     action='store',
                     default="witness",
                     help="Name of controller. Default is witness.")
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', required=True)
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument("--config-dir", "-c", dest="configDir", help="directory override for configuration data")
 parser.add_argument('--config-file',
                     dest="configFile",
                     action='store',
                     default=None,
                     help="configuration filename override")
@@ -51,15 +51,15 @@
                     help="Set log level to DEBUG | INFO | WARNING | ERROR | CRITICAL. Default is CRITICAL")
 parser.add_argument("--logfile", action="store", required=False, default=None,
                     help="path of the log file. If not defined, logs will not be written to the file.")
 
 
 def launch(args):
     help.ogler.level = logging.getLevelName(args.loglevel)
-    if(args.logfile != None):
+    if args.logfile is not None:
         help.ogler.headDirPath = args.logfile
         help.ogler.reopen(name=args.name, temp=False, clear=True)
     logger = help.ogler.getLogger()
 
     logger.info("\n******* Starting Witness for %s listening: http/%s, tcp/%s "
                 ".******\n\n", args.name, args.http, args.tcp)
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/commands/witness/submit.py` & `keri-1.2.0.dev1/src/keri/app/cli/commands/witness/submit.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,34 +6,39 @@
 import argparse
 
 from hio import help
 from hio.base import doing
 
 from keri.app import habbing, agenting, indirecting
 from keri.app.cli.common import existing, displaying
+from keri.help import helping
 
 logger = help.ogler.getLogger()
 
 parser = argparse.ArgumentParser(description='Submit current event to witnesses for receipting')
 parser.set_defaults(handler=lambda args: handler(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', required=True)
 parser.add_argument("--config", "-c", help="directory override for configuration data")
 
 # Authentication for keystore
-parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
+parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument('--aeid', help='qualified base64 of non-transferable identifier prefix for  authentication '
                                    'and encryption of secrets in keystore', default=None)
 parser.add_argument('--force', action="store_true", required=False,
                     help='True means to send witnesses all receipts even if we have a full compliment of receipts for '
                          'the current event')
+parser.add_argument("--receipt-endpoint", help="Attempt to connect to witness receipt endpoint for witness receipts.",
+                    dest="endpoint", action='store_true')
+parser.add_argument("--authenticate", '-z', help="Prompt the controller for authentication codes for each witness",
+                    action='store_true')
 
 
 def handler(args):
     """
     Submit KERI identifier prefix to its witnesses for receipts.
 
     Args:
@@ -42,61 +47,79 @@
 
     name = args.name
     base = args.base
     bran = args.bran
     alias = args.alias
     force = args.force
 
-    icpDoer = InceptDoer(name=name, base=base, alias=alias, bran=bran, force=force)
+    subDoer = SubmitDoer(name=name, base=base, alias=alias, bran=bran, force=force, authenticate=args.authenticate,
+                         endpoint=args.endpoint)
 
-    doers = [icpDoer]
+    doers = [subDoer]
     return doers
 
 
-class InceptDoer(doing.DoDoer):
+class SubmitDoer(doing.DoDoer):
     """ DoDoer for creating a new identifier prefix and Hab with an alias.
     """
 
-    def __init__(self, name, base, alias, bran, force):
+    def __init__(self, name, base, alias, bran, force, endpoint=False, authenticate=False):
 
         hby = existing.setupHby(name=name, base=base, bran=bran)
         self.hbyDoer = habbing.HaberyDoer(habery=hby)  # setup doer
         self.mbx = indirecting.MailboxDirector(hby=hby, topics=['/receipt', "/replay", "/reply"])
         self.alias = alias
         self.hby = hby
         self.force = force
+        self.endpoint = endpoint
+        self.authenticate = authenticate
 
-        self.witDoer = None
-        doers = [self.hbyDoer, self.mbx, doing.doify(self.inceptDo)]
+        doers = [self.hbyDoer, self.mbx, doing.doify(self.submitDo)]
 
-        super(InceptDoer, self).__init__(doers=doers)
+        super(SubmitDoer, self).__init__(doers=doers)
 
-    def inceptDo(self, tymth, tock=0.0):
+    def submitDo(self, tymth, tock=0.0):
         """
         Parameters:
             tymth (function): injected function wrapper closure returned by .tymen() of
                 Tymist instance. Calling tymth() returns associated Tymist .tyme.
             tock (float): injected initial tock value
 
         Returns:  doifiable Doist compatible generator method
         """
         # enter context
         self.wind(tymth)
         self.tock = tock
         _ = (yield self.tock)
 
         hab = self.hby.habByName(name=self.alias)
-        self.witDoer = agenting.WitnessReceiptor(hby=self.hby, force=self.force)
-        self.extend([self.witDoer])
+        auths = {}
+        if self.authenticate:
+            for wit in hab.kever.wits:
+                code = input(f"Entire code for {wit}: ")
+                auths[wit] = f"{code}#{helping.nowIso8601()}"
+
+        if self.endpoint:
+            receiptor = agenting.Receiptor(hby=self.hby)
+            self.extend([receiptor])
+
+            yield from receiptor.receipt(hab.pre, sn=hab.kever.sn, auths=auths)
+            self.remove([receiptor])
+
+        else:
+            witDoer = agenting.WitnessReceiptor(hby=self.hby, force=self.force, auths=auths)
+            self.extend([witDoer])
+
+            if hab.kever.wits:
+                print("Waiting for witness receipts...")
+                witDoer.msgs.append(dict(pre=hab.pre))
+                while not witDoer.cues:
+                    _ = yield self.tock
 
-        if hab.kever.wits:
-            print("Waiting for witness receipts...")
-            self.witDoer.msgs.append(dict(pre=hab.pre))
-            while not self.witDoer.cues:
-                _ = yield self.tock
+            self.remove([witDoer])
 
         displaying.printIdentifier(self.hby, hab.pre)
 
-        toRemove = [self.hbyDoer, self.witDoer, self.mbx]
+        toRemove = [self.hbyDoer, self.mbx]
         self.remove(toRemove)
 
         return
```

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/common/config.py` & `keri-1.2.0.dev1/src/keri/app/cli/common/config.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/common/displaying.py` & `keri-1.2.0.dev1/src/keri/app/cli/common/displaying.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/common/existing.py` & `keri-1.2.0.dev1/src/keri/app/cli/common/existing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/common/incepting.py` & `keri-1.2.0.dev1/src/keri/app/cli/common/incepting.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/common/rotating.py` & `keri-1.2.0.dev1/src/keri/app/cli/common/rotating.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/cli/kli.py` & `keri-1.2.0.dev1/src/keri/app/cli/kli.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/configing.py` & `keri-1.2.0.dev1/src/keri/app/configing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/connecting.py` & `keri-1.2.0.dev1/src/keri/app/connecting.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/delegating.py` & `keri-1.2.0.dev1/src/keri/app/delegating.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from hio import help
 from hio.base import doing
 
 from . import agenting, forwarding
 from .habbing import GroupHab
 from .. import kering
-from ..core import coring, eventing, serdering
+from ..core import coring, serdering
 from ..db import dbing
 from ..peer import exchanging
 
 logger = help.ogler.getLogger()
 
 
 class Anchorer(doing.DoDoer):
@@ -158,15 +158,15 @@
                 seqner = coring.Seqner(sn=dserder.sn)
                 couple = seqner.qb64b + dserder.saidb
                 dgkey = dbing.dgKey(kever.prefixer.qb64b, kever.serder.saidb)
                 self.hby.db.setAes(dgkey, couple)  # authorizer event seal (delegator/issuer)
                 self.witDoer.msgs.append(dict(pre=pre, sn=serder.sn))
 
                 # Move to escrow waiting for witness receipts
-                print(f"Waiting for fully signed witness receipts for {serder.sn}")
+                logger.info(f"Waiting for fully signed witness receipts for {serder.sn}")
                 self.hby.db.dpwe.pin(keys=(pre, said), val=serder)
                 self.hby.db.dune.rem(keys=(pre, said))
 
     def processPartialWitnessEscrow(self):
         """
         Process escrow of delegated events that do not have a full compliment of receipts
         from witnesses yet.  When receipting is complete, remove from escrow and cue up a message
@@ -184,15 +184,15 @@
                 if len(kever.wits) > 0:
                     witnessed = False
                     for cue in self.witDoer.cues:
                         if cue["pre"] == serder.pre and cue["sn"] == seqner.sn:
                             witnessed = True
                     if not witnessed:
                         continue
-                print(f"Witness receipts complete, {pre} confirmed.")
+                logger.info(f"Witness receipts complete, {pre} confirmed.")
                 self.hby.db.dpwe.rem(keys=(pre, said))
                 self.hby.db.cdel.put(keys=(pre, seqner.qb64), val=coring.Saider(qb64=serder.said))
 
 
 def loadHandlers(hby, exc, notifier):
     """ Load handlers for the peer-to-peer delegation protocols
```

### Comparing `keri-1.2.0.dev0/src/keri/app/directing.py` & `keri-1.2.0.dev1/src/keri/app/directing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/forwarding.py` & `keri-1.2.0.dev1/src/keri/app/forwarding.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/grouping.py` & `keri-1.2.0.dev1/src/keri/app/grouping.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             saider (Saider): saider of event of group identifier
 
         """
         evt = ghab.makeOwnEvent(sn=seqner.sn, allowPartiallySigned=True)
         serder = serdering.SerderKERI(raw=evt)
         del evt[:serder.size]
 
-        print(f"Waiting for other signatures for {serder.pre}:{seqner.sn}...")
+        logger.info(f"Waiting for other signatures for {serder.pre}:{seqner.sn}...")
         return self.hby.db.gpse.add(keys=(prefixer.qb64,), val=(seqner, saider))
 
     def complete(self, prefixer, seqner, saider=None):
         """ Check for completed multsig protocol for the specific event
 
         Parameters:
             prefixer (Prefixer): qb64 identifier prefix of event to check
@@ -129,32 +129,32 @@
 
                 # True if Elected to perform delegation and witnessing
                 witered = ghab.mhab.kever.verfers[0].qb64 == keys[windex]
 
                 if kever.delegated and kever.ilk in (coring.Ilks.dip, coring.Ilks.drt):
                     # We are a delegated identifier, must wait for delegator approval for dip and drt
                     if witered:  # We are elected to perform delegation and witnessing messaging
-                        print(f"We are the witnesser, sending {pre} to delegator")
+                        logger.info(f"We are the witnesser, sending {pre} to delegator")
                         self.swain.delegation(pre=pre, sn=seqner.sn)
                     else:
                         anchor = dict(i=pre, s=seqner.snh, d=saider.qb64)
                         if self.proxy:
                             self.witq.query(hab=self.proxy, pre=kever.delpre, anchor=anchor)
                         else:
                             self.witq.query(src=ghab.mhab.pre, pre=kever.delpre, anchor=anchor)
 
-                    print("Waiting for delegation approval...")
+                    logger.info("Waiting for delegation approval...")
                     self.hby.db.gdee.add(keys=(pre,), val=(seqner, saider))
                 else:  # Non-delegation, move on to witnessing
                     if witered:  # We are elected witnesser, send off event to witnesses
-                        print(f"We are the fully signed witnesser {seqner.sn}, sending to witnesses")
+                        logger.info(f"We are the fully signed witnesser {seqner.sn}, sending to witnesses")
                         self.witDoer.msgs.append(dict(pre=pre, sn=seqner.sn))
 
                     # Move to escrow waiting for witness receipts
-                    print(f"Waiting for fully signed witness receipts for {seqner.sn}")
+                    logger.info(f"Waiting for fully signed witness receipts for {seqner.sn}")
                     self.hby.db.gpwe.add(keys=(pre,), val=(seqner, saider))
 
     def processDelegateEscrow(self):
         """
         Process escrow of delegate group multisig identifiers that are
         waiting for delegator approval of a recent establishment event.
 
@@ -166,29 +166,29 @@
 
             keys = [verfer.qb64 for verfer in kever.verfers]
             witer = ghab.mhab.kever.verfers[0].qb64 == keys[0]  # We are elected to perform delegation and witnessing
 
             if witer:  # We are elected witnesser, We've already done out part in Boatswain, we are done.
                 if self.swain.complete(prefixer=kever.prefixer, seqner=coring.Seqner(sn=kever.sn)):
                     self.hby.db.gdee.rem(keys=(pre,))
-                    print(f"Delegation approval for {pre} received.")
+                    logger.info(f"Delegation approval for {pre} received.")
 
                     self.hby.db.cgms.put(keys=(pre, seqner.qb64), val=saider)
 
             else:  # Not witnesser, we need to look for the anchor and then wait for receipts
                 if serder := self.hby.db.findAnchoringSealEvent(kever.delpre, seal=anchor):
                     aseq = coring.Seqner(sn=serder.sn)
                     couple = aseq.qb64b + serder.saidb
                     dgkey = dbing.dgKey(pre, saider.qb64b)
                     self.hby.db.setAes(dgkey, couple)  # authorizer event seal (delegator/issuer)
                     self.hby.db.gdee.rem(keys=(pre,))
-                    print(f"Delegation approval for {pre} received.")
+                    logger.info(f"Delegation approval for {pre} received.")
 
                     # Move to escrow waiting for witness receipts
-                    print(f"Waiting for witness receipts for {pre}")
+                    logger.info(f"Waiting for witness receipts for {pre}")
                     self.hby.db.gdee.rem(keys=(pre,))
                     self.hby.db.gpwe.add(keys=(pre,), val=(seqner, saider))
 
     def processPartialWitnessEscrow(self):
         """
         Process escrow of group multisig events that do not have a full compliment of receipts
         from witnesses yet.  When receipting is complete, remove from escrow and cue up a message
@@ -208,15 +208,15 @@
                 if witer and len(kever.wits) > 0:
                     witnessed = False
                     for cue in self.witDoer.cues:
                         if cue["pre"] == ghab.pre and cue["sn"] == seqner.sn:
                             witnessed = True
                     if not witnessed:
                         continue
-                print(f"Witness receipts complete, {pre} confirmed.")
+                logger.info(f"Witness receipts complete, {pre} confirmed.")
                 self.hby.db.gpwe.rem(keys=(pre,))
                 self.hby.db.cgms.put(keys=(pre, seqner.qb64), val=saider)
             elif not witer:
                 self.witDoer.gets.append(dict(pre=pre, sn=seqner.sn))
 
 
 class MultisigNotificationHandler:
```

### Comparing `keri-1.2.0.dev0/src/keri/app/habbing.py` & `keri-1.2.0.dev1/src/keri/app/habbing.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from hio.base import doing
 from hio.help import hicting
 
 from keri.peer import exchanging
 from . import keeping, configing
 from .. import help
 from .. import kering
+from .. import core
 from ..core import coring, eventing, parsing, routing, serdering, indexing
 from ..db import dbing, basing
 from ..kering import MissingSignatureError, Roles
 
 logger = help.ogler.getLogger()
 
 @contextmanager
@@ -53,26 +54,27 @@
             another device from the device that runs the Manager.
         aeid (str): qb64 of non-transferable identifier prefix for
             authentication and encryption of secrets in keeper. If provided
             aeid (not None) and different from aeid stored in database then
             all secrets are re-encrypted using new aeid. In this case the
             provided prikey must not be empty. A change in aeid should require
             a second authentication mechanism besides the prikey.
-        bran (str): Base64 22 char string that is used as base material for
-            seed. bran allows alphanumeric passcodes generated by key managers
-            like 1password to be key store for seed.
+        bran (str): Base64 char string of which first 21 chars are used as
+            base material for seed. bran allows alphanumeric passcodes
+            generated by key managers like 1password to be key store for
+            bran as salt base material for seed.
         pidx (int): Initial prefix index for vacuous ks
         algo (str): algorithm (randy or salty) for creating key pairs
             default is root algo which defaults to salty
         tier (str): security tier for generating keys from salt (Tierage)
         free (boo): free resources by closing on Doer exit if any
 
     """
     habery = None
-    salt = salt if salt is not None else coring.Salter().qb64
+    salt = salt if salt is not None else core.Salter().qb64
     try:
         habery = Habery(name=name, base=base, temp=temp, salt=salt, **kwa)
         yield habery
 
     finally:
         if habery:
             habery.close(clear=habery.temp)
@@ -91,15 +93,15 @@
         in base/name
         salt(bytes): passed to habitat to use for inception raw salt not qb64
         temp(bool): indicates if this uses temporary databases
         cf(Configer): optional configer for loading configuration data
 
     """
 
-    salt = coring.Salter(raw=salt).qb64
+    salt = core.Salter(raw=salt).qb64
 
     with openHby(name=name, base=base, salt=salt, temp=temp, cf=cf) as hby:
         if (hab := hby.habByName(name)) is None:
             hab = hby.makeHab(name=name, icount=1, isith='1', ncount=1, nsith='1', **kwa)
 
         yield hby, hab
 
@@ -180,17 +182,18 @@
                 another device from the device that runs the Manager.
             aeid (str): qb64 of non-transferable identifier prefix for
                 authentication and encryption of secrets in keeper. If provided
                 aeid (not None) and different from aeid stored in database then
                 all secrets Haberyare re-encrypted using new aeid. In this case the
                 provided prikey must not be empty. A change in aeid should require
                 a second authentication mechanism besides the prikey.
-            bran (str): Base64 22 char string that is used as base material for
-                seed. bran allows alphanumeric passcodes generated by key managers
-                like 1password to be key store for seed.
+            bran (str): Base64 char string of which first 21 chars are used as
+                base material for seed. bran allows alphanumeric passcodes
+                generated by key managers like 1password to be key store for
+                bran as salt base material for seed.
             pidx (int): Initial prefix index for vacuous ks
             algo (str): algorithm (randy or salty) for creating key pairs
                 default is root algo which defaults to salty
             salt (str): qb64 salt for creating key pairs
             tier (str): security tier for generating keys from salt (Tierage)
             free (boo): free resources by closing on Doer exit if any
             temp (bool): See above
@@ -284,25 +287,25 @@
                                      "database, .ks or .db.")
         self.free = True if free else False
 
         if bran and not seed:  # create seed from stretch of bran as salt
             if len(bran) < 21:
                 raise ValueError(f"Bran (passcode seed material) too short.")
             bran = coring.MtrDex.Salt_128 + 'A' + bran[:21]  # qb64 salt for seed
-            signer = coring.Salter(qb64=bran).signer(transferable=False,
+            signer = core.Salter(qb64=bran).signer(transferable=False,
                                                      tier=tier,
                                                      temp=temp)
             seed = signer.qb64
             if not aeid:  # aeid must not be empty event on initial creation
                 aeid = signer.verfer.qb64  # lest it remove encryption
 
         if salt is None:  # salt for signing keys not aeid seed
-            salt = coring.Salter().qb64
+            salt = core.Salter().qb64
         else:
-            salt = coring.Salter(qb64=salt).qb64
+            salt = core.Salter(qb64=salt).qb64
 
         try:
             self.mgr = keeping.Manager(ks=self.ks, seed=seed, aeid=aeid, pidx=pidx,
                                        algo=algo, salt=salt, tier=tier)
         except kering.AuthError as ex:
             self.close()
             raise ex
@@ -2077,16 +2080,17 @@
             cue = cues.pull() #cues.popleft()
             cueKin = cue["kin"]  # type or kind of cue
 
             if cueKin in ("receipt",):  # cue to receipt a received event from other pre
                 cuedSerder = cue["serder"]  # Serder of received event for other pre
                 cuedKed = cuedSerder.ked
                 cuedPrefixer = coring.Prefixer(qb64=cuedKed["i"])
-                logger.info("%s got cue: kin=%s\n%s\n\n", self.pre, cueKin,
-                            json.dumps(cuedKed, indent=1))
+                logger.info("%s got cue: kin=%s%s", self.pre, cueKin,
+                            cuedSerder.said)
+                logger.debug(f"event=\n{cuedSerder.pretty()}\n")
 
                 if cuedKed["t"] == coring.Ilks.icp:
                     dgkey = dbing.dgKey(self.pre, self.iserder.said)
                     found = False
                     if cuedPrefixer.transferable:  # find if have rct from other pre for own icp
                         for quadruple in self.db.getVrcsIter(dgkey):
                             if bytes(quadruple).decode("utf-8").startswith(cuedKed["i"]):
```

### Comparing `keri-1.2.0.dev0/src/keri/app/httping.py` & `keri-1.2.0.dev1/src/keri/app/httping.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 keri.peer.httping module
 
 """
 import datetime
 import json
 from dataclasses import dataclass
 from urllib import parse
-from urllib.parse import urlparse
+from pathlib import Path
 
 import falcon
 from hio.base import doing
 from hio.core import http
 from hio.help import Hict
 
 from keri import help
@@ -148,29 +148,30 @@
         method="POST",
         path=path,
         headers=headers,
         body=body
     )
 
 
-def streamCESRRequests(client, ims, dest, path=None):
+def streamCESRRequests(client, ims, dest, path=None, headers=None):
     """
     Turns a stream of KERI messages into CESR http requests against the provided hio http Client
 
     Parameters
        client (Client): hio http Client that will send the message as a CESR request
        ims (bytearray):  stream of KERI messages parsable as Serder.raw
        dest (str): qb64 identifier prefix of destination controller
        path (str): path to post to
 
     Returns
        int: Number of individual requests posted
 
     """
     path = path if path is not None else "/"
+    path = str(Path(client.requester.path) / path)
 
     cold = kering.sniff(ims)  # check for spurious counters at front of stream
     if cold in (parsing.Colds.txt, parsing.Colds.bny):  # not message error out to flush stream
         # replace with pipelining here once CESR message format supported.
         raise kering.ColdStartError("Expecting message counter tritet={}"
                                     "".format(cold))
 
@@ -187,25 +188,27 @@
         attachment = bytearray()
         while ims and ims[0] != 0x7b:  # not new message so process attachments, must support CBOR and MsgPack
             attachment.append(ims[0])
             del ims[:1]
 
         body = serder.raw
 
-        headers = Hict([
+        headers = headers if headers is not None else Hict()
+        heads = (Hict([
             ("Content-Type", CESR_CONTENT_TYPE),
             ("Content-Length", len(body)),
             (CESR_ATTACHMENT_HEADER, attachment),
             (CESR_DESTINATION_HEADER, dest)
-        ])
+        ]))
+        heads.update(headers)
 
         client.request(
             method="POST",
             path=path,
-            headers=headers,
+            headers=heads,
             body=body
         )
         cnt += 1
 
     return cnt
```

### Comparing `keri-1.2.0.dev0/src/keri/app/indirecting.py` & `keri-1.2.0.dev1/src/keri/app/indirecting.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,15 @@
             add result of doify on this method to doers list
         """
         self.wind(tymth)
         self.tock = tock
         _ = (yield self.tock)
 
         if self.parser.ims:
-            logger.info("Client %s received:\n%s\n...\n", self.kvy, self.parser.ims[:1024])
+            logger.debug("Client %s received:\n%s\n...\n", self.kvy, self.parser.ims[:1024])
         done = yield from self.parser.parsator(local=True)  # process messages continuously
         return done  # should nover get here except forced close
 
     def escrowDo(self, tymth=None, tock=0.0):
         """
          Returns doifiable Doist compatibile generator method (doer dog) to process
             .kevery and .tevery escrows.
@@ -377,15 +377,15 @@
             add result of doify on this method to doers list
         """
         self.wind(tymth)
         self.tock = tock
         _ = (yield self.tock)
 
         if self.parser.ims:
-            logger.info("Client %s received:\n%s\n...\n", self.hab.pre, self.parser.ims[:1024])
+            logger.debug("Client %s received:\n%s\n...\n", self.hab.pre, self.parser.ims[:1024])
         done = yield from self.parser.parsator(local=True)  # process messages continuously
         return done  # should nover get here except forced close
 
     def cueDo(self, tymth=None, tock=0.0):
         """
          Returns doifiable Doist compatibile generator method (doer dog) to process
             .kevery.cues deque
@@ -440,15 +440,15 @@
             yield
 
     def sendMessage(self, msg, label=""):
         """
         Sends message msg and loggers label if any
         """
         self.client.tx(msg)  # send to remote
-        logger.info("%s sent %s:\n%s\n\n", self.hab.pre, label, bytes(msg))
+        logger.debug("%s sent %s:\n%s\n\n", self.hab.pre, label, bytes(msg))
 
 
 class MailboxDirector(doing.DoDoer):
     """
     Class for Indirect Mode KERI Controller Doer with habitat and
     TCP Clients for talking to witnesses
```

### Comparing `keri-1.2.0.dev0/src/keri/app/keeping.py` & `keri-1.2.0.dev1/src/keri/app/keeping.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from collections import namedtuple, deque
 from dataclasses import dataclass, asdict, field
 
 import pysodium
 from hio.base import doing
 
 from .. import kering
+from .. import core
 from ..core import coring
 from ..db import dbing, subing, koming
 from ..help import helping
 
 Algoage = namedtuple("Algoage", 'randy salty group extern')
 Algos = Algoage(randy='randy', salty='salty', group="group", extern="extern")  # randy is rerandomize, salty is use salt
 
@@ -263,18 +264,18 @@
         # Names end with "." as sub DB name must include a non Base64 character
         # to avoid namespace collisions with Base64 identifier prefixes.
 
         self.gbls = subing.Suber(db=self, subkey='gbls.')
         self.pris = subing.CryptSignerSuber(db=self, subkey='pris.')
         self.prxs = subing.CesrSuber(db=self,
                                      subkey='prxs.',
-                                     klas=coring.Cipher)
+                                     klas=core.Cipher)
         self.nxts = subing.CesrSuber(db=self,
                                      subkey='nxts.',
-                                     klas=coring.Cipher)
+                                     klas=core.Cipher)
         self.smids = subing.CatCesrIoSetSuber(db=self,
                                               subkey='smids.',
                                               klas=(coring.Prefixer, coring.Seqner))
         self.rmids = subing.CatCesrIoSetSuber(db=self,
                                               subkey='rmids.',
                                               klas=(coring.Prefixer, coring.Seqner))
         self.pres = subing.CesrSuber(db=self,
@@ -440,15 +441,15 @@
             transferable is Boolean, True means use trans deriv code. Otherwise nontrans
         """
         signers = []
         if not codes:  # if not codes make list len count of same code
             codes = [code for i in range(count)]
 
         for code in codes:
-            signers.append(coring.Signer(code=code, transferable=transferable))
+            signers.append(core.Signer(code=code, transferable=transferable))
         return signers
 
 
 class SaltyCreator(Creator):
     """
     Class for creating a key pair based on random salt plus path stretch algorithm.
 
@@ -473,15 +474,15 @@
             salt is unique salt from which to derive private key
             stem is path modifier used with salt to derive private keys.
                     if stem is None then uses pidx
             tier is derivation criticality that determines how much hashing to use.
 
         """
         super(SaltyCreator, self).__init__(**kwa)
-        self.salter = coring.Salter(qb64=salt, tier=tier)
+        self.salter = core.Salter(qb64=salt, tier=tier)
         self._stem = stem if stem is not None else ''
 
     @property
     def salt(self):
         """
         salt property getter
         """
@@ -592,17 +593,17 @@
 
 class Manager:
     """Manages key pairs creation, storage, and signing
     Class for managing key pair creation, storage, retrieval, and message signing.
 
     Attributes:
         ks (Keeper): key store LMDB database instance for storing public and private keys
-        encrypter (coring.Encrypter): instance for encrypting secrets. Public
+        encrypter (core.Encrypter): instance for encrypting secrets. Public
             encryption key is derived from aeid (public signing key)
-        decrypter (coring.Decrypter): instance for decrypting secrets. Private
+        decrypter (core.Decrypter): instance for decrypting secrets. Private
             decryption key is derived seed (private signing key seed)
         inited (bool): True means fully initialized wrt database.
                           False means not yet fully initialized
 
     Attributes (Hidden):
 
         _seed (str): qb64 private-signing key (seed) for the aeid from which
@@ -720,21 +721,21 @@
         if aeid is None:
             aeid = ''
         if pidx is None:
             pidx = 0
         if algo is None:
             algo = Algos.salty
         if salt is None:
-            salt = coring.Salter().qb64
+            salt = core.Salter().qb64
         else:
-            if coring.Salter(qb64=salt).qb64 != salt:
+            if core.Salter(qb64=salt).qb64 != salt:
                 raise ValueError(f"Invalid qb64 for salt={salt}.")
 
         if tier is None:
-            tier = coring.Tiers.low
+            tier = core.Tiers.low
 
         # update  database if never before initialized
         if self.pidx is None:  # never before initialized
             self.pidx = pidx  # init to default
 
         if self.algo is None:  # never before initialized
             self.algo = algo
@@ -745,21 +746,21 @@
         if self.tier is None:  # never before initialized
             self.tier = tier  # init to default
 
         # must do this after salt is initialized so gets re-encrypted correctly
         if not self.aeid:  # never before initialized
             self.updateAeid(aeid, self.seed)
         else:
-            self.encrypter = coring.Encrypter(verkey=self.aeid)  # derive encrypter from aeid
+            self.encrypter = core.Encrypter(verkey=self.aeid)  # derive encrypter from aeid
             if not self.seed or not self.encrypter.verifySeed(self.seed):
                 raise kering.AuthError("Last seed missing or provided last seed "
                                        "not associated with last aeid={}."
                                        "".format(self.aeid))
 
-            self.decrypter = coring.Decrypter(seed=self.seed)
+            self.decrypter = core.Decrypter(seed=self.seed)
 
         self.inited = True
 
     def updateAeid(self, aeid, seed):
         """
         Given seed belongs to aeid and encrypter, update aeid and re-encrypt all
         secrets
@@ -777,15 +778,15 @@
             if not self.seed or not self.encrypter.verifySeed(self.seed):
                 raise kering.AuthError("Last seed missing or provided last seed "
                                        "not associated with last aeid={}."
                                        "".format(self.aeid))
 
         if aeid:  # aeid provided
             if aeid != self.aeid:  # changing to a new aeid so update .encrypter
-                self.encrypter = coring.Encrypter(verkey=aeid)  # derive encrypter from aeid
+                self.encrypter = core.Encrypter(verkey=aeid)  # derive encrypter from aeid
                 # verifies new seed belongs to new aeid
                 if not seed or not self.encrypter.verifySeed(seed):
                     raise kering.AuthError("Seed missing or provided seed not associated"
                                            "  with provided aeid={}.".format(aeid))
         else:  # changing to empty aeid so new encrypter is None
             self.encrypter = None
 
@@ -813,15 +814,15 @@
             for keys, signer in self.ks.pris.getItemIter(decrypter=self.decrypter):
                 self.ks.pris.pin(keys, signer, encrypter=self.encrypter)
 
         self.ks.gbls.pin("aeid", aeid)  # set aeid in db
         self._seed = seed  # set .seed in memory
 
         # update .decrypter
-        self.decrypter = coring.Decrypter(seed=seed) if seed else None
+        self.decrypter = core.Decrypter(seed=seed) if seed else None
 
 
     @property
     def seed(self):
         """
         seed property getter from ._seed.
         seed (str): qb64 from which aeid is derived
@@ -1181,15 +1182,15 @@
         salt = pp.salt
         if salt:
             if self.aeid:
                 if not self.decrypter:
                     raise kering.DecryptError("Unauthorized decryption. Aeid but no decrypter.")
                 salt = self.decrypter.decrypt(ser=salt).qb64
             else:
-                salt = coring.Salter(qb64=salt).qb64  # ensures salt was unencrypted
+                salt = core.Salter(qb64=salt).qb64  # ensures salt was unencrypted
 
         creator = Creatory(algo=pp.algo).make(salt=salt, stem=pp.stem, tier=pp.tier)
 
         if not ncodes:  # all same code, make list of len count of same code
             if ncount < 0:  # next may be zero if non-trans
                 raise ValueError("Invalid count={} must be >= 0.".format(ncount))
             ncodes = [ncode for i in range(ncount)]
@@ -1527,15 +1528,15 @@
         kidx = 0
 
         verferies = []  # list of lists of verfers
         first = True
         secrecies = deque(secrecies)
         while secrecies:
             csecrets = secrecies.popleft()  # current
-            csigners = [coring.Signer(qb64=secret, transferable=transferable)
+            csigners = [core.Signer(qb64=secret, transferable=transferable)
                                                       for secret in csecrets]
             csize = len(csigners)
             verferies.append([signer.verfer for signer in csigners])
 
             if first:
                 # Secret to encrypt here
                 pp = PrePrm(pidx=pidx,
```

### Comparing `keri-1.2.0.dev0/src/keri/app/notifying.py` & `keri-1.2.0.dev1/src/keri/app/notifying.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/oobiing.py` & `keri-1.2.0.dev1/src/keri/app/oobiing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/querying.py` & `keri-1.2.0.dev1/src/keri/app/querying.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/signaling.py` & `keri-1.2.0.dev1/src/keri/app/signaling.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/signing.py` & `keri-1.2.0.dev1/src/keri/app/signing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/specing.py` & `keri-1.2.0.dev1/src/keri/app/specing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/app/storing.py` & `keri-1.2.0.dev1/src/keri/app/storing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/core/coring.py` & `keri-1.2.0.dev1/src/keri/core/coring.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,15 +43,16 @@
                       TraitDex, )
 
 from ..help import helping
 from ..help.helping import sceil, nonStringIterable, nonStringSequence
 from ..help.helping import (intToB64, intToB64b, b64ToInt, B64_CHARS,
                             codeB64ToB2, codeB2ToB64, Reb64, nabSextets)
 
-from . import indexing
+
+
 
 
 DSS_SIG_MODE = "fips-186-3"
 ECDSA_256r1_SEEDBYTES = 32
 ECDSA_256k1_SEEDBYTES = 32
 
 
@@ -179,49 +180,14 @@
     else:
         raise DeserializeError("Invalid deserialization kind: {}"
                                    "".format(kind))
 
     return ked
 
 
-def generateSigners(raw=None, count=8, transferable=True):
-    """Returns list of Signers for Ed25519
-
-    Deprecated, use Salter.signers instead.
-
-    Use this when simply need valid AIDs but not when need valid controller
-    contexts. In the latter case use openHby or openHab which create databases.
-
-    Parameters:
-        raw (bytes):  16 byte long salt cryptomatter from which seeds
-            for Signers in list are derived
-            random salt created if not provided
-        count is number of signers in list
-        transferable is boolean true means signer.verfer code is transferable
-                                non-transferable otherwise
-    """
-    if not raw:
-        raw = pysodium.randombytes(pysodium.crypto_pwhash_SALTBYTES)
-
-    signers = []
-    for i in range(count):
-        path = f"{i:x}"
-        # algorithm default is argon2id
-        seed = pysodium.crypto_pwhash(outlen=32,
-                                      passwd=path,
-                                      salt=raw,
-                                      opslimit=2,  # pysodium.crypto_pwhash_OPSLIMIT_INTERACTIVE,
-                                      memlimit=67108864,  # pysodium.crypto_pwhash_MEMLIMIT_INTERACTIVE,
-                                      alg=pysodium.crypto_pwhash_ALG_ARGON2ID13)
-
-        signers.append(Signer(raw=seed, transferable=transferable))
-
-    return signers
-
-
 # ToDo: nonces only need 128 bits of entropy. a Salt is enough
 # Just use Salter().qb64.
 # Deprecated
 
 def randomNonce():
     """ Generate a random ed25519 seed and encode as qb64
 
@@ -238,14 +204,78 @@
 
 # secret derivation security tier
 Tierage = namedtuple("Tierage", 'low med high')
 
 Tiers = Tierage(low='low', med='med', high='high')
 
 
+
+@dataclass
+class MapHood:
+    """Base class for mutable dataclasses that support map syntax
+    Adds support for dunder methods for map syntax dc[name].
+    Converts exceptions from attribute syntax to raise map syntax when using
+    map syntax.
+
+    Enables dataclass instances to use Mapping item syntax
+    """
+
+    def __getitem__(self, name):
+        try:
+            return getattr(self, name)
+        except AttributeError as ex:
+            raise IndexError(ex.args) from ex
+
+
+    def __setitem__(self, name, value):
+        try:
+            return setattr(self, name, value)
+        except AttributeError as ex:
+            raise IndexError(ex.args) from ex
+
+
+    def __delitem__(self, name):
+        try:
+            return delattr(self, name)
+        except AttributeError as ex:
+            raise IndexError(ex.args) from ex
+
+
+@dataclass(frozen=True)
+class MapDom:
+    """Base class for frozen dataclasses (codexes) that support map syntax
+    Adds support for dunder methods for map syntax dc[name].
+    Converts exceptions from attribute syntax to raise map syntax when using
+    map syntax.
+
+    Enables dataclass instances to use Mapping item syntax
+    """
+
+    def __getitem__(self, name):
+        try:
+            return getattr(self, name)
+        except AttributeError as ex:
+            raise IndexError(ex.args) from ex
+
+
+    def __setitem__(self, name, value):
+        try:
+            return setattr(self, name, value)
+        except AttributeError as ex:
+            raise IndexError(ex.args) from ex
+
+
+    def __delitem__(self, name):
+        try:
+            return delattr(self, name)
+        except AttributeError as ex:
+            raise IndexError(ex.args) from ex
+
+
+
 @dataclass(frozen=True)
 class MatterCodex:
     """
     MatterCodex is codex code (stable) part of all matter derivation codes.
     Only provide defined codes.
     Undefined are left out so that inclusion(exclusion) via 'in' operator works.
     """
@@ -331,20 +361,20 @@
     X25519_Cipher_Big_L2: str = '9AAC'  # X25519 sealed box cipher bytes of sniffable plaintext big lead size 2
     X25519_Cipher_QB64_L0:     str = '4D'  # X25519 sealed box cipher bytes of QB64 plaintext lead size 0
     X25519_Cipher_QB64_L1:     str = '5D'  # X25519 sealed box cipher bytes of QB64 plaintext lead size 1
     X25519_Cipher_QB64_L2:     str = '6D'  # X25519 sealed box cipher bytes of QB64 plaintext lead size 2
     X25519_Cipher_QB64_Big_L0: str = '7AAD'  # X25519 sealed box cipher bytes of QB64 plaintext big lead size 0
     X25519_Cipher_QB64_Big_L1: str = '8AAD'  # X25519 sealed box cipher bytes of QB64 plaintext big lead size 1
     X25519_Cipher_QB64_Big_L2: str = '9AAD'  # X25519 sealed box cipher bytes of QB64 plaintext big lead size 2
-    X25519_Cipher_QB2_L0:     str = '4D'  # X25519 sealed box cipher bytes of QB2 plaintext lead size 0
-    X25519_Cipher_QB2_L1:     str = '5D'  # X25519 sealed box cipher bytes of QB2 plaintext lead size 1
-    X25519_Cipher_QB2_L2:     str = '6D'  # X25519 sealed box cipher bytes of QB2 plaintext lead size 2
-    X25519_Cipher_QB2_Big_L0: str = '7AAD'  # X25519 sealed box cipher bytes of QB2 plaintext big lead size 0
-    X25519_Cipher_QB2_Big_L1: str = '8AAD'  # X25519 sealed box cipher bytes of QB2 plaintext big lead size 1
-    X25519_Cipher_QB2_Big_L2: str = '9AAD'  # X25519 sealed box cipher bytes of QB2 plaintext big lead size 2
+    X25519_Cipher_QB2_L0:     str = '4E'  # X25519 sealed box cipher bytes of QB2 plaintext lead size 0
+    X25519_Cipher_QB2_L1:     str = '5E'  # X25519 sealed box cipher bytes of QB2 plaintext lead size 1
+    X25519_Cipher_QB2_L2:     str = '6E'  # X25519 sealed box cipher bytes of QB2 plaintext lead size 2
+    X25519_Cipher_QB2_Big_L0: str = '7AAE'  # X25519 sealed box cipher bytes of QB2 plaintext big lead size 0
+    X25519_Cipher_QB2_Big_L1: str = '8AAE'  # X25519 sealed box cipher bytes of QB2 plaintext big lead size 1
+    X25519_Cipher_QB2_Big_L2: str = '9AAE'  # X25519 sealed box cipher bytes of QB2 plaintext big lead size 2
 
 
     def __iter__(self):
         return iter(astuple(self))  # enables inclusion test with "in"
 
 
 MtrDex = MatterCodex()  # Make instance
@@ -1332,27 +1362,31 @@
             raise InvalidCodeSizeError(f"Invalid full code={both} for raw size"
                                        f"={len(raw)}.")
         return full
 
 
     def _exfil(self, qb64b):
         """
-        Extracts self.code and self.raw from qualified base64 str or bytes qb64b
-        Detects is str and converts to bytes
+        Extracts self.code and self.raw from qualified base64 qb64b of type
+        str or bytes or bytearray or memoryview
+
+        Detects if str and converts to bytes
 
         Parameters:
-            qb64b (str | bytes | bytearray): fully qualified base64 from stream
+            qb64b (str | bytes | bytearray | memoryview): fully qualified base64 from stream
 
         """
         if not qb64b:  # empty need more bytes
             raise ShortageError("Empty material.")
 
         first = qb64b[:1]  # extract first char code selector
+        if isinstance(first, memoryview):
+            first = bytes(first)
         if hasattr(first, "decode"):
-            first = first.decode("utf-8")
+            first = first.decode()  # converts bytes/bytearray to str
         if first not in self.Hards:
             if first[0] == '-':
                 raise UnexpectedCountCodeError("Unexpected count code start"
                                                "while extracing Matter.")
             elif first[0] == '_':
                 raise UnexpectedOpCodeError("Unexpected  op code start"
                                             "while extracing Matter.")
@@ -1360,39 +1394,45 @@
                 raise UnexpectedCodeError(f"Unsupported code start char={first}.")
 
         hs = self.Hards[first]  # get hard code size
         if len(qb64b) < hs:  # need more bytes
             raise ShortageError(f"Need {hs - len(qb64b)} more characters.")
 
         hard = qb64b[:hs]  # extract hard code
+        if isinstance(hard, memoryview):
+            hard = bytes(hard)
         if hasattr(hard, "decode"):
-            hard = hard.decode("utf-8")  # converts bytes/bytearray to str
+            hard = hard.decode()  # converts bytes/bytearray to str
         if hard not in self.Sizes:
             raise UnexpectedCodeError(f"Unsupported code ={hard}.")
 
         hs, ss, fs, ls = self.Sizes[hard]  # assumes hs in both tables match
         cs = hs + ss  # both hs and ss
         # assumes that unit tests on Matter .Sizes .Hards and .Bards ensure that
         # these are well formed.
         # when fs is None then ss > 0 otherwise fs > hs + ss when ss > 0
 
         soft = qb64b[hs:hs + ss]  # extract soft chars, empty when ss==0
+        if isinstance(soft, memoryview):
+            soft = bytes(soft)
         if hasattr(soft, "decode"):
-            soft = soft.decode("utf-8")
+            soft = soft.decode()  # converts bytes/bytearray to str
 
         if not fs:  # compute fs from soft from ss part which provides size B64
             # compute variable size as int may have value 0
             fs = (b64ToInt(soft) * 4) + cs
 
         if len(qb64b) < fs:  # need more bytes
             raise ShortageError(f"Need {fs - len(qb64b)} more chars.")
 
         qb64b = qb64b[:fs]  # fully qualified primitive code plus material
+        if isinstance(qb64b, memoryview):
+            qb64b = bytes(qb64b)
         if hasattr(qb64b, "encode"):  # only convert extracted chars from stream
-            qb64b = qb64b.encode("utf-8")
+            qb64b = qb64b.encode()  # converts str to bytes
 
         # check for non-zeroed pad bits and/or lead bytes
         # net prepad ps == cs % 4 (remainer).  Assumes ps != 3 i.e ps in (0,1,2)
         # To ensure number of prepad bytes and prepad chars are same.
         # need net prepad chars ps to invert using decodeB64 of lead + raw
 
         ps = cs % 4  # net prepad bytes to ensure 24 bit align when encodeB64
@@ -1403,25 +1443,25 @@
         pi = int.from_bytes(paw[:ps+ls], "big")
         if pi != 0:
             raise ConversionError(f"Nonzero midpad bytes=0x{pi:0{(ps + ls) * 2}x}.")
 
         if len(raw) != ((len(qb64b) - cs) * 3 // 4) - ls:  # exact lengths
             raise ConversionError(f"Improperly qualified material = {qb64b}")
 
-        self._code = hard  # hard only
-        self._soft = soft  # soft only
+        self._code = hard  # hard only str
+        self._soft = soft  # soft only str
         self._raw = raw  # ensure bytes for crypto ops, may be empty
 
 
     def _bexfil(self, qb2):
         """
         Extracts self.code and self.raw from qualified base2 qb2
 
         Parameters:
-            qb2 (bytes | bytearray): fully qualified base2 from stream
+            qb2 (bytes | bytearray | memoryview): fully qualified base2 from stream
         """
         if not qb2:  # empty need more bytes
             raise ShortageError("Empty material, Need more bytes.")
 
         first = nabSextets(qb2, 1)  # extract first sextet as code selector
         if first not in self.Bards:
             if first[0] == b'\xf8':  # b64ToB2('-')
@@ -1632,16 +1672,22 @@
         qb2  (bytes): binary with derivation code + crypto material
         transferable (bool): True means transferable derivation code False otherwise
         digestive (bool): True means digest derivation code False otherwise
 
     Properties:
         num  (int): int representation of number
         humh (str): hex string representation of number with no leading zeros
+        sn (int): alias for num
+        snh (str): alias for numh
+        huge (str): qb64 of num but with code NumDex.Huge so 24 char compatible
+                    with fixed size seq num for lexicographic lmdb key space
         positive (bool): True if .num  > 0, False otherwise. Because .num must be
-            non-negative, .positive == False means .num == 0
+                         non-negative, .positive == False means .num == 0
+        inceptive (bool): True means .num == 0 False otherwise.
+
 
     Hidden:
         _code (str): value for .code property
         _raw (bytes): value for .raw property
         _rsize (bytes): value for .rsize property. Raw size in bytes when
             variable sized material else None.
         _size (int): value for .size property. Number of triplets of bytes
@@ -1652,19 +1698,21 @@
         _exfil (types.MethodType): extracts .code and .raw from qb64b
                                    (fully qualified Base64)
 
     Methods:
     """
 
     def __init__(self, raw=None, qb64b=None, qb64=None, qb2=None,
-                 code=NumDex.Short, num=None, numh=None, **kwa):
+                 code=None, num=None, numh=None, **kwa):
         """
         Inherited Parameters:  (see Matter)
             raw (bytes): unqualified crypto material usable for crypto operations
-            code (str): stable (hard) part of derivation code
+            code (str | None): stable (hard) part of derivation code.
+                               None means pick code based on value of num or numh
+                               otherwise raise error
             rize (int): raw size in bytes when variable sized material else None
             qb64b (bytes): fully qualified crypto material Base64
             qb64 (str, bytes):  fully qualified crypto material Base64
             qb2 (bytes): fully qualified crypto material Base2
             strip (bool): True means strip (delete) matter from input stream
             bytearray after parsing qb64b or qb2. False means do not strip
 
@@ -1689,41 +1737,48 @@
                         if num == '':
                             num = 0
                         else:
                             num = int(num, 16)
             except ValueError as ex:
                 raise InvalidValueError(f"Not whole number={num} .") from ex
 
-            if not isinstance(num, int) or num < 0:
-                raise InvalidValueError(f"Not whole number={num}.")
+            if code is None:  # dynamically size code
+                if not isinstance(num, int) or num < 0:
+                    raise InvalidValueError(f"Not whole number={num}.")
 
-            if num <= (256 ** 2 - 1):  # make short version of code
-                code = NumDex.Short
+                if num <= (256 ** 2 - 1):  # make short version of code
+                    code = NumDex.Short
 
-            elif num <= (256 ** 5 - 1):  # make tall version of code
-                code = code = NumDex.Tall
+                elif num <= (256 ** 5 - 1):  # make tall version of code
+                    code = code = NumDex.Tall
 
-            elif num <= (256 ** 8 - 1):  # make big version of code
-                code = code = NumDex.Big
+                elif num <= (256 ** 8 - 1):  # make big version of code
+                    code = code = NumDex.Big
 
-            elif num <= (256 ** 11 - 1):  # make large version of code
-                code = code = NumDex.Large
+                elif num <= (256 ** 11 - 1):  # make large version of code
+                    code = code = NumDex.Large
 
-            elif num <= (256 ** 14 - 1):  # make great version of code
-                code = code = NumDex.Great
+                elif num <= (256 ** 14 - 1):  # make great version of code
+                    code = code = NumDex.Great
 
-            elif num <= (256 ** 17 - 1):  # make vast version of code
-                code = code = NumDex.Vast
+                elif num <= (256 ** 17 - 1):  # make vast version of code
+                    code = code = NumDex.Vast
 
-            else:
-                raise InvalidValueError(f"Invalid num = {num}, too large to encode.")
+                else:
+                    raise InvalidValueError(f"Invalid num = {num}, too large to encode.")
 
             # default to_bytes parameter signed is False. If negative raises
             # OverflowError: can't convert negative int to unsigned
-            raw = num.to_bytes(Matter._rawSize(code), 'big')  # big endian unsigned
+            try:
+                raw = num.to_bytes(Matter._rawSize(code), 'big')  # big endian unsigned
+            except Exception as ex:
+                raise InvalidValueError(f"Not convertable to bytes {num=}.") from ex
+
+            if len(raw) > Matter._rawSize(code):
+                raise InvalidValueError(f"To big {num=} for {code=}.")
 
         super(Number, self).__init__(raw=raw, qb64b=qb64b, qb64=qb64, qb2=qb2,
                                      code=code, **kwa)
 
         if self.code not in NumDex:
             raise ValidationError(f"Invalid code = {self.code} for Number.")
 
@@ -1798,41 +1853,47 @@
         Returns:
             snh (hex str): alias for numh
         """
         return self.numh
 
 
     @property
+    def huge(self):
+        """Provides number value as qb64 but with code NumDex.huge. This is the
+        same as Seqner.qb64. Raises error if too big.
+
+        Returns:
+            huge (str): qb64 of num coded as NumDex.Huge
+        """
+        num = self.num
+        if num > MaxON:  # too big for ordinal 256 ** 16 - 1
+            raise InvalidValueError(f"Non-ordinal {num} exceeds {MaxON}.")
+
+        return Number(num=num, code=NumDex.Huge).qb64
+
+
+    @property
     def positive(self):
         """
         Returns True if .num is strictly positive non-zero False otherwise.
         Because valid number .num must be non-negative, positive False also means
         that .num is zero.
         """
         return True if self.num > 0 else False
 
 
     @property
     def inceptive(self):
         """
         Returns True if .num == 0 False otherwise.
-        Valid number .num must be non-negative,
+
         """
         return True if self.num == 0 else False
 
 
-    @property
-    def seqner(self):
-        """Seqner getter.
-
-        Returns:
-            seqner (Seqner): instance made from number
-        """
-        return Seqner(sn=self.sn)
-
 
 class Dater(Matter):
     """
     Dater is subclass of Matter, cryptographic material, for RFC-3339 profile of
     ISO-8601 formatted datetimes.
 
     Dater provides a custom Base64 coding of an ASCII RFC-3339 profile of an
@@ -3071,732 +3132,14 @@
 
     @verfer.setter
     def verfer(self, verfer):
         """ verfer property setter """
         self._verfer = verfer
 
 
-class Signer(Matter):
-    """
-    Signer is Matter subclass with method to create signature of serialization
-    using:
-        .raw as signing (private) key seed,
-        .code as cipher suite for signing
-        .verfer whose property .raw is public key for signing.
-
-    If not provided .verfer is generated from private key seed using .code
-    as cipher suite for creating key-pair.
-
-
-    See Matter for inherited attributes and properties:
-
-    Attributes:
-
-    Properties:  (inherited)
-        code (str): hard part of derivation code to indicate cypher suite
-        both (int): hard and soft parts of full text code
-        size (int): Number of triplets of bytes including lead bytes
-            (quadlets of chars) of variable sized material. Value of soft size,
-            ss, part of full text code.
-            Otherwise None.
-        rize (int): number of bytes of raw material not including
-                    lead bytes
-        raw (bytes): private signing key crypto material only without code
-        qb64 (str): private signing key Base64 fully qualified with
-                    derivation code + crypto mat
-        qb64b (bytes): private signing keyBase64 fully qualified with
-            derivation code + crypto mat
-        qb2  (bytes): private signing key binary with
-            derivation code + crypto material
-        transferable (bool): True means transferable derivation code False otherwise
-        digestive (bool): True means digest derivation code False otherwise
-
-    Properties:
-
-        .verfer is Verfer object instance of public key derived from private key
-            seed which is .raw
-
-    Methods:
-        sign: create signature
-
-    """
-
-    def __init__(self, raw=None, code=MtrDex.Ed25519_Seed, transferable=True, **kwa):
-        """
-        Assign signing cipher suite function to ._sign
-
-        Parameters:  See Matter for inherted parameters
-            raw is bytes crypto material seed or private key
-            code is derivation code
-            transferable is Boolean True means make verifier code transferable
-                                    False make non-transferable
-
-        """
-        try:
-            super(Signer, self).__init__(raw=raw, code=code, **kwa)
-        except EmptyMaterialError as ex:
-            if code == MtrDex.Ed25519_Seed:
-                raw = pysodium.randombytes(pysodium.crypto_sign_SEEDBYTES)
-                super(Signer, self).__init__(raw=raw, code=code, **kwa)
-            elif code == MtrDex.ECDSA_256r1_Seed:
-                raw = pysodium.randombytes(ECDSA_256r1_SEEDBYTES)
-                super(Signer, self).__init__(raw=bytes(raw), code=code, **kwa)
-            elif code == MtrDex.ECDSA_256k1_Seed:
-                raw = pysodium.randombytes(ECDSA_256k1_SEEDBYTES)
-                super(Signer, self).__init__(raw=bytes(raw), code=code, **kwa)
-
-            else:
-                raise ValueError("Unsupported signer code = {}.".format(code))
-
-        if self.code == MtrDex.Ed25519_Seed:
-            self._sign = self._ed25519
-            verkey, sigkey = pysodium.crypto_sign_seed_keypair(self.raw)
-            verfer = Verfer(raw=verkey,
-                            code=MtrDex.Ed25519 if transferable
-                            else MtrDex.Ed25519N)
-        elif self.code == MtrDex.ECDSA_256r1_Seed:
-            self._sign = self._secp256r1
-            d = int.from_bytes(self.raw, byteorder="big")
-            sigkey = ec.derive_private_key(d, ec.SECP256R1())
-            verkey = sigkey.public_key().public_bytes(encoding=Encoding.X962, format=PublicFormat.CompressedPoint)
-            verfer = Verfer(raw=verkey,
-                            code=MtrDex.ECDSA_256r1 if transferable
-                            else MtrDex.ECDSA_256r1N)
-        elif self.code == MtrDex.ECDSA_256k1_Seed:
-            self._sign = self._secp256k1
-            d = int.from_bytes(self.raw, byteorder="big")
-            sigkey = ec.derive_private_key(d, ec.SECP256K1())
-            verkey = sigkey.public_key().public_bytes(encoding=Encoding.X962, format=PublicFormat.CompressedPoint)
-            verfer = Verfer(raw=verkey,
-                            code=MtrDex.ECDSA_256k1 if transferable
-                            else MtrDex.ECDSA_256k1N)
-        else:
-            raise ValueError("Unsupported signer code = {}.".format(self.code))
-
-        self._verfer = verfer
-
-    @property
-    def verfer(self):
-        """
-        Property verfer:
-        Returns Verfer instance
-        Assumes ._verfer is correctly assigned
-        """
-        return self._verfer
-
-    def sign(self, ser, index=None, only=False, ondex=None, **kwa):
-        """
-        Returns either Cigar or Siger (indexed) instance of cryptographic
-        signature material on bytes serialization ser
-
-        If index is None
-            return Cigar instance
-        Else
-            return Siger instance
-
-        Parameters:
-            ser (bytes): serialization to be signed
-            index (int):  main index of associated verifier key in event keys
-            only (bool): True means main index only list, ondex ignored
-                          False means both index lists (default), ondex used
-            ondex (int | None): other index offset into list such as prior next
-
-        """
-        return (self._sign(ser=ser,
-                           seed=self.raw,
-                           verfer=self.verfer,
-                           index=index,
-                           only=only,
-                           ondex=ondex,
-                           **kwa))
-
-    @staticmethod
-    def _ed25519(ser, seed, verfer, index, only=False, ondex=None, **kwa):
-        """
-        Returns signature as either Cigar or Siger instance as appropriate for
-        Ed25519 digital signatures given index and ondex values
-
-        The seed's code determins the crypto key-pair algorithm and signing suite
-        The signature type, Cigar or Siger, and when indexed the Siger code
-        may be completely determined by the seed and index values (index, ondex)
-        by assuming that the index values are intentional.
-        Without the seed code its more difficult for Siger to
-        determine when for the Indexer code value should be changed from the
-        than the provided value with respect to provided but incompatible index
-        values versus error conditions.
-
-        Parameters:
-            ser (bytes): serialization to be signed
-            seed (bytes):  raw binary seed (private key)
-            verfer (Verfer): instance. verfer.raw is public key
-            index (int |None): main index offset into list such as current signing
-                None means return non-indexed Cigar
-                Not None means return indexed Siger with Indexer code derived
-                    from index, conly, and ondex values
-            only (bool): True means main index only list, ondex ignored
-                          False means both index lists (default), ondex used
-            ondex (int | None): other index offset into list such as prior next
-        """
-        # compute raw signature sig using seed on serialization ser
-        sig = pysodium.crypto_sign_detached(ser, seed + verfer.raw)
-
-        if index is None:  # Must be Cigar i.e. non-indexed signature
-            return Cigar(raw=sig, code=MtrDex.Ed25519_Sig, verfer=verfer)
-        else:  # Must be Siger i.e. indexed signature
-            # should add Indexer class method to get ms main index size for given code
-            if only:  # only main index ondex not used
-                ondex = None
-                if index <= 63: # (64 ** ms - 1) where ms is main index size
-                    code = indexing.IdrDex.Ed25519_Crt_Sig  # use small current only
-                else:
-                    code = indexing.IdrDex.Ed25519_Big_Crt_Sig  # use big current only
-            else:  # both
-                if ondex == None:
-                    ondex = index  # enable default to be same
-                if ondex == index and index <= 63:  # both same and small
-                    code = indexing.IdrDex.Ed25519_Sig  # use  small both same
-                else:  # otherwise big or both not same so use big both
-                    code = indexing.IdrDex.Ed25519_Big_Sig  # use use big both
-
-            return indexing.Siger(raw=sig,
-                                    code=code,
-                                    index=index,
-                                    ondex=ondex,
-                                    verfer=verfer,)
-
-    @staticmethod
-    def _secp256r1(ser, seed, verfer, index, only=False, ondex=None, **kwa):
-        """
-        Returns signature as either Cigar or Siger instance as appropriate for
-        Ed25519 digital signatures given index and ondex values
-
-        The seed's code determins the crypto key-pair algorithm and signing suite
-        The signature type, Cigar or Siger, and when indexed the Siger code
-        may be completely determined by the seed and index values (index, ondex)
-        by assuming that the index values are intentional.
-        Without the seed code its more difficult for Siger to
-        determine when for the Indexer code value should be changed from the
-        than the provided value with respect to provided but incompatible index
-        values versus error conditions.
-
-        Parameters:
-            ser (bytes): serialization to be signed
-            seed (bytes):  raw binary seed (private key)
-            verfer (Verfer): instance. verfer.raw is public key
-            index (int |None): main index offset into list such as current signing
-                None means return non-indexed Cigar
-                Not None means return indexed Siger with Indexer code derived
-                    from index, conly, and ondex values
-            only (bool): True means main index only list, ondex ignored
-                          False means both index lists (default), ondex used
-            ondex (int | None): other index offset into list such as prior next
-        """
-        # compute raw signature sig using seed on serialization ser
-        d = int.from_bytes(seed, byteorder="big")
-        sigkey = ec.derive_private_key(d, ec.SECP256R1())
-        der = sigkey.sign(ser, ec.ECDSA(hashes.SHA256()))
-        (r, s) = utils.decode_dss_signature(der)
-        sig = bytearray(r.to_bytes(32, "big"))
-        sig.extend(s.to_bytes(32, "big"))
-
-        if index is None:  # Must be Cigar i.e. non-indexed signature
-            return Cigar(raw=sig, code=MtrDex.ECDSA_256r1_Sig, verfer=verfer)
-        else:  # Must be Siger i.e. indexed signature
-            # should add Indexer class method to get ms main index size for given code
-            if only:  # only main index ondex not used
-                ondex = None
-                if index <= 63: # (64 ** ms - 1) where ms is main index size
-                    code = indexing.IdrDex.ECDSA_256r1_Crt_Sig  # use small current only
-                else:
-                    code = indexing.IdrDex.ECDSA_256r1_Big_Crt_Sig  # use big current only
-            else:  # both
-                if ondex == None:
-                    ondex = index  # enable default to be same
-                if ondex == index and index <= 63:  # both same and small
-                    code = indexing.IdrDex.ECDSA_256r1_Sig  # use  small both same
-                else:  # otherwise big or both not same so use big both
-                    code = indexing.IdrDex.ECDSA_256r1_Big_Sig  # use use big both
-
-            return indexing.Siger(raw=sig,
-                                    code=code,
-                                    index=index,
-                                    ondex=ondex,
-                                    verfer=verfer,)
-
-    @staticmethod
-    def _secp256k1(ser, seed, verfer, index, only=False, ondex=None, **kwa):
-        """
-        Returns signature as either Cigar or Siger instance as appropriate for
-        secp256k1 digital signatures given index and ondex values
-
-        The seed's code determins the crypto key-pair algorithm and signing suite
-        The signature type, Cigar or Siger, and when indexed the Siger code
-        may be completely determined by the seed and index values (index, ondex)
-        by assuming that the index values are intentional.
-        Without the seed code its more difficult for Siger to
-        determine when for the Indexer code value should be changed from the
-        than the provided value with respect to provided but incompatible index
-        values versus error conditions.
-
-        Parameters:
-            ser (bytes): serialization to be signed
-            seed (bytes):  raw binary seed (private key)
-            verfer (Verfer): instance. verfer.raw is public key
-            index (int |None): main index offset into list such as current signing
-                None means return non-indexed Cigar
-                Not None means return indexed Siger with Indexer code derived
-                    from index, conly, and ondex values
-            only (bool): True means main index only list, ondex ignored
-                          False means both index lists (default), ondex used
-            ondex (int | None): other index offset into list such as prior next
-        """
-        # compute raw signature sig using seed on serialization ser
-        d = int.from_bytes(seed, byteorder="big")
-        sigkey = ec.derive_private_key(d, ec.SECP256K1())
-        der = sigkey.sign(ser, ec.ECDSA(hashes.SHA256()))
-        (r, s) = utils.decode_dss_signature(der)
-        sig = bytearray(r.to_bytes(32, "big"))
-        sig.extend(s.to_bytes(32, "big"))
-
-        if index is None:  # Must be Cigar i.e. non-indexed signature
-            return Cigar(raw=sig, code=MtrDex.ECDSA_256k1_Sig, verfer=verfer)
-        else:  # Must be Siger i.e. indexed signature
-            # should add Indexer class method to get ms main index size for given code
-            if only:  # only main index ondex not used
-                ondex = None
-                if index <= 63: # (64 ** ms - 1) where ms is main index size
-                    code = indexing.IdrDex.ECDSA_256k1_Crt_Sig  # use small current only
-                else:
-                    code = indexing.IdrDex.ECDSA_256k1_Big_Crt_Sig  # use big current only
-            else:  # both
-                if ondex == None:
-                    ondex = index  # enable default to be same
-                if ondex == index and index <= 63:  # both same and small
-                    code = indexing.IdrDex.ECDSA_256k1_Sig  # use  small both same
-                else:  # otherwise big or both not same so use big both
-                    code = indexing.IdrDex.ECDSA_256k1_Big_Sig  # use use big both
-
-            return indexing.Siger(raw=sig,
-                                code=code,
-                                index=index,
-                                ondex=ondex,
-                                verfer=verfer,)
-
-
-class Salter(Matter):
-    """
-    Salter is Matter subclass to maintain random salt for secrets (private keys)
-    Its .raw is random salt, .code as cipher suite for salt
-
-    Attributes:
-        .level is str security level code. Provides default level
-
-    Inherited Properties
-        .pad  is int number of pad chars given raw
-        .code is  str derivation code to indicate cypher suite
-        .raw is bytes crypto material only without code
-        .index is int count of attached crypto material by context (receipts)
-        .qb64 is str in Base64 fully qualified with derivation code + crypto mat
-        .qb64b is bytes in Base64 fully qualified with derivation code + crypto mat
-        .qb2  is bytes in binary with derivation code + crypto material
-        .transferable is Boolean, True when transferable derivation code False otherwise
-
-    Properties:
-
-    Methods:
-
-    Hidden:
-        ._pad is method to compute  .pad property
-        ._code is str value for .code property
-        ._raw is bytes value for .raw property
-        ._index is int value for .index property
-        ._infil is method to compute fully qualified Base64 from .raw and .code
-        ._exfil is method to extract .code and .raw from fully qualified Base64
-
-    """
-    Tier = Tiers.low
-
-    def __init__(self, raw=None, code=MtrDex.Salt_128, tier=None, **kwa):
-        """
-        Initialize salter's raw and code
-
-        Inherited Parameters:
-            raw is bytes of unqualified crypto material usable for crypto operations
-            qb64b is bytes of fully qualified crypto material
-            qb64 is str or bytes  of fully qualified crypto material
-            qb2 is bytes of fully qualified crypto material
-            code is str of derivation code
-            index is int of count of attached receipts for CryCntDex codes
-
-        Parameters:
-
-        """
-        try:
-            super(Salter, self).__init__(raw=raw, code=code, **kwa)
-        except EmptyMaterialError as ex:
-            if code == MtrDex.Salt_128:
-                raw = pysodium.randombytes(pysodium.crypto_pwhash_SALTBYTES)
-                super(Salter, self).__init__(raw=raw, code=code, **kwa)
-            else:
-                raise ValueError("Unsupported salter code = {}.".format(code))
-
-        if self.code not in (MtrDex.Salt_128,):
-            raise ValueError("Unsupported salter code = {}.".format(self.code))
-
-        self.tier = tier if tier is not None else self.Tier
-
-    def stretch(self, *, size=32, path="", tier=None, temp=False):
-        """
-        Returns (bytes): raw binary seed (secret) derived from path and .raw
-        and stretched to size given by code using argon2d stretching algorithm.
-
-        Parameters:
-            size (int): number of bytes in stretched seed
-            path (str): unique chars used in derivation of seed (secret)
-            tier (str): value from Tierage for security level of stretch
-            temp is Boolean, True means use quick method to stretch salt
-                    for testing only, Otherwise use time set by tier to stretch
-        """
-        tier = tier if tier is not None else self.tier
-
-        if temp:
-            opslimit = 1  # pysodium.crypto_pwhash_OPSLIMIT_MIN
-            memlimit = 8192  # pysodium.crypto_pwhash_MEMLIMIT_MIN
-        else:
-            if tier == Tiers.low:
-                opslimit = 2  # pysodium.crypto_pwhash_OPSLIMIT_INTERACTIVE
-                memlimit = 67108864  # pysodium.crypto_pwhash_MEMLIMIT_INTERACTIVE
-            elif tier == Tiers.med:
-                opslimit = 3  # pysodium.crypto_pwhash_OPSLIMIT_MODERATE
-                memlimit = 268435456  # pysodium.crypto_pwhash_MEMLIMIT_MODERATE
-            elif tier == Tiers.high:
-                opslimit = 4  # pysodium.crypto_pwhash_OPSLIMIT_SENSITIVE
-                memlimit = 1073741824  # pysodium.crypto_pwhash_MEMLIMIT_SENSITIVE
-            else:
-                raise ValueError("Unsupported security tier = {}.".format(tier))
-
-        # stretch algorithm is argon2id
-        seed = pysodium.crypto_pwhash(outlen=size,
-                                      passwd=path,
-                                      salt=self.raw,
-                                      opslimit=opslimit,
-                                      memlimit=memlimit,
-                                      alg=pysodium.crypto_pwhash_ALG_ARGON2ID13)
-        return (seed)
-
-    def signer(self, *, code=MtrDex.Ed25519_Seed, transferable=True, path="",
-               tier=None, temp=False):
-        """
-        Returns Signer instance whose .raw secret is derived from path and
-        salter's .raw and stretched to size given by code. The signers public key
-        for its .verfer is derived from code and transferable.
-
-        Parameters:
-            code is str code of secret crypto suite
-            transferable is Boolean, True means use transferace code for public key
-            path is str of unique chars used in derivation of secret seed for signer
-            tier is str Tierage security level
-            temp is Boolean, True means use quick method to stretch salt
-                    for testing only, Otherwise use more time to stretch
-        """
-        seed = self.stretch(size=Matter._rawSize(code), path=path, tier=tier,
-                            temp=temp)
-
-        return (Signer(raw=seed, code=code, transferable=transferable))
-
-
-    def signers(self, count=1, start=0, path="",  **kwa):
-        """
-        Returns list of count number of Signer instances with unique derivation
-        path made from path prefix and suffix of start plus offset for each count
-        value from 0 to count - 1.
-
-        See .signer for parameters used to create each signer.
-
-        """
-        return [self.signer(path=f"{path}{i + start:x}", **kwa) for i in range(count)]
-
-
-class Cipher(Matter):
-    """
-    Cipher is Matter subclass holding a cipher text of a secret that may be
-    either a secret seed (private key) or secret salt with appropriate CESR code
-    to indicate which kind (which indicates size). The cipher text is created
-    with assymetric encryption using an unrelated (public, private)
-    encryption/decryption key pair. The public key is used for encryption the
-    private key for decryption. The default is to use X25519 sealed box encryption.
-
-    The Cipher instances .raw is the raw binary encrypted cipher text and its
-    .code indicates what type of secret has been encrypted. The cipher suite used
-    for the encryption/decryption is implied by the context where the cipher is
-    used.
-
-    See Matter for inherited attributes and properties
-
-    """
-
-    def __init__(self, raw=None, code=None, **kwa):
-        """
-        Parmeters:
-            raw (Union[bytes, str]): cipher text
-            code (str): cipher suite
-        """
-        if raw is not None and code is None:
-            if len(raw) == Matter._rawSize(MtrDex.X25519_Cipher_Salt):
-                code = MtrDex.X25519_Cipher_Salt
-            elif len(raw) == Matter._rawSize(MtrDex.X25519_Cipher_Seed):
-                code = MtrDex.X25519_Cipher_Seed
-
-        if hasattr(raw, "encode"):
-            raw = raw.encode("utf-8")  # ensure bytes not str
-
-        super(Cipher, self).__init__(raw=raw, code=code, **kwa)
-
-        if self.code not in (MtrDex.X25519_Cipher_Salt, MtrDex.X25519_Cipher_Seed):
-            raise ValueError("Unsupported cipher code = {}.".format(self.code))
-
-    def decrypt(self, prikey=None, seed=None):
-        """
-        Returns plain text as Matter instance (Signer or Salter) of cryptographic
-        cipher text material given by .raw. Encrypted plain text is fully
-        qualified (qb64) so derivaton code of plain text preserved through
-        encryption/decryption round trip.
-
-        Uses either decryption key given by prikey or derives prikey from
-        signing key derived from private seed.
-
-        Parameters:
-            prikey (Union[bytes, str]): qb64b or qb64 serialization of private
-                decryption key
-            seed (Union[bytes, str]): qb64b or qb64 serialization of private
-                signing key seed used to derive private decryption key
-        """
-        decrypter = Decrypter(qb64b=prikey, seed=seed)
-        return decrypter.decrypt(ser=self.qb64b)
-
-
-class Encrypter(Matter):
-    """
-    Encrypter is Matter subclass with method to create a cipher text of a
-    fully qualified (qb64) private key/seed where private key/seed is the plain
-    text. Encrypter uses assymetric (public, private) key encryption of a
-    serialization (plain text). Using its .raw as the encrypting (public) key and
-    its .code to indicate the cipher suite for the encryption operation.
-
-    For example .code == MtrDex.X25519 indicates that X25519 sealed box
-    encyrption is used. The encryption key may be derived from an Ed25519
-    signing public key that associated with a nontransferable or basic derivation
-    self certifying identifier. This allows use of the self certifying identifier
-    to track or manage the encryption/decryption key pair. And could be used to
-    provide additional authentication operations for using the
-    encryption/decryption key pair. Support for this is provided at init time
-    with the verkey parameter which allows deriving the encryption public key from
-    the fully qualified verkey (signature verification key).
-
-    See Matter for inherited attributes and properties:
-
-    Methods:
-        encrypt: returns cipher text
-
-    """
-
-    def __init__(self, raw=None, code=MtrDex.X25519, verkey=None, **kwa):
-        """
-        Assign encrypting cipher suite function to ._encrypt
-
-        Parameters:  See Matter for inherted parameters such as qb64, qb64b
-            raw (bytes): public encryption key
-            qb64b (bytes): fully qualified public encryption key
-            qb64 (str): fully qualified public encryption key
-            code (str): derivation code for public encryption key
-            verkey (Union[bytes, str]): qb64b or qb64 of verkey used to derive raw
-        """
-        if not raw and verkey:
-            verfer = Verfer(qb64b=verkey)
-            if verfer.code not in (MtrDex.Ed25519N, MtrDex.Ed25519):
-                raise ValueError("Unsupported verkey derivation code = {}."
-                                 "".format(verfer.code))
-            # convert signing public key to encryption public key
-            raw = pysodium.crypto_sign_pk_to_box_pk(verfer.raw)
-
-        super(Encrypter, self).__init__(raw=raw, code=code, **kwa)
-
-        if self.code == MtrDex.X25519:
-            self._encrypt = self._x25519
-        else:
-            raise ValueError("Unsupported encrypter code = {}.".format(self.code))
-
-    def verifySeed(self, seed):
-        """
-        Returns:
-            Boolean: True means private signing key seed corresponds to public
-                signing key verkey used to derive encrypter's .raw public
-                encryption key.
-
-        Parameters:
-            seed (Union(bytes,str)): qb64b or qb64 serialization of private
-                signing key seed
-        """
-        signer = Signer(qb64b=seed)
-        verkey, sigkey = pysodium.crypto_sign_seed_keypair(signer.raw)
-        pubkey = pysodium.crypto_sign_pk_to_box_pk(verkey)
-        return (pubkey == self.raw)
-
-    def encrypt(self, ser=None, matter=None):
-        """
-        Returns:
-            Cipher instance of cipher text encryption of plain text serialization
-            provided by either ser or Matter instance when provided.
-
-        Parameters:
-            ser (Union[bytes,str]): qb64b or qb64 serialization of plain text
-            matter (Matter): plain text as Matter instance of seed or salt to
-                be encrypted
-        """
-        if not (ser or matter):
-            raise EmptyMaterialError("Neither ser or plain are provided.")
-
-        if ser:
-            matter = Matter(qb64b=ser)
-
-        if matter.code == MtrDex.Salt_128:  # future other salt codes
-            code = MtrDex.X25519_Cipher_Salt
-        elif matter.code == MtrDex.Ed25519_Seed:  # future other seed codes
-            code = MtrDex.X25519_Cipher_Seed
-        else:
-            raise ValueError("Unsupported plain text code = {}.".format(matter.code))
-
-        # encrypting fully qualified qb64 version of plain text ensures its
-        # derivation code round trips through eventual decryption
-        return (self._encrypt(ser=matter.qb64b, pubkey=self.raw, code=code))
-
-    @staticmethod
-    def _x25519(ser, pubkey, code):
-        """
-        Returns cipher text as Cipher instance
-        Parameters:
-            ser (Union[bytes, str]): qb64b or qb64 serialization of seed or salt
-                to be encrypted.
-            pubkey (bytes): raw binary serialization of encryption public key
-            code (str): derivation code of serialized plain text seed or salt
-        """
-        raw = pysodium.crypto_box_seal(ser, pubkey)
-        return Cipher(raw=raw, code=code)
-
-
-class Decrypter(Matter):
-    """
-    Decrypter is Matter subclass with method to decrypt the plain text from a
-    ciper text of a fully qualified (qb64) private key/seed where private
-    key/seed is the plain text. Decrypter uses assymetric (public, private) key
-    decryption of the cipher text using its .raw as the decrypting (private) key
-    and its .code to indicate the cipher suite for the decryption operation.
-
-    For example .code == MtrDex.X25519 indicates that X25519 sealed box
-    decyrption is used. The decryption key may be derived from an Ed25519
-    signing private key that is associated with a nontransferable or basic derivation
-    self certifying identifier. This allows use of the self certifying identifier
-    to track or manage the encryption/decryption key pair. And could be used to
-    provide additional authentication operations for using the
-    encryption/decryption key pair. Support for this is provided at init time
-    with the sigkey parameter which allows deriving the decryption private key
-    from the fully qualified sigkey (signing key).
-
-    See Matter for inherited attributes and properties:
-
-    Attributes:
-
-    Properties:
-
-
-    Methods:
-        decrypt: create cipher text
-
-    """
-
-    def __init__(self, code=MtrDex.X25519_Private, seed=None, **kwa):
-        """
-        Assign decrypting cipher suite function to ._decrypt
-
-        Parameters:  See Matter for inheirted parameters
-            raw (bytes): private decryption key derived from seed (private signing key)
-            qb64b (bytes): fully qualified private decryption key
-            qb64 (str): fully qualified private decryption key
-            code (str): derivation code for private decryption key
-            seed (Union[bytes, str]): qb64b or qb64 of signing key seed used to
-                derive raw which is private decryption key
-        """
-        try:
-            super(Decrypter, self).__init__(code=code, **kwa)
-        except EmptyMaterialError as ex:
-            if seed:
-                signer = Signer(qb64b=seed)
-                if signer.code not in (MtrDex.Ed25519_Seed,):
-                    raise ValueError("Unsupported signing seed derivation code = {}."
-                                     "".format(signer.code))
-                # verkey, sigkey = pysodium.crypto_sign_seed_keypair(signer.raw)
-                sigkey = signer.raw + signer.verfer.raw  # sigkey is raw seed + raw verkey
-                raw = pysodium.crypto_sign_sk_to_box_sk(sigkey)  # raw private encrypt key
-                super(Decrypter, self).__init__(raw=raw, code=code, **kwa)
-            else:
-                raise
-
-        if self.code == MtrDex.X25519_Private:
-            self._decrypt = self._x25519
-        else:
-            raise ValueError("Unsupported decrypter code = {}.".format(self.code))
-
-    def decrypt(self, ser=None, cipher=None, transferable=False):
-        """
-        Returns:
-            Salter or Signer instance derived from plain text decrypted from
-            encrypted cipher text material given by ser or cipher. Plain text
-            that is orignally encrypt should always be fully qualified (qb64b)
-            so that derivaton code of plain text is preserved through
-            encryption/decryption round trip.
-
-        Parameters:
-            ser (Union[bytes,str]): qb64b or qb64 serialization of cipher text
-            cipher (Cipher): optional Cipher instance when ser is None
-            transferable (bool): True means associated verfer of returned
-                signer is transferable. False means non-transferable
-        """
-        if not (ser or cipher):
-            raise EmptyMaterialError("Neither ser or cipher are provided.")
-
-        if ser:  # create cipher to ensure valid derivation code of material in ser
-            cipher = Cipher(qb64b=ser)
-
-        return (self._decrypt(cipher=cipher,
-                              prikey=self.raw,
-                              transferable=transferable))
-
-    @staticmethod
-    def _x25519(cipher, prikey, transferable=False):
-        """
-        Returns plain text as Salter or Signer instance depending on the cipher
-            code and the embedded encrypted plain text derivation code.
-
-        Parameters:
-            cipher (Cipher): instance of encrypted seed or salt
-            prikey (bytes): raw binary decryption private key derived from
-                signing seed or sigkey
-            transferable (bool): True means associated verfer of returned
-                signer is transferable. False means non-transferable
-        """
-        pubkey = pysodium.crypto_scalarmult_curve25519_base(prikey)
-        plain = pysodium.crypto_box_seal_open(cipher.raw, pubkey, prikey)  # qb64b
-        # ensure raw plain text is qb64b or qb64 so its derivation code is round tripped
-        if cipher.code == MtrDex.X25519_Cipher_Salt:
-            return Salter(qb64b=plain)
-        elif cipher.code == MtrDex.X25519_Cipher_Seed:
-            return Signer(qb64b=plain, transferable=transferable)
-        else:
-            raise ValueError("Unsupported cipher text code = {}.".format(cipher.code))
-
 
 class Diger(Matter):
     """
     Diger is Matter subclass with method to verify digest of serialization
 
 
     See Matter for inherited attributes and properties:
@@ -4959,15 +4302,15 @@
     Properties:
         .weighted is Boolean True if fractional weighted threshold False if numeric
         .size is int of minimum size of keys list
                     when weighted is size of keys list
                     when unweighted is size of int thold since don't have anyway
                         to know size of keys list in this case
 
-        .limen is qualified b64 signing threshold suitable for CESR serialization.
+        .limen is qualified b64b signing threshold suitable for CESR serialization.
             either Number.qb64b or Bexter.qb64b.
             The b64 portion of limen  with code stripped (Bexter.bext) of
               [["1/2", "1/2", "1/4", "1/4", "1/4"], ["1", "1"]]
               is '1s2c1s2c1s4c1s4c1s4a1c1' basically slash is 's', comma is 'c',
             ANDed clauses are delimited by 'a'.
             Each clause top level weight may be optionally a weighted set of weights
             delimited by 'k' for the weight on the set and 'v' for the weights in
```

### Comparing `keri-1.2.0.dev0/src/keri/core/counting.py` & `keri-1.2.0.dev1/src/keri/core/counting.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from ..help.helping import sceil
 from ..help.helping import (intToB64,  b64ToInt, codeB64ToB2, codeB2ToB64, Reb64,
                             nabSextets)
 
 from .. import kering
 from ..kering import (Versionage, Vrsn_1_0, Vrsn_2_0)
 
-from ..core.coring import Sizage
+from ..core.coring import Sizage, MapDom
 
 
 
 @dataclass(frozen=True)
 class GenusCodex:
     """GenusCodex is codex of protocol genera for code table.
 
@@ -38,79 +38,25 @@
         # duplicate values above just result in multiple entries in tuple so
         # in inclusion still works
 
 GenDex = GenusCodex()  # Make instance
 
 
 
-@dataclass
-class MapDom:
-    """Base class for dataclasses that support map syntax
-    Adds support for dunder methods for map syntax dc[name].
-    Converts exceptions from attribute syntax to raise map syntax when using
-    map syntax.
-    """
-
-    def __getitem__(self, name):
-        try:
-            return getattr(self, name)
-        except AttributeError as ex:
-            raise IndexError(ex.args) from ex
-
-
-    def __setitem__(self, name, value):
-        try:
-            return setattr(self, name, value)
-        except AttributeError as ex:
-            raise IndexError(ex.args) from ex
-
-
-    def __delitem__(self, name):
-        try:
-            return delattr(self, name)
-        except AttributeError as ex:
-            raise IndexError(ex.args) from ex
 
 
 @dataclass(frozen=True)
-class MapCodex:
-    """Base class for frozen dataclasses (codexes) that support map syntax
-    Adds support for dunder methods for map syntax dc[name].
-    Converts exceptions from attribute syntax to raise map syntax when using
-    map syntax.
-    """
-
-    def __getitem__(self, name):
-        try:
-            return getattr(self, name)
-        except AttributeError as ex:
-            raise IndexError(ex.args) from ex
-
-
-    def __setitem__(self, name, value):
-        try:
-            return setattr(self, name, value)
-        except AttributeError as ex:
-            raise IndexError(ex.args) from ex
-
-
-    def __delitem__(self, name):
-        try:
-            return delattr(self, name)
-        except AttributeError as ex:
-            raise IndexError(ex.args) from ex
-
-
-
-@dataclass(frozen=True)
-class CounterCodex_1_0(MapCodex):
+class CounterCodex_1_0(MapDom):
     """
     CounterCodex is codex hard (stable) part of all counter derivation codes.
     Only provide defined codes.
     Undefined are left out so that inclusion(exclusion) via 'in' operator works.
+
+    As subclass of MapCodex can get codes with item syntax using tag variables.
+    Example: codex[tag]
     """
     ControllerIdxSigs: str = '-A'  # Qualified Base64 Indexed Signature.
     WitnessIdxSigs: str = '-B'  # Qualified Base64 Indexed Signature.
     NonTransReceiptCouples: str = '-C'  # Composed Base64 Couple, pre+cig.
     TransReceiptQuadruples: str = '-D'  # Composed Base64 Quadruple, pre+snu+dig+sig.
     FirstSeenReplayCouples: str = '-E'  # Composed Base64 Couple, fnu+dts.
     TransIdxSigGroups: str = '-F'  # Composed Base64 Group, pre+snu+dig+ControllerIdxSigs group.
@@ -127,19 +73,22 @@
 
     def __iter__(self):
         return iter(astuple(self))  # enables value not key inclusion test with "in"
 
 CtrDex_1_0 = CounterCodex_1_0()
 
 @dataclass(frozen=True)
-class CounterCodex_2_0(MapCodex):
+class CounterCodex_2_0(MapDom):
     """
     CounterCodex is codex hard (stable) part of all counter derivation codes.
     Only provide defined codes.
     Undefined are left out so that inclusion(exclusion) via 'in' operator works.
+
+    As subclass of MapCodex can get codes with item syntax using tag variables.
+    Example: codex[tag]
     """
     GenericGroup: str = '-A'  # Generic Group (Universal with Override).
     BigGenericGroup: str = '-0A'  # Big Generic Group (Universal with Override).
     MessageGroup: str = '-B'  # Message Body plus Attachments Group (Universal with Override).
     BigMessageGroup: str = '-0B'  # Big Message Body plus Attachments Group (Universal with Override).
     AttachmentGroup: str = '-C'  # Message Attachments Only Group (Universal with Override).
     BigAttachmentGroup: str = '-0C'  # Big Attachments Only Group (Universal with Override).
@@ -161,40 +110,40 @@
     BigWitnessIdxSigs: str = '-0K'  # Big Witness Indexed Signature(s) of qb64.
     NonTransReceiptCouples: str = '-L'  # NonTrans Receipt Couple(s), pre+cig.
     BigNonTransReceiptCouples: str = '-0L'  # Big NonTrans Receipt Couple(s), pre+cig.
     TransReceiptQuadruples: str = '-M'  # Trans Receipt Quadruple(s), pre+snu+dig+sig.
     BigTransReceiptQuadruples: str = '-0M'  # Big Trans Receipt Quadruple(s), pre+snu+dig+sig.
     FirstSeenReplayCouples: str = '-N'  # First Seen Replay Couple(s), fnu+dts.
     BigFirstSeenReplayCouples: str = '-0N'  # First Seen Replay Couple(s), fnu+dts.
-    TransIdxSigGroups: str = '-O'  # Trans Indexed Signature Group(s), pre+snu+dig+ControllerIdxSigs of qb64.
-    TransIdxSigGroups: str = '-0O'  # Big Trans Indexed Signature Group(s), pre+snu+dig+ControllerIdxSigs of qb64.
-    TransLastIdxSigGroups: str = '-P'  # Trans Last Est Evt Indexed Signature Group(s), pre+ControllerIdxSigs of qb64.
-    BigTransLastIdxSigGroups: str = '-0P'  # Big Trans Last Est Evt Indexed Signature Group(s), pre+ControllerIdxSigs of qb64.
+    TransIdxSigGroups: str = '-O'  # Trans Indexed Signature Group(s), pre+snu+dig+CtrControllerIdxSigs of qb64.
+    BigTransIdxSigGroups: str = '-0O'  # Big Trans Indexed Signature Group(s), pre+snu+dig+CtrControllerIdxSigs of qb64.
+    TransLastIdxSigGroups: str = '-P'  # Trans Last Est Evt Indexed Signature Group(s), pre+CtrControllerIdxSigs of qb64.
+    BigTransLastIdxSigGroups: str = '-0P'  # Big Trans Last Est Evt Indexed Signature Group(s), pre+CtrControllerIdxSigs of qb64.
     SealSourceCouples: str = '-Q'  # Seal Source Couple(s), snu+dig of source sealing or sealed event.
     BigSealSourceCouples: str = '-0Q'  # Seal Source Couple(s), snu+dig of source sealing or sealed event.
     SealSourceTriples: str = '-R'  # Seal Source Triple(s), pre+snu+dig of source sealing or sealed event.
     BigSealSourceTriples: str = '-0R'  # Seal Source Triple(s), pre+snu+dig of source sealing or sealed event.
     PathedMaterialGroup: str = '-S'  # Pathed Material Group.
     BigPathedMaterialGroup: str = '-0S'  # Big Pathed Material Group.
-    SadPathSigGroups: str = '-T'  # SAD Path Group(s) sadpath+TransIdxSigGroup(s) of SAID qb64 of content.
-    BigSadPathSigGroups: str = '-0T'  # Big SAD Path Group(s) sadpath+TransIdxSigGroup(s) of SAID qb64 of content.
+    SadPathSigGroups: str = '-T'  # SAD Path Group(s) sadpath+CtrTransIdxSigGroup(s) of SAID qb64 of content.
+    BigSadPathSigGroups: str = '-0T'  # Big SAD Path Group(s) sadpath+CtrTransIdxSigGroup(s) of SAID qb64 of content.
     RootSadPathSigGroups: str = '-U'  # Root Path SAD Path Group(s), rootpath+SadPathGroup(s).
     BigRootSadPathSigGroups: str = '-0U'  # Big Root Path SAD Path Group(s), rootpath+SadPathGroup(s).
     DigestSealSingles: str = '-V'  # Digest Seal Single(s), dig of sealed data.
     BigDigestSealSingles: str = '-0V'  # Big Digest Seal Single(s), dig of sealed data.
     MerkleRootSealSingles: str = '-W'  # Merkle Tree Root Digest Seal Single(s), dig of sealed data.
     BigMerkleRootSealSingles: str = '-0W'  # Merkle Tree Root Digest Seal Single(s), dig of sealed data.
     BackerRegistrarSealCouples: str = '-X'  # Backer Registrar Seal Couple(s), brid+dig of sealed data.
     BigBackerRegistrarSealCouples: str = '-0X'  # Big Backer Registrar Seal Couple(s), brid+dig of sealed data.
+    SealSourceLastSingles: str = '-Y'  # Seal Source Couple(s), pre of last source sealing or sealed event.
+    BigSealSourceLastSingles: str = '-0Y'  # Big Seal Source Couple(s), pre of last source sealing or sealed event.
     ESSRPayloadGroup: str = '-Z'  # ESSR Payload Group.
     BigESSRPayloadGroup: str = '-0Z'  # Big ESSR Payload Group.
     KERIACDCGenusVersion: str = '--AAA'  # KERI ACDC Stack CESR Protocol Genus Version (Universal)
 
-
-
     def __iter__(self):
         return iter(astuple(self))  # enables value not key inclusion test with "in"
 
 CtrDex_2_0 = CounterCodex_2_0()
 
 # keys and values as strings of keys
 Codict1 = asdict(CtrDex_1_0)
@@ -206,14 +155,43 @@
 Tags_2_0 = Tagage_2_0()  # uses defaults
 
 CodictAll = Codict2 | Codict1
 AllTagage = namedtuple("AllTagage", list(CodictAll), defaults=list(CodictAll))
 AllTags = AllTagage()  # uses defaults
 
 
+@dataclass(frozen=True)
+class SealCodex_2_0(MapDom):
+    """
+    SealCodex_2_0 is codex of seal counter derivation codes.
+    Only provide defined codes.
+    Undefined are left out so that inclusion(exclusion) via 'in' operator works.
+
+    As subclass of MapCodex can get codes with item syntax using tag variables.
+    Example: codex[tag]
+    """
+    SealSourceCouples: str = '-Q'  # Seal Source Couple(s), snu+dig of source sealing or sealed event.
+    BigSealSourceCouples: str = '-0Q'  # Seal Source Couple(s), snu+dig of source sealing or sealed event.
+    SealSourceTriples: str = '-R'  # Seal Source Triple(s), pre+snu+dig of source sealing or sealed event.
+    BigSealSourceTriples: str = '-0R'  # Seal Source Triple(s), pre+snu+dig of source sealing or sealed event.
+    DigestSealSingles: str = '-V'  # Digest Seal Single(s), dig of sealed data.
+    BigDigestSealSingles: str = '-0V'  # Big Digest Seal Single(s), dig of sealed data.
+    MerkleRootSealSingles: str = '-W'  # Merkle Tree Root Digest Seal Single(s), dig of sealed data.
+    BigMerkleRootSealSingles: str = '-0W'  # Merkle Tree Root Digest Seal Single(s), dig of sealed data.
+    BackerRegistrarSealCouples: str = '-X'  # Backer Registrar Seal Couple(s), brid+dig of sealed data.
+    BigBackerRegistrarSealCouples: str = '-0X'  # Big Backer Registrar Seal Couple(s), brid+dig of sealed data.
+    SealSourceLastSingles: str = '-Y'  # Seal Source Couple(s), pre of last source sealing event.
+    BigSealSourceLastSingles: str = '-0Y'  # Big Seal Source Couple(s), pre of last source sealing event.
+
+    def __iter__(self):
+        return iter(astuple(self))  # enables value not key inclusion test with "in"
+
+SealDex_2_0 = SealCodex_2_0()
+
+
 class Counter:
     """
     Counter is fully qualified cryptographic material primitive base class for
     counter primitives (framing composition grouping count codes).
 
     Sub classes are derivation code and key event element context specific.
 
@@ -230,33 +208,33 @@
     Attributes:
 
 
     Properties:
         .version (Versionage): current CESR code table protocol genus version
         .codes (CounterCodex_1_0 | CounterCodex_1_0): version specific codex
         .sizes (dict): version specific sizes table
-        .code (str) derivation code to indicate cypher suite
-        .raw is bytes crypto material only without code
-        .pad  is int number of pad chars given raw
-        .count is int count of quadlets/triplets of following framed material
-            (not including code)
-        .qb64 is str in Base64 fully qualified with derivation code + crypto mat
-        .qb64b is bytes in Base64 fully qualified with derivation code + crypto mat
-        .qb2  is bytes in binary with derivation code + crypto material
+        .code (str): hard part of derivation code to indicate cypher suite
+        .raw (bytes): crypto material only without code
+        .pad  (int): number of pad chars given raw
+        .count (int): count of quadlets/triplets of following framed material
+                      (not including code)
+        .qb64 (str | bytes | bytearray): in Base64 fully qualified with
+                                          derivation code + crypto mat
+        .qb64b (bytes | bytearray): in Base64 fully qualified with
+                                    derivation code + crypto mat
+        .qb2  (bytes | bytearray): in binary with derivation code +
+                                  crypto material
 
     Hidden:
         ._version (Versionage): value for .version property
         ._codes (CounterCodex_1_0 | CounterCodex_1_0): version specific codex
         ._sizes (dict): version specific sizes table
-        ._code is str value for .code property
-        ._raw is bytes value for .raw property
-        ._pad is method to compute  .pad property
-        ._count is int value for .count property
-        ._infil is method to compute fully qualified Base64 from .raw and .code
-        ._exfil is method to extract .code and .raw from fully qualified Base64
+        ._code (str): value for .code property
+        ._raw (bytes): value for .raw property
+        ._count (int): value for .count property
 
 
     Versioning:
         CESR Genus specific code tables have a major and a minor version.
 
         For a given major version all minor versions must be backwards compatible.
         This means that minor version changes to tables are append only. New
@@ -422,14 +400,16 @@
                 '-0V': Sizage(hs=3, ss=5, fs=8, ls=0),
                 '-W': Sizage(hs=2, ss=2, fs=4, ls=0),
                 '-0W': Sizage(hs=3, ss=5, fs=8, ls=0),
                 '-X': Sizage(hs=2, ss=2, fs=4, ls=0),
                 '-0X': Sizage(hs=3, ss=5, fs=8, ls=0),
                 '-Y': Sizage(hs=2, ss=2, fs=4, ls=0),
                 '-0Y': Sizage(hs=3, ss=5, fs=8, ls=0),
+                '-Z': Sizage(hs=2, ss=2, fs=4, ls=0),
+                '-0Z': Sizage(hs=3, ss=5, fs=8, ls=0),
                 '--AAA': Sizage(hs=5, ss=3, fs=8, ls=0),
             },
         },
     }
 
 
     def __init__(self, tag=None, *, code = None, count=None, countB64=None,
@@ -439,21 +419,20 @@
         Parameters:
             tag (str | None):  label of stable (hard) part of derivation code
                                to lookup in codex so it can depend on version.
                                takes precedence over tag
             code (str | None):  stable (hard) part of derivation code
                             if tag provided lookup code from tag
                             else if tag is None and code provided use code
-            count (int | None): count of framed material for composition
-                Count does not include code.
-                Count represents quadlets/triplets
-                When both count and countB64 are None then count defaults to 1
-            countB64 (str | None): count of framed material for composition
-                as Base64
-                countB64 represents quadlets/triplets
+            count (int | None): count of framed material in quadlets/triplets
+                               for composition. Count does not include code.
+                               When both count and countB64 are None then count
+                               defaults to 1
+            countB64 (str | None): count of framed material in quadlets/triplets
+                                for composition as Base64 representation of int.
             qb64b (bytes | bytearray | None): fully qualified crypto material text domain
                 if code nor tag is provided
             qb64 (str | None) fully qualified crypto material text domain
                 if code nor tag not qb64b is provided
             qb2 (bytes | bytearray | None)  fully qualified crypto material binary domain
                 if code nor tag not qb64b nor qb54 is provided
             strip (bool):  True means strip counter contents from input stream
```

### Comparing `keri-1.2.0.dev0/src/keri/core/eventing.py` & `keri-1.2.0.dev1/src/keri/core/eventing.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,44 +3,42 @@
 keri.core.eventing module
 
 """
 import datetime
 import json
 import logging
 from collections import namedtuple
-from dataclasses import dataclass, astuple, asdict, field
 from urllib.parse import urlsplit
 from math import ceil
 from ordered_set import OrderedSet as oset
 from hio.help import decking
 
 
 from .. import kering
 from ..kering import (MissingEntryError,
-                      ValidationError, DerivationError, MissingSignatureError,
+                      ValidationError, MissingSignatureError,
                       MissingWitnessSignatureError, UnverifiedReplyError,
                       MissingDelegationError, OutOfOrderError,
                       LikelyDuplicitousError, UnverifiedWitnessReceiptError,
                       UnverifiedReceiptError, UnverifiedTransferableReceiptError,
                       QueryNotFoundError, MisfitEventSourceError,
                       MissingDelegableApprovalError)
-from ..kering import Version, Versionage, TraitCodex, TraitDex
-from ..kering import Coldage, Colds, ColdDex
+from ..kering import Version, Versionage, TraitDex
 
 from .. import help
 from ..help import helping
 
 from . import coring
-from .coring import (versify, Serials, Ilks, MtrDex, PreDex, DigDex,
+from .coring import (versify, Serials, Ilks, PreDex, DigDex,
                      NonTransDex, CtrDex, Counter,
                      Number, Seqner, Cigar, Dater,
                      Verfer, Diger, Prefixer, Tholder, Saider)
 
 from . import indexing
-from .indexing import (IdrDex, Indexer, Siger)
+from .indexing import Siger
 
 from . import serdering
 
 from ..db import basing, dbing
 from ..db.basing import KeyStateRecord, StateEERecord
 from ..db.dbing import dgKey, snKey, fnKey, splitKeySN, splitKey
 
@@ -72,41 +70,43 @@
 SealRoot = namedtuple("SealRoot", 'rd')
 
 # Backer Seal: couple (bi, d)
 # bi = pre qb64 backer nontrans identifier prefix
 # d = digest qb64 of backer metadata anchored to event usually SAID of data
 SealBacker = namedtuple("SealBacker", 'bi d')
 
+# Last Estalishment Event Seal: uniple (i,)
+# i = pre is qb64 of identifier prefix of KEL from which to get last est, event
+# used to indicate to get the latest keys available from KEL for 'i'
+SealLast = namedtuple("SealLast", 'i')
+
+# Transaction Event Seal for Transaction Event: duple (s, d)
+# s = sn of transaction event as lowercase hex string  no leading zeros,
+# d = SAID digest qb64 of transaction event
+# the pre is provided in the 'i' field  qb64 of identifier prefix of KEL
+# key event that this seal appears.
+# use SealSourceCouples count code for attachment
+SealTrans = namedtuple("SealTrans", 's d')
+
 # Event Seal: triple (i, s, d)
 # i = pre is qb64 of identifier prefix of KEL for event,
 # s = sn of event as lowercase hex string  no leading zeros,
 # d = SAID digest qb64 of event
 SealEvent = namedtuple("SealEvent", 'i s d')
 
-# Last Estalishment Event Seal: uniple (i,)
-# i = pre is qb64 of identifier prefix of KEL from which to get last est, event
-# used to indicate to get the latest keys available from KEL for 'i'
-SealLast = namedtuple("SealLast", 'i')
+# Following are not seals only used in database
 
 # State Establishment Event (latest current) : quadruple (s, d, br, ba)
 # s = sn of latest est event as lowercase hex string  no leading zeros,
 # d = SAID digest qb64  of latest establishment event
 # br = backer (witness) remove list (cuts) from latest est event
 # ba = backer (witness) add list (adds) from latest est event
 StateEstEvent = namedtuple("StateEstEvent", 's d br ba')
 
-# Transaction Event Seal for Transaction Event: duple (s, d)
-# s = sn of transaction event as lowercase hex string  no leading zeros,
-# d = SAID digest qb64 of transaction event
-# the pre is provided in the 'i' field  qb64 of identifier prefix of KEL
-# key event that this seal appears.
-# use SealSourceCouples count code for attachment
-SealTrans = namedtuple("SealTrans", 's d')
-
-# not used should this be depricated
+# not used should this be depricated?
 # State Event (latest current) : triple (s, t, d)
 # s = sn of latest event as lowercase hex string  no leading zeros,
 # t = message type of latest event (ilk)
 # d = SAID digest qb64 of latest event
 StateEvent = namedtuple("StateEvent", 's t d')
 
 
@@ -384,15 +384,15 @@
     usigs = oset([siger.qb64 for siger in sigers])
     usigers = [Siger(qb64=sig) for sig in usigs]
 
     # verify indexes of attached signatures against verifiers and assign
     # verfer to each siger
     for siger in usigers:
         if siger.index >= len(verfers):
-            logger.info("Skipped sig: Index=%s to large.\n", siger.index)
+            logger.info("Skipped sig: Index=%s to large.", siger.index)
         siger.verfer = verfers[siger.index]  # assign verfer
 
     # create lists of unique verified signatures and indices
     vindices = []
     vsigers = []
     for siger in usigers:
         if siger.verfer.verify(siger.raw, raw):
@@ -637,15 +637,16 @@
                b=wits,  # list of qb64 may be empty
                c=cnfg if cnfg is not None else [],
                ee=StateEERecord._fromdict(eevt._asdict()),  # latest est event dict
                di=dpre if dpre is not None else "",
                )
     return ksr  # return KeyStateRecord  use asdict(ksr) to get dict version
 
-
+# should remove intive as its not standard KERI so confusing and leads to errors
+# this is an old feature that is now deprecated.
 
 def incept(keys,
            *,
            isith=None,
            ndigs=None,
            nsith=None,
            toad=None,
@@ -660,17 +661,17 @@
            ):
     """
     Returns serder of inception event message.
     Utility function to automate creation of inception events.
 
     Parameters:
         keys  (list): current signing keys qb64
-        sith (int | str | list | None): current signing threshold input to Tholder
+        isith (int | str | list | None): current signing threshold input to Tholder
         ndigs (list | None): current signing key digests qb64
-        nsith int | str | list | None): next signing threshold input to Tholder
+        nsith (int | str | list | None): next signing threshold input to Tholder
         toad (int | str | None): witness threshold number if str then hex str
         wits (list | None): witness identifier prefixes qb64
         cnfg (list | None): configuration traits from TraitDex
         data (list | None): seal dicts
         version (Version): KERI protocol version string
         kind (str): serialization kind from Serials
         code (str | None): derivation code for computed prefix
@@ -811,17 +812,17 @@
 
     Parameters:
         pre (str): identifier prefix qb64
         keys  (list): current signing keys qb64
         dig (str): SAID of previous event qb64
         ilk (str): ilk of event. Must be in (Ilks.rot, Ilks.drt)
         sn (int | str): sequence number int or hex str
-        sith (int | str | list | None): current signing threshold input to Tholder
+        isith (int | str | list | None): current signing threshold input to Tholder
         ndigs (list | None): current signing key digests qb64
-        nsith int | str | list | None): next signing threshold input to Tholder
+        nsith (int | str | list | None): next signing threshold input to Tholder
         toad (int | str | None): witness threshold number if str then hex str
         wits (list | None): prior witness identifier prefixes qb64
         cuts (list | None): witness prefixes to cut qb64
         adds (list | None): witness prefixes to add qb64
         data (list | None): seal dicts
         version (Version): KERI protocol version string
         kind (str): serialization kind from Serials
@@ -2253,15 +2254,14 @@
                                   "".format(serder.ked))
 
         # Misfit check events that must be locally sourced (protected) get
         # escrowed in order to repair the protection when appropriate
         if (not local and
                 (self.locallyOwned() or
                  self.locallyWitnessed(wits=wits))):
-
             self.escrowMFEvent(serder=serder, sigers=sigers, wigers=wigers,
                                    seqner=delseqner, saider=delsaider, local=local)
             raise MisfitEventSourceError(f"Nonlocal source for locally owned"
                                              f"or locally witnessed event"
                                                  f" = {serder.ked}.")
 
 
@@ -2887,27 +2887,30 @@
             if seqner and saider:  # delegation for authorized delegated or issued event
                 couple = seqner.qb64b + saider.qb64b
                 self.db.setAes(dgkey, couple)  # authorizer (delegator/issuer) event seal
             fn = self.db.appendFe(serder.preb, serder.saidb)
             if firner and fn != firner.sn:  # cloned replay but replay fn not match
                 if self.cues is not None:  # cue to notice BadCloneFN
                     self.cues.push(dict(kin="noticeBadCloneFN", serder=serder,
-                                          fn=fn, firner=firner, dater=dater))
+                                        fn=fn, firner=firner, dater=dater))
                 logger.info("Kever Mismatch Cloned Replay FN: %s First seen "
-                            "ordinal fn %s and clone fn %s \nEvent=\n%s\n",
-                            serder.preb, fn, firner.sn, serder.pretty())
+                            "ordinal fn %s and clone fn %s, said=%s",
+                            serder.preb, fn, firner.sn, serder.said)
+                logger.debug(f"event=\n{serder.pretty()}\n")
             if dater:  # cloned replay use original's dts from dater
                 dtsb = dater.dtsb
             self.db.setDts(dgkey, dtsb)  # first seen so set dts to now
             self.db.fons.pin(keys=dgkey, val=Seqner(sn=fn))
-            logger.info("Kever state: %s First seen ordinal %s at %s\nEvent=\n%s\n",
-                        serder.preb, fn, dtsb.decode("utf-8"), serder.pretty())
+            logger.info("Kever state: %s First seen ordinal %s at %s, said=%s",
+                        serder.pre, fn, dtsb.decode("utf-8"), serder.said)
+            logger.debug(f"event=\n{serder.pretty()}\n")
         self.db.addKe(snKey(serder.preb, serder.sn), serder.saidb)
-        logger.info("Kever state: %s Added to KEL valid event=\n%s\n",
-                    serder.preb, serder.pretty())
+        logger.info("Kever state: %s Added to KEL valid said=%s",
+                    serder.pre, serder.said)
+        logger.debug(f"event=\n{serder.pretty()}\n")
         return (fn, dtsb.decode("utf-8"))  # (fn int, dts str) if first else (None, dts str)
 
 
     def escrowMFEvent(self, serder, sigers, wigers=None,
                       seqner=None, saider=None, local=True):
         """
         Update associated logs for escrow of MisFit event
@@ -2938,17 +2941,18 @@
         self.db.putSigs(dgkey, [siger.qb64b for siger in sigers])
         self.db.putEvt(dgkey, serder.raw)
         if wigers:
             self.db.putWigs(dgkey, [siger.qb64b for siger in wigers])
         if seqner and saider:
             couple = seqner.qb64b + saider.qb64b
             self.db.putPde(dgkey, couple)  # idempotent
-        self.db.misfits.add(snKey(serder.preb, serder.sn), serder.saidb)
+
+        res = self.db.misfits.add(keys=(serder.pre, serder.snh), val=serder.saidb)
         # log escrowed
-        logger.info("Kever state: escrowed misfit event=\n%s\n",
+        logger.debug("Kever state: escrowed misfit event=\n%s\n",
                     json.dumps(serder.ked, indent=1))
 
 
     def escrowDelegableEvent(self, serder, sigers, wigers=None, local=True):
         """
         Update associated logs for escrow of Delegable event that needs delegation
         via an anchored seal in delegator's KEl
@@ -2978,15 +2982,15 @@
         self.db.putDts(dgkey, helping.nowIso8601().encode("utf-8"))
         self.db.putSigs(dgkey, [siger.qb64b for siger in sigers])
         self.db.putEvt(dgkey, serder.raw)
         if wigers:
             self.db.putWigs(dgkey, [siger.qb64b for siger in wigers])
         self.db.delegables.add(snKey(serder.preb, serder.sn), serder.saidb)
         # log escrowed
-        logger.info("Kever state: escrowed delegable event=\n%s\n",
+        logger.debug("Kever state: escrowed delegable event=\n%s\n",
                     json.dumps(serder.ked, indent=1))
 
 
     def escrowPSEvent(self, serder, sigers, wigers=None, local=True):
         """
         Update associated logs for escrow of partially signed event
         or fully signed delegated event but not yet verified delegation.
@@ -3016,15 +3020,15 @@
             # otherwise don't change
         else:  # not preexisting so put
             esr = basing.EventSourceRecord(local=local)
             self.db.esrs.put(keys=dgkey, val=esr)
 
         snkey = snKey(serder.preb, serder.sn)
         self.db.addPse(snkey, serder.saidb)  # b'EOWwyMU3XA7RtWdelFt-6waurOTH_aW_Z9VTaU-CshGk.00000000000000000000000000000001'
-        logger.info("Kever state: Escrowed partially signed or delegated "
+        logger.debug("Kever state: Escrowed partially signed or delegated "
                     "event = %s\n", serder.ked)
 
 
     def escrowPACouple(self, serder, seqner, saider, local=True):
         """
         Update associated logs for escrow of partially authenticated issued event.
         Assuming signatures are provided elsewhere. Partial authentication results
@@ -3044,15 +3048,15 @@
                 False means event source is remote (unprotected).
                 Event validation logic is a function of local or remote
         """
         local = True if local else False  # ignored since not escrowing serder here
         dgkey = dgKey(serder.preb, serder.saidb)
         couple = seqner.qb64b + saider.qb64b
         self.db.putPde(dgkey, couple)  # idempotent
-        logger.info("Kever state: Escrowed source couple for partially signed "
+        logger.debug("Kever state: Escrowed source couple for partially signed "
                     "or delegated event = %s\n", serder.ked)
 
 
     def escrowPWEvent(self, serder, wigers, sigers=None,
                       seqner=None, saider=None, local=True):
         """
         Update associated logs for escrow of partially witnessed event
@@ -3087,15 +3091,15 @@
                 esr.local = local
                 self.db.esrs.pin(keys=dgkey, val=esr)
             # otherwise don't change
         else: # not preexisting so put
             esr = basing.EventSourceRecord(local=local)
             self.db.esrs.put(keys=dgkey, val=esr)
 
-        logger.info("Kever state: Escrowed partially witnessed "
+        logger.debug("Kever state: Escrowed partially witnessed "
                     "event = %s\n", serder.ked)
         return self.db.addPwe(snKey(serder.preb, serder.sn), serder.saidb)
 
 
     def state(self):
         """
         Returns KeyStateRecord instance of current key state
@@ -3701,19 +3705,22 @@
                 if wiger.verfer.transferable:  # skip transferable verfers
                     continue  # skip invalid witness prefix
 
                 if not self.lax and wiger.verfer.qb64 in self.prefixes:  # own is witness
                     if pre in self.prefixes:  # skip own receiptor of own event
                         # sign own events not receipt them
                         logger.info("Kevery process: skipped own receipt attachment"
-                                    " on own event receipt=\n%s\n", serder.pretty())
+                                    " on own event receipt=%s", serder.said)
+                        logger.debug(f"event=\n{serder.pretty()}\n")
+
                         continue  # skip own receipt attachment on own event
                     if not local:  # so skip own receipt on other event when non-local source
                         logger.info("Kevery process: skipped own receipt attachment"
-                                    " on nonlocal event receipt=\n%s\n", serder.pretty())
+                                    " on nonlocal event receipt=%s", serder.said)
+                        logger.debug(f"event=\n{serder.pretty()}\n")
                         continue  # skip own receipt attachment on non-local event
 
                 if wiger.verfer.verify(wiger.raw, lserder.raw):
                     # write receipt indexed sig to database
                     self.db.addWig(key=dgkey, val=wiger.qb64b)
 
         else:  # no events to be receipted yet at that sn so escrow
@@ -3773,19 +3780,22 @@
                 if cigar.verfer.transferable:  # skip transferable verfers
                     continue  # skip invalid couplets
 
                 if not self.lax and cigar.verfer.qb64 in self.prefixes:  # own is receiptor
                     if pre in self.prefixes:  # skip own receipter of own event
                         # sign own events not receipt them
                         logger.info("Kevery process: skipped own receipt attachment"
-                                    " on own event receipt=\n%s\n", serder.pretty())
+                                    " on own event receipt=%s", serder.said)
+                        logger.debug(f"event=\n{serder.pretty()}\n")
+
                         continue  # skip own receipt attachment on own event
                     if not local:  # skip own receipt on other event when not local
                         logger.info("Kevery process: skipped own receipt attachment"
-                                    " on nonlocal event receipt=\n%s\n", serder.pretty())
+                                    " on nonlocal event receipt=%s", serder.said)
+                        logger.debug(f"event=\n{serder.pretty()}\n")
                         continue  # skip own receipt attachment on non-local event
 
                 if cigar.verfer.verify(cigar.raw, lserder.raw):
                     wits = [wit.qb64 for wit in self.fetchWitnessState(pre, sn)]
                     rpre = cigar.verfer.qb64  # prefix of receiptor
                     if rpre in wits:  # its a witness receipt write in .wigs
                         index = wits.index(rpre)
@@ -3854,19 +3864,23 @@
         for cigar in cigars:
             if cigar.verfer.transferable:  # skip transferable verfers
                 continue  # skip invalid couplets
             if not self.lax and cigar.verfer.qb64 in self.prefixes:  # own is receiptor
                 if pre in self.prefixes:  # skip own receipter on own event
                     # sign own events not receipt them
                     logger.info("Kevery process: skipped own receipt attachment"
-                                " on own event receipt=\n%s\n", serder.pretty())
+                                " on own event receipt=%s", serder.said)
+                    logger.debug(f"event=\n{serder.pretty()}\n")
+
                     continue  # skip own receipt attachment on own event
                 if not local:  # own receipt on other event when not local
                     logger.info("Kevery process: skipped own receipt attachment"
-                                " on nonlocal event receipt=\n%s\n", serder.pretty())
+                                " on nonlocal event receipt=%s", serder.said)
+                    logger.debug(f"event=\n{serder.pretty()}\n")
+
                     continue  # skip own receipt attachment on non-local event
 
             if cigar.verfer.verify(cigar.raw, serder.raw):
                 wits = self.fetchWitnessState(pre, sn)
                 rpre = cigar.verfer.qb64  # prefix of receiptor
                 if rpre in wits:  # its a witness receipt
                     index = wits.index(rpre)
@@ -4064,15 +4078,15 @@
                 if siger.index >= len(sverfers):
                     raise ValidationError("Index = {} to large for keys."
                                           "".format(siger.index))
 
                 siger.verfer = sverfers[siger.index]  # assign verfer
                 if not siger.verfer.verify(siger.raw, serder.raw):  # verify sig
                     logger.info("Kevery unescrow error: Bad trans receipt sig."
-                                "pre=%s sn=%x receipter=%s\n", pre, sn, sprefixer.qb64)
+                                "pre=%s sn=%x receipter=%s", pre, sn, sprefixer.qb64)
 
                     raise ValidationError("Bad escrowed trans receipt sig at "
                                           "pre={} sn={:x} receipter={}."
                                           "".format(pre, sn, sprefixer.qb64))
 
                 # good sig so write receipt quadruple to database
 
@@ -4192,14 +4206,16 @@
             raise ValidationError(f"Invalid role={role} from attributes in "
                                   f"{Ilks.rpy} msg={serder.ked}.")
         eider = coring.Prefixer(qb64=data["eid"])  # raises error if unsupported code
         eid = eider.qb64  # controller of endpoint at role
         aid = cid  # authorizing attribution id
         keys = (aid, role, eid)
         osaider = self.db.eans.get(keys=keys)  # get old said if any
+        if osaider is not None and osaider.qb64b == saider.qb64b: # check idempotent
+            osaider = None
         # BADA Logic
         accepted = self.rvy.acceptReply(serder=serder, saider=saider, route=route,
                                         aid=aid, osaider=osaider, cigars=cigars,
                                         tsgs=tsgs)
         if not accepted:
             raise UnverifiedReplyError(f"Unverified end role reply. {serder.ked}")
 
@@ -4651,17 +4667,17 @@
         self.db.putSigs(dgkey, [siger.qb64b for siger in sigers])
         self.db.putEvt(dgkey, serder.raw)
         if wigers:
             self.db.putWigs(dgkey, [siger.qb64b for siger in wigers])
         if seqner and saider:
             couple = seqner.qb64b + saider.qb64b
             self.db.putPde(dgkey, couple)  # idempotent
-        self.db.misfits.add(snKey(serder.preb, serder.sn), serder.saidb)
+        self.db.misfits.add(keys=(serder.pre, serder.snh), val=serder.saidb)
         # log escrowed
-        logger.info("Kevery process: escrowed misfit event=\n%s\n",
+        logger.debug("Kevery process: escrowed misfit event=\n%s",
                     json.dumps(serder.ked, indent=1))
 
 
     def escrowOOEvent(self, serder, sigers, seqner=None, saider=None, wigers=None, local=True):
         """
         Update associated logs for escrow of Out-of-Order event
 
@@ -4693,16 +4709,16 @@
         if wigers:
             self.db.putWigs(dgkey, [siger.qb64b for siger in wigers])
         if seqner and saider:
             couple = seqner.qb64b + saider.qb64b
             self.db.putPde(dgkey, couple)  # idempotent
         self.db.addOoe(snKey(serder.preb, serder.sn), serder.saidb)
         # log escrowed
-        logger.info("Kevery process: escrowed out of order event=\n%s\n",
-                    json.dumps(serder.ked, indent=1))
+        logger.debug("Kevery process: escrowed out of order event=\n%s",
+                     json.dumps(serder.ked, indent=1))
 
     def escrowQueryNotFoundEvent(self, prefixer, serder, sigers, cigars=None):
         """
         Update associated logs for escrow of Out-of-Order event
 
         Parameters:
             prefixer (Prefixer): source of query message
@@ -4717,16 +4733,16 @@
         self.db.putEvt(dgkey, serder.raw)
         self.db.addQnf(dgkey, serder.saidb)
 
         for cigar in cigars:
             self.db.addRct(key=dgkey, val=cigar.verfer.qb64b + cigar.qb64b)
 
         # log escrowed
-        logger.info("Kevery process: escrowed query not found event=\n%s\n",
-                    json.dumps(serder.ked, indent=1))
+        logger.debug("Kevery process: escrowed query not found event=\n%s",
+                     json.dumps(serder.ked, indent=1))
 
     def escrowLDEvent(self, serder, sigers, local=True):
         """
         Update associated logs for escrow of Likely Duplicitous event
 
         Parameters:
             serder is SerderKERI instance of  event
@@ -4748,16 +4764,16 @@
             self.db.esrs.put(keys=dgkey, val=esr)
 
         self.db.putDts(dgkey, helping.nowIso8601().encode("utf-8"))
         self.db.putSigs(dgkey, [siger.qb64b for siger in sigers])
         self.db.putEvt(dgkey, serder.raw)
         self.db.addLde(snKey(serder.preb, serder.sn), serder.saidb)
         # log duplicitous
-        logger.info("Kevery process: escrowed likely duplicitous event=\n%s\n",
-                    json.dumps(serder.ked, indent=1))
+        logger.debug("Kevery process: escrowed likely duplicitous event=\n%s",
+                     json.dumps(serder.ked, indent=1))
 
     def escrowUWReceipt(self, serder, wigers, said):
         """
         Update associated logs for escrow of Unverified Event Witness Receipt
         (non-transferable)
         Escrowed value is couple edig+wig where:
            edig is receipted event dig not serder.dig
@@ -4784,16 +4800,16 @@
         for wiger in wigers:  # escrow each couple
             # don't know witness pre yet without witness list so no verfer in wiger
             # if wiger.verfer.transferable:  # skip transferable verfers
             # continue  # skip invalid triplets
             couple = said.encode("utf-8") + wiger.qb64b
             self.db.addUwe(key=snKey(serder.preb, serder.sn), val=couple)
         # log escrowed
-        logger.info("Kevery process: escrowed unverified witness indexed receipt"
-                    " of pre= %s sn=%x dig=%s\n", serder.pre, serder.sn, said)
+        logger.debug("Kevery process: escrowed unverified witness indexed receipt"
+                     " of pre= %s sn=%x dig=%s", serder.pre, serder.sn, said)
 
     def escrowUReceipt(self, serder, cigars, said):
         """
         Update associated logs for escrow of Unverified Event Receipt (non-transferable)
         Escrowed value is triple edig+rpre+cig where:
            edig is event dig
            rpre is nontrans receiptor prefix
@@ -4815,16 +4831,16 @@
         self.db.putDts(dgKey(serder.preb, said), helping.nowIso8601().encode("utf-8"))
         for cigar in cigars:  # escrow each triple
             if cigar.verfer.transferable:  # skip transferable verfers
                 continue  # skip invalid triplets
             triple = said.encode("utf-8") + cigar.verfer.qb64b + cigar.qb64b
             self.db.addUre(key=snKey(serder.preb, serder.sn), val=triple)  # should be snKey
         # log escrowed
-        logger.info("Kevery process: escrowed unverified receipt of pre= %s "
-                    " sn=%x dig=%s\n", serder.pre, serder.sn, said)
+        logger.debug("Kevery process: escrowed unverified receipt of pre= %s "
+                     " sn=%x dig=%s", serder.pre, serder.sn, said)
 
     def escrowTRGroups(self, serder, tsgs):
         """
         Update associated logs for escrow of Transferable Receipt Groups for
         event (transferable)
 
         Parameters:
@@ -4859,17 +4875,17 @@
             # serder.ked["d"] not serder.dig
             prelet = (serder.ked["d"].encode("utf-8") + prefixer.qb64b +
                       seqner.qb64b + saider.qb64b)
             for siger in sigers:  # escrow each quintlet
                 quintuple = prelet + siger.qb64b  # quintuple
                 self.db.addVre(key=snKey(serder.preb, serder.sn), val=quintuple)
             # log escrowed
-            logger.info("Kevery process: escrowed unverified transferable receipt "
-                        "of pre=%s sn=%x dig=%s by pre=%s\n", serder.pre,
-                        serder.sn, serder.ked["d"], prefixer.qb64)
+            logger.debug("Kevery process: escrowed unverified transferable receipt "
+                         "of pre=%s sn=%x dig=%s by pre=%s", serder.pre,
+                         serder.sn, serder.ked["d"], prefixer.qb64)
 
     def escrowTReceipts(self, serder, prefixer, seqner, saider, sigers):
         """
         Update associated logs for escrow of Transferable Event Receipt Group
         (transferable)
 
         Parameters:
@@ -4901,16 +4917,16 @@
         # serder.ked["d"] not serder.dig
         prelet = (serder.ked["d"].encode("utf-8") + prefixer.qb64b +
                   seqner.qb64b + saider.qb64b)
         for siger in sigers:  # escrow each quintlet
             quintuple = prelet + siger.qb64b  # quintuple
             self.db.addVre(key=snKey(serder.preb, serder.sn), val=quintuple)
         # log escrowed
-        logger.info("Kevery process: escrowed unverified transferable receipt "
-                    "of pre=%s sn=%x dig=%s by pre=%s\n", serder.pre,
+        logger.debug("Kevery process: escrowed unverified transferable receipt "
+                    "of pre=%s sn=%x dig=%s by pre=%s", serder.pre,
                     serder.sn, serder.ked["d"], prefixer.qb64)
 
     def escrowTRQuadruple(self, serder, sprefixer, sseqner, saider, siger):
         """
         Update associated logs for escrow of Unverified Transferable Receipt
         (transferable)
 
@@ -4934,17 +4950,17 @@
         # with different algos.  Can't lookup by dig for the same reason. Must
         # lookup last event by sn not by dig.
         self.db.putDts(dgKey(serder.preb, serder.said), helping.nowIso8601().encode("utf-8"))
         quintuple = (serder.saidb + sprefixer.qb64b + sseqner.qb64b +
                      saider.qb64b + siger.qb64b)
         self.db.addVre(key=snKey(serder.preb, serder.sn), val=quintuple)
         # log escrowed
-        logger.info("Kevery process: escrowed unverified transferabe validator "
-                    "receipt of pre= %s sn=%x dig=%s\n", serder.pre, serder.sn,
-                    serder.said)
+        logger.debug("Kevery process: escrowed unverified transferabe validator "
+                     "receipt of pre= %s sn=%x dig=%s", serder.pre, serder.sn,
+                     serder.said)
 
     def processEscrows(self):
         """
         Iterate throush escrows and process any that may now be finalized
 
         Parameters:
         """
@@ -4957,17 +4973,17 @@
             self.processEscrowPartialWigs()
             self.processEscrowPartialSigs()
             self.processEscrowDuplicitous()
             self.processQueryNotFound()
 
         except Exception as ex:  # log diagnostics errors etc
             if logger.isEnabledFor(logging.DEBUG):
-                logger.exception("Kevery escrow process error: %s\n", ex.args[0])
+                logger.exception("Kevery escrow process error: %s", ex.args[0])
             else:
-                logger.error("Kevery escrow process error: %s\n", ex.args[0])
+                logger.error("Kevery escrow process error: %s", ex.args[0])
             raise ex
 
     def processEscrowOutOfOrders(self):
         """
         Process events escrowed by Kever that are recieved out-of-order.
         An event is out of order if its prior event has not been accepted into its KEL.
         Without the prior event there is no way to know the key state and therefore no way
@@ -5016,48 +5032,48 @@
                                               "at dig = {}.".format(bytes(edig)))
 
                     # check date if expired then remove escrow.
                     dtb = self.db.getDts(dgkey)
                     if dtb is None:  # othewise is a datetime as bytes
                         # no date time so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Missing event datetime"
-                                    " at dig = %s\n", bytes(edig))
+                                    " at dig = %s", bytes(edig))
 
                         raise ValidationError("Missing escrowed event datetime "
                                               "at dig = {}.".format(bytes(edig)))
 
                     # do date math here and discard if stale nowIso8601() bytes
                     dtnow = helping.nowUTC()
                     dte = helping.fromIso8601(bytes(dtb))
                     if (dtnow - dte) > datetime.timedelta(seconds=self.TimeoutOOE):
                         # escrow stale so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Stale event escrow "
-                                    " at dig = %s\n", bytes(edig))
+                                    " at dig = %s", bytes(edig))
 
                         raise ValidationError("Stale event escrow "
                                               "at dig = {}.".format(bytes(edig)))
 
                     # get the escrowed event using edig
                     eraw = self.db.getEvt(dgKey(pre, bytes(edig)))
                     if eraw is None:
                         # no event so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Missing event at."
-                                    "dig = %s\n", bytes(edig))
+                                    "dig = %s", bytes(edig))
 
                         raise ValidationError("Missing escrowed evt at dig = {}."
                                               "".format(bytes(edig)))
 
                     eserder = serdering.SerderKERI(raw=bytes(eraw))  # escrowed event
 
                     #  get sigs and attach
                     sigs = self.db.getSigs(dgKey(pre, bytes(edig)))
                     if not sigs:  # otherwise its a list of sigs
                         # no sigs so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Missing event sigs at."
-                                    "dig = %s\n", bytes(edig))
+                                    "dig = %s", bytes(edig))
 
                         raise ValidationError("Missing escrowed evt sigs at "
                                               "dig = {}.".format(bytes(edig)))
 
                     # process event
                     sigers = [Siger(qb64b=bytes(sig)) for sig in sigs]
 
@@ -5080,33 +5096,34 @@
                     # So re-escrow attempt will not change the escrowed ooe db.
                     # Non re-escrow ValidationError means some other issue so unescrow.
                     # No error at all means processed successfully so also unescrow.
 
                 except OutOfOrderError as ex:
                     # still waiting on missing prior event to validate
                     if logger.isEnabledFor(logging.DEBUG):
-                        logger.exception("Kevery unescrow failed: %s\n", ex.args[0])
+                        logger.exception("Kevery unescrow failed: %s", ex.args[0])
                     else:
-                        logger.error("Kevery unescrow failed: %s\n", ex.args[0])
+                        logger.error("Kevery unescrow failed: %s", ex.args[0])
 
                 except Exception as ex:  # log diagnostics errors etc
                     # error other than out of order so remove from OO escrow
                     self.db.delOoe(snKey(pre, sn), edig)  # removes one escrow at key val
                     if logger.isEnabledFor(logging.DEBUG):
-                        logger.exception("Kevery unescrowed: %s\n", ex.args[0])
+                        logger.exception("Kevery unescrowed: %s", ex.args[0])
                     else:
-                        logger.error("Kevery unescrowed: %s\n", ex.args[0])
+                        logger.error("Kevery unescrowed: %s", ex.args[0])
 
                 else:  # unescrow succeeded, remove from escrow
                     # We don't remove all escrows at pre,sn because some might be
                     # duplicitous so we process remaining escrows in spite of found
                     # valid event escrow.
                     self.db.delOoe(snKey(pre, sn), edig)  # removes one escrow at key val
                     logger.info("Kevery unescrow succeeded in valid event: "
-                                "event=\n%s\n", json.dumps(eserder.ked, indent=1))
+                                "event=%s", eserder.said)
+                    logger.debug(f"event=\n{eserder.pretty()}\n")
 
             if ekey == key:  # still same so no escrows found on last while iteration
                 break
             key = ekey  # setup next while iteration, with key after ekey
 
     def processEscrowPartialSigs(self):
         """
@@ -5156,47 +5173,47 @@
                                               "at dig = {}.".format(bytes(edig)))
 
                     # check date if expired then remove escrow.
                     dtb = self.db.getDts(dgkey)
                     if dtb is None:  # othewise is a datetime as bytes
                         # no date time so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Missing event datetime"
-                                    " at dig = %s\n", bytes(edig))
+                                    " at dig = %s", bytes(edig))
 
                         raise ValidationError("Missing escrowed event datetime "
                                               "at dig = {}.".format(bytes(edig)))
 
                     # do date math here and discard if stale nowIso8601() bytes
                     dtnow = helping.nowUTC()
                     dte = helping.fromIso8601(bytes(dtb))
                     if (dtnow - dte) > datetime.timedelta(seconds=self.TimeoutPSE):
                         # escrow stale so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Stale event escrow "
-                                    " at dig = %s\n", bytes(edig))
+                                    " at dig = %s", bytes(edig))
 
                         raise ValidationError("Stale event escrow "
                                               "at dig = {}.".format(bytes(edig)))
 
                     # get the escrowed event using edig
                     eraw = self.db.getEvt(dgkey)
                     if eraw is None:
                         # no event so so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Missing event at."
-                                    "dig = %s\n", bytes(edig))
+                                    "dig = %s", bytes(edig))
 
                         raise ValidationError("Missing escrowed evt at dig = {}."
                                               "".format(bytes(edig)))
 
                     eserder = serdering.SerderKERI(raw=bytes(eraw))  # escrowed event
                     #  get sigs and attach
                     sigs = self.db.getSigs(dgkey)
                     if not sigs:  # otherwise its a list of sigs
                         # no sigs so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Missing event sigs at."
-                                    "dig = %s\n", bytes(edig))
+                                    "dig = %s", bytes(edig))
 
                         raise ValidationError("Missing escrowed evt sigs at "
                                               "dig = {}.".format(bytes(edig)))
 
                     # seal source (delegator issuer if any)
                     delseqner = delsaider = None
                     couple = self.db.getPde(dgkey)
@@ -5235,42 +5252,43 @@
                     # So re-escrow attempt will not change the escrowed pse db.
                     # Non re-escrow ValidationError means some other issue so unescrow.
                     # No error at all means processed successfully so also unescrow.
 
                 except (MissingSignatureError, MissingDelegationError) as ex:
                     # still waiting on missing sigs or missing seal to validate
                     if logger.isEnabledFor(logging.DEBUG):
-                        logger.exception("Kevery unescrow failed: %s\n", ex.args[0])
+                        logger.exception("Kevery unescrow failed: %s", ex.args[0])
                     else:
-                        logger.error("Kevery unescrow failed: %s\n", ex.args[0])
+                        logger.error("Kevery unescrow failed: %s", ex.args[0])
 
                 except Exception as ex:  # log diagnostics errors etc
                     # error other than waiting on sigs or seal so remove from escrow
                     self.db.delPse(snKey(pre, sn), edig)  # removes one escrow at key val
 
                     if eserder is not None and eserder.ked["t"] in (Ilks.dip, Ilks.drt,):
                         self.cues.push(dict(kin="psUnescrow", serder=eserder))
 
                     if logger.isEnabledFor(logging.DEBUG):
-                        logger.exception("Kevery unescrowed: %s\n", ex.args[0])
+                        logger.exception("Kevery unescrowed: %s", ex.args[0])
                     else:
-                        logger.error("Kevery unescrowed: %s\n", ex.args[0])
+                        logger.error("Kevery unescrowed: %s", ex.args[0])
 
                 else:  # unescrow succeeded, remove from escrow
                     # We don't remove all escrows at pre,sn because some might be
                     # duplicitous so we process remaining escrows in spite of found
                     # valid event escrow.
                     self.db.delPse(snKey(pre, sn), edig)  # removes one escrow at key val
                     self.db.delPde(dgkey)  # remove escrow if any
 
                     if eserder is not None and eserder.ked["t"] in (Ilks.dip, Ilks.drt,):
                         self.cues.push(dict(kin="psUnescrow", serder=eserder))
 
                     logger.info("Kevery unescrow succeeded in valid event: "
-                                "event=\n%s\n", json.dumps(eserder.ked, indent=1))
+                                "event=%s", eserder.said)
+                    logger.debug(f"event=\n{eserder.pretty()}\n")
 
             if ekey == key:  # still same so no escrows found on last while iteration
                 break
             key = ekey  # setup next while iteration, with key after ekey
 
     def processEscrowPartialWigs(self):
         """
@@ -5321,62 +5339,62 @@
                                               "at dig = {}.".format(bytes(edig)))
 
                     # check date if expired then remove escrow.
                     dtb = self.db.getDts(dgkey)
                     if dtb is None:  # othewise is a datetime as bytes
                         # no date time so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Missing event datetime"
-                                    " at dig = %s\n", bytes(edig))
+                                    " at dig = %s", bytes(edig))
 
                         raise ValidationError("Missing escrowed event datetime "
                                               "at dig = {}.".format(bytes(edig)))
 
                     # do date math here and discard if stale nowIso8601() bytes
                     dtnow = helping.nowUTC()
                     dte = helping.fromIso8601(bytes(dtb))
                     if (dtnow - dte) > datetime.timedelta(seconds=self.TimeoutPWE):
                         # escrow stale so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Stale event escrow "
-                                    " at dig = %s\n", bytes(edig))
+                                    " at dig = %s", bytes(edig))
 
                         raise ValidationError("Stale event escrow "
                                               "at dig = {}.".format(bytes(edig)))
 
                     # get the escrowed event using edig
                     eraw = self.db.getEvt(dgKey(pre, bytes(edig)))
                     if eraw is None:
                         # no event so so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Missing event at."
-                                    "dig = %s\n", bytes(edig))
+                                    "dig = %s", bytes(edig))
 
                         raise ValidationError("Missing escrowed evt at dig = {}."
                                               "".format(bytes(edig)))
 
                     eserder = serdering.SerderKERI(raw=bytes(eraw))  # escrowed event
 
                     #  get sigs
                     sigs = self.db.getSigs(dgKey(pre, bytes(edig)))  # list of sigs
                     if not sigs:  # empty list
                         # no sigs so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Missing event sigs at."
-                                    "dig = %s\n", bytes(edig))
+                                    "dig = %s", bytes(edig))
 
                         raise ValidationError("Missing escrowed evt sigs at "
                                               "dig = {}.".format(bytes(edig)))
 
                     #  get wigs
                     wigs = self.db.getWigs(dgKey(pre, bytes(edig)))  # list of wigs
 
                     if not wigs:  # empty list
                         # wigs maybe empty while waiting for first witness signature
                         # which may not arrive until some time after event is fully signed
                         # so just log for debugging but do not unescrow by raising
                         # ValidationError
-                        logger.info("Kevery unescrow wigs: No event wigs yet at."
-                                    "dig = %s\n", bytes(edig))
+                        logger.debug("Kevery unescrow wigs: No event wigs yet at."
+                                     "dig = %s", bytes(edig))
 
                         # raise ValidationError("Missing escrowed evt wigs at "
                         # "dig = {}.".format(bytes(edig)))
 
                     # process event
                     sigers = [Siger(qb64b=bytes(sig)) for sig in sigs]
                     wigers = [Siger(qb64b=bytes(wig)) for wig in wigs]
@@ -5406,33 +5424,34 @@
                     # Assumes that controller signature validation and delegation
                     # validation will be successful as event would not be in
                     # partially witnessed escrow unless they had already validated
 
                 except MissingWitnessSignatureError as ex:
                     # still waiting on missing witness sigs
                     if logger.isEnabledFor(logging.DEBUG):
-                        logger.exception("Kevery unescrow failed: %s\n", ex.args[0])
+                        logger.exception("Kevery unescrow failed: %s", ex.args[0])
                     else:
-                        logger.error("Kevery unescrow failed: %s\n", ex.args[0])
+                        logger.error("Kevery unescrow failed: %s", ex.args[0])
 
                 except Exception as ex:  # log diagnostics errors etc
                     # error other than waiting on sigs or seal so remove from escrow
                     self.db.delPwe(snKey(pre, sn), edig)  # removes one escrow at key val
                     if logger.isEnabledFor(logging.DEBUG):
-                        logger.exception("Kevery unescrowed: %s\n", ex.args[0])
+                        logger.exception("Kevery unescrowed: %s", ex.args[0])
                     else:
-                        logger.error("Kevery unescrowed: %s\n", ex.args[0])
+                        logger.error("Kevery unescrowed: %s", ex.args[0])
 
                 else:  # unescrow succeeded, remove from escrow
                     # We don't remove all escrows at pre,sn because some might be
                     # duplicitous so we process remaining escrows in spite of found
                     # valid event escrow.
                     self.db.delPwe(snKey(pre, sn), edig)  # removes one escrow at key val
                     logger.info("Kevery unescrow succeeded in valid event: "
-                                "event=\n%s\n", json.dumps(eserder.ked, indent=1))
+                                "event=%s", eserder.said)
+                    logger.debug(f"event=\n{eserder.pretty()}\n")
 
             if ekey == key:  # still same so no escrows found on last while iteration
                 break
             key = ekey  # setup next while iteration, with key after ekey
 
     def processEscrowUnverWitness(self):
         """
@@ -5495,68 +5514,68 @@
                     rdiger, wiger = deWitnessCouple(ecouple)
 
                     # check date if expired then remove escrow.
                     dtb = self.db.getDts(dgKey(pre, bytes(rdiger.qb64b)))
                     if dtb is None:  # othewise is a datetime as bytes
                         # no date time so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Missing event datetime"
-                                    " at dig = %s\n", rdiger.qb64b)
+                                    " at dig = %s", rdiger.qb64b)
 
                         raise ValidationError("Missing escrowed event datetime "
                                               "at dig = {}.".format(rdiger.qb64b))
 
                     # do date math here and discard if stale nowIso8601() bytes
                     dtnow = helping.nowUTC()
                     dte = helping.fromIso8601(bytes(dtb))
                     if (dtnow - dte) > datetime.timedelta(seconds=self.TimeoutUWE):
                         # escrow stale so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Stale event escrow "
-                                    " at dig = %s\n", rdiger.qb64b)
+                                    " at dig = %s", rdiger.qb64b)
 
                         raise ValidationError("Stale event escrow "
                                               "at dig = {}.".format(rdiger.qb64b))
 
                     # lookup database dig of the receipted event in pwes escrow
                     # using pre and sn lastEvt
                     found = self._processEscrowFindUnver(pre=pre,
                                                          sn=sn,
                                                          rsaider=rdiger,
                                                          wiger=wiger)
 
                     if not found:  # no partial witness escrow of event found
                         # so keep in escrow by raising UnverifiedWitnessReceiptError
-                        logger.info("Kevery unescrow error: Missing witness "
-                                    "receipted evt at pre=%s sn=%x\n", (pre, sn))
+                        logger.debug("Kevery unescrow error: Missing witness "
+                                    "receipted evt at pre=%s sn=%x", (pre, sn))
 
                         raise UnverifiedWitnessReceiptError("Missing witness "
                                                             "receipted evt at pre={}  sn={:x}".format(pre, sn))
 
                 except UnverifiedWitnessReceiptError as ex:
                     # still waiting on missing prior event to validate
                     # only happens if we process above
                     if logger.isEnabledFor(logging.DEBUG):  # adds exception data
-                        logger.exception("Kevery unescrow failed: %s\n", ex.args[0])
+                        logger.exception("Kevery unescrow failed: %s", ex.args[0])
                     else:
-                        logger.error("Kevery unescrow failed: %s\n", ex.args[0])
+                        logger.error("Kevery unescrow failed: %s", ex.args[0])
 
                 except Exception as ex:  # log diagnostics errors etc
                     # error other than out of order so remove from OO escrow
                     self.db.delUwe(snKey(pre, sn), ecouple)  # removes one escrow at key val
                     if logger.isEnabledFor(logging.DEBUG):  # adds exception data
-                        logger.exception("Kevery unescrowed: %s\n", ex.args[0])
+                        logger.exception("Kevery unescrowed: %s", ex.args[0])
                     else:
-                        logger.error("Kevery unescrowed: %s\n", ex.args[0])
+                        logger.error("Kevery unescrowed: %s", ex.args[0])
 
                 else:  # unescrow succeeded, remove from escrow
                     # We don't remove all escrows at pre,sn because some might be
                     # duplicitous so we process remaining escrows in spite of found
                     # valid event escrow.
                     self.db.delUwe(snKey(pre, sn), ecouple)  # removes one escrow at key val
                     logger.info("Kevery unescrow succeeded for event pre=%s "
-                                "sn=%s\n", pre, sn)
+                                "sn=%s", pre, sn)
 
             if ekey == key:  # still same so no escrows found on last while iteration
                 break
             key = ekey  # setup next while iteration, with key after ekey
 
     def processEscrowUnverNonTrans(self):
         """
@@ -5615,26 +5634,26 @@
                     cigar.verfer = Verfer(qb64b=sprefixer.qb64b)
 
                     # check date if expired then remove escrow.
                     dtb = self.db.getDts(dgKey(pre, bytes(rsaider.qb64b)))
                     if dtb is None:  # othewise is a datetime as bytes
                         # no date time so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Missing event datetime"
-                                    " at dig = %s\n", rsaider.qb64b)
+                                    " at dig = %s", rsaider.qb64b)
 
                         raise ValidationError("Missing escrowed event datetime "
                                               "at dig = {}.".format(rsaider.qb64b))
 
                     # do date math here and discard if stale nowIso8601() bytes
                     dtnow = helping.nowUTC()
                     dte = helping.fromIso8601(bytes(dtb))
                     if (dtnow - dte) > datetime.timedelta(seconds=self.TimeoutURE):
                         # escrow stale so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Stale event escrow "
-                                    " at dig = %s\n", rsaider.qb64b)
+                                    " at dig = %s", rsaider.qb64b)
 
                         raise ValidationError("Stale event escrow "
                                               "at dig = {}.".format(rsaider.qb64b))
 
                     # Is receipt for unverified witnessed event in .Pwes escrow
                     # if found then try else clause will remove from escrow
                     found = self._processEscrowFindUnver(pre=pre,
@@ -5646,45 +5665,45 @@
                         # so process as escrow of receipt for accept event
                         # not two stage witnessed event escrow
                         # get dig of receipted accepted event in kel using lastEvt
                         # at pre and sn
 
                         dig = self.db.getKeLast(snKey(pre, sn))
                         if dig is None:  # no receipted event so keep in escrow
-                            logger.info("Kevery unescrow error: Missing receipted "
-                                        "event at pre=%s sn=%x\n", pre, sn)
+                            logger.debug("Kevery unescrow error: Missing receipted "
+                                        "event at pre=%s sn=%x", pre, sn)
 
                             raise UnverifiedReceiptError("Missing receipted evt "
                                                          "at pre={} sn={:x}".format(pre, sn))
 
                         # get receipted event using pre and edig
                         raw = self.db.getEvt(dgKey(pre, dig))
                         if raw is None:  # receipted event superseded so remove from escrow
                             logger.info("Kevery unescrow error: Invalid receipted "
-                                        "event refereance at pre=%s sn=%x\n", pre, sn)
+                                        "event refereance at pre=%s sn=%x", pre, sn)
 
                             raise ValidationError("Invalid receipted evt reference"
                                                   " at pre={} sn={:x}".format(pre, sn))
 
                         serder = serdering.SerderKERI(raw=bytes(raw))  # receipted event
 
                         #  compare digs
                         if rsaider.qb64b != serder.saidb:
                             logger.info("Kevery unescrow error: Bad receipt dig."
-                                        "pre=%s sn=%x receipter=%s\n", pre, sn, sprefixer.qb64)
+                                        "pre=%s sn=%x receipter=%s", pre, sn, sprefixer.qb64)
 
                             raise ValidationError("Bad escrowed receipt dig at "
                                                   "pre={} sn={:x} receipter={}."
                                                   "".format(pre, sn, sprefixer.qb64))
 
                         #  verify sig verfer key is prefixer from triple
                         if not cigar.verfer.verify(cigar.raw, serder.raw):
                             # no sigs so raise ValidationError which unescrows below
                             logger.info("Kevery unescrow error: Bad receipt sig."
-                                        "pre=%s sn=%x receipter=%s\n", pre, sn, sprefixer.qb64)
+                                        "pre=%s sn=%x receipter=%s", pre, sn, sprefixer.qb64)
 
                             raise ValidationError("Bad escrowed receipt sig at "
                                                   "pre={} sn={:x} receipter={}."
                                                   "".format(pre, sn, sprefixer.qb64))
 
                         # get current wits from kever state assuming not stale
                         # receipt. Need function here to compute wits for actual
@@ -5703,33 +5722,33 @@
                             self.db.addRct(key=dgKey(pre, serder.said), val=couple)
 
 
                 except UnverifiedReceiptError as ex:
                     # still waiting on missing prior event to validate
                     # only happens if we process above
                     if logger.isEnabledFor(logging.DEBUG):  # adds exception data
-                        logger.exception("Kevery unescrow failed: %s\n", ex.args[0])
+                        logger.exception("Kevery unescrow failed: %s", ex.args[0])
                     else:
-                        logger.error("Kevery unescrow failed: %s\n", ex.args[0])
+                        logger.error("Kevery unescrow failed: %s", ex.args[0])
 
                 except Exception as ex:  # log diagnostics errors etc
                     # error other than out of order so remove from OO escrow
                     self.db.delUre(snKey(pre, sn), etriplet)  # removes one escrow at key val
                     if logger.isEnabledFor(logging.DEBUG):  # adds exception data
-                        logger.exception("Kevery unescrowed: %s\n", ex.args[0])
+                        logger.exception("Kevery unescrowed: %s", ex.args[0])
                     else:
-                        logger.error("Kevery unescrowed: %s\n", ex.args[0])
+                        logger.error("Kevery unescrowed: %s", ex.args[0])
 
                 else:  # unescrow succeeded, remove from escrow
                     # We don't remove all escrows at pre,sn because some might be
                     # duplicitous so we process remaining escrows in spite of found
                     # valid event escrow.
                     self.db.delUre(snKey(pre, sn), etriplet)  # removes one escrow at key val
                     logger.info("Kevery unescrow succeeded for event pre=%s "
-                                "sn=%s\n", pre, sn)
+                                "sn=%s", pre, sn)
 
             if ekey == key:  # still same so no escrows found on last while iteration
                 break
             key = ekey  # setup next while iteration, with key after ekey
 
     def processQueryNotFound(self):
         """
@@ -5764,48 +5783,48 @@
                 try:
                     pre, _ = splitKey(ekey)  # get pre and sn from escrow item
                     # check date if expired then remove escrow.
                     dtb = self.db.getDts(dgKey(pre, bytes(edig)))
                     if dtb is None:  # othewise is a datetime as bytes
                         # no date time so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Missing event datetime"
-                                    " at dig = %s\n", bytes(edig))
+                                    " at dig = %s", bytes(edig))
 
                         raise ValidationError("Missing escrowed event datetime "
                                               "at dig = {}.".format(bytes(edig)))
 
                     # do date math here and discard if stale nowIso8601() bytes
                     dtnow = helping.nowUTC()
                     dte = helping.fromIso8601(bytes(dtb))
                     if (dtnow - dte) > datetime.timedelta(seconds=self.TimeoutQNF):
                         # escrow stale so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Stale qry event escrow "
-                                    " at dig = %s\n", bytes(edig))
+                                    " at dig = %s", bytes(edig))
 
                         raise ValidationError("Stale qry event escrow "
                                               "at dig = {}.".format(bytes(edig)))
 
                     # get the escrowed event using edig
                     eraw = self.db.getEvt(dgKey(pre, bytes(edig)))
                     if eraw is None:
                         # no event so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Missing event at."
-                                    "dig = %s\n", bytes(edig))
+                                    "dig = %s", bytes(edig))
 
                         raise ValidationError("Missing escrowed evt at dig = {}."
                                               "".format(bytes(edig)))
 
                     eserder = serdering.SerderKERI(raw=bytes(eraw))  # escrowed event
 
                     #  get sigs and attach
                     sigs = self.db.getSigs(dgKey(pre, bytes(edig)))
                     if not sigs:  # otherwise its a list of sigs
                         # no sigs so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Missing event sigs at."
-                                    "dig = %s\n", bytes(edig))
+                                    "dig = %s", bytes(edig))
 
                         raise ValidationError("Missing escrowed evt sigs at "
                                               "dig = {}.".format(bytes(edig)))
 
                     # process event
                     sigers = [Siger(qb64b=bytes(sig)) for sig in sigs]
 
@@ -5824,32 +5843,33 @@
 
                     source = coring.Prefixer(qb64b=pre)
                     self.processQuery(serder=eserder, source=source, sigers=sigers, cigars=cigars)
 
                 except QueryNotFoundError as ex:
                     # still waiting on missing prior event to validate
                     if logger.isEnabledFor(logging.DEBUG):
-                        logger.exception("Kevery unescrow failed: %s\n", ex.args[0])
+                        logger.exception("Kevery unescrow failed: %s", ex.args[0])
                     else:
-                        logger.error("Kevery unescrow failed: %s\n", ex.args[0])
+                        logger.error("Kevery unescrow failed: %s", ex.args[0])
 
                 except Exception as ex:  # log diagnostics errors etc
                     # error other than out of order so remove from OO escrow
                     self.db.delQnf(dgKey(pre, edig), edig)  # removes one escrow at key val
                     if logger.isEnabledFor(logging.DEBUG):
-                        logger.exception("Kevery unescrowed: %s\n", ex.args[0])
+                        logger.exception("Kevery unescrowed: %s", ex.args[0])
                     else:
-                        logger.error("Kevery unescrowed: %s\n", ex.args[0])
+                        logger.error("Kevery unescrowed: %s", ex.args[0])
                 else:  # unescrow succeeded, remove from escrow
                     # We don't remove all escrows at pre,sn because some might be
                     # duplicitous so we process remaining escrows in spite of found
                     # valid event escrow.
                     self.db.delQnf(dgKey(pre, edig), edig)  # removes one escrow at key val
                     logger.info("Kevery unescrow succeeded in valid event: "
-                                "event=\n%s\n", json.dumps(eserder.ked, indent=1))
+                                "event=%s", eserder.said)
+                    logger.debug(f"event=\n{eserder.pretty()}\n")
 
             if ekey == key:  # still same so no escrows found on last while iteration
                 break
             key = ekey  # setup next while iteration, with key after ekey
 
 
     def _processEscrowFindUnver(self, pre, sn, rsaider, wiger=None, cigar=None):
@@ -5933,27 +5953,27 @@
                     found = True
                     break  # done with search have caller add wig.
 
             elif wiger:  # check index and assign verfier to wiger
                 if wiger.index >= len(wits):  # bad index
                     # raise ValidationError which removes from escrow by caller
                     logger.info("Kevery unescrow error: Bad witness receipt"
-                                " index=%i for pre=%s sn=%x\n", wiger.index, pre, sn)
+                                " index=%i for pre=%s sn=%x", wiger.index, pre, sn)
                     raise ValidationError("Bad escrowed witness receipt index={}"
                                           " at pre={} sn={:x}.".format(wiger.index, pre, sn))
 
                 wiger.verfer = Verfer(qb64=wits[wiger.index])
                 found = True
                 break  # done with search have caller add wig.
 
         if found:  # verify signature and if verified write to .Wigs
             if not wiger.verfer.verify(wiger.raw, serder.raw):  # not verify
                 # raise ValidationError which unescrows .Uwes or .Ures in caller
                 logger.info("Kevery unescrow error: Bad witness receipt"
-                            " wig. pre=%s sn=%x\n", pre, sn)
+                            " wig. pre=%s sn=%x", pre, sn)
 
                 raise ValidationError("Bad escrowed witness receipt wig"
                                       " at pre={} sn={:x}."
                                       "".format(pre, sn))
             self.db.addWig(key=dgKey(pre, serder.said), val=wiger.qb64b)
             # processEscrowPartialWigs removes from this .Pwes escrow
             # when fully witnessed using self.db.delPwe(snkey, dig)
@@ -6014,69 +6034,69 @@
                     esaider, sprefixer, sseqner, ssaider, siger = deTransReceiptQuintuple(equinlet)
 
                     # check date if expired then remove escrow.
                     dtb = self.db.getDts(dgKey(pre, bytes(esaider.qb64b)))
                     if dtb is None:  # othewise is a datetime as bytes
                         # no date time so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Missing event datetime"
-                                    " at dig = %s\n", esaider.qb64b)
+                                    " at dig = %s", esaider.qb64b)
 
                         raise ValidationError("Missing escrowed event datetime "
                                               "at dig = {}.".format(esaider.qb64b))
 
                     # do date math here and discard if stale nowIso8601() bytes
                     dtnow = helping.nowUTC()
                     dte = helping.fromIso8601(bytes(dtb))
                     if (dtnow - dte) > datetime.timedelta(seconds=self.TimeoutVRE):
                         # escrow stale so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Stale event escrow "
-                                    " at dig = %s\n", esaider.qb64b)
+                                    " at dig = %s", esaider.qb64b)
 
                         raise ValidationError("Stale event escrow "
                                               "at dig = {}.".format(esaider.qb64b))
 
                     # get dig of the receipted event using pre and sn lastEvt
                     raw = self.db.getKeLast(snKey(pre, sn))
                     if raw is None:
                         # no event so keep in escrow
-                        logger.info("Kevery unescrow error: Missing receipted "
-                                    "event at pre=%s sn=%x\n", pre, sn)
+                        logger.debug("Kevery unescrow error: Missing receipted "
+                                    "event at pre=%s sn=%x", pre, sn)
 
                         raise UnverifiedTransferableReceiptError("Missing receipted evt at pre={} "
                                                                  " sn={:x}".format(pre, sn))
 
                     dig = bytes(raw)
                     # get receipted event using pre and edig
                     raw = self.db.getEvt(dgKey(pre, dig))
                     if raw is None:  # receipted event superseded so remove from escrow
                         logger.info("Kevery unescrow error: Invalid receipted "
-                                    "event referenace at pre=%s sn=%x\n", pre, sn)
+                                    "event referenace at pre=%s sn=%x", pre, sn)
 
                         raise ValidationError("Invalid receipted evt reference "
                                               "at pre={} sn={:x}".format(pre, sn))
 
                     serder = serdering.SerderKERI(raw=bytes(raw))  # receipted event
 
                     #  compare digs
                     if esaider.qb64b != serder.saidb:
                         logger.info("Kevery unescrow error: Bad receipt dig."
-                                    "pre=%s sn=%x receipter=%s\n", (pre, sn, sprefixer.qb64))
+                                    "pre=%s sn=%x receipter=%s", (pre, sn, sprefixer.qb64))
 
                         raise ValidationError("Bad escrowed receipt dig at "
                                               "pre={} sn={:x} receipter={}."
                                               "".format(pre, sn, sprefixer.qb64))
 
                     # get receipter's last est event
                     # retrieve dig of last event at sn of receipter.
                     sdig = self.db.getKeLast(key=snKey(pre=sprefixer.qb64b,
                                                        sn=sseqner.sn))
                     if sdig is None:
                         # no event so keep in escrow
-                        logger.info("Kevery unescrow error: Missing receipted "
-                                    "event at pre=%s sn=%x\n", pre, sn)
+                        logger.debug("Kevery unescrow error: Missing receipted "
+                                    "event at pre=%s sn=%x", pre, sn)
 
                         raise UnverifiedTransferableReceiptError("Missing receipted evt at pre={} "
                                                                  " sn={:x}".format(pre, sn))
 
                     # retrieve last event itself of receipter
                     sraw = self.db.getEvt(key=dgKey(pre=sprefixer.qb64b, dig=bytes(sdig)))
                     # assumes db ensures that sraw must not be none because sdig was in KE
@@ -6099,47 +6119,48 @@
                     if siger.index >= len(verfers):
                         raise ValidationError("Index = {} to large for keys."
                                               "".format(siger.index))
 
                     siger.verfer = verfers[siger.index]  # assign verfer
                     if not siger.verfer.verify(siger.raw, serder.raw):  # verify sig
                         logger.info("Kevery unescrow error: Bad trans receipt sig."
-                                    "pre=%s sn=%x receipter=%s\n", pre, sn, sprefixer.qb64)
+                                    "pre=%s sn=%x receipter=%s", pre, sn, sprefixer.qb64)
 
                         raise ValidationError("Bad escrowed trans receipt sig at "
                                               "pre={} sn={:x} receipter={}."
                                               "".format(pre, sn, sprefixer.qb64))
 
                     # good sig so write receipt quadruple to database
                     quadruple = sealet + siger.qb64b
                     self.db.addVrc(key=dgKey(pre, serder.said), val=quadruple)
 
 
                 except UnverifiedTransferableReceiptError as ex:
                     # still waiting on missing prior event to validate
                     # only happens if we process above
                     if logger.isEnabledFor(logging.DEBUG):  # adds exception data
-                        logger.exception("Kevery unescrow failed: %s\n", ex.args[0])
+                        logger.exception("Kevery unescrow failed: %s", ex.args[0])
                     else:
-                        logger.error("Kevery unescrow failed: %s\n", ex.args[0])
+                        logger.error("Kevery unescrow failed: %s", ex.args[0])
 
                 except Exception as ex:  # log diagnostics errors etc
                     # error other than out of order so remove from OO escrow
                     self.db.delVre(snKey(pre, sn), equinlet)  # removes one escrow at key val
                     if logger.isEnabledFor(logging.DEBUG):  # adds exception data
-                        logger.exception("Kevery unescrowed: %s\n", ex.args[0])
+                        logger.exception("Kevery unescrowed: %s", ex.args[0])
                     else:
-                        logger.error("Kevery unescrowed: %s\n", ex.args[0])
+                        logger.error("Kevery unescrowed: %s", ex.args[0])
 
                 else:  # unescrow succeeded, remove from escrow
                     # We don't remove all escrows at pre,sn because some might be
                     # duplicitous so we process remaining escrows in spite of found
                     # valid event escrow.
                     self.db.delVre(snKey(pre, sn), equinlet)  # removes one escrow at key val
-                    logger.info("Kevery unescrow succeeded for event = %s\n", serder.ked)
+                    logger.info("Kevery unescrow succeeded for event = %s", serder.said)
+                    logger.debug(f"event=\n{serder.pretty()}\n")
 
             if ekey == key:  # still same so no escrows found on last while iteration
                 break
             key = ekey  # setup next while iteration, with key after ekey
 
     def processEscrowDuplicitous(self):
         """
@@ -6189,48 +6210,48 @@
                                               "at dig = {}.".format(bytes(edig)))
 
                     # check date if expired then remove escrow.
                     dtb = self.db.getDts(dgkey)
                     if dtb is None:  # othewise is a datetime as bytes
                         # no date time so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Missing event datetime"
-                                    " at dig = %s\n", bytes(edig))
+                                    " at dig = %s", bytes(edig))
 
                         raise ValidationError("Missing escrowed event datetime "
                                               "at dig = {}.".format(bytes(edig)))
 
                     # do date math here and discard if stale nowIso8601() bytes
                     dtnow = helping.nowUTC()
                     dte = helping.fromIso8601(bytes(dtb))
                     if (dtnow - dte) > datetime.timedelta(seconds=self.TimeoutLDE):
                         # escrow stale so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Stale event escrow "
-                                    " at dig = %s\n", bytes(edig))
+                                    " at dig = %s", bytes(edig))
 
                         raise ValidationError("Stale event escrow "
                                               "at dig = {}.".format(bytes(edig)))
 
                     # get the escrowed event using edig
                     eraw = self.db.getEvt(dgKey(pre, bytes(edig)))
                     if eraw is None:
                         # no event so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Missing event at."
-                                    "dig = %s\n", bytes(edig))
+                                    "dig = %s", bytes(edig))
 
                         raise ValidationError("Missing escrowed evt at dig = {}."
                                               "".format(bytes(edig)))
 
                     eserder = serdering.SerderKERI(raw=bytes(eraw))  # escrowed event
 
                     #  get sigs and attach
                     sigs = self.db.getSigs(dgKey(pre, bytes(edig)))
                     if not sigs:  # otherwise its a list of sigs
                         # no sigs so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Missing event sigs at."
-                                    "dig = %s\n", bytes(edig))
+                                    "dig = %s", bytes(edig))
 
                         raise ValidationError("Missing escrowed evt sigs at "
                                               "dig = {}.".format(bytes(edig)))
 
                     sigers = [Siger(qb64b=bytes(sig)) for sig in sigs]
                     self.processEvent(serder=eserder, sigers=sigers, local=esr.local)
 
@@ -6247,33 +6268,34 @@
                     # So re-escrow attempt will not change the escrowed ooe db.
                     # Non re-escrow ValidationError means some other issue so unescrow.
                     # No error at all means processed successfully so also unescrow.
 
                 except LikelyDuplicitousError as ex:
                     # still can't determine if duplicitous
                     if logger.isEnabledFor(logging.DEBUG):
-                        logger.exception("Kevery unescrow failed: %s\n", ex.args[0])
+                        logger.exception("Kevery unescrow failed: %s", ex.args[0])
                     else:
-                        logger.error("Kevery unescrow failed: %s\n", ex.args[0])
+                        logger.error("Kevery unescrow failed: %s", ex.args[0])
 
                 except Exception as ex:  # log diagnostics errors etc
                     # error other than likely duplicitous so remove from escrow
                     self.db.delLde(snKey(pre, sn), edig)  # removes one escrow at key val
                     if logger.isEnabledFor(logging.DEBUG):
-                        logger.exception("Kevery unescrowed: %s\n", ex.args[0])
+                        logger.exception("Kevery unescrowed: %s", ex.args[0])
                     else:
-                        logger.error("Kevery unescrowed: %s\n", ex.args[0])
+                        logger.error("Kevery unescrowed: %s", ex.args[0])
 
                 else:  # unescrow succeeded, remove from escrow
                     # We don't remove all escrows at pre,sn because some might be
                     # duplicitous so we process remaining escrows in spite of found
                     # valid event escrow.
                     self.db.delLde(snKey(pre, sn), edig)  # removes one escrow at key val
                     logger.info("Kevery unescrow succeeded in valid event: "
-                                "event=\n%s\n", json.dumps(eserder.ked, indent=1))
+                                "event=%s", eserder.said)
+                    logger.debug(f"event=\n{eserder.pretty()}\n")
 
             if ekey == key:  # still same so no escrows found on last while iteration
                 break
             key = ekey  # setup next while iteration, with key after ekey
 
     def duplicity(self, serder, sigers):
         """
```

### Comparing `keri-1.2.0.dev0/src/keri/core/indexing.py` & `keri-1.2.0.dev1/src/keri/core/indexing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/core/parsing.py` & `keri-1.2.0.dev1/src/keri/core/parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,22 @@
 """
 keri.core.parsing module
 
 message stream parsing support
 """
 
 import logging
-import traceback
-from collections import namedtuple
-from dataclasses import dataclass, astuple
 
 from .coring import (Ilks, CtrDex, Counter, Seqner, Cigar,
-                     Dater, Verfer, Prefixer, Saider, Pather, Protocols )
+                     Dater, Verfer, Prefixer, Saider, Pather)
 from .indexing import (Siger, )
 from . import serdering
 from .. import help
 from .. import kering
-from ..kering import ColdDex, Colds, sniff
+from ..kering import Colds, sniff
 
 logger = help.ogler.getLogger()
 
 
 class Parser:
     """
     Parser is stream parser that processes an incoming message stream.
@@ -426,33 +423,33 @@
                                                    exc=exc,
                                                    rvy=rvy,
                                                    vry=vry,
                                                    local=local)
 
             except kering.SizedGroupError as ex:  # error inside sized group
                 # processOneIter already flushed group so do not flush stream
-                if logger.isEnabledFor(logging.ERROR):
-                    logger.exception("Parser msg extraction error: %s\n", ex.args[0])
+                if logger.isEnabledFor(logging.DEBUG):
+                    logger.exception("Parser msg extraction error: %s", ex.args[0])
                 else:
-                    logger.error("Parser msg extraction error: %s\n", ex.args[0])
+                    logger.error("Parser msg extraction error: %s", ex.args[0])
 
             except (kering.ColdStartError, kering.ExtractionError) as ex:  # some extraction error
-                if logger.isEnabledFor(logging.ERROR):
-                    logger.exception("Parser msg extraction error: %s\n", ex.args[0])
+                if logger.isEnabledFor(logging.DEBUG):
+                    logger.exception("Parser msg extraction error: %s", ex.args[0])
                 else:
-                    logger.error("Parser msg extraction error: %s\n", ex.args[0])
+                    logger.error("Parser msg extraction error: %s", ex.args[0])
                 del ims[:]  # delete rest of stream to force cold restart
 
             except (kering.ValidationError, Exception) as ex:  # non Extraction Error
                 # Non extraction errors happen after successfully extracted from stream
                 # so we don't flush rest of stream just resume
-                if logger.isEnabledFor(logging.ERROR):
-                    logger.exception("Parser msg non-extraction error: %s\n", ex)
+                if logger.isEnabledFor(logging.DEBUG):
+                    logger.exception("Parser msg non-extraction error: %s", ex)
                 else:
-                    logger.error("Parser msg non-extraction error: %s\n", ex)
+                    logger.error("Parser msg non-extraction error: %s", ex)
             yield
 
         return True
 
 
     def onceParsator(self, ims=None, framed=None, pipeline=None, kvy=None,
                      tvy=None, exc=None, rvy=None, vry=None, local=None):
@@ -511,33 +508,33 @@
                                                    exc=exc,
                                                    rvy=rvy,
                                                    vry=vry,
                                                    local=local)
 
             except kering.SizedGroupError as ex:  # error inside sized group
                 # processOneIter already flushed group so do not flush stream
-                if logger.isEnabledFor(logging.ERROR):
-                    logger.exception("Kevery msg extraction error: %s\n", ex.args[0])
+                if logger.isEnabledFor(logging.DEBUG):
+                    logger.exception("Kevery msg extraction error: %s", ex.args[0])
                 else:
-                    logger.error("Kevery msg extraction error: %s\n", ex.args[0])
+                    logger.error("Kevery msg extraction error: %s", ex.args[0])
 
             except (kering.ColdStartError, kering.ExtractionError) as ex:  # some extraction error
-                if logger.isEnabledFor(logging.ERROR):
-                    logger.exception("Kevery msg extraction error: %s\n", ex.args[0])
+                if logger.isEnabledFor(logging.DEBUG):
+                    logger.exception("Kevery msg extraction error: %s", ex.args[0])
                 else:
-                    logger.error("Kevery msg extraction error: %s\n", ex.args[0])
+                    logger.error("Kevery msg extraction error: %s", ex.args[0])
                 del ims[:]  # delete rest of stream to force cold restart
 
             except (kering.ValidationError, Exception) as ex:  # non Extraction Error
                 # Non extraction errors happen after successfully extracted from stream
                 # so we don't flush rest of stream just resume
-                if logger.isEnabledFor(logging.ERROR):
-                    logger.exception("Kevery msg non-extraction error: %s\n", ex.args[0])
+                if logger.isEnabledFor(logging.DEBUG):
+                    logger.exception("Kevery msg non-extraction error: %s", ex.args[0])
                 else:
-                    logger.error("Kevery msg non-extraction error: %s\n", ex.args[0])
+                    logger.error("Kevery msg non-extraction error: %s", ex.args[0])
             finally:
                 done = True
 
         return done
 
 
     def parsator(self, ims=None, framed=None, pipeline=None, kvy=None, tvy=None,
@@ -601,33 +598,33 @@
                                                    exc=exc,
                                                    rvy=rvy,
                                                    vry=vry,
                                                    local=local)
 
             except kering.SizedGroupError as ex:  # error inside sized group
                 # processOneIter already flushed group so do not flush stream
-                if logger.isEnabledFor(logging.ERROR):
-                    logger.exception("Parser msg extraction error: %s\n", ex.args[0])
+                if logger.isEnabledFor(logging.DEBUG):
+                    logger.exception("Parser msg extraction error: %s", ex.args[0])
                 else:
-                    logger.error("Parser msg extraction error: %s\n", ex.args[0])
+                    logger.error("Parser msg extraction error: %s", ex.args[0])
 
             except (kering.ColdStartError, kering.ExtractionError) as ex:  # some extraction error
-                if logger.isEnabledFor(logging.ERROR):
-                    logger.exception("Parser msg extraction error: %s\n", ex.args[0])
+                if logger.isEnabledFor(logging.DEBUG):
+                    logger.exception("Parser msg extraction error: %s", ex.args[0])
                 else:
-                    logger.error("Parser msg extraction error: %s\n", ex.args[0])
+                    logger.error("Parser msg extraction error: %s", ex.args[0])
                 del ims[:]  # delete rest of stream to force cold restart
 
             except (kering.ValidationError, Exception) as ex:  # non Extraction Error
                 # Non extraction errors happen after successfully extracted from stream
                 # so we don't flush rest of stream just resume
-                if logger.isEnabledFor(logging.ERROR):
-                    logger.exception("Parser msg non-extraction error: %s\n", ex.args[0])
+                if logger.isEnabledFor(logging.DEBUG):
+                    logger.exception("Parser msg non-extraction error: %s", ex.args[0])
                 else:
-                    logger.error("Parser msg non-extraction error: %s\n", ex.args[0])
+                    logger.error("Parser msg non-extraction error: %s", ex.args[0])
             yield
 
         return True  # should never return
 
 
     def msgParsator(self, ims=None, framed=True, pipeline=False,
                     kvy=None, tvy=None, exc=None, rvy=None, vry=None, local=None):
```

### Comparing `keri-1.2.0.dev0/src/keri/core/routing.py` & `keri-1.2.0.dev1/src/keri/core/routing.py`

 * *Files 6% similar despite different names*

```diff
@@ -263,70 +263,79 @@
         for cigar in cigars:  # process each couple to verify sig and write to db
             if cigar.verfer.transferable:  # ignore invalid transferable verfers
                 continue  # skip invalid transferable
 
             if not self.lax and cigar.verfer.qb64 in self.prefixes:  # own cig
                 if not self.local:  # own cig when not local so ignore
                     logger.info("Kevery process: skipped own attachment"
-                                " on nonlocal reply msg=\n%s\n", serder.pretty())
+                                " on nonlocal reply said=", serder.said)
+                    logger.debug(f"event=\n{serder.pretty()}\n")
+
                     continue  # skip own cig attachment on non-local reply msg
 
             if aid != cigar.verfer.qb64:  # cig not by aid
                 logger.info("Kevery process: skipped cig not from aid="
-                            "%s on reply msg=\n%s\n", aid, serder.pretty())
+                            "%s on reply said=%s", aid, serder.said)
+                logger.debug(f"event=\n{serder.pretty()}\n")
                 continue  # skip invalid cig's verfer is not aid
 
             if odater:  # get old compare datetimes to see if later
                 if dater.datetime <= odater.datetime:
                     logger.info("Kevery process: skipped stale update from "
-                                "%s of reply msg=\n%s\n", aid, serder.pretty())
+                                "%s of reply said=%s", aid, serder.said)
+                    logger.debug(f"event=\n{serder.pretty()}\n")
                     continue  # skip if not later
                     # raise ValidationError(f"Stale update of {route} from {aid} "
                     # f"via {Ilks.rpy}={serder.ked}.")
 
             if not cigar.verfer.verify(cigar.raw, serder.raw):  # cig not verify
                 logger.info("Kevery process: skipped nonverifying cig from "
-                            "%s on reply msg=\n%s\n", cigar.verfer.qb64, serder.pretty())
+                            "%s on reply said=%s", cigar.verfer.qb64, serder.said)
+                logger.debug(f"event=\n{serder.pretty()}\n")
                 continue  # skip if cig not verify
 
             # All constraints satisfied so update
             self.updateReply(serder=serder, saider=saider, dater=dater, cigar=cigar)
             self.removeReply(saider=osaider)  # remove obsoleted reply artifacts
             accepted = True
             break  # first valid cigar sufficient ignore any duplicates in cigars
 
         for prefixer, seqner, ssaider, sigers in tsgs:  # iterate over each tsg
             if not self.lax and prefixer.qb64 in self.prefixes:  # own sig
                 if not self.local:  # own sig when not local so ignore
                     logger.info("Kevery process: skipped own attachment"
-                                " on nonlocal reply msg=\n%s\n", serder.pretty())
+                                " on nonlocal reply said=%s", serder.said)
+                    logger.debug(f"event=\n{serder.pretty()}\n")
                     continue  # skip own sig attachment on non-local reply msg
 
             spre = prefixer.qb64
             if aid != spre:  # sig not by aid
                 logger.info("Kevery process: skipped signature not from aid="
-                            "%s on reply msg=\n%s\n", aid, serder.pretty())
+                            "%s on reply said=%s", aid, serder.said)
+                logger.debug(f"event=\n{serder.pretty()}\n")
                 continue  # skip invalid signature is not from aid
 
             if osaider:  # check if later logic  sn > or sn == and dt >
                 if otsgs := eventing.fetchTsgs(db=self.db.ssgs, saider=osaider):
                     _, osqr, _, _ = otsgs[0]  # zeroth should be authoritative
 
                     if seqner.sn < osqr.sn:  # sn earlier
                         logger.info("Kevery process: skipped stale key state sig"
-                                    "from %s sn=%s<%s on reply msg=\n%s\n",
-                                    aid, seqner.sn, osqr.sn, serder.pretty())
+                                    "from %s sn=%s<%s on reply said=%s",
+                                    aid, seqner.sn, osqr.sn, serder.said)
+                        logger.debug(f"event=\n{serder.pretty()}\n")
                         continue  # skip if sn earlier
 
                     if seqner.sn == osqr.sn:  # sn same so check datetime
                         if odater:
                             if dater.datetime <= odater.datetime:
                                 logger.info("Kevery process: skipped stale key"
-                                            "state sig datetime from %s on reply msg=\n%s\n",
-                                            aid, serder.pretty())
+                                            "state sig datetime from %s on reply said=%s",
+                                            aid, serder.said)
+                                logger.debug(f"event=\n{serder.pretty()}\n")
                                 continue  # skip if not later
 
             # retrieve sdig of last event at sn of signer.
             sdig = self.db.getKeLast(key=dbing.snKey(pre=spre, sn=seqner.sn))
             if sdig is None:
                 # create cue here to request key state for sprefixer signer
                 # signer's est event not yet in signer's KEL
@@ -471,47 +480,48 @@
                                          f"for route={route}.")
 
                     # do date math for stale escrow
                     if ((helping.nowUTC() - dater.datetime) >
                             datetime.timedelta(seconds=self.TimeoutRPE)):
                         # escrow stale so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Stale reply escrow "
-                                    " at route = %s\n", route)
+                                    " at route = %s", route)
 
                         raise kering.ValidationError(f"Stale reply escrow at route = {route}.")
 
                     self.processReply(serder=serder, tsgs=tsgs)
 
                 except kering.UnverifiedReplyError as ex:
                     # still waiting on missing prior event to validate
                     if logger.isEnabledFor(logging.DEBUG):
-                        logger.exception("Kevery unescrow attempt failed: %s\n", ex.args[0])
+                        logger.exception("Kevery unescrow attempt failed: %s", ex.args[0])
                     else:
-                        logger.error("Kevery unescrow attempt failed: %s\n", ex.args[0])
+                        logger.error("Kevery unescrow attempt failed: %s", ex.args[0])
 
                 except Exception as ex:  # other error so remove from reply escrow
                     self.db.rpes.rem(keys=(route, ), val=saider)  # remove escrow only
                     self.removeReply(saider)  # remove escrow reply artifacts
                     if logger.isEnabledFor(logging.DEBUG):
-                        logger.exception("Kevery unescrowed due to error: %s\n", ex.args[0])
+                        logger.exception("Kevery unescrowed due to error: %s", ex.args[0])
                     else:
-                        logger.error("Kevery unescrowed due to error: %s\n", ex.args[0])
+                        logger.error("Kevery unescrowed due to error: %s", ex.args[0])
 
                 else:  # unescrow succeded
                     self.db.rpes.rem(keys=(route, ), val=saider)  # remove escrow only
-                    logger.info("Kevery unescrow succeeded for reply=\n%s\n",
-                                serder.pretty())
+                    logger.info("Kevery unescrow succeeded for reply said=%s",
+                                serder.said)
+                    logger.debug(f"event=\n{serder.pretty()}\n")
 
             except Exception as ex:  # log diagnostics errors etc
                 self.db.rpes.rem(keys=(route,), val=saider)  # remove escrow only
                 self.removeReply(saider)  # remove escrow reply artifacts
                 if logger.isEnabledFor(logging.DEBUG):
-                    logger.exception("Kevery unescrowed due to error: %s\n", ex.args[0])
+                    logger.exception("Kevery unescrowed due to error: %s", ex.args[0])
                 else:
-                    logger.error("Kevery unescrowed due to error: %s\n", ex.args[0])
+                    logger.error("Kevery unescrowed due to error: %s", ex.args[0])
 
 
 class Route:
     """ Route class for registration of reply message handlers
 
     This class represents a registered route internally to the Revery.
     the properties are created by using the Falcon compile route utility method
```

### Comparing `keri-1.2.0.dev0/src/keri/core/scheming.py` & `keri-1.2.0.dev1/src/keri/core/scheming.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/core/serdering.py` & `keri-1.2.0.dev1/src/keri/core/serdering.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,34 +15,38 @@
 import blake3
 import hashlib
 from  ordered_set import OrderedSet as oset
 
 
 from .. import kering
 from ..kering import (ValidationError,  MissingFieldError, ExtraFieldError,
-                      AlternateFieldError,
+                      AlternateFieldError, InvalidValueError,
                       ShortageError, VersionError, ProtocolError, KindError,
                       DeserializeError, FieldError, SerializeError)
 from ..kering import (Versionage, Version, Vrsn_1_0, Vrsn_2_0,
                       VERRAWSIZE, VERFMT,
                       MAXVERFULLSPAN, VER1FULLSPAN,  VER2FULLSPAN)
 from ..kering import SMELLSIZE, Smellage, smell
 
-from ..kering import Protocols, Serials, Rever, versify, deversify, Ilks
-from ..core import coring
+from ..kering import Protocols, Serials, versify, deversify, Ilks
+
+from .. import help
+from ..help import helping
+
+
+from . import coring
 from .coring import MtrDex, DigDex, PreDex, Saids,  Digestage
 from .coring import (Matter, Saider, Verfer, Diger, Number, Tholder, Tagger,
                      Ilker, Traitor, Verser, )
 
-from ..core import counting
-from ..core.counting import GenDex, AllTags, Counter
+from .counting import GenDex, AllTags, Counter, SealDex_2_0
+
+from .structing import Sealer, SClanDom
+
 
-from .. import help
-from ..help import helping
-from ..help.helping import nonStringSequence
 
 logger = help.ogler.getLogger()
 
 
 
 
 @dataclass
@@ -339,28 +343,42 @@
 
     """
     Dummy = "#"  # dummy spaceholder char for SAID. Must not be a valid Base64 char
 
     # Spans dict keyed by version (Versionage instance) of version string span (size)
     Spans = {Vrsn_1_0: VER1FULLSPAN, Vrsn_2_0: VER2FULLSPAN}
 
-    # should be same set of codes as in coring.DigestCodex coring.DigDex so
-    # .digestive property works. Use unit tests to ensure codex sets match
+    # Maps digest codes to Digestages of algorithms for computing digest.
+    # Should be based on the same set of codes as in coring.DigestCodex
+    # coring.DigDex so .digestive property works.
+    # Use unit tests to ensure codex elements sets match
     Digests = {
         DigDex.Blake3_256: Digestage(klas=blake3.blake3, size=None, length=None),
         DigDex.Blake2b_256: Digestage(klas=hashlib.blake2b, size=32, length=None),
         DigDex.Blake2s_256: Digestage(klas=hashlib.blake2s, size=None, length=None),
         DigDex.SHA3_256: Digestage(klas=hashlib.sha3_256, size=None, length=None),
         DigDex.SHA2_256: Digestage(klas=hashlib.sha256, size=None, length=None),
         DigDex.Blake3_512: Digestage(klas=blake3.blake3, size=None, length=64),
         DigDex.Blake2b_512: Digestage(klas=hashlib.blake2b, size=None, length=None),
         DigDex.SHA3_512: Digestage(klas=hashlib.sha3_512, size=None, length=None),
         DigDex.SHA2_512: Digestage(klas=hashlib.sha512, size=None, length=None),
     }
 
+    # map seal clan names to seal counter code for grouping seals in anchor list
+    ClanCodes = dict()
+    ClanCodes[SClanDom.SealDigest.__name__] = SealDex_2_0.DigestSealSingles
+    ClanCodes[SClanDom.SealRoot.__name__] = SealDex_2_0.MerkleRootSealSingles
+    ClanCodes[SClanDom.SealBacker.__name__] = SealDex_2_0.BackerRegistrarSealCouples
+    ClanCodes[SClanDom.SealLast.__name__] = SealDex_2_0.SealSourceLastSingles
+    ClanCodes[SClanDom.SealTrans.__name__] = SealDex_2_0.SealSourceCouples
+    ClanCodes[SClanDom.SealEvent.__name__] = SealDex_2_0.SealSourceTriples
+
+    # map seal counter code to seal clan name for parsing seal groups in anchor list
+    CodeClans = { val: key for key, val in ClanCodes.items()}  # invert dict
+
     #override in subclass to enforce specific protocol
     Protocol = None  # class based message protocol, None means any in Protocols is ok
     Proto = Protocols.keri  # default message protocol type for makify on base Serder
     Vrsn = Vrsn_1_0  # default protocol version for protocol type
     Kind = Serials.json  # default serialization kind
     CVrsn = Vrsn_2_0  # default CESR code table version
 
@@ -638,15 +656,16 @@
                 except Exception as ex:
                     logger.error("Invalid sad for Serder %s\n%s",
                                  self.pretty(), ex.args[0])
                     raise ValidationError(f"Invalid sad for Serder ="
                                               f"{self._sad}.") from ex
 
         else:
-            raise ValueError("Improper initialization need raw or sad or makify.")
+            raise InvalidValueError("Improper initialization need raw or sad "
+                                    f"or makify.")
 
 
 
     def verify(self):
         """Verifies said(s) in sad against raw
         Override for protocol and ilk specific verification behavior. Especially
         for inceptive ilks that have more than one said field like a said derived
@@ -836,15 +855,15 @@
                    - the code extracted from sad[said label] when valid CESR
                    - the code provided in .Fields...saids
         """
         sproto = svrsn = skind = silk = None
         if sad and 'v' in sad:  # attempt to get from vs in sad
             try:  # extract version string elements as defaults if provided
                 sproto, svrsn, skind, _, _ = deversify(sad["v"])
-            except ValueError as ex:
+            except VersionError as ex:
                 pass
             else:
                 silk = sad.get('t')  # if 't' not in sad .get returns None which may be valid
 
         if proto is None:
             proto = sproto if sproto is not None else self.Proto
 
@@ -978,28 +997,28 @@
             # generate new version string with correct size
             vs = versify(protocol=proto, version=vrsn, kind=kind, size=size)
             sad["v"] = vs  # update version string in sad
             # now have correctly sized version string in sad
 
 
         # compute saidive digestive field values using raw from sized dummied sad
-        raw = self.dumps(sad, kind=kind)  # serialize sized dummied sad
+        raw = self.dumps(sad, kind=kind, proto=proto, vrsn=vrsn)  # serialize sized dummied sad
         for label, code in _saids.items():
             if code in DigDex:  # subclass override if non digestive allowed
                 klas, dsize, dlen = self.Digests[code]  # digest algo size & length
                 ikwa = dict()  # digest algo class initi keyword args
                 if dsize:
                     ikwa.update(digest_size=dsize)  # optional digest_size
                 dkwa = dict()  # digest method keyword args
                 if dlen:
                     dkwa.update(length=dlen)
                 dig = Matter(raw=klas(raw, **ikwa).digest(**dkwa), code=code).qb64
                 sad[label] = dig
 
-        raw = self.dumps(sad, kind=kind)  # compute final raw
+        raw = self.dumps(sad, kind=kind, proto=proto, vrsn=vrsn)  # compute final raw
         if kind == Serials.cesr:# cesr kind version string does not set size
             size = len(raw) # size of whole message
 
         self._raw = raw
         self._sad = sad
         self._proto = proto
         self._vrsn = vrsn
@@ -1141,114 +1160,130 @@
         self._sad = sad
         self._proto = proto
         self._vrsn = vrsn
         self._kind = kind
         self._size = size
 
 
-    def dumps(self, sad, kind=Serials.json):
+    def dumps(self, sad=None, kind=Serials.json, proto=None, vrsn=None):
         """Method to handle serialization by kind
         Assumes sad fields are properly filled out for serialization kind.
 
         Returns:
-           raw (bytes): serialization of sad dict using serialization kind
+            raw (bytes): serialization of sad dict using serialization kind
 
         Parameters:
-           sad (dict | list)): serializable dict or list to serialize
-           kind (str): value of Serials (Serialage) serialization kind
+            sad (dict | list | None)): serializable dict or list to serialize
+            kind (str): value of Serials (Serialage) serialization kind
                 "JSON", "MGPK", "CBOR", "CSER"
+            proto (str | None): desired protocol type str value of Protocols
+                If None then eventually use self.proto
+            vrsn (Versionage | None): instance desired protocol version
+                If None then eventually self.vrsn
+
 
         Notes:
             dumps of json uses str whereas dumps of cbor and msgpack use bytes
             crypto opts want bytes not bytearray
         """
+        sad = sad if sad is not None else self.sad
+
         if kind == Serials.json:
             raw = json.dumps(sad, separators=(",", ":"),
                              ensure_ascii=False).encode("utf-8")
 
         elif kind == Serials.mgpk:
             raw = msgpack.dumps(sad)
 
         elif kind == Serials.cbor:
             raw = cbor.dumps(sad)
 
-        elif kind == Serials.cser:
-            raw = self._dumps(sad)
+        elif kind == Serials.cesr:  # does not support list only dict
+            raw = self._dumps(sad, proto=proto, vrsn=vrsn)
 
         else:
             raise SerializeError(f"Invalid serialization kind = {kind}")
 
         return raw
 
 
-    def _dumps(self, sad):
+    def _dumps(self, sad=None, proto=None, vrsn=None):
         """CESR native serialization of sad
 
         Returns:
             raw (bytes): CESR native serialization of sad dict
 
         Parameters:
-            sad (dict | list)): serializable dict or list to serialize
+            sad (dict | None)): serializable dict to serialize
+            proto (str | None): desired protocol type str value of Protocols
+                If None then self.proto
+            vrsn (Versionage | None): instance desired protocol version
+                If None then self.vrsn
 
         Versioning:
             CESR native serialization includes in its fixed version field
             a version primitive that includes message protocol+protocol version
             +genus version: 0NPPPPMmmMmm (12 B64 characters)
 
             This assumes that genus is compatible with message
             protocol so genus is not needed. This protects from malleability attack
             and ensure compatible cesr codes especially count (group) codes.
             Primitive codes are less problematic since so far all primitive codes
             tables are backwards compatible across major versions.
 
         """
-        if (self.gvrsn.major < Vrsn_2_0.major or
-            self.vrsn.major < Vrsn_2_0.major):
-                raise SerializeError(f"Invalid major genus version={self.gvrsn}"
-                                f"or Invalid major protocol version={self.vrsn}"
+        sad = sad if sad is not None else self.sad
+        proto = proto if proto is not None else self.proto
+        vrsn = vrsn if vrsn is not None else self.vrsn
+
+        if (self.gvrsn.major < Vrsn_2_0.major or vrsn.major < Vrsn_2_0.major):
+            raise SerializeError(f"Invalid major genus version={self.gvrsn}"
+                                f"or Invalid major protocol version={vrsn}"
                                 f" for native CESR serialization.")
 
         if self.genus not in GenDex:  # ensures self.genus != None
             raise SerializeError(f"Invalid genus={self.genus}.")
 
-        if getattr(GenDex, self.proto, None) != self.genus:
-            raise SerializeError(f"Incompatible protocol={self.proto} with "
+        if getattr(GenDex, proto, None) != self.genus:
+            raise SerializeError(f"Incompatible protocol={proto} with "
                                  f"genus={self.genus}.")
 
 
-        fixed = True  # True = use fixed field, False= use field map
 
-        raw = bytearray()
-        ilks = self.Fields[self.proto][self.vrsn]  # get fields keyed by ilk
+
+        raw = bytearray()  # message as qb64
+        bdy = bytearray()  # message body as qb64
+        ilks = self.Fields[proto][vrsn]  # get fields keyed by ilk
 
         ilk = sad.get('t')  # returns None if missing message type (ilk)
         if ilk not in ilks:  #
             raise SerializeError(f"Missing message type field "
-                                 f"'t' for protocol={self.proto} "
-                                 f"version={self.vrsn} with {sad=}.")
+                                 f"'t' for protocol={proto} "
+                                 f"version={vrsn} with {sad=}.")
 
         fields = ilks[ilk]  # FieldDom for given protocol and ilk
 
         if fields.opts or not fields.strict:  # optional or extra fields allowed
             fixed = False  # so must use field map
+        else:
+            fixed = True  #fixed field
 
 
         # assumes that sad's field ordering and field inclusion is correct
         # so can serialize in order to compute saidive fields
         # need to fix ._verify and .makify to account for CESR native serialization
 
-        if self.proto == Protocols.keri:
-            for l, v in sad.items():  # assumes valid field order & presence
-                if not fixed:  # prepend label
-                    pass
+        if proto == Protocols.keri:
+            if not fixed:  # prepend label
+                pass  # raise error
 
-                # should dispatch or use match instead of big if else
+            for l, v in sad.items():  # assumes valid field order & presence
                 match l:  # label
                     case "v":  # protocol+version  do not use version string itself
-                        val = Verser(proto=self.proto, vrsn=self.vrsn).qb64b
+                        val = Verser(proto=proto, vrsn=vrsn).qb64b
 
                     case "t":  # message type (ilk), already got ilk
                         val = Ilker(ilk=v).qb64b  # assumes same
 
                     case "d" | "i" | "p" | "di":  # said or aid
                         val = v.encode("utf-8")  # already primitive qb64 make qb6b
 
@@ -1260,82 +1295,96 @@
 
                     case "k" | "n" | "b" | "ba" | "br":  # list of primitives
                         frame = bytearray()
                         for e in v:  # list
                             frame.extend(e.encode("utf-8"))
 
                         val = bytearray(Counter(tag=AllTags.GenericListGroup,
-                                                count=len(frame) % 4).qb64b)
+                                                count=len(frame) // 4).qb64b)
                         val.extend(frame)
 
                     case "c":  # list of config traits strings
                         frame = bytearray()
                         for e in v:  # list
-                            frame.extend(Traitor(trait=e).qb64n)
+                            frame.extend(Traitor(trait=e).qb64b)
 
                         val = bytearray(Counter(tag=AllTags.GenericListGroup,
-                                                count=len(frame) % 4).qb64b)
+                                                count=len(frame) // 4).qb64b)
                         val.extend(frame)
 
                     case "a":  # list of seals or field map of attributes
-                        frame = bytearray()
+                        frame = bytearray()  # whole list
+                        gcode = None  # code for counter for consecutive same type seals
+                        gframe = bytearray()  # consecutive same type seals
                         for e in v:  # list of seal dicts
-                            pass
-                            #if tuple(v) == eventing.SealEvent._fields:
-                                #eseal = eventing.SealEvent(**v)  # convert to namedtuple
-                                #SealSourceCouples: str = '-Q'  # Seal Source Couple(s), snu+dig of source sealing or sealed event.
-                                #SealSourceTriples: str = '-R'  # Seal Source Triple(s), pre+snu+dig of source sealing or sealed event.
-                                #DigestSealSingles: str = '-V'  # Digest Seal Single(s), dig of sealed data.
-                                #MerkleRootSealSingles: str = '-W'  # Merkle Tree Root Digest Seal Single(s), dig of sealed data.
-                                #BackerRegistrarSealCouples: str = '-X'  # Backer Registrar Seal Couple(s), brid+dig of sealed data.
-
-                                # SealMark == tuple of seal dict field names tuple(dict)
-                                #d = dict(a=1, b=2)
-                                #tuple(d)
-                                #('a', 'b')
+                            # need support for grouping consecutive seals of same type with same counter
 
-                            #frame.extend(Anchor(seal=e).qb64b)
-                            # else:  generic seal no count type (v, Mapping):
+                            try:
+                                sealer = Sealer(crew=e)
+                                code = self.ClanCodes[sealer.name]
+                                if gcode and gcode == code:
+                                    gframe.extend(sealer.qb64b)
+                                else:
+                                    if gframe:  # not same so close off and rotate group
+                                        counter = Counter(code=gcode, count=len(gframe) // 4)
+                                        frame.extend(counter.qb64b + gframe)
+                                        gframe = bytearray()  # new group
+                                    gcode = code  # new group or keep same group
+                                    gframe.extend(sealer.qb64b)  # extend in new group
+
+                            except kering.InvalidValueError:
+                                if gframe:
+                                    counter = Counter(code=gcode, count=len(gframe) // 4)
+                                    frame.extend(counter.qb64b + gframe)
+                                    gframe = bytearray()
+                                    gcode = None
+
+                                #unknown seal type so serialize as field map
+                                #generic seal no count type (v, Mapping):
                                 #for l, e in v.items():
                                     #pass
                                 #val = bytearray(Counter(tag=AllTags.GenericMapGroup,
-                                               # count=len(frame) % 4).qb64b)
+                                               # count=len(frame) // 4).qb64b)
                                 #val.extend(mapframe)
 
+                        if gframe:  # close off last group if any
+                            counter = Counter(code=gcode, count=len(gframe) // 4)
+                            frame.extend(counter.qb64b + gframe)
+                            gframe = bytearray()
+                            gcode = None
+
                         val = bytearray(Counter(tag=AllTags.GenericListGroup,
-                                                count=len(frame) % 4).qb64b)
+                                                count=len(frame) // 4).qb64b)
                         val.extend(frame)
 
-
                     case _:  # if extra fields this is where logic would be
                         raise SerializeError(f"Unsupported protocol field label"
-                                             f"='{l}' for protocol={self.proto}"
-                                             f" version={self.vrsn}.")
-
+                                             f"='{l}' for protocol={proto}"
+                                             f" version={vrsn}.")
 
-                raw.extend(val)
+                bdy.extend(val)
 
 
-        elif self.protocol == Protocols.acdc:
+        elif proto == Protocols.acdc:
             for l, val in sad.items():  # assumes valid field order & presence
                 if not fixed:
                     pass  # prepend label
 
 
 
         else:
             raise SerializeError(f"Unsupported protocol={self.proto}.")
 
 
         # prepend count code for message
         if fixed:
 
-            val = bytearray(Counter(tag=AllTags.FixedMessageBodyGroup,
-                                    count=len(raw) % 4).qb64b)
-            val.extend(raw)
+            raw = bytearray(Counter(tag=AllTags.FixedMessageBodyGroup,
+                                    count=len(bdy) // 4).qb64b)
+            raw.extend(bdy)
         else:
             pass
 
 
         return raw
```

### Comparing `keri-1.2.0.dev0/src/keri/db/basing.py` & `keri-1.2.0.dev1/src/keri/db/basing.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from ordered_set import OrderedSet as oset
 
 from hio.base import doing
 
 import keri
 from . import dbing, koming, subing
 from .. import kering
-
+from .. import core
 from ..core import coring, eventing, parsing, serdering, indexing
 
 from .. import help
 from ..help import helping
 
 
 logger = help.ogler.getLogger()
@@ -942,21 +942,21 @@
 
         # event source local (protected) or non-local (remote not protected)
         self.esrs = koming.Komer(db=self,
                                    schema=EventSourceRecord,
                                    subkey='esrs.')
 
         # misfit escrows whose processing may change the .esrs event source record
-        self.misfits = subing.CesrIoSetSuber(db=self, subkey='mfes.', klas=coring.Diger)
+        self.misfits = subing.IoSetSuber(db=self, subkey='mfes.')
 
         # delegable events escrows. events with local delegator that need approval
         self.delegables = subing.CesrIoSetSuber(db=self, subkey='dees.', klas=coring.Diger)
 
         # events as ordered by first seen ordinals
-        self.fons = subing.CesrSuber(db=self, subkey='fons.', klas=coring.Seqner)
+        self.fons = subing.CesrSuber(db=self, subkey='fons.', klas=core.Number)
         # Kever state made of KeyStateRecord key states
         # TODO: clean
         self.states = koming.Komer(db=self,
                                    schema=KeyStateRecord,
                                    subkey='stts.')
 
         self.wits = subing.CesrIoSetSuber(db=self, subkey="wits.", klas=coring.Prefixer)
@@ -1020,23 +1020,23 @@
         # TODO: clean
         self.tops = koming.Komer(db=self,
                                  subkey='witm.',
                                  schema=TopicsRecord, )
 
         # group partial signature escrow
         self.gpse = subing.CatCesrIoSetSuber(db=self, subkey='gpse.',
-                                             klas=(coring.Seqner, coring.Saider))
+                                             klas=(core.Number, coring.Saider))
 
         # group delegate escrow
         self.gdee = subing.CatCesrIoSetSuber(db=self, subkey='gdee.',
-                                             klas=(coring.Seqner, coring.Saider))
+                                             klas=(core.Number, coring.Saider))
 
         # group partial witness escrow
         self.gpwe = subing.CatCesrIoSetSuber(db=self, subkey='gdwe.',
-                                             klas=(coring.Seqner, coring.Saider))
+                                             klas=(core.Number, coring.Saider))
 
         # completed group multisig
         # TODO: clean
         self.cgms = subing.CesrSuber(db=self, subkey='cgms.',
                                      klas=coring.Saider)
 
         # exchange message partial signature escrow
@@ -1518,15 +1518,15 @@
                 atc.extend(coup)
 
         # add first seen replay couple to attachments
         if not (dts := self.getDts(key=dgkey)):
             raise kering.MissingEntryError("Missing datetime for dig={}.".format(dig))
         atc.extend(coring.Counter(code=coring.CtrDex.FirstSeenReplayCouples,
                                   count=1).qb64b)
-        atc.extend(coring.Seqner(sn=fn).qb64b)
+        atc.extend(core.Number(num=fn, code=core.NumDex.Huge).qb64b)  # may not need to be Huge
         atc.extend(coring.Dater(dts=bytes(dts)).qb64b)
 
         # prepend pipelining counter to attachments
         if len(atc) % 4:
             raise ValueError("Invalid attachments size={}, nonintegral"
                              " quadlets.".format(len(atc)))
         pcnt = coring.Counter(code=coring.CtrDex.AttachmentGroup,
```

### Comparing `keri-1.2.0.dev0/src/keri/db/dbing.py` & `keri-1.2.0.dev1/src/keri/db/dbing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/db/escrowing.py` & `keri-1.2.0.dev1/src/keri/db/escrowing.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,47 +100,48 @@
                             cigars.append(cigar)
 
                     # do date math for stale escrow
                     if ((helping.nowUTC() - dater.datetime) >
                             datetime.timedelta(seconds=self.timeout)):
                         # escrow stale so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Stale txn state escrow "
-                                    " at pre = %s\n", pre)
+                                    " at pre = %s", pre)
 
                         raise kering.ValidationError(f"Stale txn state escrow at pre = {pre}.")
 
                     processReply(serder=serder, saider=saider, route=serder.ked["r"],
                                  cigars=cigars, tsgs=tsgs, aid=aid)
 
                 except extype as ex:
                     # still waiting on missing prior event to validate
                     if logger.isEnabledFor(logging.DEBUG):
-                        logger.exception("Kevery unescrow attempt failed: %s\n", ex.args[0])
+                        logger.exception("Kevery unescrow attempt failed: %s", ex.args[0])
                     else:
-                        logger.error("Kevery unescrow attempt failed: %s\n", ex.args[0])
+                        logger.error("Kevery unescrow attempt failed: %s", ex.args[0])
 
                 except Exception as ex:  # other error so remove from reply escrow
                     self.escrowdb.remIokey(iokeys=(typ, pre, aid, ion))  # remove escrow
                     if logger.isEnabledFor(logging.DEBUG):
-                        logger.exception("Kevery unescrowed due to error: %s\n", ex.args[0])
+                        logger.exception("Kevery unescrowed due to error: %s", ex.args[0])
                     else:
-                        logger.error("Kevery unescrowed due to error: %s\n", ex.args[0])
+                        logger.error("Kevery unescrowed due to error: %s", ex.args[0])
 
                 else:  # unescrow succeded
                     self.escrowdb.remIokey(iokeys=(typ, pre, aid, ion))  # remove escrow only
-                    logger.info("Kevery unescrow succeeded for txn state=\n%s\n",
-                                serder.pretty())
+                    logger.info("Kevery unescrow succeeded for txn state=%s",
+                                serder.said)
+                    logger.debug(f"event=\n{serder.pretty()}\n")
 
             except Exception as ex:  # log diagnostics errors etc
                 self.escrowdb.remIokey(iokeys=(typ, pre, aid, ion))  # remove escrow
                 self.removeState(saider)
                 if logger.isEnabledFor(logging.DEBUG):
-                    logger.exception("Kevery unescrowed due to error: %s\n", ex.args[0])
+                    logger.exception("Kevery unescrowed due to error: %s", ex.args[0])
                 else:
-                    logger.error("Kevery unescrowed due to error: %s\n", ex.args[0])
+                    logger.error("Kevery unescrowed due to error: %s", ex.args[0])
 
     def escrowStateNotice(self, *, typ, pre, aid, serder, saider, dater, cigars=None, tsgs=None):
         """
         Escrow reply by route
 
         Parameters:
             typ (str): escrow type
```

### Comparing `keri-1.2.0.dev0/src/keri/db/koming.py` & `keri-1.2.0.dev1/src/keri/db/koming.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/db/migrations/rekey_habs.py` & `keri-1.2.0.dev1/src/keri/db/migrations/rekey_habs.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/db/subing.py` & `keri-1.2.0.dev1/src/keri/db/subing.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
 """
 from typing import Type, Union
 from collections.abc import Iterable, Iterator
 
 from .. import help
 from ..help.helping import nonStringIterable
+from .. import core
 from ..core import coring, scheming, serdering
 from . import dbing
 
 logger = help.ogler.getLogger()
 
 
 class SuberBase():
@@ -312,15 +313,15 @@
         """
         Deserialize val to str
         Parameters:
             val (Union[str, memoryview, bytes]): convertable to coring.matter
         """
         if isinstance(val, memoryview):  # memoryview is always bytes
             val = bytes(val)  # convert to bytes
-        return self.klas(qb64b=val)  # converts to bytes
+        return self.klas(qb64b=val)
 
 
 class CesrSuber(CesrSuberBase, Suber):
     """
     Sub class of Suber where data is CESR encode/decode ducktyped subclass
     instance such as Matter, Indexer, Counter with .qb64b property when provided
     as fully qualified serialization.
@@ -851,24 +852,24 @@
     Automatically serializes and deserializes from qb64b to/from Signer instances
 
     Assumes that last or only element of db key from keys for all entries is the qb64
     of a public key for the associated Verfer instance. This allows returned
     Signer instance to have its .transferable property set correctly.
     """
 
-    def __init__(self, *pa, klas: Type[coring.Signer] = coring.Signer, **kwa):
+    def __init__(self, *pa, klas: Type[core.Signer] = core.Signer, **kwa):
         """
         Parameters:
             db (dbing.LMDBer): base db
             subkey (str):  LMDB sub database key
             klas (Type[coring.Matter]): Class reference to subclass of Matter
         """
-        if not (issubclass(klas, coring.Signer)):
+        if not (issubclass(klas, core.Signer)):
             raise ValueError("Invalid klas type={}, expected {}."
-                             "".format(klas, coring.Signer))
+                             "".format(klas, core.Signer))
         super(SignerSuber, self).__init__(*pa, **kwa)
         self.klas = klas
 
 
     def get(self, keys: Union[str, Iterable]):
         """
         Gets Signer instance at keys
@@ -929,72 +930,72 @@
 
     Assumes that last or only element of db key from keys for all entries is the qb64
     of a public key for the associated Verfer instance. This allows returned
     Signer instance to have its .transferable property set correctly.
     """
 
     def put(self, keys: Union[str, Iterable], val: coring.Matter,
-            encrypter: coring.Encrypter = None):
+            encrypter: core.Encrypter = None):
         """
         Puts qb64 of Matter instance val at key made from keys. Does not overwrite
         If encrypter provided then encrypts first
 
         Parameters:
             keys (tuple): of key strs to be combined in order to form key
             val (Signer): instance of self.klas
-            encrypter (coring.Encrypter): optional
+            encrypter (core.Encrypter): optional
 
         Returns:
             result (bool): True If successful, False otherwise, such as key
                               already in database.
         """
         if encrypter:
             val = encrypter.encrypt(matter=val)  # returns Cipher instance
         return (self.db.putVal(db=self.sdb,
                                key=self._tokey(keys),
                                val=val.qb64b))
 
 
     def pin(self, keys: Union[str, Iterable], val: coring.Matter,
-            encrypter: coring.Encrypter = None):
+            encrypter: core.Encrypter = None):
         """
         Pins (sets) qb64 of Matter instance val at key made from keys. Overwrites.
         If encrypter provided then encrypts first
 
         Parameters:
             keys (tuple): of key strs to be combined in order to form key
             val (Signer): instance of self.klas
-            encrypter (coring.Encrypter): optional
+            encrypter (core.Encrypter): optional
 
         Returns:
             result (bool): True If successful. False otherwise.
         """
         if encrypter:
             val = encrypter.encrypt(matter=val)  # returns Cipher instance
         return (self.db.setVal(db=self.sdb,
                                key=self._tokey(keys),
                                val=val.qb64b))
 
 
 
-    def get(self, keys: Union[str, Iterable], decrypter: coring.Decrypter = None):
+    def get(self, keys: Union[str, Iterable], decrypter: core.Decrypter = None):
         """
         Gets Signer instance at keys. If decrypter then assumes value in db was
         encrypted and so decrypts value in db before converting to Signer.
 
 
         Returns:
             val (Signer):  transferable determined by key which is verfer
             None if no entry at keys
 
         Parameters:
             keys (Union[str, iterable]): key strs to be combined in order to
                 form key. Last element of keys is verkey used to determin
                 .transferable for Signer
-            decrypter (coring.Decrypter): optional. If provided assumes value in
+            decrypter (core.Decrypter): optional. If provided assumes value in
                 db was encrypted and so decrypts before converting to Signer.
 
         Usage:
             Use walrus operator to catch and raise missing entry
             if (signer := mydb.get(keys)) is None:
                 raise ExceptionHere
             use signer here
@@ -1010,23 +1011,23 @@
             return (decrypter.decrypt(ser=bytes(val),
                                       transferable=verfer.transferable))
         return (self.klas(qb64b=bytes(val), transferable=verfer.transferable))
 
 
 
     def getItemIter(self, keys: Union[str, Iterable]=b"",
-                       decrypter: coring.Decrypter = None):
+                       decrypter: core.Decrypter = None):
         """
         Returns:
             iterator (Iterator): of tuples (key, val) over the all the items in
             subdb whose key startswith key made from keys. Keys may be keyspace
             prefix to return branches of key space. When keys is empty then
             returns all items in subdb
 
-        decrypter (coring.Decrypter): optional. If provided assumes value in
+        decrypter (core.Decrypter): optional. If provided assumes value in
                 db was encrypted and so decrypts before converting to Signer.
 
         Parameters:
             keys (Iterator): tuple of bytes or strs that may be a truncation of
                 a full keys tuple in  in order to get all the items from
                 multiple branches of the key space. If keys is empty then gets
                 all items in database.
```

### Comparing `keri-1.2.0.dev0/src/keri/demo/demo_bob.py` & `keri-1.2.0.dev1/src/keri/demo/demo_eve.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,65 +6,69 @@
 Utilities for demos
 """
 import os
 import argparse
 import logging
 
 from keri import __version__
+from keri import help  # logger support
+
+from keri import core
+
 from keri.app import directing
 from keri.demo import demoing
-from keri.core import coring
-from keri import help
 
 
-def runDemo(name="bob", remote=5621, local=5620, expire=0.0):
+
+def runDemo(name="eve", remote=5620, local=5621, expire=0.0):
     """
-    Setup and run one demo controller for Bob
+    Setup and run one demo controller for Eve
     """
+
     raw = b"raw salt to test"
 
     #  create secrecies
     secrecies = [[signer.qb64] for signer in
-                 coring.Salter(raw=raw).signers(count=8,
+                 core.Salter(raw=raw).signers(count=8,
                                                 path=name,
                                                 temp=True)]
 
     doers = demoing.setupDemoController(secrecies=secrecies,
                                         name=name,
                                         remotePort=remote,
                                         localPort=local)
 
     directing.runController(doers=doers, expire=expire)
 
 
 
 def parseArgs(version=__version__):
     d = "Runs KERI direct mode demo controller.\n"
-    d += "Example:\nkeri_bob -r 5621 -l 5620 --e 10.0'\n"
+    d += "Example:\nkeri_eve -r 5620 -l 5621 --e 10.0\n"
     p = argparse.ArgumentParser(description=d)
     p.add_argument('-V', '--version',
                    action='version',
                    version=version,
                    help="Prints out version of script runner.")
     p.add_argument('-r', '--remote',
                    action='store',
-                   default=5621,
+                   default=5620,
                    help="Remote port number the client connects to. Default is 5621.")
     p.add_argument('-l', '--local',
                    action='store',
-                   default=5620,
+                   default=5621,
                    help="Local port number the server listens on. Default is 5620.")
     p.add_argument('-e', '--expire',
                    action='store',
                    default=0.0,
                    help="Expire time for demo. 0.0 means not expire. Default is 0.0.")
     p.add_argument('-n', '--name',
                    action='store',
-                   default="bob",
-                   help="Name of controller. Default is bob. Choices are bob, sam, or eve.")
+                   default="eve",
+                   help="Name of controller. Default is eve. Choices are bob, sam, or eve.")
 
 
     args = p.parse_args()
 
     return args
```

### Comparing `keri-1.2.0.dev0/src/keri/demo/demo_eve.py` & `keri-1.2.0.dev1/src/keri/demo/demo_bob.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,65 +6,70 @@
 Utilities for demos
 """
 import os
 import argparse
 import logging
 
 from keri import __version__
+
+from keri import help
+
+from keri import core
+
 from keri.app import directing
 from keri.demo import demoing
-from keri.core import coring
-from keri import help  # logger support
 
-def runDemo(name="eve", remote=5620, local=5621, expire=0.0):
+
+
+
+def runDemo(name="bob", remote=5621, local=5620, expire=0.0):
     """
-    Setup and run one demo controller for Eve
+    Setup and run one demo controller for Bob
     """
-
     raw = b"raw salt to test"
 
     #  create secrecies
     secrecies = [[signer.qb64] for signer in
-                 coring.Salter(raw=raw).signers(count=8,
+                 core.Salter(raw=raw).signers(count=8,
                                                 path=name,
                                                 temp=True)]
 
     doers = demoing.setupDemoController(secrecies=secrecies,
                                         name=name,
                                         remotePort=remote,
                                         localPort=local)
 
     directing.runController(doers=doers, expire=expire)
 
 
 
 def parseArgs(version=__version__):
     d = "Runs KERI direct mode demo controller.\n"
-    d += "Example:\nkeri_eve -r 5620 -l 5621 --e 10.0\n"
+    d += "Example:\nkeri_bob -r 5621 -l 5620 --e 10.0'\n"
     p = argparse.ArgumentParser(description=d)
     p.add_argument('-V', '--version',
                    action='version',
                    version=version,
                    help="Prints out version of script runner.")
     p.add_argument('-r', '--remote',
                    action='store',
-                   default=5620,
+                   default=5621,
                    help="Remote port number the client connects to. Default is 5621.")
     p.add_argument('-l', '--local',
                    action='store',
-                   default=5621,
+                   default=5620,
                    help="Local port number the server listens on. Default is 5620.")
     p.add_argument('-e', '--expire',
                    action='store',
                    default=0.0,
                    help="Expire time for demo. 0.0 means not expire. Default is 0.0.")
     p.add_argument('-n', '--name',
                    action='store',
-                   default="eve",
-                   help="Name of controller. Default is eve. Choices are bob, sam, or eve.")
+                   default="bob",
+                   help="Name of controller. Default is bob. Choices are bob, sam, or eve.")
 
 
     args = p.parse_args()
 
     return args
```

### Comparing `keri-1.2.0.dev0/src/keri/demo/demo_kev.py` & `keri-1.2.0.dev1/src/keri/demo/demo_kev.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/demo/demo_sam.py` & `keri-1.2.0.dev1/src/keri/demo/demo_sam.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,29 +7,33 @@
 """
 import os
 import argparse
 import logging
 
 
 from keri import __version__
+from keri import help  # logger support
+
+from keri import core
+
 from keri.app import directing
 from keri.demo import demoing
-from keri.core import coring
-from keri import help  # logger support
+
+
 
 def runDemo(name="sam", remote=5621, local=5620, expire=0.0):
     """
     Setup and run one demo controller for sam, like bob only better
     """
 
     raw = b"raw salt to test"
 
     #  create secrecies
     secrecies = [[signer.qb64] for signer in
-                 coring.Salter(raw=raw).signers(count=8,
+                 core.Salter(raw=raw).signers(count=8,
                                                 path=name,
                                                 temp=True)]
 
 
     doers = demoing.setupDemoController(secrecies=secrecies,
                                         name=name,
                                         remotePort=remote,
```

### Comparing `keri-1.2.0.dev0/src/keri/demo/demoing.py` & `keri-1.2.0.dev1/src/keri/demo/demoing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/end/ending.py` & `keri-1.2.0.dev1/src/keri/end/ending.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/end/priming.py` & `keri-1.2.0.dev1/src/keri/end/priming.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/help/__init__.py` & `keri-1.2.0.dev1/src/keri/help/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 #  if need be
 
 from hio.help import ogling
 
 #  want help.ogler always defined by default
 ogler = ogling.initOgler(prefix='keri', syslogged=False)  # inits once only on first import
 
-from .helping import nowIso8601, toIso8601, fromIso8601
+from .helping import (nowIso8601, toIso8601, fromIso8601,
+                      nonStringSequence, nonStringIterable)
```

### Comparing `keri-1.2.0.dev0/src/keri/help/helping.py` & `keri-1.2.0.dev1/src/keri/help/helping.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,15 +350,15 @@
     """
     Return first l sextets from front (left) of b as bytes (byte string).
     Length of bytes returned is minimum sufficient to hold all l sextets.
     Last byte returned is right bit padded with zeros
     b is bytes or str
     """
     if hasattr(b, 'encode'):
-        b = b.encode("utf-8")  # convert to bytes
+        b = b.encode()  # convert to bytes
     n = sceil(l * 3 / 4)  # number of bytes needed for l sextets
     if n > len(b):
         raise ValueError("Not enough bytes in {} to nab {} sextets.".format(b, l))
     i = int.from_bytes(b[:n], 'big')
     p = 2 * (l % 4)
     i >>= p  # strip of last bits
     i <<= p  # pad with empty bits
```

### Comparing `keri-1.2.0.dev0/src/keri/kering.py` & `keri-1.2.0.dev1/src/keri/kering.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/peer/exchanging.py` & `keri-1.2.0.dev1/src/keri/peer/exchanging.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,29 +117,32 @@
             if pather.startswith(e):
                 np = pather.strip(e)
                 attachments.append((np, pattach))
 
         # Perform behavior specific verification, think IPEX chaining requirements
         try:
             if not behavior.verify(serder=serder, attachments=attachments):
-                logger.info(f"exn event for route {route} failed behavior verfication.  exn={serder.ked}")
+                logger.info(f"exn event for route {route} failed behavior verfication.  said={serder.said}")
+                logger.debug(f"event=\n{serder.pretty()}\n")
                 return
 
         except AttributeError:
-            logger.info(f"Behavior for {route} missing or does not have verify for exn={serder.ked}")
+            logger.info(f"Behavior for {route} missing or does not have verify for said={serder.said}")
+            logger.debug(f"event=\n{serder.pretty()}\n")
 
         # Always persis events
         self.logEvent(serder, pathed, tsgs, cigars)
         self.cues.append(dict(kin="saved", said=serder.said))
 
         # Execute any behavior specific handling, not sure if this should be different than verify
         try:
             behavior.handle(serder=serder, attachments=attachments)
         except AttributeError:
-            logger.info(f"Behavior for {route} missing or does not have handle for exn={serder.ked}")
+            logger.info(f"Behavior for {route} missing or does not have handle for said={serder.said}")
+            logger.debug(f"event=\n{serder.pretty()}\n")
 
     def processEscrow(self):
         """ Process all escrows for `exn` messages
 
         """
         self.processEscrowPartialSigned()
 
@@ -186,29 +189,30 @@
             pathed = [bytearray(p.encode("utf-8")) for p in self.hby.db.epath.get(keys=(dig,))]
 
             try:
                 self.processEvent(serder=serder, tsgs=tsgs, pathed=pathed)
 
             except MissingSignatureError as ex:
                 if logger.isEnabledFor(logging.DEBUG):
-                    logger.info("Exchange partially signed unescrow failed: %s\n", ex.args[0])
+                    logger.info("Exchange partially signed unescrow failed: %s", ex.args[0])
                 else:
-                    logger.info("Exchange partially signed failed: %s\n", ex.args[0])
+                    logger.info("Exchange partially signed failed: %s", ex.args[0])
             except Exception as ex:
                 self.hby.db.epse.rem(dig)
                 self.hby.db.esigs.rem(dig)
                 if logger.isEnabledFor(logging.DEBUG):
-                    logger.info("Exchange partially signed unescrowed: %s\n", ex.args[0])
+                    logger.info("Exchange partially signed unescrowed: %s", ex.args[0])
                 else:
-                    logger.info("Exchange partially signed unescrowed: %s\n", ex.args[0])
+                    logger.info("Exchange partially signed unescrowed: %s", ex.args[0])
             else:
                 self.hby.db.epse.rem(dig)
                 self.hby.db.esigs.rem(dig)
                 logger.info("Exchanger unescrow succeeded in valid exchange: "
-                            "creder=\n%s\n", serder.pretty())
+                            "creder=%s", serder.said)
+                logger.debug(f"event=\n{serder.pretty()}\n")
 
     def logEvent(self, serder, pathed=None, tsgs=None, cigars=None):
         dig = serder.said
         pdig = serder.ked['p']
         pathed = pathed or []
         tsgs = tsgs or []
         cigars = cigars or []
```

### Comparing `keri-1.2.0.dev0/src/keri/vc/protocoling.py` & `keri-1.2.0.dev1/src/keri/vc/protocoling.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/vc/proving.py` & `keri-1.2.0.dev1/src/keri/vc/proving.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 """
 
 from collections.abc import Iterable
 from typing import Union
 
 from .. import help
+
+from .. import core
 from ..core import coring, serdering
 from ..core.coring import (Serials, versify)
 from ..db import subing
 from ..kering import Version
 from ..help import helping
 
 KERI_REGISTRY_TYPE = "KERICredentialRegistry"
@@ -58,16 +60,16 @@
     )
 
     subject = dict(
         d="",
     )
 
     if private:
-        vc["u"] = salt if salt is not None else coring.Salter().qb64
-        subject["u"] = salt if salt is not None else coring.Salter().qb64
+        vc["u"] = salt if salt is not None else core.Salter().qb64
+        subject["u"] = salt if salt is not None else core.Salter().qb64
 
     if recipient is not None:
         subject['i'] = recipient
 
     subject["dt"] = data["dt"] if "dt" in data else helping.nowIso8601()
 
     subject |= data
```

### Comparing `keri-1.2.0.dev0/src/keri/vc/walleting.py` & `keri-1.2.0.dev1/src/keri/vc/walleting.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri/vdr/credentialing.py` & `keri-1.2.0.dev1/src/keri/vdr/credentialing.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,16 @@
             serder (Serder): Registry TEL event to process
 
         """
 
         try:
             self.tvy.processEvent(serder=serder)
         except kering.MissingAnchorError:
-            logger.info("Credential registry missing anchor for inception = {}".format(serder.ked))
+            logger.info("Credential registry missing anchor for inception = {}".format(serder.said))
+            logger.debug(f"event=\n{serder.pretty()}\n")
 
     def anchorMsg(self, pre, regd, seqner, saider):
         """  Create key event with seal to serder anchored as data.
 
         Performs a rotation or interaction event for single sig or multiple sig identifier
         to anchor the provide registry event.  Inserts outbound cues for external processing
         of resulting events or multisig handling.
```

### Comparing `keri-1.2.0.dev0/src/keri/vdr/eventing.py` & `keri-1.2.0.dev1/src/keri/vdr/eventing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1261,16 +1261,17 @@
             self.reger.putTibs(key, [biger.qb64b for biger in bigers])
         if baks:
             self.reger.delBaks(key)
             self.reger.putBaks(key, [bak.encode("utf-8") for bak in baks])
         self.reger.tets.pin(keys=(pre.decode("utf-8"), dig.decode("utf-8")), val=coring.Dater())
         self.reger.putTvt(key, serder.raw)
         self.reger.putTel(snKey(pre, sn), dig)
-        logger.info("Tever state: %s Added to TEL valid event=\n%s\n",
-                    pre, json.dumps(serder.ked, indent=1))
+        logger.info("Tever state: %s Added to TEL valid said=%s",
+                    pre, serder.said)
+        logger.debug(f"event=\n{serder.pretty()}\n")
 
     def valAnchorBigs(self, serder, seqner, saider, bigers, toad, baks):
         """ Validate anchor and backer signatures (bigers) when provided.
 
         Validates sigers signatures by validating indexes, verifying signatures, and
             validating threshold sith.
         Validate backer receipts by validating indexes, verifying
@@ -1390,16 +1391,16 @@
         """
         dgkey = dgKey(serder.preb, serder.saidb)
         sealet = seqner.qb64b + saider.qb64b
         self.reger.putAnc(dgkey, sealet)
         self.reger.putTibs(dgkey, [biger.qb64b for biger in bigers])
         self.reger.putTvt(dgkey, serder.raw)
         self.reger.putTwe(snKey(serder.preb, serder.sn), serder.saidb)
-        logger.info("Tever state: Escrowed partially witnessed "
-                    "event = %s\n", serder.ked)
+        logger.debug("Tever state: Escrowed partially witnessed "
+                     "event = %s", serder.ked)
 
     def escrowALEvent(self, serder, seqner, saider, bigers=None, baks=None):
         """ Update associated logs for escrow of anchorless event
 
         Parameters:
             serder (Serder): instance of  event
             seqner (Seqner): sequence number for anchor seal
@@ -1417,16 +1418,16 @@
             self.reger.putAnc(key, sealet)
         if bigers:
             self.reger.putTibs(key, [biger.qb64b for biger in bigers])
         if baks:
             self.reger.delBaks(key)
             self.reger.putBaks(key, [bak.encode("utf-8") for bak in baks])
         self.reger.putTvt(key, serder.raw)
-        logger.info("Tever state: Escrowed anchorless event "
-                    "event = %s\n", serder.ked)
+        logger.debug("Tever state: Escrowed anchorless event "
+                     "event = %s", serder.ked)
         return self.reger.putTae(snKey(serder.preb, serder.sn), serder.saidb)
 
     def getBackerState(self, ked):
         """ Calculate and return the current list of backers for event dict
 
         Parameters:
             ked (dict):  event dict
@@ -2001,16 +2002,16 @@
 
         """
         key = dgKey(serder.preb, serder.saidb)
         self.reger.putTvt(key, serder.raw)
         sealet = seqner.qb64b + saider.qb64b
         self.reger.putAnc(key, sealet)
         self.reger.putOot(snKey(serder.preb, serder.sn), serder.saidb)
-        logger.info("Tever state: Escrowed our of order TEL event "
-                    "event = %s\n", serder.ked)
+        logger.debug("Tever state: Escrowed our of order TEL event "
+                     "event = %s", serder.ked)
 
     def processEscrows(self):
         """ Loop through escrows and process and events that may now be finalized """
 
         try:
             self.processEscrowAnchorless()
             self.processEscrowOutOfOrders()
@@ -2023,17 +2024,17 @@
             self.reger.txnsb.processEscrowState(typ="registry-mae", processReply=self.processReplyRegistryTxnState,
                                                 extype=kering.MissingAnchorError)
             self.reger.txnsb.processEscrowState(typ="registry-ooo", processReply=self.processReplyRegistryTxnState,
                                                 extype=kering.OutOfOrderTxnStateError)
 
         except Exception as ex:  # log diagnostics errors etc
             if logger.isEnabledFor(logging.DEBUG):
-                logger.exception("Tevery escrow process error: %s\n", ex.args[0])
+                logger.exception("Tevery escrow process error: %s", ex.args[0])
             else:
-                logger.error("Tevery escrow process error: %s\n", ex.args[0])
+                logger.error("Tevery escrow process error: %s", ex.args[0])
 
     def processEscrowOutOfOrders(self):
         """ Loop through out of order escrow:
 
          Process out of order events in the following way:
            1. loop over event digests saved in oots
            2. deserialize event out of tvts
@@ -2046,60 +2047,61 @@
             try:
                 sn = int(snb, 16)
                 dgkey = dgKey(pre, digb)
                 traw = self.reger.getTvt(dgkey)
                 if traw is None:
                     # no event so raise ValidationError which unescrows below
                     logger.info("Tevery unescrow error: Missing event at."
-                                "dig = %s\n", bytes(digb))
+                                "dig = %s", bytes(digb))
 
                     raise ValidationError("Missing escrowed evt at dig = {}."
                                           "".format(bytes(digb)))
 
                 tserder = serdering.SerderKERI(raw=bytes(traw))  # escrowed event
 
                 bigers = None
                 if tibs := self.reger.getTibs(key=dgkey):
                     bigers = [indexing.Siger(qb64b=tib) for tib in tibs]
 
                 couple = self.reger.getAnc(dgkey)
                 if couple is None:
                     logger.info("Tevery unescrow error: Missing anchor at."
-                                "dig = %s\n", bytes(digb))
+                                "dig = %s", bytes(digb))
 
                     raise ValidationError("Missing escrowed anchor at dig = {}."
                                           "".format(bytes(digb)))
                 ancb = bytearray(couple)
                 seqner = coring.Seqner(qb64b=ancb, strip=True)
                 saider = coring.Saider(qb64b=ancb, strip=True)
 
                 self.processEvent(serder=tserder, seqner=seqner, saider=saider, wigers=bigers)
 
             except OutOfOrderError as ex:
                 # still waiting on missing prior event to validate
                 if logger.isEnabledFor(logging.DEBUG):
-                    logger.exception("Tevery unescrow failed: %s\n", ex.args[0])
+                    logger.exception("Tevery unescrow failed: %s", ex.args[0])
                 else:
-                    logger.error("Tevery unescrow failed: %s\n", ex.args[0])
+                    logger.error("Tevery unescrow failed: %s", ex.args[0])
 
             except Exception as ex:  # log diagnostics errors etc
                 # error other than out of order so remove from OO escrow
                 self.reger.delOot(snKey(pre, sn))  # removes one escrow at key val
                 if logger.isEnabledFor(logging.DEBUG):
-                    logger.exception("Tevery unescrowed: %s\n", ex.args[0])
+                    logger.exception("Tevery unescrowed: %s", ex.args[0])
                 else:
-                    logger.error("Tevery unescrowed: %s\n", ex.args[0])
+                    logger.error("Tevery unescrowed: %s", ex.args[0])
 
             else:  # unescrow succeeded, remove from escrow
                 # We don't remove all escrows at pre,sn because some might be
                 # duplicitous so we process remaining escrows in spite of found
                 # valid event escrow.
                 self.reger.delOot(snKey(pre, sn))  # removes from escrow
                 logger.info("Tevery unescrow succeeded in valid event: "
-                            "event=\n%s\n", json.dumps(tserder.ked, indent=1))
+                            "said=%s", tserder.said)
+                logger.debug(f"event=\n{tserder.pretty()}\n")
 
     def processEscrowAnchorless(self):
         """ Process escrow of TEL events received before the anchoring KEL event.
 
         Process anchorless events in the following way:
            1. loop over event digests saved in taes
            2. deserialize event out of tvts
@@ -2113,53 +2115,54 @@
             sn = int(snb, 16)
             try:
                 dgkey = dgKey(pre, digb)
                 traw = self.reger.getTvt(dgkey)
                 if traw is None:
                     # no event so raise ValidationError which unescrows below
                     logger.info("Tevery unescrow error: Missing event at."
-                                "dig = %s\n", bytes(digb))
+                                "dig = %s", bytes(digb))
 
                     raise ValidationError("Missing escrowed evt at dig = {}."
                                           "".format(bytes(digb)))
 
                 tserder = serdering.SerderKERI(raw=bytes(traw))  # escrowed event
 
                 bigers = None
                 if tibs := self.reger.getTibs(key=dgkey):
                     bigers = [indexing.Siger(qb64b=tib) for tib in tibs]
 
                 couple = self.reger.getAnc(dgkey)
                 if couple is None:
                     logger.info("Tevery unescrow error: Missing anchor at."
-                                "dig = %s\n", bytes(digb))
+                                "dig = %s", bytes(digb))
 
                     raise MissingAnchorError("Missing escrowed anchor at dig = {}."
                                              "".format(bytes(digb)))
                 ancb = bytearray(couple)
                 seqner = coring.Seqner(qb64b=ancb, strip=True)
                 saider = coring.Saider(qb64b=ancb, strip=True)
 
                 self.processEvent(serder=tserder, seqner=seqner, saider=saider, wigers=bigers)
 
             except MissingAnchorError as ex:
                 # still waiting on missing prior event to validate
                 if logger.isEnabledFor(logging.DEBUG):
-                    logger.exception("Tevery unescrow failed: %s\n", ex.args[0])
+                    logger.exception("Tevery unescrow failed: %s", ex.args[0])
                 else:
-                    logger.error("Tevery unescrow failed: %s\n", ex.args[0])
+                    logger.error("Tevery unescrow failed: %s", ex.args[0])
 
             except Exception as ex:  # log diagnostics errors etc
                 # error other than out of order so remove from OO escrow
                 self.reger.delTae(snKey(pre, sn))  # removes one escrow at key val
                 if logger.isEnabledFor(logging.DEBUG):
-                    logger.exception("Tevery unescrowed: %s\n", ex.args[0])
+                    logger.exception("Tevery unescrowed: %s", ex.args[0])
                 else:
-                    logger.error("Tevery unescrowed: %s\n", ex.args[0])
+                    logger.error("Tevery unescrowed: %s", ex.args[0])
 
             else:  # unescrow succeeded, remove from escrow
                 # We don't remove all escrows at pre,sn because some might be
                 # duplicitous so we process remaining escrows in spite of found
                 # valid event escrow.
                 self.reger.delTae(snKey(pre, sn))  # removes from escrow
                 logger.info("Tevery unescrow succeeded in valid event: "
-                            "event=\n%s\n", json.dumps(tserder.ked, indent=1))
+                            "said=%s", tserder.said)
+                logger.debug(f"event=\n{tserder.pretty()}\n")
```

### Comparing `keri-1.2.0.dev0/src/keri/vdr/verifying.py` & `keri-1.2.0.dev1/src/keri/vdr/verifying.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,37 +251,38 @@
             try:
 
                 dtnow = helping.nowUTC()
                 dte = helping.fromIso8601(dater.dts)
                 if (dtnow - dte) > datetime.timedelta(seconds=timeout):
                     # escrow stale so raise ValidationError which unescrows below
                     logger.info("Verifier unescrow error: Stale event escrow "
-                                " at said = %s\n", said)
+                                " at said = %s", said)
 
                     raise kering.ValidationError("Stale event escrow "
                                                  "at said = {}.".format(said))
 
                 self.processCredential(creder, prefixer, seqner, saider)
 
             except etype as ex:
                 if logger.isEnabledFor(logging.DEBUG):
-                    logger.exception("Verifiery unescrow failed: %s\n", ex.args[0])
+                    logger.exception("Verifiery unescrow failed: %s", ex.args[0])
                 else:
-                    logger.error("Verifier unescrow failed: %s\n", ex.args[0])
+                    logger.error("Verifier unescrow failed: %s", ex.args[0])
             except Exception as ex:  # log diagnostics errors etc
                 # error other than missing sigs so remove from PA escrow
                 db.rem(said)
                 if logger.isEnabledFor(logging.DEBUG):
-                    logger.exception("Verifier unescrowed: %s\n", ex.args[0])
+                    logger.exception("Verifier unescrowed: %s", ex.args[0])
                 else:
-                    logger.error("Verifier unescrowed: %s\n", ex.args[0])
+                    logger.error("Verifier unescrowed: %s", ex.args[0])
             else:
                 db.rem(said)
                 logger.info("Verifier unescrow succeeded in valid group op: "
-                            "creder=\n%s\n", creder.pretty())
+                            "creder=%s", creder.said)
+                logger.debug(f"event=\n{creder.pretty()}\n")
 
     def saveCredential(self, creder, prefixer, seqner, saider):
         """ Write the credential and associated indicies to the database
 
         Parameters:
             creder (Creder): that contains the credential to process
             prefixer (Prefixer): prefix (AID or TEL) of event anchoring credential
```

### Comparing `keri-1.2.0.dev0/src/keri/vdr/viring.py` & `keri-1.2.0.dev1/src/keri/vdr/viring.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev0/src/keri.egg-info/PKG-INFO` & `keri-1.2.0.dev1/src/keri.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keri
-Version: 1.2.0.dev0
+Version: 1.2.0.dev1
 Summary: Key Event Receipt Infrastructure
 Home-page: https://github.com/WebOfTrust/keripy
 Author: Samuel M. Smith
 Author-email: smith.samuel.m@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://keri.readthedocs.io/
 Project-URL: Changelog, https://keri.readthedocs.io/en/latest/changelog.html
@@ -35,9 +35,10 @@
 Requires-Dist: PyYaml>=6.0.1
 Requires-Dist: apispec>=6.6.0
 Requires-Dist: mnemonic>=0.21
 Requires-Dist: PrettyTable>=3.10.0
 Requires-Dist: http_sfv>=0.9.9
 Requires-Dist: cryptography>=42.0.5
 Requires-Dist: semver>=3.0.2
+Requires-Dist: qrcode>=7.4.2
 
 KERI Decentralized Key Management Infrastructure
```

### Comparing `keri-1.2.0.dev0/src/keri.egg-info/SOURCES.txt` & `keri-1.2.0.dev1/src/keri.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,26 +20,26 @@
 src/keri/app/directing.py
 src/keri/app/forwarding.py
 src/keri/app/grouping.py
 src/keri/app/habbing.py
 src/keri/app/httping.py
 src/keri/app/indirecting.py
 src/keri/app/keeping.py
-src/keri/app/kiwiing.py
 src/keri/app/notifying.py
 src/keri/app/oobiing.py
 src/keri/app/querying.py
 src/keri/app/signaling.py
 src/keri/app/signing.py
 src/keri/app/specing.py
 src/keri/app/storing.py
 src/keri/app/cli/__init__.py
 src/keri/app/cli/kli.py
 src/keri/app/cli/commands/__init__.py
 src/keri/app/cli/commands/clean.py
+src/keri/app/cli/commands/decrypt.py
 src/keri/app/cli/commands/escrow.py
 src/keri/app/cli/commands/export.py
 src/keri/app/cli/commands/incept.py
 src/keri/app/cli/commands/init.py
 src/keri/app/cli/commands/interact.py
 src/keri/app/cli/commands/kevers.py
 src/keri/app/cli/commands/list.py
@@ -115,14 +115,15 @@
 src/keri/app/cli/commands/vc/list.py
 src/keri/app/cli/commands/vc/revoke.py
 src/keri/app/cli/commands/vc/registry/__init__.py
 src/keri/app/cli/commands/vc/registry/incept.py
 src/keri/app/cli/commands/vc/registry/list.py
 src/keri/app/cli/commands/vc/registry/status.py
 src/keri/app/cli/commands/witness/__init__.py
+src/keri/app/cli/commands/witness/authenticate.py
 src/keri/app/cli/commands/witness/demo.py
 src/keri/app/cli/commands/witness/start.py
 src/keri/app/cli/commands/witness/submit.py
 src/keri/app/cli/common/__init__.py
 src/keri/app/cli/common/config.py
 src/keri/app/cli/common/displaying.py
 src/keri/app/cli/common/existing.py
@@ -134,14 +135,16 @@
 src/keri/core/counting.py
 src/keri/core/eventing.py
 src/keri/core/indexing.py
 src/keri/core/parsing.py
 src/keri/core/routing.py
 src/keri/core/scheming.py
 src/keri/core/serdering.py
+src/keri/core/signing.py
+src/keri/core/structing.py
 src/keri/db/__init__.py
 src/keri/db/basing.py
 src/keri/db/dbing.py
 src/keri/db/escrowing.py
 src/keri/db/koming.py
 src/keri/db/subing.py
 src/keri/db/migrations/__init__.py
```

### Comparing `keri-1.2.0.dev0/tests/test_kering.py` & `keri-1.2.0.dev1/tests/test_kering.py`

 * *Files identical despite different names*


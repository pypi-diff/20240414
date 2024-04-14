# Comparing `tmp/cpop-34.0.0.tar.gz` & `tmp/cpop-34.1.0.tar.gz`

## Comparing `cpop-34.0.0.tar` & `cpop-34.1.0.tar`

### file list

```diff
@@ -1,175 +1,176 @@
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 cpop-34.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/Makefile
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/make.bat
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/outline.rst
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/source/conf.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/source/index.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/source/releases/32.rst
--rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/source/topics/app_merging.rst
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/source/topics/conf.rst
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/source/topics/conf_integrate.rst
--rw-r--r--   0        0        0     7381 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/source/topics/contracts.rst
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/source/topics/dyne_name.rst
--rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/source/topics/func_alias.rst
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/source/topics/glossary.rst
--rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/source/topics/hub_overview.rst
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/source/topics/ideas_that_were_not_used.rst
--rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/source/topics/learning.rst
--rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/source/topics/pop.rst
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/source/topics/pre_contract_returns.rst
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/source/topics/story.rst
--rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/source/topics/sub_patterns.rst
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/source/topics/subs_overview.rst
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/source/topics/virtual.rst
--rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 cpop-34.0.0/docs/source/tutorial/quickstart.rst
--rw-r--r--   0        0        0     8402 2020-02-02 00:00:00.000000 cpop-34.0.0/src/cpop/contract.pyx
--rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 cpop-34.0.0/src/cpop/data.pyx
--rw-r--r--   0        0        0     5069 2020-02-02 00:00:00.000000 cpop-34.0.0/src/cpop/dirs.pyx
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 cpop-34.0.0/src/cpop/exc.pyx
--rw-r--r--   0        0        0    25026 2020-02-02 00:00:00.000000 cpop-34.0.0/src/cpop/hub.pyx
--rw-r--r--   0        0        0     9936 2020-02-02 00:00:00.000000 cpop-34.0.0/src/cpop/loader.pyx
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 cpop-34.0.0/src/cpop/ref.pyx
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 cpop-34.0.0/src/cpop/scanner.pyx
--rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 cpop-34.0.0/src/cpop/verify.pyx
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 cpop-34.0.0/src/pop/config.yaml
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 cpop-34.0.0/src/pop/log/basic.py
--rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 cpop-34.0.0/src/pop/log/init.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 cpop-34.0.0/src/pop/log/timed_rolling.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-34.0.0/src/pop/log/contracts/init.py
--rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 cpop-34.0.0/src/pop/mods/config.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 cpop-34.0.0/src/pop/mods/contract.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-34.0.0/src/pop/mods/dyne.py
--rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 cpop-34.0.0/src/pop/mods/sub.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 cpop-34.0.0/src/pop/mods/task.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cpop-34.0.0/src/pop/mods/test.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/conftest.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/alias/init.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/cmods/ctest.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/cmods/contracts/ctest.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/contracts/ctx.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/contracts/ctx_args.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/contracts/ctx_update.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/contracts/many.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/contracts/priv.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/contracts/test.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/coro/test.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/coro/contracts/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/func/__init__.py
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/func/test_basic.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/func/test_bench.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/func/test_cli.py
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/func/test_config.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/func/test_contract_ctx.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/func/test_coro.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/func/test_cpop.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/func/test_dyne.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/func/test_fail.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/func/test_hub.py
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/func/test_log.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/func/test_no_raise_on_pre_failure.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/func/test_raise_on_pre_failure.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/func/test_ref.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/func/test_serial.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/func/test_sub.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/integration/contract_ordering/single_module/thing.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/integration/contract_ordering/single_module/contracts/default.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/integration/contract_ordering/single_module/contracts/dunder.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/integration/contract_ordering/single_module/contracts/init.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/integration/contract_ordering/single_module/contracts/thing.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/integration/contracted/test_contracted_access.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/integration/contracted/mods/contracted_access.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/integration/contracted/mods/contracts/contracted_access.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/integration/recursive_contract/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/integration/recursive_contract/test_sub.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/bad.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/falias_dict.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/falias_func.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/foo.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/fork.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/many.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/priv.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/proc.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/test.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/testing.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/vbad.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/virt.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/vtrue.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/bad_import/bad_import.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/contract_ctx/ctx.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/contract_ctx/ctx_args.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/contract_ctx/ctx_update.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/contract_sig/fail_sigs.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/contract_sig/pass_sigs.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/contract_sig/contracts/init.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/coro/coro.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/iter/bar.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/iter/foo.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/iter/init.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/nest/basic.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/same_vname/will_load.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/same_vname/will_not_load.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/subinit/init.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/mods/subinit/subinit.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/regression/contract_masking/test_contract_masking.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/regression/contract_masking/test_duplicate_contracts.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/regression/contract_masking/contract1/init.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/regression/contract_masking/contract2/init.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/regression/contract_masking/sub/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/sdirs/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/sdirs/l11/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/sdirs/l11/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/sdirs/l12/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/sdirs/l12/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/sdirs/l13/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/sdirs/l13/l2/test.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/README.rst
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/cn/config.yaml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/cn/contract/test.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/cn/contract/contracts/test.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dn1/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dn1/dn1/nest/dn1.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dn1/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dn2/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dn2/dn1/nest/dn2.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dn2/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dn3/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dn3/dn1/nest/dn3.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dn3/dn1/nest/over.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dn3/dn1/nest/next/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dn3/dn1/nest/next/last/test.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dyne1/config.yaml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dyne1/dyne1/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dyne1/dyne1/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dyne1/nest/dyne/nest.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dyne2/config.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dyne2/dyne2/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dyne2/dyne2/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dyne2/nest/dyne/nest.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dyne3/config.yaml
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dyne3/dyne3/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dyne3/dyne3/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dyne3/nest/dyne/nest.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dyne4/config.yaml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dyne4/dyne4/nest/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/dyne4/dyne4/nest/subvert.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/fork/config.yaml
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/fork/fork/rsub.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/fork/fork/nest/init.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/v1/config.yaml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/tpath/v1/v1/load.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/unit/__init__.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/unit/test_contract.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 cpop-34.0.0/tests/unit/test_sigs.py
--rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-34.0.0/.gitignore
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 cpop-34.0.0/README.rst
--rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 cpop-34.0.0/pyproject.toml
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 cpop-34.0.0/PKG-INFO
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 cpop-34.1.0/.coveragerc
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 cpop-34.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/Makefile
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/make.bat
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/outline.rst
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/source/conf.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/source/index.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/source/releases/32.rst
+-rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/source/topics/app_merging.rst
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/source/topics/conf.rst
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/source/topics/conf_integrate.rst
+-rw-r--r--   0        0        0     7381 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/source/topics/contracts.rst
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/source/topics/dyne_name.rst
+-rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/source/topics/func_alias.rst
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/source/topics/glossary.rst
+-rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/source/topics/hub_overview.rst
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/source/topics/ideas_that_were_not_used.rst
+-rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/source/topics/learning.rst
+-rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/source/topics/pop.rst
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/source/topics/pre_contract_returns.rst
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/source/topics/story.rst
+-rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/source/topics/sub_patterns.rst
+-rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/source/topics/subs_overview.rst
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/source/topics/virtual.rst
+-rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 cpop-34.1.0/docs/source/tutorial/quickstart.rst
+-rw-r--r--   0        0        0     9507 2020-02-02 00:00:00.000000 cpop-34.1.0/src/cpop/contract.pyx
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 cpop-34.1.0/src/cpop/data.pyx
+-rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 cpop-34.1.0/src/cpop/dirs.pyx
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 cpop-34.1.0/src/cpop/exc.pyx
+-rw-r--r--   0        0        0    26594 2020-02-02 00:00:00.000000 cpop-34.1.0/src/cpop/hub.pyx
+-rw-r--r--   0        0        0     9936 2020-02-02 00:00:00.000000 cpop-34.1.0/src/cpop/loader.pyx
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 cpop-34.1.0/src/cpop/ref.pyx
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-34.1.0/src/cpop/scanner.pyx
+-rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 cpop-34.1.0/src/cpop/verify.pyx
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 cpop-34.1.0/src/pop/config.yaml
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 cpop-34.1.0/src/pop/log/basic.py
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 cpop-34.1.0/src/pop/log/init.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 cpop-34.1.0/src/pop/log/timed_rolling.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-34.1.0/src/pop/log/contracts/init.py
+-rw-r--r--   0        0        0     9680 2020-02-02 00:00:00.000000 cpop-34.1.0/src/pop/mods/config.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 cpop-34.1.0/src/pop/mods/contract.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-34.1.0/src/pop/mods/dyne.py
+-rw-r--r--   0        0        0     6986 2020-02-02 00:00:00.000000 cpop-34.1.0/src/pop/mods/sub.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 cpop-34.1.0/src/pop/mods/task.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cpop-34.1.0/src/pop/mods/test.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/conftest.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/alias/init.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/cmods/ctest.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/cmods/contracts/ctest.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/contracts/ctx.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/contracts/ctx_args.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/contracts/ctx_update.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/contracts/many.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/contracts/priv.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/contracts/test.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/coro/test.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/coro/contracts/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/func/__init__.py
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/func/test_basic.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/func/test_bench.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/func/test_cli.py
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/func/test_config.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/func/test_contract_ctx.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/func/test_coro.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/func/test_cpop.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/func/test_dyne.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/func/test_fail.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/func/test_hub.py
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/func/test_log.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/func/test_no_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/func/test_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/func/test_ref.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/func/test_serial.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/func/test_sub.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/integration/contract_ordering/single_module/thing.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/integration/contract_ordering/single_module/contracts/default.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/integration/contract_ordering/single_module/contracts/dunder.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/integration/contract_ordering/single_module/contracts/init.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/integration/contract_ordering/single_module/contracts/thing.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/integration/contracted/test_contracted_access.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/integration/contracted/mods/contracted_access.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/integration/contracted/mods/contracts/contracted_access.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/integration/recursive_contract/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/integration/recursive_contract/test_sub.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/bad.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/falias_dict.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/falias_func.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/foo.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/fork.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/many.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/priv.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/proc.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/test.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/testing.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/vbad.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/virt.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/vtrue.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/bad_import/bad_import.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/contract_ctx/ctx.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/contract_ctx/ctx_args.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/contract_ctx/ctx_update.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/contract_sig/fail_sigs.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/contract_sig/pass_sigs.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/contract_sig/contracts/init.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/coro/coro.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/iter/bar.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/iter/foo.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/iter/init.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/nest/basic.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/same_vname/will_load.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/same_vname/will_not_load.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/subinit/init.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/mods/subinit/subinit.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/regression/contract_masking/test_contract_masking.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/regression/contract_masking/test_duplicate_contracts.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/regression/contract_masking/contract1/init.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/regression/contract_masking/contract2/init.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/regression/contract_masking/sub/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/sdirs/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/sdirs/l11/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/sdirs/l11/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/sdirs/l12/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/sdirs/l12/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/sdirs/l13/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/sdirs/l13/l2/test.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/README.rst
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/cn/config.yaml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/cn/contract/test.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/cn/contract/contracts/test.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dn1/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dn1/dn1/nest/dn1.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dn1/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dn2/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dn2/dn1/nest/dn2.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dn2/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dn3/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dn3/dn1/nest/dn3.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dn3/dn1/nest/over.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dn3/dn1/nest/next/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dn3/dn1/nest/next/last/test.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dyne1/config.yaml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dyne1/dyne1/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dyne1/dyne1/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dyne1/nest/dyne/nest.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dyne2/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dyne2/dyne2/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dyne2/dyne2/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dyne2/nest/dyne/nest.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dyne3/config.yaml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dyne3/dyne3/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dyne3/dyne3/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dyne3/nest/dyne/nest.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dyne4/config.yaml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dyne4/dyne4/nest/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/dyne4/dyne4/nest/subvert.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/fork/config.yaml
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/fork/fork/rsub.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/fork/fork/nest/init.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/v1/config.yaml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/tpath/v1/v1/load.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/unit/test_contract.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 cpop-34.1.0/tests/unit/test_sigs.py
+-rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-34.1.0/.gitignore
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 cpop-34.1.0/README.rst
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 cpop-34.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 cpop-34.1.0/PKG-INFO
```

### Comparing `cpop-34.0.0/.pre-commit-config.yaml` & `cpop-34.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/docs/Makefile` & `cpop-34.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/docs/make.bat` & `cpop-34.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/docs/outline.rst` & `cpop-34.1.0/docs/outline.rst`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/docs/source/conf.py` & `cpop-34.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/docs/source/index.rst` & `cpop-34.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/docs/source/topics/app_merging.rst` & `cpop-34.1.0/docs/source/topics/app_merging.rst`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/docs/source/topics/conf.rst` & `cpop-34.1.0/docs/source/topics/conf.rst`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/docs/source/topics/conf_integrate.rst` & `cpop-34.1.0/docs/source/topics/conf_integrate.rst`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/docs/source/topics/contracts.rst` & `cpop-34.1.0/docs/source/topics/contracts.rst`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/docs/source/topics/dyne_name.rst` & `cpop-34.1.0/docs/source/topics/dyne_name.rst`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/docs/source/topics/func_alias.rst` & `cpop-34.1.0/docs/source/topics/func_alias.rst`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/docs/source/topics/glossary.rst` & `cpop-34.1.0/docs/source/topics/glossary.rst`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/docs/source/topics/hub_overview.rst` & `cpop-34.1.0/docs/source/topics/hub_overview.rst`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/docs/source/topics/ideas_that_were_not_used.rst` & `cpop-34.1.0/docs/source/topics/ideas_that_were_not_used.rst`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/docs/source/topics/learning.rst` & `cpop-34.1.0/docs/source/topics/learning.rst`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/docs/source/topics/pop.rst` & `cpop-34.1.0/docs/source/topics/pop.rst`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/docs/source/topics/pre_contract_returns.rst` & `cpop-34.1.0/docs/source/topics/pre_contract_returns.rst`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/docs/source/topics/story.rst` & `cpop-34.1.0/docs/source/topics/story.rst`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/docs/source/topics/sub_patterns.rst` & `cpop-34.1.0/docs/source/topics/sub_patterns.rst`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/docs/source/topics/subs_overview.rst` & `cpop-34.1.0/docs/source/topics/subs_overview.rst`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/docs/source/topics/virtual.rst` & `cpop-34.1.0/docs/source/topics/virtual.rst`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/docs/source/tutorial/quickstart.rst` & `cpop-34.1.0/docs/source/tutorial/quickstart.rst`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/src/cpop/contract.pyx` & `cpop-34.1.0/src/cpop/contract.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import inspect
+import sys
+import traceback
 from collections.abc import Iterable
 from collections.abc import Mapping
 from cpython cimport dict
 from cython cimport pint
 from cpython.ref cimport PyObject
 
 cdef class ContractedContext:
@@ -158,44 +160,45 @@
             "pre": self._get_contracts_by_type("pre"),
             "call": self._get_contracts_by_type("call")[:1],
             "post": self._get_contracts_by_type("post"),
         }
         self._has_contracts = sum(len(l) for l in self.contract_functions.values()) > 0
 
     async def __call__(self, *args, **kwargs):
-        if self.implicit_hub:
-            args = (self.hub,) + args
+        async with CallStack(self):
+            if self.implicit_hub:
+                args = (self.hub,) + args
+
+            if not self._has_contracts:
+                ret = await self.func(*args, **kwargs)
+                return ret
+            contract_context = ContractedContext(
+                self.func, args, kwargs, self.signature, self.ref, self.__name__
+            )
 
-        if not self._has_contracts:
-            ret = await self.func(*args, **kwargs)
-            return ret
-        contract_context = ContractedContext(
-            self.func, args, kwargs, self.signature, self.ref, self.__name__
-        )
-
-        # Process pre contracts
-        for fn in self.contract_functions["pre"]:
-            pre_ret = await fn(contract_context)
-
-            await self.hub.pop.contract.process_pre_result(pre_ret, fn, self)
-
-        # Call the one call contract
-        if self.contract_functions["call"]:
-            ret = await self.contract_functions["call"][0](contract_context)
-        else:
-            ret = await self.func(*contract_context.args, **contract_context.kwargs)
-
-        # Handle post contracts
-        for fn in self.contract_functions["post"]:
-            contract_context.ret = ret
-            post_ret = await fn(contract_context)
-            if post_ret is not None:
-                ret = post_ret
+            # Process pre contracts
+            for fn in self.contract_functions["pre"]:
+                pre_ret = await fn(contract_context)
+
+                await self.hub.pop.contract.process_pre_result(pre_ret, fn, self)
+
+            # Call the one call contract
+            if self.contract_functions["call"]:
+                ret = await self.contract_functions["call"][0](contract_context)
+            else:
+                ret = await self.func(*contract_context.args, **contract_context.kwargs)
+
+            # Handle post contracts
+            for fn in self.contract_functions["post"]:
+                contract_context.ret = ret
+                post_ret = await fn(contract_context)
+                if post_ret is not None:
+                    ret = post_ret
 
-        return ret
+            return ret
 
     def __getstate__(self):
         return {
             "ref": self.ref,
             "name": self.__name__,
             "implicit_hub": self.implicit_hub,
             "contracts": self.contracts,
@@ -204,48 +207,71 @@
     def __setstate__(self, state:dict[str, object]):
         self.ref = state["ref"]
         self.__name__ = state["name"]
         self.func = self.hub[self.ref][self.__name__].func
         self.implicit_hub = state["implicit_hub"]
         self.contracts = state["contracts"]
 
+    def __repr__(self):
+        return f"<{self.__class__.__name__} {self.ref}.{self.__name__}>"
+
 
 
 class ContractedAsyncGen(Contracted):
     async def __call__(self, *args, **kwargs):
-        if self.implicit_hub:
-            args = (self.hub,) + args
+        async with CallStack(self):
+            if self.implicit_hub:
+                args = (self.hub,) + args
+
+            if not self._has_contracts:
+                async for chunk in self.func(*args, **kwargs):
+                    yield chunk
+                return
+            contract_context = ContractedContext(
+                self.func, args, kwargs, self.signature, self.ref, self.__name__
+            )
+
+            for fn in self.contract_functions["pre"]:
+                pre_ret = await fn(contract_context)
+
+                await self.hub.pop.contract.process_pre_result(pre_ret, fn, self)
+            chunk = None
+            if self.contract_functions["call"]:
+                async for chunk in self.contract_functions["call"][0](contract_context):
+                    yield chunk
+            else:
+                async for chunk in self.func(
+                    *contract_context.args, **contract_context.kwargs
+                ):
+                    yield chunk
+            ret = chunk
+            for fn in self.contract_functions["post"]:
+                contract_context.ret = ret
+                post_ret = await fn(contract_context)
+                if post_ret is not None:
+                    ret = post_ret
+
+class CallStack:
+    """
+    A wrapper for functions to add and remove their context from the stack securely
+    """
+    def __init__(self, contract: Contracted):
+        self.contract = contract
+
+    async def __aenter__(self):
+        # Get the caller's frame
+        frame = sys._getframe(1)
+        stack_summary = traceback.StackSummary.extract(traceback.walk_stack(frame))
+        # Push the ref and the stack summary onto the call stack
+        self.contract.hub._call_stack_push(f"{self.contract.ref}.{self.contract.__name__}", stack_summary)
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        # Remove the entry from the call stack
+        self.contract.hub._call_stack_pop()
 
-        if not self._has_contracts:
-            async for chunk in self.func(*args, **kwargs):
-                yield chunk
-            return
-        contract_context = ContractedContext(
-            self.func, args, kwargs, self.signature, self.ref, self.__name__
-        )
-
-        for fn in self.contract_functions["pre"]:
-            pre_ret = await fn(contract_context)
-
-            await self.hub.pop.contract.process_pre_result(pre_ret, fn, self)
-        chunk = None
-        if self.contract_functions["call"]:
-            async for chunk in self.contract_functions["call"][0](contract_context):
-                yield chunk
-        else:
-            async for chunk in self.func(
-                *contract_context.args, **contract_context.kwargs
-            ):
-                yield chunk
-        ret = chunk
-        for fn in self.contract_functions["post"]:
-            contract_context.ret = ret
-            post_ret = await fn(contract_context)
-            if post_ret is not None:
-                ret = post_ret
 
 def create_contracted(
     hub,
     contracts: list["cpop.loader.LoadedMod"],
     func,
     ref: str,
     name: str,
```

### Comparing `cpop-34.0.0/src/cpop/data.pyx` & `cpop-34.1.0/src/cpop/data.pyx`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/src/cpop/dirs.pyx` & `cpop-34.1.0/src/cpop/dirs.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         path = aiopath.Path(dir_)
         if not await path.is_dir():
             continue
         async for sub in path.iterdir():
             full = path / sub
             if str(sub).endswith(".egg-link"):
                 async with full.open() as rfh:
-                    dirs.add(aiopath.Path(await rfh.read().strip()))
+                    dirs.add(aiopath.Path((await rfh.read()).strip()))
             elif await full.is_dir():
                 dirs.add(full)
 
     # Set up the _dynamic return
     ret = cpop.data.NamespaceDict(
         dyne=cpop.data.NamespaceDict(),
         config=cpop.data.NamespaceDict(),
```

### Comparing `cpop-34.0.0/src/cpop/exc.pyx` & `cpop-34.1.0/src/cpop/exc.pyx`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/src/cpop/hub.pyx` & `cpop-34.1.0/src/cpop/hub.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import asyncio
 import importlib.machinery
 import os
 import secrets
 import signal
 import sys
+import traceback
+from contextvars import ContextVar, copy_context
 from collections.abc import Iterable
 from types import ModuleType
 from typing import Any
 
 import cpop.contract
 import cpop.data
 import cpop.dirs
@@ -62,14 +64,15 @@
 
 
 class Hub(PopMeta):
     """
     The redistributed pop central hub. All components of the system are
     rooted to the Hub.
     """
+    _call_stack = ContextVar("_call_stack", default=[])
 
     def __init__(self, *args, **kwargs):
         subs = {}
         sub_alias = {}
         imports = {}
         PopMeta.__init__(self, [subs, sub_alias, imports])
         self._subs = subs
@@ -78,14 +81,17 @@
         self._dynamic = None
         self._dscan = False
         # Set up the conf OPT structure so it is always available
         self._opt = None
         self._task_count = 0
         self._aio_alive = {}
 
+        # Set up the custom traceback hook
+        sys.excepthook = self._traceback
+
     async def __ainit__(
         self,
         load_all_dynes: bool = True,
         load_all_subdirs: bool = True,
         recurse_subdirs: bool = True,
         pop_mods: list[str] = None,
         cli: str = None,
@@ -117,14 +123,15 @@
 
             # Add the pop sub to the hub, this should always use pypath and
             # Should never be made dynamic. This is a core system sub and should
             # NOT be app-merged
             self._subs["pop"] = await AsyncSub(self, subname="pop", pypath=pop_mods)
             await self._subs["pop"]._load_all()
 
+
         self._load_all_dynes = load_all_dynes
         self._load_all_subdirs = load_all_subdirs
         self._recurse_subdirs = recurse_subdirs
         if self._load_all_dynes:
             await self._scan_dynamic()
             await self._load_all()
 
@@ -190,30 +197,65 @@
             await complete["task"]
             if complete["cb"]:
                 await self._auto(complete["cb"])
             self._task_count -= 1
             if self.task_count == 0:
                 break
 
-    def _auto(hub, coro, cb_coro=None):
+    def _auto(self, coro, cb_coro=None):
         """
         Start a task that will be automatically awaited
 
         coro: An unscheduled coroutine object to run
         cb_coro: An unscheduled coroutine to run when the main coroutine completes
         """
-        hub._task_count += 1
+        current_context = copy_context()
+        current_stack = self._call_stack.get().copy()
+
+        # Create a new context for the task to carry its own call stack
+        token = self._call_stack.set(current_stack)
+        try:
+            self._task_count += 1
 
-        task = asyncio.create_task(coro)
+            task = current_context.run(asyncio.create_task, coro)
 
-        def _callback(task):
-            hub._tasks.put_nowait({"task": task, "cb": cb_coro})
+            def _callback(task):
+                original_context = copy_context()
+                original_context.run(self._tasks.put_nowait, {"task": task, "cb": cb_coro})
 
-        task.add_done_callback(_callback)
-        return task
+            task.add_done_callback(_callback)
+            return task
+        finally:
+            # Cleanup, reset the context when add_done_callback
+            self._call_stack.reset(token)
+
+    @classmethod
+    def _call_stack_push(cls, ref:str, stack_summary):
+        stack = cls._call_stack.get()
+        stack.append((ref, stack_summary))
+
+    @classmethod
+    def _call_stack_pop(cls):
+        stack = cls._call_stack.get()
+        if stack:
+            stack.pop()
+
+
+    def _traceback(self, exctype, value, tb):
+        for ref, stack in reversed(self._call_stack.get()):
+            print(f"\nCalled from {ref}:", file=sys.stderr)
+            for frame in stack:
+                print(f"  File \"{frame.filename}\", line {frame.lineno}, in {frame.name}", file=sys.stderr)
+                line = frame.line.strip() if frame.line else None
+                if not line:
+                    continue
+                print(f"    {line}", file=sys.stderr)
+        else:
+            # Print the standard traceback
+            traceback.print_exception(exctype, value, tb)
 
     def __getstate__(self) -> dict:
         attrs = {}
         for k, v in self._attrs.items():
             if isinstance(v, cpop.loader.BASE_TYPES):
                 attrs[k] = v
             elif isinstance(v, dict):
```

### Comparing `cpop-34.0.0/src/cpop/loader.pyx` & `cpop-34.1.0/src/cpop/loader.pyx`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/src/cpop/ref.pyx` & `cpop-34.1.0/src/cpop/ref.pyx`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/src/cpop/scanner.pyx` & `cpop-34.1.0/src/cpop/scanner.pyx`

 * *Files 23% similar despite different names*

```diff
@@ -10,16 +10,19 @@
 
 def scan(dirs: Iterable[str]) -> dict:
     ret = {}
     ret["python"] = {}
     ret["cython"] = {}
     ret["imp"] = {}
     for dir_ in dirs:
-        for fn_ in os.listdir(dir_):
-            _apply_scan(ret, str(dir_), str(fn_))
+        try:
+            for fn_ in os.listdir(dir_):
+                _apply_scan(ret, str(dir_), str(fn_))
+        except FileNotFoundError:
+            ...
     return ret
 
 
 cdef _apply_scan(dict ret, str dir_, str fn_):
     if fn_.startswith("_"):
         return
     full = os.path.join(dir_, fn_)
```

### Comparing `cpop-34.0.0/src/cpop/verify.pyx` & `cpop-34.1.0/src/cpop/verify.pyx`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/src/pop/config.yaml` & `cpop-34.1.0/src/pop/config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -80,8 +80,9 @@
   - cpop.exc
   - cpop.contract
   - cpop.data
   - cpop.hub
   - msgpack
   - signal
   - sys
+  - traceback
   - yaml
```

### Comparing `cpop-34.0.0/src/pop/log/basic.py` & `cpop-34.1.0/src/pop/log/basic.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/src/pop/log/init.py` & `cpop-34.1.0/src/pop/log/init.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,26 +12,23 @@
     hub.log.warn = hub.log.warning
     hub.log.critical = hub.log.init.critical
     hub.log.fatal = hub.log.critical
 
 
 async def get_caller(hub) -> tuple[str, int]:
     """
-    Inspect the stack and find the first contracted ref that does not contain "log"
+    Inspect the stack and get the function that called get_caller
     """
-    stack = hub.lib.inspect.stack(context=0)
-    for frame in stack:
-        if not frame.code_context:
-            continue
-        context = frame.code_context[0].strip()
-        match = hub.lib.re.search(r"(hub\..*?)\(", context)
-        if match:
-            return match.group(1), frame.lineno
-
-    return "hub", 0
+    try:
+        # Grab the third ref back, fall back to closer refs
+        ref, stack_summary = (hub._call_stack.get()[-3:] or [None])[0]
+        filename, lineno, *_ = stack_summary
+        return ref, lineno
+    except Exception:
+        return "hub", 0
 
 
 async def get_logger(hub, name: str):
     """
     Create a logger for the given ref with all the configured handlers
     """
     if name not in hub.log.LOGGER:
```

### Comparing `cpop-34.0.0/src/pop/log/timed_rolling.py` & `cpop-34.1.0/src/pop/log/timed_rolling.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/src/pop/mods/config.py` & `cpop-34.1.0/src/pop/mods/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,19 +49,21 @@
     # Load the config file parameter in the proper order
     pop_config = config.get("pop", {}).get("config") or {}
     config_file = (
         cli_opts.get("config")
         or hub.lib.os.environ.get("POP_CONFIG", pop_config.get("os"))
         or pop_config.get("default")
     )
-    if config_file and hub.lib.os.path.exists(config_file):
-        async with hub.lib.aiofiles.open(config_file, "r") as fh:
-            config_data = hub.lib.yaml.safe_load(await fh.read())
-    else:
-        config_data = {}
+
+    config_data = {}
+    if config_file:
+        config_file = hub.lib.aiopath.Path(config_file)
+        if await config_file.exists():
+            async with config_file.open("r") as fh:
+                config_data = hub.lib.yaml.safe_load(await fh.read())
 
     OPT = await hub.pop.config.prioritize(
         cli=cli,
         cli_opts=cli_opts,
         config=config,
         config_file_data=config_data,
         global_clis=global_clis,
```

### Comparing `cpop-34.0.0/src/pop/mods/contract.py` & `cpop-34.1.0/src/pop/mods/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/src/pop/mods/sub.py` & `cpop-34.1.0/src/pop/mods/sub.py`

 * *Files 10% similar despite different names*

```diff
@@ -119,30 +119,30 @@
     :param hub: The redistributed pop central hub
     :param sub: The pop object that contains the loaded module data
     :param recurse: Recursively iterate over nested subs
     """
     if not sub._sub_virtual:
         return
     dirs = await hub.pop.sub.get_dirs(sub)
-    roots = {}
+    roots = hub.lib.collections.defaultdict(list)
     for dir_ in dirs:
-        for fn in hub.lib.os.listdir(dir_):
-            if fn.startswith("_"):
+        dir_ = hub.lib.aiopath.Path(dir_)
+        if not await dir_.exists():
+            continue
+        async for fn in dir_.iterdir():
+            if fn.name.startswith("_"):
                 continue
-            if fn == "contracts":
+            if fn.name == "contracts":
                 continue
-            if fn == "recursive_contracts":
+            if fn.name == "recursive_contracts":
                 continue
-            full = hub.lib.os.path.join(dir_, fn)
-            if not hub.lib.os.path.isdir(full):
+            full = dir_/ fn
+            if not await full.is_dir():
                 continue
-            if fn not in roots:
-                roots[fn] = [full]
-            else:
-                roots[fn].append(full)
+            roots[fn.name].append(str(full))
     for name, sub_dirs in roots.items():
         if name.startswith("."):
             continue
         # Load er up!
         await hub.pop.sub.add(
             subname=name,
             sub=sub,
```

### Comparing `cpop-34.0.0/src/pop/mods/task.py` & `cpop-34.1.0/src/pop/mods/task.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/src/pop/mods/test.py` & `cpop-34.1.0/src/pop/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/conftest.py` & `cpop-34.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/contracts/ctx.py` & `cpop-34.1.0/tests/contracts/ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/contracts/many.py` & `cpop-34.1.0/tests/contracts/many.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/contracts/test.py` & `cpop-34.1.0/tests/contracts/test.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/func/test_basic.py` & `cpop-34.1.0/tests/func/test_basic.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/func/test_config.py` & `cpop-34.1.0/tests/func/test_config.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/func/test_contract_ctx.py` & `cpop-34.1.0/tests/func/test_contract_ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/func/test_fail.py` & `cpop-34.1.0/tests/func/test_fail.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/func/test_log.py` & `cpop-34.1.0/tests/func/test_log.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/func/test_no_raise_on_pre_failure.py` & `cpop-34.1.0/tests/func/test_no_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/func/test_raise_on_pre_failure.py` & `cpop-34.1.0/tests/func/test_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/func/test_ref.py` & `cpop-34.1.0/tests/func/test_ref.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/func/test_serial.py` & `cpop-34.1.0/tests/func/test_serial.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/integration/contract_ordering/single_module/contracts/default.py` & `cpop-34.1.0/tests/integration/contract_ordering/single_module/contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/integration/contract_ordering/single_module/contracts/dunder.py` & `cpop-34.1.0/tests/integration/contract_ordering/single_module/contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/integration/contract_ordering/single_module/contracts/init.py` & `cpop-34.1.0/tests/integration/contract_ordering/single_module/contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/integration/contract_ordering/single_module/contracts/thing.py` & `cpop-34.1.0/tests/integration/contract_ordering/single_module/contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/default.py` & `cpop-34.1.0/tests/integration/contract_ordering/single_module/recursive_contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py` & `cpop-34.1.0/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/init.py` & `cpop-34.1.0/tests/integration/contract_ordering/single_module/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py` & `cpop-34.1.0/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py` & `cpop-34.1.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py` & `cpop-34.1.0/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/mods/proc.py` & `cpop-34.1.0/tests/mods/proc.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/mods/test.py` & `cpop-34.1.0/tests/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/regression/contract_masking/test_contract_masking.py` & `cpop-34.1.0/tests/regression/contract_masking/test_contract_masking.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/regression/contract_masking/test_duplicate_contracts.py` & `cpop-34.1.0/tests/regression/contract_masking/test_duplicate_contracts.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/tpath/cn/contract/test.py` & `cpop-34.1.0/tests/tpath/cn/contract/test.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/tests/unit/test_contract.py` & `cpop-34.1.0/tests/unit/test_contract.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import inspect
 
 import cpop.data
 from cpop.contract import Contracted
 
 
-async def test_contracted_shortcut():
+async def test_contracted_shortcut(hub):
     async def f(hub):
         pass
 
-    mock_hub = cpop.data.NamespaceDict(_tasks=[])
-    c = Contracted(hub=mock_hub, contracts=[], func=f, ref="", name="")
+    c = Contracted(hub=hub, contracts=[], func=f, ref="", name="")
     c.contract_functions["pre"] = [
         None
     ]  # add some garbage so we raise if we try to evaluate contracts
 
     await c()
```

### Comparing `cpop-34.0.0/tests/unit/test_sigs.py` & `cpop-34.1.0/tests/unit/test_sigs.py`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/.gitignore` & `cpop-34.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/README.rst` & `cpop-34.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `cpop-34.0.0/pyproject.toml` & `cpop-34.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-cython", "hatch-compile-yaml>=18.0.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cpop"
-version = "34.0.0"
+version = "34.1.0"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch45@gmail.com"},
 ]
 classifiers = [
@@ -41,15 +41,14 @@
 
 build = [
     "Cython",
     "hatch",
     "hatch-cython",
 ]
 
-
 [tool.hatch.build.targets.wheel]
 packages = [
     "src/cpop",
     "src/pop",
 ]
 
 [tool.hatch.build.hooks.convert-data-file.options]
```

### Comparing `cpop-34.0.0/PKG-INFO` & `cpop-34.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 34.0.0
+Version: 34.1.0
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch45@gmail.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


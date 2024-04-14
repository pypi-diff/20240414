# Comparing `tmp/chikvdf-1.1.3.tar.gz` & `tmp/chikvdf-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chikvdf-1.1.3.tar", last modified: Fri Apr 12 14:54:08 2024, max compression
+gzip compressed data, was "chikvdf-1.1.4.tar", last modified: Sun Apr 14 05:03:32 2024, max compression
```

## Comparing `chikvdf-1.1.3.tar` & `chikvdf-1.1.4.tar`

### file list

```diff
@@ -1,153 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:08.475519 chikvdf-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 14:54:03.000000 chikvdf-1.1.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:08.443519 chikvdf-1.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:08.451519 chikvdf-1.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-12 14:54:03.000000 chikvdf-1.1.3/.github/workflows/build-riscv64.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7761 2024-04-12 14:54:03.000000 chikvdf-1.1.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-12 14:54:03.000000 chikvdf-1.1.3/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-12 14:54:03.000000 chikvdf-1.1.3/.github/workflows/hw-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-12 14:54:03.000000 chikvdf-1.1.3/.github/workflows/stale-issue.yml.bak
--rwxr-xr-x   0 runner    (1001) docker     (127)     2016 2024-04-12 14:54:03.000000 chikvdf-1.1.3/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-12 14:54:03.000000 chikvdf-1.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-12 14:54:03.000000 chikvdf-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20300 2024-04-12 14:54:08.475519 chikvdf-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19985 2024-04-12 14:54:03.000000 chikvdf-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-12 14:54:03.000000 chikvdf-1.1.3/README_ASIC.md
--rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-12 14:54:03.000000 chikvdf-1.1.3/README_AVX512.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:08.447519 chikvdf-1.1.3/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:08.451519 chikvdf-1.1.3/assets/deb/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-12 14:54:03.000000 chikvdf-1.1.3/assets/deb/control.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:08.471519 chikvdf-1.1.3/chikvdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20300 2024-04-12 14:54:08.000000 chikvdf-1.1.3/chikvdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-12 14:54:08.000000 chikvdf-1.1.3/chikvdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:54:08.000000 chikvdf-1.1.3/chikvdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:54:08.000000 chikvdf-1.1.3/chikvdf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 14:54:08.000000 chikvdf-1.1.3/chikvdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)   464444 2024-04-12 14:54:03.000000 chikvdf-1.1.3/classgroups.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-04-12 14:54:03.000000 chikvdf-1.1.3/comparenweso.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-12 14:54:03.000000 chikvdf-1.1.3/lgtm.yml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 14:54:03.000000 chikvdf-1.1.3/mypi.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-12 14:54:03.000000 chikvdf-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:54:08.475519 chikvdf-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-12 14:54:03.000000 chikvdf-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:08.463519 chikvdf-1.1.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/1weso_test.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/2weso_test.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/ClassGroup.h
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/Makefile.vdf-client
--rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/Reducer.h
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/alloc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    29480 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/asm_avx512_ifma.h
--rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/asm_base.h
--rw-r--r--   0 runner    (1001) docker     (127)    25992 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/asm_gcd_128.h
--rw-r--r--   0 runner    (1001) docker     (127)    14791 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/asm_gcd_base_continued_fractions.h
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/asm_gcd_base_divide_table.h
--rw-r--r--   0 runner    (1001) docker     (127)    29721 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/asm_gcd_unsigned.h
--rw-r--r--   0 runner    (1001) docker     (127)    15548 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/asm_main.h
--rw-r--r--   0 runner    (1001) docker     (127)    17155 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/asm_types.h
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/asm_vm.h
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/avx512_integer.h
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/avx512_test.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/bit_manipulation.h
--rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/bqfc.c
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/bqfc.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:08.467519 chikvdf-1.1.3/src/c_bindings/
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/c_bindings/c_wrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/c_bindings/c_wrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/c_bindings/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/callback.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:08.467519 chikvdf-1.1.3/src/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/cmake/FindGMP.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/cmake/FindGMPXX.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/compile_asm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/create_discriminant.h
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/double_utility.h
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/fast_storage.h
--rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/gcd_128.h
--rw-r--r--   0 runner    (1001) docker     (127)    25108 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/gcd_base_continued_fractions.h
--rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/gcd_base_divide_table.h
--rw-r--r--   0 runner    (1001) docker     (127)    12852 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/gcd_unsigned.h
--rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/generic.h
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/generic_macros.h
--rw-r--r--   0 runner    (1001) docker     (127)    19274 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/gpu_integer.h
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/gpu_integer_divide.h
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/gpu_integer_gcd.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:08.471519 chikvdf-1.1.3/src/hw/
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/chik_driver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/chik_driver.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17561 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/chik_registers.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/clock.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/emu_funcs.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8909 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/emu_runner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/emu_runner.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    26213 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/ftdi_driver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/ftdi_driver.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/hw_interface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/hw_interface.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    25757 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/hw_proof.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/hw_proof.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/hw_test.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/hw_util.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/hw_util.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18045 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/hw_vdf_client.cpp
--rw-r--r--   0 runner    (1001) docker     (127)   269094 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/pll_freqs.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/pll_freqs.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/pvt.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/real_hw.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    18220 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/vdf_driver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/hw/vdf_driver.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/include.h
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/integer.h
--rw-r--r--   0 runner    (1001) docker     (127)    10598 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/integer_common.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:08.447519 chikvdf-1.1.3/src/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:08.471519 chikvdf-1.1.3/src/lib/gmp-patch-6.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/lib/gmp-patch-6.2.1/compat.c
--rw-r--r--   0 runner    (1001) docker     (127)    85426 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/lib/gmp-patch-6.2.1/longlong.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:08.471519 chikvdf-1.1.3/src/lib/gmp-patch-6.2.1/mpz/
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/lib/gmp-patch-6.2.1/mpz/inp_raw.c
--rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/nucomp.h
--rw-r--r--   0 runner    (1001) docker     (127)     9406 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/parameters.h
--rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/picosha2.h
--rw-r--r--   0 runner    (1001) docker     (127)    19946 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/pprods.h
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/primetest.h
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/proof_common.h
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/prover_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/prover_parallel.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/prover_slow.h
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/prover_test.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/provers.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:08.471519 chikvdf-1.1.3/src/python_bindings/
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/python_bindings/fastvdf.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:08.471519 chikvdf-1.1.3/src/refcode/
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/refcode/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    17395 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/refcode/lzcnt.c
--rw-r--r--   0 runner    (1001) docker     (127)    22775 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/threading.h
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/tl_emu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:08.471519 chikvdf-1.1.3/src/uint128_t/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/uint128_t/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/uint128_t/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/uint128_t/uint128_t.build
--rw-r--r--   0 runner    (1001) docker     (127)    13370 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/uint128_t/uint128_t.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/uint128_t/uint128_t.h
--rw-r--r--   0 runner    (1001) docker     (127)    19142 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/uint128_t/uint128_t.include
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/uint128_t/uint128_t_config.include
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/util.h
--rw-r--r--   0 runner    (1001) docker     (127)    29502 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/vdf.h
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/vdf_base.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/vdf_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/vdf_bench.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13004 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/vdf_client.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    34151 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/vdf_fast.h
--rw-r--r--   0 runner    (1001) docker     (127)    12701 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/vdf_new.h
--rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/vdf_original.h
--rw-r--r--   0 runner    (1001) docker     (127)    15641 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/vdf_test.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/vdf_test.h
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/verifier.h
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/verifier_test.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-12 14:54:03.000000 chikvdf-1.1.3/src/xgcd_partial.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:08.471519 chikvdf-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-12 14:54:03.000000 chikvdf-1.1.3/tests/test_n_weso_verifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-12 14:54:03.000000 chikvdf-1.1.3/tests/test_verifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:08.471519 chikvdf-1.1.3/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1890 2024-04-12 14:54:03.000000 chikvdf-1.1.3/tools/gen_pprods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:03:32.933069 chikvdf-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-14 05:03:28.000000 chikvdf-1.1.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:03:32.909069 chikvdf-1.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:03:32.913069 chikvdf-1.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-14 05:03:28.000000 chikvdf-1.1.4/.github/workflows/build-c-libraries.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-14 05:03:28.000000 chikvdf-1.1.4/.github/workflows/build-riscv64.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7761 2024-04-14 05:03:28.000000 chikvdf-1.1.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-14 05:03:28.000000 chikvdf-1.1.4/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-14 05:03:28.000000 chikvdf-1.1.4/.github/workflows/hw-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-14 05:03:28.000000 chikvdf-1.1.4/.github/workflows/stale-issue.yml.bak
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2016 2024-04-14 05:03:28.000000 chikvdf-1.1.4/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-14 05:03:28.000000 chikvdf-1.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-14 05:03:28.000000 chikvdf-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20300 2024-04-14 05:03:32.933069 chikvdf-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19985 2024-04-14 05:03:28.000000 chikvdf-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-14 05:03:28.000000 chikvdf-1.1.4/README_ASIC.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-14 05:03:28.000000 chikvdf-1.1.4/README_AVX512.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:03:32.909069 chikvdf-1.1.4/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:03:32.913069 chikvdf-1.1.4/assets/deb/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-14 05:03:28.000000 chikvdf-1.1.4/assets/deb/control.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:03:32.933069 chikvdf-1.1.4/chikvdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20300 2024-04-14 05:03:32.000000 chikvdf-1.1.4/chikvdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-14 05:03:32.000000 chikvdf-1.1.4/chikvdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 05:03:32.000000 chikvdf-1.1.4/chikvdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 05:03:32.000000 chikvdf-1.1.4/chikvdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 05:03:32.000000 chikvdf-1.1.4/chikvdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   464444 2024-04-14 05:03:28.000000 chikvdf-1.1.4/classgroups.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-04-14 05:03:28.000000 chikvdf-1.1.4/comparenweso.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-14 05:03:28.000000 chikvdf-1.1.4/lgtm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-14 05:03:28.000000 chikvdf-1.1.4/mypi.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-14 05:03:28.000000 chikvdf-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 05:03:32.933069 chikvdf-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-14 05:03:28.000000 chikvdf-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:03:32.925069 chikvdf-1.1.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/1weso_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/2weso_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/ClassGroup.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/Makefile.vdf-client
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/Reducer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/alloc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    29480 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/asm_avx512_ifma.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/asm_base.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25992 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/asm_gcd_128.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14791 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/asm_gcd_base_continued_fractions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/asm_gcd_base_divide_table.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29721 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/asm_gcd_unsigned.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15548 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/asm_main.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17155 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/asm_types.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/asm_vm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/avx512_integer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/avx512_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/bit_manipulation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/bqfc.c
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/bqfc.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:03:32.925069 chikvdf-1.1.4/src/c_bindings/
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/c_bindings/c_wrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/c_bindings/c_wrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/c_bindings/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/callback.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:03:32.925069 chikvdf-1.1.4/src/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/cmake/FindGMP.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/cmake/FindGMPXX.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/compile_asm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/create_discriminant.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/double_utility.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/fast_storage.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/gcd_128.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25108 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/gcd_base_continued_fractions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/gcd_base_divide_table.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12852 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/gcd_unsigned.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/generic.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/generic_macros.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19274 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/gpu_integer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/gpu_integer_divide.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/gpu_integer_gcd.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:03:32.929069 chikvdf-1.1.4/src/hw/
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/chik_driver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/chik_driver.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17561 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/chik_registers.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/clock.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/emu_funcs.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8909 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/emu_runner.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/emu_runner.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    26213 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/ftdi_driver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/ftdi_driver.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/hw_interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/hw_interface.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    25757 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/hw_proof.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/hw_proof.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/hw_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/hw_util.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/hw_util.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18045 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/hw_vdf_client.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)   269094 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/pll_freqs.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/pll_freqs.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/pvt.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/real_hw.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18220 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/vdf_driver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/hw/vdf_driver.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/include.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/integer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10598 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/integer_common.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:03:32.909069 chikvdf-1.1.4/src/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:03:32.933069 chikvdf-1.1.4/src/lib/gmp-patch-6.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/lib/gmp-patch-6.2.1/compat.c
+-rw-r--r--   0 runner    (1001) docker     (127)    85426 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/lib/gmp-patch-6.2.1/longlong.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:03:32.933069 chikvdf-1.1.4/src/lib/gmp-patch-6.2.1/mpz/
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/lib/gmp-patch-6.2.1/mpz/inp_raw.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/nucomp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9406 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/parameters.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/picosha2.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19946 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/pprods.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/primetest.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/proof_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/prover_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/prover_parallel.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/prover_slow.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/prover_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/provers.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:03:32.933069 chikvdf-1.1.4/src/python_bindings/
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/python_bindings/fastvdf.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:03:32.933069 chikvdf-1.1.4/src/refcode/
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/refcode/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17395 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/refcode/lzcnt.c
+-rw-r--r--   0 runner    (1001) docker     (127)    22775 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/threading.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/tl_emu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:03:32.933069 chikvdf-1.1.4/src/uint128_t/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/uint128_t/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/uint128_t/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/uint128_t/uint128_t.build
+-rw-r--r--   0 runner    (1001) docker     (127)    13370 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/uint128_t/uint128_t.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/uint128_t/uint128_t.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19142 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/uint128_t/uint128_t.include
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/uint128_t/uint128_t_config.include
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/util.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29502 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/vdf.h
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/vdf_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/vdf_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/vdf_bench.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13004 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/vdf_client.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    34151 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/vdf_fast.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12701 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/vdf_new.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/vdf_original.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15641 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/vdf_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/vdf_test.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/verifier.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/verifier_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-14 05:03:28.000000 chikvdf-1.1.4/src/xgcd_partial.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:03:32.933069 chikvdf-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-14 05:03:28.000000 chikvdf-1.1.4/tests/test_n_weso_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-14 05:03:28.000000 chikvdf-1.1.4/tests/test_verifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:03:32.933069 chikvdf-1.1.4/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1890 2024-04-14 05:03:28.000000 chikvdf-1.1.4/tools/gen_pprods.py
```

### Comparing `chikvdf-1.1.3/.github/workflows/build-riscv64.yml` & `chikvdf-1.1.4/.github/workflows/build-riscv64.yml`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/.github/workflows/build.yml` & `chikvdf-1.1.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/.github/workflows/codeql-analysis.yml` & `chikvdf-1.1.4/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/.github/workflows/hw-build.yml` & `chikvdf-1.1.4/.github/workflows/hw-build.yml`

 * *Files 1% similar despite different names*

```diff
@@ -100,13 +100,14 @@
           GH_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         run: |
           gh release upload \
             $RELEASE_TAG \
             dist/${{ env.DEB_NAME }}
 
       - uses: Chik-Network/actions/github/jwt@main
+        if: env.RELEASE == 'true'
 
       - name: Trigger repo update
         if: env.RELEASE == 'true'
         run: |
           curl -s -XPOST -H "Authorization: Bearer ${{ env.JWT_TOKEN }}" --data '{"release_version":"${{ env.RELEASE_TAG }}"}' ${{ secrets.GLUE_API_URL }}/api/v1/chikvdf-hw/${{ env.RELEASE_TAG }}/start
           curl -s -XPOST -H "Authorization: Bearer ${{ env.JWT_TOKEN }}" --data '{"release_version":"${{ env.RELEASE_TAG }}"}' ${{ secrets.GLUE_API_URL }}/api/v1/chikvdf-hw/${{ env.RELEASE_TAG }}/success/release_hw
```

### Comparing `chikvdf-1.1.3/.github/workflows/stale-issue.yml.bak` & `chikvdf-1.1.4/.github/workflows/stale-issue.yml.bak`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/.github/workflows/test.yaml` & `chikvdf-1.1.4/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/.gitignore` & `chikvdf-1.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/LICENSE` & `chikvdf-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/PKG-INFO` & `chikvdf-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chikvdf
-Version: 1.1.3
+Version: 1.1.4
 Summary: Chik vdf verification (wraps C++)
 Home-page: https://github.com/Chik-Network/chikvdf
 Author: Florin Chirica
 Author-email: florin@chiknetwork.com
 License: Apache License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `chikvdf-1.1.3/README.md` & `chikvdf-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/README_ASIC.md` & `chikvdf-1.1.4/README_ASIC.md`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/README_AVX512.md` & `chikvdf-1.1.4/README_AVX512.md`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/chikvdf.egg-info/PKG-INFO` & `chikvdf-1.1.4/chikvdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chikvdf
-Version: 1.1.3
+Version: 1.1.4
 Summary: Chik vdf verification (wraps C++)
 Home-page: https://github.com/Chik-Network/chikvdf
 Author: Florin Chirica
 Author-email: florin@chiknetwork.com
 License: Apache License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `chikvdf-1.1.3/chikvdf.egg-info/SOURCES.txt` & `chikvdf-1.1.4/chikvdf.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 classgroups.pdf
 comparenweso.py
 lgtm.yml
 mypi.ini
 pyproject.toml
 setup.py
 ./
+.github/workflows/build-c-libraries.yml
 .github/workflows/build-riscv64.yml
 .github/workflows/build.yml
 .github/workflows/codeql-analysis.yml
 .github/workflows/hw-build.yml
 .github/workflows/stale-issue.yml.bak
 .github/workflows/test.yaml
 assets/deb/control.j2
```

### Comparing `chikvdf-1.1.3/classgroups.pdf` & `chikvdf-1.1.4/classgroups.pdf`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/comparenweso.py` & `chikvdf-1.1.4/comparenweso.py`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/pyproject.toml` & `chikvdf-1.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -39,10 +39,11 @@
 [tool.cibuildwheel.windows]
 build-verbosity = 0
 before-all = "git clone https://github.com/Chik-Network/mpir_gc_x64.git"
 environment = {BUILD_VDF_CLIENT="N"}
 before-build = "pip install delvewheel"
 repair-wheel-command = """
 delvewheel repair -v -w {dest_dir} {wheel} \
+--no-mangle-all \
 --add-path mpir_gc_x64 \
 --add-dll mpir.dll;mpir_gc.dll;mpir_broadwell.dll;mpir_broadwell_avx.dll;mpir_bulldozer.dll;mpir_haswell.dll;mpir_piledriver.dll;mpir_sandybridge.dll;mpir_skylake_avx.dll \
 """
```

### Comparing `chikvdf-1.1.3/setup.py` & `chikvdf-1.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/1weso_test.cpp` & `chikvdf-1.1.4/src/1weso_test.cpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/2weso_test.cpp` & `chikvdf-1.1.4/src/2weso_test.cpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/CMakeLists.txt` & `chikvdf-1.1.4/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/ClassGroup.h` & `chikvdf-1.1.4/src/ClassGroup.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/Makefile.vdf-client` & `chikvdf-1.1.4/src/Makefile.vdf-client`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/Reducer.h` & `chikvdf-1.1.4/src/Reducer.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/alloc.hpp` & `chikvdf-1.1.4/src/alloc.hpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/asm_avx512_ifma.h` & `chikvdf-1.1.4/src/asm_avx512_ifma.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/asm_base.h` & `chikvdf-1.1.4/src/asm_base.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/asm_gcd_128.h` & `chikvdf-1.1.4/src/asm_gcd_128.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/asm_gcd_base_continued_fractions.h` & `chikvdf-1.1.4/src/asm_gcd_base_continued_fractions.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/asm_gcd_base_divide_table.h` & `chikvdf-1.1.4/src/asm_gcd_base_divide_table.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/asm_gcd_unsigned.h` & `chikvdf-1.1.4/src/asm_gcd_unsigned.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/asm_main.h` & `chikvdf-1.1.4/src/asm_main.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/asm_types.h` & `chikvdf-1.1.4/src/asm_types.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/asm_vm.h` & `chikvdf-1.1.4/src/asm_vm.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/avx512_integer.h` & `chikvdf-1.1.4/src/avx512_integer.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/avx512_test.cpp` & `chikvdf-1.1.4/src/avx512_test.cpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/bit_manipulation.h` & `chikvdf-1.1.4/src/bit_manipulation.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/bqfc.c` & `chikvdf-1.1.4/src/bqfc.c`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/bqfc.h` & `chikvdf-1.1.4/src/bqfc.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/c_bindings/c_wrapper.cpp` & `chikvdf-1.1.4/src/c_bindings/c_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/c_bindings/c_wrapper.h` & `chikvdf-1.1.4/src/c_bindings/c_wrapper.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/callback.h` & `chikvdf-1.1.4/src/callback.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/cmake/FindGMP.cmake` & `chikvdf-1.1.4/src/cmake/FindGMP.cmake`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/cmake/FindGMPXX.cmake` & `chikvdf-1.1.4/src/cmake/FindGMPXX.cmake`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/compile_asm.cpp` & `chikvdf-1.1.4/src/compile_asm.cpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/double_utility.h` & `chikvdf-1.1.4/src/double_utility.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/fast_storage.h` & `chikvdf-1.1.4/src/fast_storage.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/gcd_128.h` & `chikvdf-1.1.4/src/gcd_128.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/gcd_base_continued_fractions.h` & `chikvdf-1.1.4/src/gcd_base_continued_fractions.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/gcd_base_divide_table.h` & `chikvdf-1.1.4/src/gcd_base_divide_table.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/gcd_unsigned.h` & `chikvdf-1.1.4/src/gcd_unsigned.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/generic.h` & `chikvdf-1.1.4/src/generic.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/generic_macros.h` & `chikvdf-1.1.4/src/generic_macros.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/gpu_integer.h` & `chikvdf-1.1.4/src/gpu_integer.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/gpu_integer_divide.h` & `chikvdf-1.1.4/src/gpu_integer_divide.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/gpu_integer_gcd.h` & `chikvdf-1.1.4/src/gpu_integer_gcd.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/hw/chik_driver.cpp` & `chikvdf-1.1.4/src/hw/chik_driver.cpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/hw/chik_driver.hpp` & `chikvdf-1.1.4/src/hw/chik_driver.hpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/hw/chik_registers.hpp` & `chikvdf-1.1.4/src/hw/chik_registers.hpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/hw/clock.hpp` & `chikvdf-1.1.4/src/hw/clock.hpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/hw/emu_funcs.cpp` & `chikvdf-1.1.4/src/hw/emu_funcs.cpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/hw/emu_runner.cpp` & `chikvdf-1.1.4/src/hw/emu_runner.cpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/hw/ftdi_driver.cpp` & `chikvdf-1.1.4/src/hw/ftdi_driver.cpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/hw/ftdi_driver.hpp` & `chikvdf-1.1.4/src/hw/ftdi_driver.hpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/hw/hw_interface.cpp` & `chikvdf-1.1.4/src/hw/hw_interface.cpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/hw/hw_interface.hpp` & `chikvdf-1.1.4/src/hw/hw_interface.hpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/hw/hw_proof.cpp` & `chikvdf-1.1.4/src/hw/hw_proof.cpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/hw/hw_proof.hpp` & `chikvdf-1.1.4/src/hw/hw_proof.hpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/hw/hw_test.cpp` & `chikvdf-1.1.4/src/hw/hw_test.cpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/hw/hw_util.hpp` & `chikvdf-1.1.4/src/hw/hw_util.hpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/hw/hw_vdf_client.cpp` & `chikvdf-1.1.4/src/hw/hw_vdf_client.cpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/hw/pll_freqs.cpp` & `chikvdf-1.1.4/src/hw/pll_freqs.cpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/hw/pll_freqs.hpp` & `chikvdf-1.1.4/src/hw/pll_freqs.hpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/hw/pvt.hpp` & `chikvdf-1.1.4/src/hw/pvt.hpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/hw/vdf_driver.cpp` & `chikvdf-1.1.4/src/hw/vdf_driver.cpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/hw/vdf_driver.hpp` & `chikvdf-1.1.4/src/hw/vdf_driver.hpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/include.h` & `chikvdf-1.1.4/src/include.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/integer.h` & `chikvdf-1.1.4/src/integer.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/integer_common.h` & `chikvdf-1.1.4/src/integer_common.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/lib/gmp-patch-6.2.1/compat.c` & `chikvdf-1.1.4/src/lib/gmp-patch-6.2.1/compat.c`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/lib/gmp-patch-6.2.1/longlong.h` & `chikvdf-1.1.4/src/lib/gmp-patch-6.2.1/longlong.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/lib/gmp-patch-6.2.1/mpz/inp_raw.c` & `chikvdf-1.1.4/src/lib/gmp-patch-6.2.1/mpz/inp_raw.c`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/nucomp.h` & `chikvdf-1.1.4/src/nucomp.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/parameters.h` & `chikvdf-1.1.4/src/parameters.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/picosha2.h` & `chikvdf-1.1.4/src/picosha2.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/pprods.h` & `chikvdf-1.1.4/src/pprods.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/primetest.h` & `chikvdf-1.1.4/src/primetest.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/proof_common.h` & `chikvdf-1.1.4/src/proof_common.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/prover_base.hpp` & `chikvdf-1.1.4/src/prover_base.hpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/prover_parallel.hpp` & `chikvdf-1.1.4/src/prover_parallel.hpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/prover_slow.h` & `chikvdf-1.1.4/src/prover_slow.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/prover_test.cpp` & `chikvdf-1.1.4/src/prover_test.cpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/provers.h` & `chikvdf-1.1.4/src/provers.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/python_bindings/fastvdf.cpp` & `chikvdf-1.1.4/src/python_bindings/fastvdf.cpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/refcode/README.md` & `chikvdf-1.1.4/src/refcode/README.md`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/refcode/lzcnt.c` & `chikvdf-1.1.4/src/refcode/lzcnt.c`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/threading.h` & `chikvdf-1.1.4/src/threading.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/tl_emu.py` & `chikvdf-1.1.4/src/tl_emu.py`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/uint128_t/LICENSE` & `chikvdf-1.1.4/src/uint128_t/LICENSE`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/uint128_t/README.md` & `chikvdf-1.1.4/src/uint128_t/README.md`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/uint128_t/uint128_t.cpp` & `chikvdf-1.1.4/src/uint128_t/uint128_t.cpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/uint128_t/uint128_t.include` & `chikvdf-1.1.4/src/uint128_t/uint128_t.include`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/uint128_t/uint128_t_config.include` & `chikvdf-1.1.4/src/uint128_t/uint128_t_config.include`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/util.h` & `chikvdf-1.1.4/src/util.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/vdf.h` & `chikvdf-1.1.4/src/vdf.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/vdf_base.hpp` & `chikvdf-1.1.4/src/vdf_base.hpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/vdf_bench.cpp` & `chikvdf-1.1.4/src/vdf_bench.cpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/vdf_client.cpp` & `chikvdf-1.1.4/src/vdf_client.cpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/vdf_fast.h` & `chikvdf-1.1.4/src/vdf_fast.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/vdf_new.h` & `chikvdf-1.1.4/src/vdf_new.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/vdf_original.h` & `chikvdf-1.1.4/src/vdf_original.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/vdf_test.cpp` & `chikvdf-1.1.4/src/vdf_test.cpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/vdf_test.h` & `chikvdf-1.1.4/src/vdf_test.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/verifier.h` & `chikvdf-1.1.4/src/verifier.h`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/verifier_test.cpp` & `chikvdf-1.1.4/src/verifier_test.cpp`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/src/xgcd_partial.c` & `chikvdf-1.1.4/src/xgcd_partial.c`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/tests/test_n_weso_verifier.py` & `chikvdf-1.1.4/tests/test_n_weso_verifier.py`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/tests/test_verifier.py` & `chikvdf-1.1.4/tests/test_verifier.py`

 * *Files identical despite different names*

### Comparing `chikvdf-1.1.3/tools/gen_pprods.py` & `chikvdf-1.1.4/tools/gen_pprods.py`

 * *Files identical despite different names*


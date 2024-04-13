# Comparing `tmp/pixi_kernel-0.2.0.tar.gz` & `tmp/pixi_kernel-0.2.1.tar.gz`

## Comparing `pixi_kernel-0.2.0.tar` & `pixi_kernel-0.2.1.tar`

### file list

```diff
@@ -1,56 +1,57 @@
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/codecov.yml
--rw-r--r--   0        0        0   494805 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/pixi.lock
--rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/pixi.toml
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0   169085 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/assets/launch-dark.png
--rw-r--r--   0        0        0   176986 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/assets/launch-light.png
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-bash/kernel.json
--rw-r--r--   0        0        0   801365 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-bash/logo-svg.svg
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-ir/kernel.js
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-ir/kernel.json
--rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-ir/logo-64x64.png
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-ir/logo-svg.svg
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-python3/kernel.json
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-python3/logo-32x32.png
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-python3/logo-64x64.png
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-python3/logo-svg.svg
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp11/kernel.json
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp11/logo-32x32.png
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp11/logo-64x64.png
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp11/logo-svg.svg
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp14/kernel.json
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp14/logo-32x32.png
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp14/logo-64x64.png
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp14/logo-svg.svg
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp17/kernel.json
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp17/logo-32x32.png
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp17/logo-64x64.png
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp17/logo-svg.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/src/pixi_kernel/__init__.py
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/src/pixi_kernel/errors.py
--rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/src/pixi_kernel/pixi.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/src/pixi_kernel/provisioner.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/bash_kernel/kernel.py
--rw-r--r--   0        0        0   123358 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/bash_kernel/pixi.lock
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/bash_kernel/pixi.toml
--rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/ipykernel/kernel.py
--rw-r--r--   0        0        0   119641 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/ipykernel/pixi.lock
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/ipykernel/pixi.toml
--rw-r--r--   0        0        0    16817 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/r-irkernel/kernel.py
--rw-r--r--   0        0        0   329338 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/r-irkernel/pixi.lock
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/r-irkernel/pixi.toml
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/xeus-cling/kernel.py
--rw-r--r--   0        0        0    77254 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/xeus-cling/pixi.lock
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/xeus-cling/pixi.toml
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/unit/conftest.py
--rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/unit/test_pixi.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/unit/data/missing_ipykernel/pixi.toml
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/unit/data/pixi_project/pixi.toml
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/unit/data/pyproject_project/pyproject.toml
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/LICENSE
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/README.md
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4724 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/codecov.yml
+-rw-r--r--   0        0        0   494805 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/pixi.lock
+-rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/pixi.toml
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0   169085 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/assets/launch-dark.png
+-rw-r--r--   0        0        0   176986 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/assets/launch-light.png
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-bash/kernel.json
+-rw-r--r--   0        0        0   801365 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-bash/logo-svg.svg
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-ir/kernel.js
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-ir/kernel.json
+-rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-ir/logo-64x64.png
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-ir/logo-svg.svg
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-python3/kernel.json
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-python3/logo-32x32.png
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-python3/logo-64x64.png
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-python3/logo-svg.svg
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp11/kernel.json
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp11/logo-32x32.png
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp11/logo-64x64.png
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp11/logo-svg.svg
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp14/kernel.json
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp14/logo-32x32.png
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp14/logo-64x64.png
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp14/logo-svg.svg
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp17/kernel.json
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp17/logo-32x32.png
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp17/logo-64x64.png
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp17/logo-svg.svg
+-rwxr-xr-x   0        0        0      466 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/scripts/update-lock.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/src/pixi_kernel/__init__.py
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/src/pixi_kernel/errors.py
+-rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/src/pixi_kernel/pixi.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/src/pixi_kernel/provisioner.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/bash_kernel/kernel.py
+-rw-r--r--   0        0        0   123358 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/bash_kernel/pixi.lock
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/bash_kernel/pixi.toml
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/ipykernel/kernel.py
+-rw-r--r--   0        0        0   119641 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/ipykernel/pixi.lock
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/ipykernel/pixi.toml
+-rw-r--r--   0        0        0    16817 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/r-irkernel/kernel.py
+-rw-r--r--   0        0        0   329298 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/r-irkernel/pixi.lock
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/r-irkernel/pixi.toml
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/xeus-cling/kernel.py
+-rw-r--r--   0        0        0    77254 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/xeus-cling/pixi.lock
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/xeus-cling/pixi.toml
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/unit/conftest.py
+-rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/unit/test_pixi.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/unit/data/missing_ipykernel/pixi.toml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/unit/data/pixi_project/pixi.toml
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/unit/data/pyproject_project/pyproject.toml
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/README.md
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/PKG-INFO
```

### Comparing `pixi_kernel-0.2.0/CONTRIBUTING.md` & `pixi_kernel-0.2.1/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 pixi run lint
 ```
 
 ## Making a release
 
 1. Bump
    1. Increment version in `pyproject.toml` and in `pixi.toml`
-   2. Update all Pixi lock files
+   2. Update all Pixi lock files by running `pixi run update-lock`
    3. Commit with message "Bump version number to X.Y.Z"
    4. Push commit to GitHub
    5. Check [CI](https://github.com/renan-r-santos/pixi-kernel/actions/workflows/ci.yml) to ensure
       all tests pass
 2. Tag
    1. Tag commit with "vX.Y.Z"
    2. Push tag to GitHub
```

### Comparing `pixi_kernel-0.2.0/pixi.lock` & `pixi_kernel-0.2.1/pixi.lock`

 * *Files 0% similar despite different names*

```diff
@@ -444,15 +444,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.2-hab00c5b_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.2-py312h886d080_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/ruff-0.3.6-py312h9118e91_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/ruff-0.3.7-py312h9118e91_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/secretstorage-3.3.3-py312h7900ff3_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
@@ -543,15 +543,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.2-h43d1f9e_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/pyzmq-25.1.2-py312h1c32067_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/readline-8.2-h8fc344f_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ruff-0.3.6-py312hb434743_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ruff-0.3.7-py312hb434743_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/secretstorage-3.3.3-py312h8025657_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/tk-8.6.13-h194ca79_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
@@ -628,15 +628,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.2-h9f0c242_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.2-py312hc789acb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/ruff-0.3.6-py312h1bc86af_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/ruff-0.3.7-py312h1bc86af_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
@@ -712,15 +712,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.2-hdf0ec26_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pyzmq-25.1.2-py312h1edf716_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ruff-0.3.6-py312h1ae9fbf_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ruff-0.3.7-py312h1ae9fbf_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
@@ -795,15 +795,15 @@
       - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.2-h2628c8c_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/pywin32-306-py312h53d5487_2.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/pywin32-ctypes-0.2.2-py312h2e8e312_1.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.2-py312h1ac6f91_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/ruff-0.3.6-py312h60fbdae_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/ruff-0.3.7-py312h60fbdae_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
@@ -2818,15 +2818,15 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.2-hab00c5b_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/ruff-0.3.6-py312h9118e91_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/ruff-0.3.7-py312h9118e91_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
       linux-aarch64:
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/_openmp_mutex-4.5-2_gnu.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/bzip2-1.0.8-h31becfc_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ca-certificates-2024.2.2-hcefe29a_0.conda
@@ -2842,15 +2842,15 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libxcrypt-4.4.36-h31becfc_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libzlib-1.2.13-h31becfc_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ncurses-6.4.20240210-h0425590_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/openssl-3.2.1-h31becfc_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.2-h43d1f9e_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/readline-8.2-h8fc344f_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ruff-0.3.6-py312hb434743_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ruff-0.3.7-py312hb434743_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/tk-8.6.13-h194ca79_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/xz-5.2.6-h9cdd2b7_0.tar.bz2
       osx-64:
       - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda
@@ -2859,15 +2859,15 @@
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.2-h92b6c6a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4.20240210-h73e2aa4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.2.1-hd75f5a5_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.2-h9f0c242_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/ruff-0.3.6-py312h1bc86af_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/ruff-0.3.7-py312h1bc86af_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
       osx-arm64:
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ca-certificates-2024.2.2-hf0a4a13_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libcxx-16.0.6-h4653b0c_0.conda
@@ -2876,29 +2876,29 @@
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsqlite-3.45.2-h091b4b1_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libzlib-1.2.13-h53f4e23_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.4.20240210-h078ce10_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.2.1-h0d3ecfb_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.2-hdf0ec26_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ruff-0.3.6-py312h1ae9fbf_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ruff-0.3.7-py312h1ae9fbf_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
       win-64:
       - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libexpat-2.6.2-h63175ca_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.2-hcfcfb64_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/openssl-3.2.1-hcfcfb64_1.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.2-h2628c8c_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.12-4_cp312.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/ruff-0.3.6-py312h60fbdae_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/ruff-0.3.7-py312h60fbdae_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hcf57466_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33130-h82b7239_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33130-hcb4865c_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
@@ -6905,17 +6905,17 @@
   - ptyprocess >=0.5
   - python >=3.7
   license: ISC
   size: 53600
   timestamp: 1706113273252
 - kind: pypi
   name: pixi-kernel
-  version: 0.2.0
+  version: 0.2.1
   path: .
-  sha256: d505b18617c43a2be12c4af779636bca35effc06c2b873b9584f4193c0933f2e
+  sha256: fc89be37749334e0eb20e8656e5ffcdace662e69fd273fa798213fdf1e64b7cb
   requires_dist:
   - jupyter-client >=7
   - msgspec >=0.18
   requires_python: <4.0,>=3.8
   editable: true
 - kind: conda
   name: platformdirs
@@ -8530,112 +8530,112 @@
   - typing_extensions >=4.0.0,<5.0.0
   license: MIT
   license_family: MIT
   size: 184347
   timestamp: 1709150578093
 - kind: conda
   name: ruff
-  version: 0.3.6
+  version: 0.3.7
   build: py312h1ae9fbf_0
   subdir: osx-arm64
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/ruff-0.3.6-py312h1ae9fbf_0.conda
-  sha256: f8d5d283ee136250864a070e50dec6738ff28453fd73af739ece49826f80b59b
-  md5: c2fe33d8dd7c679cc8c7acfc34f336e7
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/ruff-0.3.7-py312h1ae9fbf_0.conda
+  sha256: d410024c1f5007dded6cde0336ef66eb1f20c6012541cdfab8098bf92f88f76f
+  md5: 19a5d0d42b93d6705a430836e27a72e8
   depends:
   - libcxx >=16
   - python >=3.12,<3.13.0a0
   - python >=3.12,<3.13.0a0 *_cpython
   - python_abi 3.12.* *_cp312
   constrains:
   - __osx >=11.0
   license: MIT
   license_family: MIT
   purls:
   - pkg:pypi/ruff
-  size: 5883291
-  timestamp: 1712912010322
+  size: 5873488
+  timestamp: 1712963468673
 - kind: conda
   name: ruff
-  version: 0.3.6
+  version: 0.3.7
   build: py312h1bc86af_0
   subdir: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/ruff-0.3.6-py312h1bc86af_0.conda
-  sha256: abc77a56d0a1789511da5d11c97f4ebc9d52dce63687447603b13c8894734953
-  md5: 5650ad2040677c884c026519561d90d2
+  url: https://conda.anaconda.org/conda-forge/osx-64/ruff-0.3.7-py312h1bc86af_0.conda
+  sha256: 34453d115397fb697c5786f25382f3419e418dcbb5a185d0e6217388b1edfd9b
+  md5: 43f114392c6f66ef9238edbd9c229815
   depends:
   - libcxx >=16
   - python >=3.12,<3.13.0a0
   - python_abi 3.12.* *_cp312
   constrains:
   - __osx >=10.12
   license: MIT
   license_family: MIT
   purls:
   - pkg:pypi/ruff
-  size: 6194513
-  timestamp: 1712912348068
+  size: 6190521
+  timestamp: 1712963528403
 - kind: conda
   name: ruff
-  version: 0.3.6
+  version: 0.3.7
   build: py312h60fbdae_0
   subdir: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/ruff-0.3.6-py312h60fbdae_0.conda
-  sha256: bb2ee817a0837a305765b3ccb3547590660791d1023b7d2db660993393cce740
-  md5: 6fc51382fa7126f757983c0a379b0f9d
+  url: https://conda.anaconda.org/conda-forge/win-64/ruff-0.3.7-py312h60fbdae_0.conda
+  sha256: e1f2debb0daa31da527aa45281c8f5097c9bda74589ad7c8c6056011528a86e0
+  md5: fbed1c59af89011cd6f286e5c12771a2
   depends:
   - python >=3.12,<3.13.0a0
   - python_abi 3.12.* *_cp312
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: MIT
   license_family: MIT
   purls:
   - pkg:pypi/ruff
-  size: 6338814
-  timestamp: 1712911917602
+  size: 6336660
+  timestamp: 1712963199532
 - kind: conda
   name: ruff
-  version: 0.3.6
+  version: 0.3.7
   build: py312h9118e91_0
   subdir: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/ruff-0.3.6-py312h9118e91_0.conda
-  sha256: ef3015d88abb3a13e165504d07fd55316b823d315df7e789b53772548b4a7a42
-  md5: ad31febc156789922ae37dddb6426073
+  url: https://conda.anaconda.org/conda-forge/linux-64/ruff-0.3.7-py312h9118e91_0.conda
+  sha256: 457e71eb4a877715353510ec1fc28742bb21f874551a1ca1ef9f91456e18c202
+  md5: 76dc72c065cc15f69b96656b3431a5a4
   depends:
   - libgcc-ng >=12
   - libstdcxx-ng >=12
   - python >=3.12,<3.13.0a0
   - python_abi 3.12.* *_cp312
   license: MIT
   license_family: MIT
   purls:
   - pkg:pypi/ruff
-  size: 6397725
-  timestamp: 1712911131299
+  size: 6410120
+  timestamp: 1712962253616
 - kind: conda
   name: ruff
-  version: 0.3.6
+  version: 0.3.7
   build: py312hb434743_0
   subdir: linux-aarch64
-  url: https://conda.anaconda.org/conda-forge/linux-aarch64/ruff-0.3.6-py312hb434743_0.conda
-  sha256: d00396eeabfcd1dfbc94c3f576acf1b2db5673ca5c75d0a6d5c10e33b4925cb8
-  md5: 6d78c355f878086b0335dcf8ff3b7491
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/ruff-0.3.7-py312hb434743_0.conda
+  sha256: b51878dde6ac030d2aacedd9262856d197cc91c624601af21a387c4c38a927a9
+  md5: e19b2f69c44d0084cdd048648f405065
   depends:
   - libgcc-ng >=12
   - libstdcxx-ng >=12
   - python >=3.12,<3.13.0a0
   - python >=3.12,<3.13.0a0 *_cpython
   - python_abi 3.12.* *_cp312
   license: MIT
   license_family: MIT
   purls:
   - pkg:pypi/ruff
-  size: 6044573
-  timestamp: 1712911062472
+  size: 6047817
+  timestamp: 1712962191320
 - kind: conda
   name: secretstorage
   version: 3.3.3
   build: py310hbbe02a8_2
   build_number: 2
   subdir: linux-aarch64
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/secretstorage-3.3.3-py310hbbe02a8_2.conda
```

### Comparing `pixi_kernel-0.2.0/pixi.toml` & `pixi_kernel-0.2.1/pixi.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pixi-kernel"
-version = "0.2.0"
+version = "0.2.1"
 description = "Python Jupyter kernel using Pixi for reproducible notebooks"
 authors = ["Renan Rodrigues dos Santos <renan.engmec@gmail.com>"]
 channels = ["conda-forge"]
 platforms = ["linux-64", "linux-aarch64", "osx-64", "osx-arm64", "win-64"]
 
 
 # Dependencies
@@ -14,41 +14,49 @@
 msgspec = ">=0.18"
 
 
 # Development
 [feature.dev.pypi-dependencies]
 pixi-kernel = { path = ".", editable = true }
 
+[feature.dev.tasks]
+update-lock = "scripts/update-lock.sh"
+
 
 # Testing
 [feature.test.dependencies]
 pytest = ">=8.1,<9"
 pytest-cov = "*"
 
 [feature.test.tasks]
 # Unit tests
 unit = "COVERAGE_FILE=.coverage.$(python -c 'import platform; print(platform.system())').$PIXI_ENVIRONMENT_NAME python -m pytest --cov pixi_kernel"
 
 # Integration tests
 bash-kernel = { cwd = "tests/integration/bash_kernel", cmd = "PYDEVD_DISABLE_FILE_VALIDATION=1 pixi run --locked --manifest-path=pixi.toml python kernel.py" }
 ipykernel = { cwd = "tests/integration/ipykernel", cmd = "PYDEVD_DISABLE_FILE_VALIDATION=1 pixi run --locked --manifest-path=pixi.toml python kernel.py" }
 r-irkernel = { cwd = "tests/integration/r-irkernel", cmd = "pixi run --locked --manifest-path=pixi.toml python kernel.py" }
+xeus-cling = { cwd = "tests/integration/xeus-cling", cmd = "pixi run --locked --manifest-path=pixi.toml python kernel.py" }
 
 # Combined
 test = { depends_on = ["unit", "ipykernel", "r-irkernel"] }
 coverage = "coverage combine && coverage html && coverage xml"
 
 # Integration tests for platform-specific kernels
 [feature.test.target.linux-64.tasks]
-xeus-cling = { cwd = "tests/integration/xeus-cling", cmd = "pixi run --locked --manifest-path=pixi.toml python kernel.py" }
-test = { depends_on = ["unit", "ipykernel", "r-irkernel", "xeus-cling"] }
+test = { depends_on = ["unit", "bash-kernel", "ipykernel", "r-irkernel", "xeus-cling"] }
 
 [feature.test.target.linux-aarch64.tasks]
-xeus-cling = { cwd = "tests/integration/xeus-cling", cmd = "pixi run --locked --manifest-path=pixi.toml python kernel.py" }
-test = { depends_on = ["unit", "ipykernel", "r-irkernel", "xeus-cling"] }
+test = { depends_on = ["unit", "bash-kernel", "ipykernel", "r-irkernel", "xeus-cling"] }
+
+[feature.test.target.osx-64.tasks]
+test = { depends_on = ["unit", "bash-kernel", "ipykernel", "r-irkernel"] }
+
+[feature.test.target.osx-arm64.tasks]
+test = { depends_on = ["unit", "bash-kernel", "ipykernel", "r-irkernel"] }
 
 
 # Linting and formatting
 [feature.ruff.dependencies]
 ruff = ">=0.3.5,<0.4"
 
 [feature.ruff.tasks]
@@ -95,21 +103,15 @@
 python = "3.12.*"
 
 [feature.py312.tasks]
 test-py312 = { depends_on = ["install", "test"] }
 
 
 [environments]
-default = { features = [
-    "base",
-    "build",
-    "dev",
-    "ruff",
-    "test",
-], solve-group = "pixi-kernel" }
+default = { features = ["base", "build", "dev", "ruff", "test"], solve-group = "pixi-kernel" }
 build = { features = ["build"], solve-group = "pixi-kernel" }
 ruff = { features = ["ruff"], solve-group = "pixi-kernel" }
 test = { features = ["test"], solve-group = "pixi-kernel" }
 
 # Python testing matrix
 py38 = ["py38", "build", "test"]
 py39 = ["py39", "build", "test"]
```

### Comparing `pixi_kernel-0.2.0/.github/workflows/ci.yml` & `pixi_kernel-0.2.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/.github/workflows/release.yml` & `pixi_kernel-0.2.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/assets/launch-dark.png` & `pixi_kernel-0.2.1/assets/launch-dark.png`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/assets/launch-light.png` & `pixi_kernel-0.2.1/assets/launch-light.png`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/kernels/pixi-kernel-bash/logo-svg.svg` & `pixi_kernel-0.2.1/kernels/pixi-kernel-bash/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/kernels/pixi-kernel-ir/kernel.js` & `pixi_kernel-0.2.1/kernels/pixi-kernel-ir/kernel.js`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/kernels/pixi-kernel-ir/logo-64x64.png` & `pixi_kernel-0.2.1/kernels/pixi-kernel-ir/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/kernels/pixi-kernel-ir/logo-svg.svg` & `pixi_kernel-0.2.1/kernels/pixi-kernel-ir/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/kernels/pixi-kernel-python3/logo-32x32.png` & `pixi_kernel-0.2.1/kernels/pixi-kernel-python3/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/kernels/pixi-kernel-python3/logo-64x64.png` & `pixi_kernel-0.2.1/kernels/pixi-kernel-python3/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/kernels/pixi-kernel-python3/logo-svg.svg` & `pixi_kernel-0.2.1/kernels/pixi-kernel-python3/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp11/logo-32x32.png` & `pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp11/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp11/logo-64x64.png` & `pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp11/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp11/logo-svg.svg` & `pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp11/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp14/logo-32x32.png` & `pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp14/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp14/logo-64x64.png` & `pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp14/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp14/logo-svg.svg` & `pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp14/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp17/logo-32x32.png` & `pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp17/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp17/logo-64x64.png` & `pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp17/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp17/logo-svg.svg` & `pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp17/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/src/pixi_kernel/errors.py` & `pixi_kernel-0.2.1/src/pixi_kernel/errors.py`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/src/pixi_kernel/pixi.py` & `pixi_kernel-0.2.1/src/pixi_kernel/pixi.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 def find_project_manifest(
     *,
     cwd: Path,
     package_name: str,
     kernel_display_name: str,
     logger: Logger,
-) -> str:
+) -> Path:
     # Ensure Pixi is in PATH
     if shutil.which("pixi") is None:
         raise RuntimeError(PIXI_NOT_FOUND.format(kernel_display_name=kernel_display_name))
 
     # Ensure a supported Pixi version is installed
     result = subprocess.run(["pixi", "--version"], capture_output=True, text=True)
     if result.returncode != 0 or not result.stdout.startswith("pixi "):
@@ -98,10 +98,10 @@
                         )
                         raise RuntimeError(
                             PIXI_KERNEL_NOT_FOUND.format(
                                 kernel_display_name=kernel_display_name,
                                 package_name=package_name,
                             )
                         )
-                    return str(dir / project_filename)
+                    return dir / project_filename
 
     raise RuntimeError(PIXI_MANIFEST_NOT_FOUND.format(cwd=cwd))
```

### Comparing `pixi_kernel-0.2.0/tests/integration/bash_kernel/kernel.py` & `pixi_kernel-0.2.1/tests/integration/bash_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/tests/integration/bash_kernel/pixi.lock` & `pixi_kernel-0.2.1/tests/integration/bash_kernel/pixi.lock`

 * *Files 0% similar despite different names*

```diff
@@ -738,16 +738,16 @@
   - libstdcxx-ng >=12
   - python >=3.12,<3.13.0a0
   - python >=3.12,<3.13.0a0 *_cpython
   - python_abi 3.12.* *_cp312
   license: MIT
   license_family: MIT
   purls:
-  - pkg:pypi/bytecode
   - pkg:pypi/debugpy
+  - pkg:pypi/bytecode
   size: 2089528
   timestamp: 1707444654939
 - kind: conda
   name: debugpy
   version: 1.8.1
   build: py312h30efb56_0
   subdir: linux-64
@@ -758,16 +758,16 @@
   - libgcc-ng >=12
   - libstdcxx-ng >=12
   - python >=3.12,<3.13.0a0
   - python_abi 3.12.* *_cp312
   license: MIT
   license_family: MIT
   purls:
-  - pkg:pypi/debugpy
   - pkg:pypi/bytecode
+  - pkg:pypi/debugpy
   size: 2079306
   timestamp: 1707444570818
 - kind: conda
   name: debugpy
   version: 1.8.1
   build: py312h53d5487_0
   subdir: win-64
@@ -798,16 +798,16 @@
   depends:
   - libcxx >=16
   - python >=3.12,<3.13.0a0
   - python_abi 3.12.* *_cp312
   license: MIT
   license_family: MIT
   purls:
-  - pkg:pypi/bytecode
   - pkg:pypi/debugpy
+  - pkg:pypi/bytecode
   size: 2065572
   timestamp: 1707444822563
 - kind: conda
   name: decorator
   version: 5.1.1
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -1873,16 +1873,16 @@
   - tomli-w ; extra == 'toml'
   - tomli ; python_version < '3.11' and extra == 'toml'
   - pyyaml ; extra == 'yaml'
   requires_python: '>=3.8'
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/3f/76/30d8f152299f65c85c46a2cbeaf95ad1d18516b5ce730acdaef696d4cfe6/msgspec-0.18.6-cp312-cp312-win_amd64.whl
-  sha256: 1003c20bfe9c6114cc16ea5db9c5466e49fae3d7f5e2e59cb70693190ad34da0
+  url: https://files.pythonhosted.org/packages/1d/b5/c8fbf1db814eb29eda402952374b594b2559419ba7ec6d0997a9e5687530/msgspec-0.18.6-cp312-cp312-macosx_10_9_x86_64.whl
+  sha256: d86f5071fe33e19500920333c11e2267a31942d18fed4d9de5bc2fbab267d28c
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -1912,16 +1912,16 @@
   - tomli-w ; extra == 'toml'
   - tomli ; python_version < '3.11' and extra == 'toml'
   - pyyaml ; extra == 'yaml'
   requires_python: '>=3.8'
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/73/16/dfef780ced7d690dd5497846ed242ef3e27e319d59d1ddaae816a4f2c15e/msgspec-0.18.6-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: ad237100393f637b297926cae1868b0d500f764ccd2f0623a380e2bcfb2809ca
+  url: https://files.pythonhosted.org/packages/3f/76/30d8f152299f65c85c46a2cbeaf95ad1d18516b5ce730acdaef696d4cfe6/msgspec-0.18.6-cp312-cp312-win_amd64.whl
+  sha256: 1003c20bfe9c6114cc16ea5db9c5466e49fae3d7f5e2e59cb70693190ad34da0
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -1951,16 +1951,16 @@
   - tomli-w ; extra == 'toml'
   - tomli ; python_version < '3.11' and extra == 'toml'
   - pyyaml ; extra == 'yaml'
   requires_python: '>=3.8'
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/1d/b5/c8fbf1db814eb29eda402952374b594b2559419ba7ec6d0997a9e5687530/msgspec-0.18.6-cp312-cp312-macosx_10_9_x86_64.whl
-  sha256: d86f5071fe33e19500920333c11e2267a31942d18fed4d9de5bc2fbab267d28c
+  url: https://files.pythonhosted.org/packages/d7/9a/235d2dbab078a0b8e6f338205dc59be0b027ce000554ee6a9c41b19339e5/msgspec-0.18.6-cp312-cp312-macosx_11_0_arm64.whl
+  sha256: ce13981bfa06f5eb126a3a5a38b1976bddb49a36e4f46d8e6edecf33ccf11df1
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -1990,16 +1990,16 @@
   - tomli-w ; extra == 'toml'
   - tomli ; python_version < '3.11' and extra == 'toml'
   - pyyaml ; extra == 'yaml'
   requires_python: '>=3.8'
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/d7/9a/235d2dbab078a0b8e6f338205dc59be0b027ce000554ee6a9c41b19339e5/msgspec-0.18.6-cp312-cp312-macosx_11_0_arm64.whl
-  sha256: ce13981bfa06f5eb126a3a5a38b1976bddb49a36e4f46d8e6edecf33ccf11df1
+  url: https://files.pythonhosted.org/packages/73/16/dfef780ced7d690dd5497846ed242ef3e27e319d59d1ddaae816a4f2c15e/msgspec-0.18.6-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: ad237100393f637b297926cae1868b0d500f764ccd2f0623a380e2bcfb2809ca
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -2252,17 +2252,17 @@
   license_family: MIT
   purls:
   - pkg:pypi/pickleshare
   size: 9332
   timestamp: 1602536313357
 - kind: pypi
   name: pixi-kernel
-  version: 0.2.0
+  version: 0.2.1
   path: ../../../../pixi-kernel
-  sha256: d505b18617c43a2be12c4af779636bca35effc06c2b873b9584f4193c0933f2e
+  sha256: fc89be37749334e0eb20e8656e5ffcdace662e69fd273fa798213fdf1e64b7cb
   requires_dist:
   - jupyter-client >=7
   - msgspec >=0.18
   requires_python: <4.0,>=3.8
   editable: true
 - kind: conda
   name: platformdirs
@@ -2871,34 +2871,34 @@
   version: 0.18.0
   url: https://files.pythonhosted.org/packages/5a/57/2fcfd462cc53876ac4acef69dbf4fb941da971440049ca72051da54ea60d/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
   sha256: cd5bf1af8efe569654bbef5a3e0a56eca45f87cfcffab31dd8dde70da5982475
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/14/8c/e69f5636f4ab6ee0855aef3b16e6c97f8b636e9e04fa5a4bcc75126acb13/rpds_py-0.18.0-cp312-none-win_amd64.whl
-  sha256: e003b002ec72c8d5a3e3da2989c7d6065b47d9eaa70cd8808b5384fbb970f4ec
+  url: https://files.pythonhosted.org/packages/09/b6/45690f5d3f8c551bb462e063a2f336d72c8884ed26aa19beb53a374d3854/rpds_py-0.18.0-cp312-cp312-macosx_10_12_x86_64.whl
+  sha256: 7f2facbd386dd60cbbf1a794181e6aa0bd429bd78bfdf775436020172e2a23f0
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/c3/96/2211a1ca4b4e259e222169074ec0fa41f0ee18665dfc68988a139dc7e6e8/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: 4457a94da0d5c53dc4b3e4de1158bdab077db23c53232f37a3cb7afdb053a4e3
+  url: https://files.pythonhosted.org/packages/14/8c/e69f5636f4ab6ee0855aef3b16e6c97f8b636e9e04fa5a4bcc75126acb13/rpds_py-0.18.0-cp312-none-win_amd64.whl
+  sha256: e003b002ec72c8d5a3e3da2989c7d6065b47d9eaa70cd8808b5384fbb970f4ec
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/09/b6/45690f5d3f8c551bb462e063a2f336d72c8884ed26aa19beb53a374d3854/rpds_py-0.18.0-cp312-cp312-macosx_10_12_x86_64.whl
-  sha256: 7f2facbd386dd60cbbf1a794181e6aa0bd429bd78bfdf775436020172e2a23f0
+  url: https://files.pythonhosted.org/packages/7a/58/9bfc53b266df92f0515e72fd16e4890dc6b56fc3bfc216b3a2a729c866b5/rpds_py-0.18.0-cp312-cp312-macosx_11_0_arm64.whl
+  sha256: 1d9a5be316c15ffb2b3c405c4ff14448c36b4435be062a7f578ccd8b01f0c4d8
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/7a/58/9bfc53b266df92f0515e72fd16e4890dc6b56fc3bfc216b3a2a729c866b5/rpds_py-0.18.0-cp312-cp312-macosx_11_0_arm64.whl
-  sha256: 1d9a5be316c15ffb2b3c405c4ff14448c36b4435be062a7f578ccd8b01f0c4d8
+  url: https://files.pythonhosted.org/packages/c3/96/2211a1ca4b4e259e222169074ec0fa41f0ee18665dfc68988a139dc7e6e8/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: 4457a94da0d5c53dc4b3e4de1158bdab077db23c53232f37a3cb7afdb053a4e3
   requires_python: '>=3.8'
 - kind: conda
   name: six
   version: 1.16.0
   build: pyh6c4a22f_0
   subdir: noarch
   noarch: python
```

### Comparing `pixi_kernel-0.2.0/tests/integration/ipykernel/kernel.py` & `pixi_kernel-0.2.1/tests/integration/ipykernel/kernel.py`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/tests/integration/ipykernel/pixi.lock` & `pixi_kernel-0.2.1/tests/integration/ipykernel/pixi.lock`

 * *Files 0% similar despite different names*

```diff
@@ -608,16 +608,16 @@
   - libcxx >=16
   - python >=3.12,<3.13.0a0
   - python >=3.12,<3.13.0a0 *_cpython
   - python_abi 3.12.* *_cp312
   license: MIT
   license_family: MIT
   purls:
-  - pkg:pypi/debugpy
   - pkg:pypi/bytecode
+  - pkg:pypi/debugpy
   size: 2077038
   timestamp: 1707445014387
 - kind: conda
   name: debugpy
   version: 1.8.1
   build: py312h2aa54b4_0
   subdir: linux-aarch64
@@ -649,16 +649,16 @@
   - libgcc-ng >=12
   - libstdcxx-ng >=12
   - python >=3.12,<3.13.0a0
   - python_abi 3.12.* *_cp312
   license: MIT
   license_family: MIT
   purls:
-  - pkg:pypi/debugpy
   - pkg:pypi/bytecode
+  - pkg:pypi/debugpy
   size: 2079306
   timestamp: 1707444570818
 - kind: conda
   name: debugpy
   version: 1.8.1
   build: py312h53d5487_0
   subdir: win-64
@@ -689,16 +689,16 @@
   depends:
   - libcxx >=16
   - python >=3.12,<3.13.0a0
   - python_abi 3.12.* *_cp312
   license: MIT
   license_family: MIT
   purls:
-  - pkg:pypi/debugpy
   - pkg:pypi/bytecode
+  - pkg:pypi/debugpy
   size: 2065572
   timestamp: 1707444822563
 - kind: conda
   name: decorator
   version: 5.1.1
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -1725,16 +1725,16 @@
   purls:
   - pkg:pypi/matplotlib-inline
   size: 12273
   timestamp: 1660814913405
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/3f/76/30d8f152299f65c85c46a2cbeaf95ad1d18516b5ce730acdaef696d4cfe6/msgspec-0.18.6-cp312-cp312-win_amd64.whl
-  sha256: 1003c20bfe9c6114cc16ea5db9c5466e49fae3d7f5e2e59cb70693190ad34da0
+  url: https://files.pythonhosted.org/packages/1d/b5/c8fbf1db814eb29eda402952374b594b2559419ba7ec6d0997a9e5687530/msgspec-0.18.6-cp312-cp312-macosx_10_9_x86_64.whl
+  sha256: d86f5071fe33e19500920333c11e2267a31942d18fed4d9de5bc2fbab267d28c
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -1764,16 +1764,16 @@
   - tomli-w ; extra == 'toml'
   - tomli ; python_version < '3.11' and extra == 'toml'
   - pyyaml ; extra == 'yaml'
   requires_python: '>=3.8'
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/73/16/dfef780ced7d690dd5497846ed242ef3e27e319d59d1ddaae816a4f2c15e/msgspec-0.18.6-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: ad237100393f637b297926cae1868b0d500f764ccd2f0623a380e2bcfb2809ca
+  url: https://files.pythonhosted.org/packages/d7/9a/235d2dbab078a0b8e6f338205dc59be0b027ce000554ee6a9c41b19339e5/msgspec-0.18.6-cp312-cp312-macosx_11_0_arm64.whl
+  sha256: ce13981bfa06f5eb126a3a5a38b1976bddb49a36e4f46d8e6edecf33ccf11df1
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -1803,16 +1803,16 @@
   - tomli-w ; extra == 'toml'
   - tomli ; python_version < '3.11' and extra == 'toml'
   - pyyaml ; extra == 'yaml'
   requires_python: '>=3.8'
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/d7/9a/235d2dbab078a0b8e6f338205dc59be0b027ce000554ee6a9c41b19339e5/msgspec-0.18.6-cp312-cp312-macosx_11_0_arm64.whl
-  sha256: ce13981bfa06f5eb126a3a5a38b1976bddb49a36e4f46d8e6edecf33ccf11df1
+  url: https://files.pythonhosted.org/packages/73/16/dfef780ced7d690dd5497846ed242ef3e27e319d59d1ddaae816a4f2c15e/msgspec-0.18.6-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: ad237100393f637b297926cae1868b0d500f764ccd2f0623a380e2bcfb2809ca
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -1881,16 +1881,16 @@
   - tomli-w ; extra == 'toml'
   - tomli ; python_version < '3.11' and extra == 'toml'
   - pyyaml ; extra == 'yaml'
   requires_python: '>=3.8'
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/1d/b5/c8fbf1db814eb29eda402952374b594b2559419ba7ec6d0997a9e5687530/msgspec-0.18.6-cp312-cp312-macosx_10_9_x86_64.whl
-  sha256: d86f5071fe33e19500920333c11e2267a31942d18fed4d9de5bc2fbab267d28c
+  url: https://files.pythonhosted.org/packages/3f/76/30d8f152299f65c85c46a2cbeaf95ad1d18516b5ce730acdaef696d4cfe6/msgspec-0.18.6-cp312-cp312-win_amd64.whl
+  sha256: 1003c20bfe9c6114cc16ea5db9c5466e49fae3d7f5e2e59cb70693190ad34da0
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -2143,17 +2143,17 @@
   license_family: MIT
   purls:
   - pkg:pypi/pickleshare
   size: 9332
   timestamp: 1602536313357
 - kind: pypi
   name: pixi-kernel
-  version: 0.2.0
+  version: 0.2.1
   path: ../../../../pixi-kernel
-  sha256: d505b18617c43a2be12c4af779636bca35effc06c2b873b9584f4193c0933f2e
+  sha256: fc89be37749334e0eb20e8656e5ffcdace662e69fd273fa798213fdf1e64b7cb
   requires_dist:
   - jupyter-client >=7
   - msgspec >=0.18
   requires_python: <4.0,>=3.8
   editable: true
 - kind: conda
   name: platformdirs
@@ -2756,40 +2756,40 @@
   requires_dist:
   - attrs >=22.2.0
   - rpds-py >=0.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/14/8c/e69f5636f4ab6ee0855aef3b16e6c97f8b636e9e04fa5a4bcc75126acb13/rpds_py-0.18.0-cp312-none-win_amd64.whl
-  sha256: e003b002ec72c8d5a3e3da2989c7d6065b47d9eaa70cd8808b5384fbb970f4ec
+  url: https://files.pythonhosted.org/packages/09/b6/45690f5d3f8c551bb462e063a2f336d72c8884ed26aa19beb53a374d3854/rpds_py-0.18.0-cp312-cp312-macosx_10_12_x86_64.whl
+  sha256: 7f2facbd386dd60cbbf1a794181e6aa0bd429bd78bfdf775436020172e2a23f0
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/c3/96/2211a1ca4b4e259e222169074ec0fa41f0ee18665dfc68988a139dc7e6e8/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: 4457a94da0d5c53dc4b3e4de1158bdab077db23c53232f37a3cb7afdb053a4e3
+  url: https://files.pythonhosted.org/packages/7a/58/9bfc53b266df92f0515e72fd16e4890dc6b56fc3bfc216b3a2a729c866b5/rpds_py-0.18.0-cp312-cp312-macosx_11_0_arm64.whl
+  sha256: 1d9a5be316c15ffb2b3c405c4ff14448c36b4435be062a7f578ccd8b01f0c4d8
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/7a/58/9bfc53b266df92f0515e72fd16e4890dc6b56fc3bfc216b3a2a729c866b5/rpds_py-0.18.0-cp312-cp312-macosx_11_0_arm64.whl
-  sha256: 1d9a5be316c15ffb2b3c405c4ff14448c36b4435be062a7f578ccd8b01f0c4d8
+  url: https://files.pythonhosted.org/packages/c3/96/2211a1ca4b4e259e222169074ec0fa41f0ee18665dfc68988a139dc7e6e8/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: 4457a94da0d5c53dc4b3e4de1158bdab077db23c53232f37a3cb7afdb053a4e3
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
   url: https://files.pythonhosted.org/packages/5a/57/2fcfd462cc53876ac4acef69dbf4fb941da971440049ca72051da54ea60d/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
   sha256: cd5bf1af8efe569654bbef5a3e0a56eca45f87cfcffab31dd8dde70da5982475
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/09/b6/45690f5d3f8c551bb462e063a2f336d72c8884ed26aa19beb53a374d3854/rpds_py-0.18.0-cp312-cp312-macosx_10_12_x86_64.whl
-  sha256: 7f2facbd386dd60cbbf1a794181e6aa0bd429bd78bfdf775436020172e2a23f0
+  url: https://files.pythonhosted.org/packages/14/8c/e69f5636f4ab6ee0855aef3b16e6c97f8b636e9e04fa5a4bcc75126acb13/rpds_py-0.18.0-cp312-none-win_amd64.whl
+  sha256: e003b002ec72c8d5a3e3da2989c7d6065b47d9eaa70cd8808b5384fbb970f4ec
   requires_python: '>=3.8'
 - kind: conda
   name: six
   version: 1.16.0
   build: pyh6c4a22f_0
   subdir: noarch
   noarch: python
```

### Comparing `pixi_kernel-0.2.0/tests/integration/r-irkernel/kernel.py` & `pixi_kernel-0.2.1/tests/integration/r-irkernel/kernel.py`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/tests/integration/r-irkernel/pixi.lock` & `pixi_kernel-0.2.1/tests/integration/r-irkernel/pixi.lock`

 * *Files 0% similar despite different names*

```diff
@@ -543,17 +543,17 @@
       - pypi: https://files.pythonhosted.org/packages/d9/5a/e7c31adbe875f2abbb91bd84cf2dc52d792b5a01506781dbcf25c91daf11/six-1.16.0-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/4a/2e/3ba930e3af171847d610e07ae878e04fcb7e4d7822f1a2d29a27b128ea24/tornado-6.4-cp38-abi3-macosx_10_9_universal2.whl
       - pypi: https://files.pythonhosted.org/packages/7c/c4/366a09036c07f46eb8c9b2af39c97f502ef24f11f2a6e4d763655d9f2708/traitlets-5.14.2-py3-none-any.whl
       - pypi: ../../../../pixi-kernel
       win-64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/_r-mutex-1.0.1-anacondar_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2024.1.0-h57928b3_964.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2024.1.0-h57928b3_965.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libblas-3.9.0-22_win64_mkl.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.9.3-default_haede6df_1009.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.10.0-default_h2fffb23_1000.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libiconv-1.17-hcfcfb64_2.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/liblapack-3.9.0-22_win64_mkl.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.2-hcfcfb64_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libxml2-2.12.6-h8a06e1b_1.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.3.1-hcfcfb64_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-bwidget-1.9.10-2.tar.bz2
@@ -610,15 +610,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/r-pillar-1.9.0-r41hc72bb7e_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/r-repr-1.1.6-r41h785f33e_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/r-rlang-1.1.3-r41ha856d6a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/r-utf8-1.2.4-r41h6d2157b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/r-uuid-1.2_0-r41h6d2157b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/r-vctrs-0.6.5-r41ha856d6a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/sqlite-3.45.2-hcfcfb64_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/tbb-2021.11.0-h91493d7_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/tbb-2021.12.0-h91493d7_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hcf57466_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33130-h82b7239_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33130-hcb4865c_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.5-h63175ca_1.conda
       - pypi: https://files.pythonhosted.org/packages/e0/44/827b2a91a5816512fcaf3cc4ebc465ccd5d598c45cefa6703fcf4a79018f/attrs-23.2.0-py3-none-any.whl
@@ -2461,24 +2461,24 @@
   - jaraco-test >=5.4 ; extra == 'testing'
   - pytest-mypy ; platform_python_implementation != 'PyPy' and extra == 'testing'
   - importlib-resources >=1.3 ; python_version < '3.9' and extra == 'testing'
   requires_python: '>=3.8'
 - kind: conda
   name: intel-openmp
   version: 2024.1.0
-  build: h57928b3_964
-  build_number: 964
+  build: h57928b3_965
+  build_number: 965
   subdir: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2024.1.0-h57928b3_964.conda
-  sha256: bea54e995cd79b0961ded5f0d6d1b8a55513283ccda74cedb3421a3764f7d679
-  md5: 30ebb9fd99666d8b8675fcee541a09f3
+  url: https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2024.1.0-h57928b3_965.conda
+  sha256: 7b029e476ad6d401d645636ee3e4b40130bfcc9534f7415209dd5b666c6dd292
+  md5: c66eb2fd33b999ccc258aef85689758e
   license: LicenseRef-ProprietaryIntel
   license_family: Proprietary
-  size: 1616281
-  timestamp: 1712153179165
+  size: 1617555
+  timestamp: 1712943333029
 - kind: conda
   name: isl
   version: '0.26'
   build: imath32_h2e86a7b_101
   build_number: 101
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/isl-0.26-imath32_h2e86a7b_101.conda
@@ -3959,31 +3959,31 @@
   md5: 379be2f115ffb73860e4e260dd2170b7
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
   size: 423091
   timestamp: 1706820564165
 - kind: conda
   name: libhwloc
-  version: 2.9.3
-  build: default_haede6df_1009
-  build_number: 1009
-  subdir: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.9.3-default_haede6df_1009.conda
-  sha256: 2e8c4bb7173f281a8e13f333a23c9fb7a1c86d342d7dccdd74f2eb583ddde450
-  md5: 87da045f6d26ce9fe20ad76a18f6a18a
+  version: 2.10.0
+  build: default_h2fffb23_1000
+  build_number: 1000
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.10.0-default_h2fffb23_1000.conda
+  sha256: e0d75da50e67a81e3cb37e2ee3b0d6ddc6543ec0f7b3828f884558552a1c4d93
+  md5: ee944f0d41d9e2048f9d7492c1623ca3
   depends:
-  - libxml2 >=2.11.5,<3.0.0a0
+  - libxml2 >=2.12.6,<3.0a0
   - pthreads-win32
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: BSD-3-Clause
   license_family: BSD
-  size: 2578462
-  timestamp: 1694533393675
+  size: 2376728
+  timestamp: 1711491473761
 - kind: conda
   name: libiconv
   version: '1.17'
   build: h0d3ecfb_2
   build_number: 2
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/libiconv-1.17-h0d3ecfb_2.conda
@@ -5863,16 +5863,16 @@
   license: LGPL-3.0-only
   license_family: LGPL
   size: 373442
   timestamp: 1712339833358
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/0e/f2/f864ed36a8a62c26b57c3e08d212bd8f3d12a3ca3ef64600be5452aa3c82/msgspec-0.18.6-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
-  sha256: e97dec6932ad5e3ee1e3c14718638ba333befc45e0661caa57033cd4cc489466
+  url: https://files.pythonhosted.org/packages/73/16/dfef780ced7d690dd5497846ed242ef3e27e319d59d1ddaae816a4f2c15e/msgspec-0.18.6-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: ad237100393f637b297926cae1868b0d500f764ccd2f0623a380e2bcfb2809ca
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -5902,16 +5902,16 @@
   - tomli-w ; extra == 'toml'
   - tomli ; python_version < '3.11' and extra == 'toml'
   - pyyaml ; extra == 'yaml'
   requires_python: '>=3.8'
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/1d/b5/c8fbf1db814eb29eda402952374b594b2559419ba7ec6d0997a9e5687530/msgspec-0.18.6-cp312-cp312-macosx_10_9_x86_64.whl
-  sha256: d86f5071fe33e19500920333c11e2267a31942d18fed4d9de5bc2fbab267d28c
+  url: https://files.pythonhosted.org/packages/cd/b2/283d010db6836db2fe059f7ee3c13823927229975ffbe1edcbeded85a556/msgspec-0.18.6-cp39-cp39-win_amd64.whl
+  sha256: b5c390b0b0b7da879520d4ae26044d74aeee5144f83087eb7842ba59c02bc090
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -5941,16 +5941,16 @@
   - tomli-w ; extra == 'toml'
   - tomli ; python_version < '3.11' and extra == 'toml'
   - pyyaml ; extra == 'yaml'
   requires_python: '>=3.8'
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/73/16/dfef780ced7d690dd5497846ed242ef3e27e319d59d1ddaae816a4f2c15e/msgspec-0.18.6-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: ad237100393f637b297926cae1868b0d500f764ccd2f0623a380e2bcfb2809ca
+  url: https://files.pythonhosted.org/packages/1d/b5/c8fbf1db814eb29eda402952374b594b2559419ba7ec6d0997a9e5687530/msgspec-0.18.6-cp312-cp312-macosx_10_9_x86_64.whl
+  sha256: d86f5071fe33e19500920333c11e2267a31942d18fed4d9de5bc2fbab267d28c
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -6019,16 +6019,16 @@
   - tomli-w ; extra == 'toml'
   - tomli ; python_version < '3.11' and extra == 'toml'
   - pyyaml ; extra == 'yaml'
   requires_python: '>=3.8'
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/cd/b2/283d010db6836db2fe059f7ee3c13823927229975ffbe1edcbeded85a556/msgspec-0.18.6-cp39-cp39-win_amd64.whl
-  sha256: b5c390b0b0b7da879520d4ae26044d74aeee5144f83087eb7842ba59c02bc090
+  url: https://files.pythonhosted.org/packages/0e/f2/f864ed36a8a62c26b57c3e08d212bd8f3d12a3ca3ef64600be5452aa3c82/msgspec-0.18.6-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
+  sha256: e97dec6932ad5e3ee1e3c14718638ba333befc45e0661caa57033cd4cc489466
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -6350,17 +6350,17 @@
   - libzlib >=1.2.13,<1.3.0a0
   license: BSD-3-Clause
   license_family: BSD
   size: 944649
   timestamp: 1698610795381
 - kind: pypi
   name: pixi-kernel
-  version: 0.2.0
+  version: 0.2.1
   path: ../../../../pixi-kernel
-  sha256: d505b18617c43a2be12c4af779636bca35effc06c2b873b9584f4193c0933f2e
+  sha256: fc89be37749334e0eb20e8656e5ffcdace662e69fd273fa798213fdf1e64b7cb
   requires_dist:
   - jupyter-client >=7
   - msgspec >=0.18
   requires_python: <4.0,>=3.8
   editable: true
 - kind: conda
   name: pixman
@@ -6622,40 +6622,40 @@
   name: pywin32
   version: '306'
   url: https://files.pythonhosted.org/packages/1c/f7/24d8ed4fd9c43b90354df7764f81f0dd5e623f9a50f1538f90fe085d6dff/pywin32-306-cp39-cp39-win_amd64.whl
   sha256: 39b61c15272833b5c329a2989999dcae836b1eed650252ab1b7bfbe1d59f30f4
 - kind: pypi
   name: pyzmq
   version: 25.1.2
-  url: https://files.pythonhosted.org/packages/72/55/cc3163e20f40615a49245fa7041badec6103e8ee7e482dbb0feea00a7b84/pyzmq-25.1.2-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
-  sha256: 1b3cbba2f47062b85fe0ef9de5b987612140a9ba3a9c6d2543c6dec9f7c2ab27
+  url: https://files.pythonhosted.org/packages/93/b7/6e291eafbbbc66d0e87658dd21383ec2b4ab35edcfb283902c580a6db76f/pyzmq-25.1.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: 02c9087b109070c5ab0b383079fa1b5f797f8d43e9a66c07a4b8b8bdecfd88ee
   requires_dist:
   - cffi ; implementation_name == 'pypy'
   requires_python: '>=3.6'
 - kind: pypi
   name: pyzmq
   version: 25.1.2
-  url: https://files.pythonhosted.org/packages/6e/f0/d71cf69dc039c9adc8b625efc3bad3684f3660a570e47f0f0c64df787b41/pyzmq-25.1.2-cp312-cp312-macosx_10_15_universal2.whl
-  sha256: 11e70516688190e9c2db14fcf93c04192b02d457b582a1f6190b154691b4c93a
+  url: https://files.pythonhosted.org/packages/11/ae/d573f1c3854fff3714fe3cbf8ed3ce4200cc2aa81ab159dfe74b660d6523/pyzmq-25.1.2-cp39-cp39-win_amd64.whl
+  sha256: 8e9f3fabc445d0ce320ea2c59a75fe3ea591fdbdeebec5db6de530dd4b09412e
   requires_dist:
   - cffi ; implementation_name == 'pypy'
   requires_python: '>=3.6'
 - kind: pypi
   name: pyzmq
   version: 25.1.2
-  url: https://files.pythonhosted.org/packages/93/b7/6e291eafbbbc66d0e87658dd21383ec2b4ab35edcfb283902c580a6db76f/pyzmq-25.1.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: 02c9087b109070c5ab0b383079fa1b5f797f8d43e9a66c07a4b8b8bdecfd88ee
+  url: https://files.pythonhosted.org/packages/6e/f0/d71cf69dc039c9adc8b625efc3bad3684f3660a570e47f0f0c64df787b41/pyzmq-25.1.2-cp312-cp312-macosx_10_15_universal2.whl
+  sha256: 11e70516688190e9c2db14fcf93c04192b02d457b582a1f6190b154691b4c93a
   requires_dist:
   - cffi ; implementation_name == 'pypy'
   requires_python: '>=3.6'
 - kind: pypi
   name: pyzmq
   version: 25.1.2
-  url: https://files.pythonhosted.org/packages/11/ae/d573f1c3854fff3714fe3cbf8ed3ce4200cc2aa81ab159dfe74b660d6523/pyzmq-25.1.2-cp39-cp39-win_amd64.whl
-  sha256: 8e9f3fabc445d0ce320ea2c59a75fe3ea591fdbdeebec5db6de530dd4b09412e
+  url: https://files.pythonhosted.org/packages/72/55/cc3163e20f40615a49245fa7041badec6103e8ee7e482dbb0feea00a7b84/pyzmq-25.1.2-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
+  sha256: 1b3cbba2f47062b85fe0ef9de5b987612140a9ba3a9c6d2543c6dec9f7c2ab27
   requires_dist:
   - cffi ; implementation_name == 'pypy'
   requires_python: '>=3.6'
 - kind: conda
   name: r-base
   version: 4.1.3
   build: hdca333a_12
@@ -8348,40 +8348,40 @@
   requires_dist:
   - attrs >=22.2.0
   - rpds-py >=0.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/5a/57/2fcfd462cc53876ac4acef69dbf4fb941da971440049ca72051da54ea60d/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
-  sha256: cd5bf1af8efe569654bbef5a3e0a56eca45f87cfcffab31dd8dde70da5982475
+  url: https://files.pythonhosted.org/packages/c3/96/2211a1ca4b4e259e222169074ec0fa41f0ee18665dfc68988a139dc7e6e8/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: 4457a94da0d5c53dc4b3e4de1158bdab077db23c53232f37a3cb7afdb053a4e3
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/09/b6/45690f5d3f8c551bb462e063a2f336d72c8884ed26aa19beb53a374d3854/rpds_py-0.18.0-cp312-cp312-macosx_10_12_x86_64.whl
-  sha256: 7f2facbd386dd60cbbf1a794181e6aa0bd429bd78bfdf775436020172e2a23f0
+  url: https://files.pythonhosted.org/packages/a0/62/c896cec9434e09fb933f3cadd5c699e9cea49ab8934d694b6634650748db/rpds_py-0.18.0-cp39-none-win_amd64.whl
+  sha256: 6ef687afab047554a2d366e112dd187b62d261d49eb79b77e386f94644363294
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/c3/96/2211a1ca4b4e259e222169074ec0fa41f0ee18665dfc68988a139dc7e6e8/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: 4457a94da0d5c53dc4b3e4de1158bdab077db23c53232f37a3cb7afdb053a4e3
+  url: https://files.pythonhosted.org/packages/09/b6/45690f5d3f8c551bb462e063a2f336d72c8884ed26aa19beb53a374d3854/rpds_py-0.18.0-cp312-cp312-macosx_10_12_x86_64.whl
+  sha256: 7f2facbd386dd60cbbf1a794181e6aa0bd429bd78bfdf775436020172e2a23f0
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
   url: https://files.pythonhosted.org/packages/7a/58/9bfc53b266df92f0515e72fd16e4890dc6b56fc3bfc216b3a2a729c866b5/rpds_py-0.18.0-cp312-cp312-macosx_11_0_arm64.whl
   sha256: 1d9a5be316c15ffb2b3c405c4ff14448c36b4435be062a7f578ccd8b01f0c4d8
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/a0/62/c896cec9434e09fb933f3cadd5c699e9cea49ab8934d694b6634650748db/rpds_py-0.18.0-cp39-none-win_amd64.whl
-  sha256: 6ef687afab047554a2d366e112dd187b62d261d49eb79b77e386f94644363294
+  url: https://files.pythonhosted.org/packages/5a/57/2fcfd462cc53876ac4acef69dbf4fb941da971440049ca72051da54ea60d/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
+  sha256: cd5bf1af8efe569654bbef5a3e0a56eca45f87cfcffab31dd8dde70da5982475
   requires_python: '>=3.8'
 - kind: conda
   name: sed
   version: '4.8'
   build: ha0d5d3d_0
   subdir: linux-aarch64
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/sed-4.8-ha0d5d3d_0.tar.bz2
@@ -8514,30 +8514,28 @@
   - libcxx >=11.0.0.a0
   license: NCSA
   license_family: MIT
   size: 191416
   timestamp: 1602687595316
 - kind: conda
   name: tbb
-  version: 2021.11.0
-  build: h91493d7_1
-  build_number: 1
+  version: 2021.12.0
+  build: h91493d7_0
   subdir: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/tbb-2021.11.0-h91493d7_1.conda
-  sha256: aa30c089fdd6f66c7808592362e29963586e094159964a5fb61fb8efa9e349bc
-  md5: 21069f3ed16812f9f4f2700667b6ec86
+  url: https://conda.anaconda.org/conda-forge/win-64/tbb-2021.12.0-h91493d7_0.conda
+  sha256: 621926aae93513408bdca3dd21c97e2aa8ba7dcd2c400dab804fb0ce7da1387b
+  md5: 21745fdd12f01b41178596143cbecffd
   depends:
-  - libhwloc >=2.9.3,<2.9.4.0a0
+  - libhwloc >=2.10.0,<2.10.1.0a0
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: Apache-2.0
-  license_family: APACHE
-  size: 161382
-  timestamp: 1706164225098
+  size: 161618
+  timestamp: 1712960215111
 - kind: conda
   name: tk
   version: 8.6.13
   build: h194ca79_0
   subdir: linux-aarch64
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/tk-8.6.13-h194ca79_0.conda
   sha256: 7fa27cc512d3a783f38bd16bbbffc008807372499d5b65d089a8e43bde9db267
@@ -8652,40 +8650,40 @@
   - tk >=8.6.13,<8.7.0a0
   license: TCL
   size: 79797
   timestamp: 1695716570153
 - kind: pypi
   name: tornado
   version: '6.4'
-  url: https://files.pythonhosted.org/packages/62/e5/3ee2ba523a13bae5c17d1658580d13597116c1639374ca5033d58fd04724/tornado-6.4-cp38-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
-  sha256: f7894c581ecdcf91666a0912f18ce5e757213999e183ebfc2c3fdbf4d5bd764e
+  url: https://files.pythonhosted.org/packages/9f/12/11d0a757bb67278d3380d41955ae98527d5ad18330b2edbdc8de222b569b/tornado-6.4-cp38-abi3-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: f0251554cdd50b4b44362f73ad5ba7126fc5b2c2895cc62b14a1c2d7ea32f212
   requires_python: '>=3.8'
 - kind: pypi
   name: tornado
   version: '6.4'
-  url: https://files.pythonhosted.org/packages/34/7a/e7ec972db24513ea69ac7132c1a5eef62309dc978566a4afffa314417a45/tornado-6.4-cp38-abi3-macosx_10_9_x86_64.whl
-  sha256: 27787de946a9cffd63ce5814c33f734c627a87072ec7eed71f7fc4417bb16263
+  url: https://files.pythonhosted.org/packages/af/2b/4649926f17c1634d21c584cc855b5c5021f148b934919d26932a595bc034/tornado-6.4-cp38-abi3-win_amd64.whl
+  sha256: 10aeaa8006333433da48dec9fe417877f8bcc21f48dda8d661ae79da357b2a63
   requires_python: '>=3.8'
 - kind: pypi
   name: tornado
   version: '6.4'
-  url: https://files.pythonhosted.org/packages/9f/12/11d0a757bb67278d3380d41955ae98527d5ad18330b2edbdc8de222b569b/tornado-6.4-cp38-abi3-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: f0251554cdd50b4b44362f73ad5ba7126fc5b2c2895cc62b14a1c2d7ea32f212
+  url: https://files.pythonhosted.org/packages/34/7a/e7ec972db24513ea69ac7132c1a5eef62309dc978566a4afffa314417a45/tornado-6.4-cp38-abi3-macosx_10_9_x86_64.whl
+  sha256: 27787de946a9cffd63ce5814c33f734c627a87072ec7eed71f7fc4417bb16263
   requires_python: '>=3.8'
 - kind: pypi
   name: tornado
   version: '6.4'
   url: https://files.pythonhosted.org/packages/4a/2e/3ba930e3af171847d610e07ae878e04fcb7e4d7822f1a2d29a27b128ea24/tornado-6.4-cp38-abi3-macosx_10_9_universal2.whl
   sha256: 02ccefc7d8211e5a7f9e8bc3f9e5b0ad6262ba2fbb683a6443ecc804e5224ce0
   requires_python: '>=3.8'
 - kind: pypi
   name: tornado
   version: '6.4'
-  url: https://files.pythonhosted.org/packages/af/2b/4649926f17c1634d21c584cc855b5c5021f148b934919d26932a595bc034/tornado-6.4-cp38-abi3-win_amd64.whl
-  sha256: 10aeaa8006333433da48dec9fe417877f8bcc21f48dda8d661ae79da357b2a63
+  url: https://files.pythonhosted.org/packages/62/e5/3ee2ba523a13bae5c17d1658580d13597116c1639374ca5033d58fd04724/tornado-6.4-cp38-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
+  sha256: f7894c581ecdcf91666a0912f18ce5e757213999e183ebfc2c3fdbf4d5bd764e
   requires_python: '>=3.8'
 - kind: pypi
   name: traitlets
   version: 5.14.2
   url: https://files.pythonhosted.org/packages/7c/c4/366a09036c07f46eb8c9b2af39c97f502ef24f11f2a6e4d763655d9f2708/traitlets-5.14.2-py3-none-any.whl
   sha256: fcdf85684a772ddeba87db2f398ce00b40ff550d1528c03c14dbf6a02003cd80
   requires_dist:
```

### Comparing `pixi_kernel-0.2.0/tests/integration/xeus-cling/kernel.py` & `pixi_kernel-0.2.1/tests/integration/xeus-cling/kernel.py`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/tests/integration/xeus-cling/pixi.lock` & `pixi_kernel-0.2.1/tests/integration/xeus-cling/pixi.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1548,17 +1548,17 @@
   - pyopenssl >=22.1
   license: Apache-2.0
   license_family: Apache
   size: 2865379
   timestamp: 1710793235846
 - kind: pypi
   name: pixi-kernel
-  version: 0.2.0
+  version: 0.2.1
   path: ../../../../pixi-kernel
-  sha256: d505b18617c43a2be12c4af779636bca35effc06c2b873b9584f4193c0933f2e
+  sha256: fc89be37749334e0eb20e8656e5ffcdace662e69fd273fa798213fdf1e64b7cb
   requires_dist:
   - jupyter-client >=7
   - msgspec >=0.18
   requires_python: <4.0,>=3.8
   editable: true
 - kind: pypi
   name: platformdirs
```

### Comparing `pixi_kernel-0.2.0/tests/unit/conftest.py` & `pixi_kernel-0.2.1/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/tests/unit/test_pixi.py` & `pixi_kernel-0.2.1/tests/unit/test_pixi.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,22 +115,22 @@
 
     result = find_project_manifest(
         cwd=cwd,
         package_name=package_name,
         kernel_display_name=kernel_display_name,
         logger=logger,
     )
-    assert result == str((cwd / "pixi.toml").resolve())
+    assert result == (cwd / "pixi.toml").resolve()
 
 
 def test_pyproject_project():
     cwd = data_dir / "pyproject_project"
     package_name = "ipykernel"
     kernel_display_name = "Pixi - Python 3 (ipykernel)"
 
     result = find_project_manifest(
         cwd=cwd,
         package_name=package_name,
         kernel_display_name=kernel_display_name,
         logger=logger,
     )
-    assert result == str((cwd / "pyproject.toml").resolve())
+    assert result == (cwd / "pyproject.toml").resolve()
```

### Comparing `pixi_kernel-0.2.0/LICENSE` & `pixi_kernel-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/README.md` & `pixi_kernel-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.0/pyproject.toml` & `pixi_kernel-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "pixi-kernel"
-version = "0.2.0"
-description = "Python Jupyter kernel using Pixi for reproducible notebooks"
+version = "0.2.1"
+description = "Jupyter kernels using Pixi for reproducible notebooks"
 license = { text = "MIT" }
 authors = [
     { name = "Renan Rodrigues dos Santos", email = "renan.engmec@gmail.com" },
 ]
 
 readme = "README.md"
 keywords = ["kernel", "jupyter", "pixi"]
@@ -68,16 +68,13 @@
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.paths]
 source = ["src/", ".pixi/envs/**/lib/python*/site-packages/"]
 
-[tool.coverage.report]
-fail_under = 65
-
 [tool.hatch.build.targets.wheel.shared-data]
 "kernels" = "share/jupyter/kernels"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

### Comparing `pixi_kernel-0.2.0/PKG-INFO` & `pixi_kernel-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.3
 Name: pixi-kernel
-Version: 0.2.0
-Summary: Python Jupyter kernel using Pixi for reproducible notebooks
+Version: 0.2.1
+Summary: Jupyter kernels using Pixi for reproducible notebooks
 Project-URL: Documentation, https://github.com/renan-r-santos/pixi-kernel
 Project-URL: Homepage, https://github.com/renan-r-santos/pixi-kernel
 Project-URL: Repository, https://github.com/renan-r-santos/pixi-kernel
 Author-email: Renan Rodrigues dos Santos <renan.engmec@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: jupyter,kernel,pixi
```


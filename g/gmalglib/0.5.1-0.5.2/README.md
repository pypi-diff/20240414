# Comparing `tmp/gmalglib-0.5.1.tar.gz` & `tmp/gmalglib-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmalglib-0.5.1.tar", last modified: Sun Apr 14 09:56:57 2024, max compression
+gzip compressed data, was "gmalglib-0.5.2.tar", last modified: Sun Apr 14 11:50:49 2024, max compression
```

## Comparing `gmalglib-0.5.1.tar` & `gmalglib-0.5.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:57.068384 gmalglib-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-14 09:56:49.000000 gmalglib-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-14 09:56:57.068384 gmalglib-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-14 09:56:49.000000 gmalglib-0.5.1/README.en.md
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-14 09:56:49.000000 gmalglib-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:57.060384 gmalglib-0.5.1/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:57.064384 gmalglib-0.5.1/include/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-14 09:56:49.000000 gmalglib-0.5.1/include/gmalglib/bignum.h
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-14 09:56:49.000000 gmalglib-0.5.1/include/gmalglib/random.h
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-14 09:56:49.000000 gmalglib-0.5.1/include/gmalglib/sm2.h
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-14 09:56:49.000000 gmalglib-0.5.1/include/gmalglib/sm2curve.h
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-14 09:56:49.000000 gmalglib-0.5.1/include/gmalglib/sm3.h
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-14 09:56:49.000000 gmalglib-0.5.1/include/gmalglib/sm4.h
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-14 09:56:49.000000 gmalglib-0.5.1/include/gmalglib/zuc.h
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-14 09:56:49.000000 gmalglib-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 09:56:57.068384 gmalglib-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-14 09:56:49.000000 gmalglib-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:57.060384 gmalglib-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:57.068384 gmalglib-0.5.1/src/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:57.068384 gmalglib-0.5.1/src/gmalglib/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/core/bignum.c
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/core/random.c
--rw-r--r--   0 runner    (1001) docker     (127)    17508 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/core/sm2.c
--rw-r--r--   0 runner    (1001) docker     (127)    18937 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/core/sm2curve.c
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/core/sm3.c
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/core/sm4.c
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/core/zuc.c
--rw-r--r--   0 runner    (1001) docker     (127)    33914 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/coremodule.c
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/sm2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/sm2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/sm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/sm3.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/sm4.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/sm4.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/wrapped.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/zuc.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/zuc.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:57.068384 gmalglib-0.5.1/src/gmalglib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-14 09:56:57.000000 gmalglib-0.5.1/src/gmalglib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-14 09:56:57.000000 gmalglib-0.5.1/src/gmalglib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 09:56:57.000000 gmalglib-0.5.1/src/gmalglib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 09:56:57.000000 gmalglib-0.5.1/src/gmalglib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:50:49.051865 gmalglib-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-14 11:50:40.000000 gmalglib-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-14 11:50:49.047865 gmalglib-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-14 11:50:40.000000 gmalglib-0.5.2/README.en.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-14 11:50:40.000000 gmalglib-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:50:49.043865 gmalglib-0.5.2/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:50:49.043865 gmalglib-0.5.2/include/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-14 11:50:40.000000 gmalglib-0.5.2/include/gmalglib/bignum.h
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-14 11:50:40.000000 gmalglib-0.5.2/include/gmalglib/random.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-14 11:50:40.000000 gmalglib-0.5.2/include/gmalglib/sm2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-14 11:50:40.000000 gmalglib-0.5.2/include/gmalglib/sm2curve.h
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-14 11:50:40.000000 gmalglib-0.5.2/include/gmalglib/sm3.h
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-14 11:50:40.000000 gmalglib-0.5.2/include/gmalglib/sm4.h
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-14 11:50:40.000000 gmalglib-0.5.2/include/gmalglib/zuc.h
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-14 11:50:40.000000 gmalglib-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 11:50:49.051865 gmalglib-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-14 11:50:40.000000 gmalglib-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:50:49.043865 gmalglib-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:50:49.047865 gmalglib-0.5.2/src/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:50:49.047865 gmalglib-0.5.2/src/gmalglib/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/core/bignum.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/core/random.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18369 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/core/sm2.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18937 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/core/sm2curve.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/core/sm3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/core/sm4.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/core/zuc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    36380 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/coremodule.c
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/sm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/sm2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/sm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/sm3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/sm4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/sm4.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/wrapped.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/zuc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/zuc.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:50:49.047865 gmalglib-0.5.2/src/gmalglib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-14 11:50:49.000000 gmalglib-0.5.2/src/gmalglib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-14 11:50:49.000000 gmalglib-0.5.2/src/gmalglib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 11:50:49.000000 gmalglib-0.5.2/src/gmalglib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 11:50:49.000000 gmalglib-0.5.2/src/gmalglib.egg-info/top_level.txt
```

### Comparing `gmalglib-0.5.1/LICENSE` & `gmalglib-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.1/PKG-INFO` & `gmalglib-0.5.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python package implementing GM algorithms in C.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
@@ -15,25 +15,40 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gmalglib
 
 [![Unittest](https://github.com/ww-rm/gmalglib/actions/workflows/python-test.yml/badge.svg)](https://github.com/ww-rm/gmalglib/actions/workflows/python-test.yml)
 [![PyPI](https://github.com/ww-rm/gmalglib/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ww-rm/gmalglib/actions/workflows/python-publish.yml)
+[![docs](https://readthedocs.org/projects/gmalglib/badge/?version=latest)](https://gmalglib.readthedocs.io/zh-cn/latest/?badge=latest)
 
 Python extension library for GM (GuoMi) cryptographic algorithms, providing a set of fundamental cryptographic algorithms.
 
 Implemented in C language, encapsulated based on the native CPython interface, without dependencies on any third-party libraries.
 
 ## Installation
 
-```bat
+### Windows
+
+For `python3.8` and higher versions, you can directly install using `pip`.
+
+```bash
 pip install gmalglib
 ```
 
+Alternatively, refer to the source code installation for other platforms.
+
+### Other Platforms
+
+Visit the PyPI project file list [Download files](https://pypi.org/project/gmalglib/#files) page to download the source distribution package `gmalglib-x.y.z.tar.gz`, then proceed with the source code installation.
+
+```bash
+pip install gmalglib-x.y.z.tar.gz
+```
+
 ## Core Algorithms Implemented
 
 - SM2 Public Key Cryptograhpic Algorithm Based on Elliptic Curves
   - Sign/Verify
   - Encrypt/Decrypt
 - SM3 Cryptogrpahic Hash Algorithm
 - SM4 Block Cipher Algorithm
@@ -64,10 +79,10 @@
 
 For all sections involving random number generators, custom parameters for random number generation are provided, implemented in the form of callback functions. The function type is `Callable[[int], bytes]`, meaning it generates a byte string of a specified length.
 
 ```python
 def rnd_fn(n: int) -> bytes: ...
 ```
 
-If no random number generator is passed, the default system-related random number generator is used. On Windows, it utilizes `BCryptGenRandom`, while other systems use `/dev/urandom` for implementation, which is similar to the Python standard library function `os.urandom`.
+If no random number generator is passed, the default system-related random number generator is used. On Windows, it utilizes `BCryptGenRandom`, while other systems use `/dev/urandom` for implementation, which is similar to the Python standard library function [`os.urandom`](https://docs.python.org/3/library/os.html#os.urandom).
 
 For specific implementation details, refer to [random.c](https://github.com/ww-rm/gmalglib/blob/main/src/gmalglib/core/random.c) under the `OsRandomProc` function.
```

### Comparing `gmalglib-0.5.1/README.en.md` & `gmalglib-0.5.2/README.en.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 # gmalglib
 
 [![Unittest](https://github.com/ww-rm/gmalglib/actions/workflows/python-test.yml/badge.svg)](https://github.com/ww-rm/gmalglib/actions/workflows/python-test.yml)
 [![PyPI](https://github.com/ww-rm/gmalglib/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ww-rm/gmalglib/actions/workflows/python-publish.yml)
+[![docs](https://readthedocs.org/projects/gmalglib/badge/?version=latest)](https://gmalglib.readthedocs.io/zh-cn/latest/?badge=latest)
 
 Python extension library for GM (GuoMi) cryptographic algorithms, providing a set of fundamental cryptographic algorithms.
 
 Implemented in C language, encapsulated based on the native CPython interface, without dependencies on any third-party libraries.
 
 ## Installation
 
-```bat
+### Windows
+
+For `python3.8` and higher versions, you can directly install using `pip`.
+
+```bash
 pip install gmalglib
 ```
 
+Alternatively, refer to the source code installation for other platforms.
+
+### Other Platforms
+
+Visit the PyPI project file list [Download files](https://pypi.org/project/gmalglib/#files) page to download the source distribution package `gmalglib-x.y.z.tar.gz`, then proceed with the source code installation.
+
+```bash
+pip install gmalglib-x.y.z.tar.gz
+```
+
 ## Core Algorithms Implemented
 
 - SM2 Public Key Cryptograhpic Algorithm Based on Elliptic Curves
   - Sign/Verify
   - Encrypt/Decrypt
 - SM3 Cryptogrpahic Hash Algorithm
 - SM4 Block Cipher Algorithm
@@ -47,10 +62,10 @@
 
 For all sections involving random number generators, custom parameters for random number generation are provided, implemented in the form of callback functions. The function type is `Callable[[int], bytes]`, meaning it generates a byte string of a specified length.
 
 ```python
 def rnd_fn(n: int) -> bytes: ...
 ```
 
-If no random number generator is passed, the default system-related random number generator is used. On Windows, it utilizes `BCryptGenRandom`, while other systems use `/dev/urandom` for implementation, which is similar to the Python standard library function `os.urandom`.
+If no random number generator is passed, the default system-related random number generator is used. On Windows, it utilizes `BCryptGenRandom`, while other systems use `/dev/urandom` for implementation, which is similar to the Python standard library function [`os.urandom`](https://docs.python.org/3/library/os.html#os.urandom).
 
 For specific implementation details, refer to [random.c](https://github.com/ww-rm/gmalglib/blob/main/src/gmalglib/core/random.c) under the `OsRandomProc` function.
```

### Comparing `gmalglib-0.5.1/README.md` & `gmalglib-0.5.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 # gmalglib
 
 [![Unittest](https://github.com/ww-rm/gmalglib/actions/workflows/python-test.yml/badge.svg)](https://github.com/ww-rm/gmalglib/actions/workflows/python-test.yml)
 [![PyPI](https://github.com/ww-rm/gmalglib/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ww-rm/gmalglib/actions/workflows/python-publish.yml)
+[![docs](https://readthedocs.org/projects/gmalglib/badge/?version=latest)](https://gmalglib.readthedocs.io/zh-cn/latest/?badge=latest)
 
 国密算法的 Python 扩展库, 提供一些原始基础算法.
 
 使用 C 语言实现, 基于原生 CPython 接口进行封装, 不依赖其他任何第三方库.
 
 ## 安装
 
-```bat
+### Windows
+
+对于 `python3.8` 及以上, 可以直接使用 `pip` 进行安装.
+
+```bash
 pip install gmalglib
 ```
 
+或者参考其他平台使用源码安装.
+
+### 其他平台
+
+前往 PyPI 项目文件列表 [Download files](https://pypi.org/project/gmalglib/#files) 页面下载源码发布包 `gmalglib-x.y.z.tar.gz`, 之后使用源码安装.
+
+```bash
+pip install gmalglib-x.y.z.tar.gz
+```
+
 ## 已实现的核心算法
 
 - SM3 密码杂凑算法
     - 消息摘要
     - 密钥派生
     - 消息认证
 - SM4 分组密码算法
@@ -50,10 +65,10 @@
 
 所有涉及随机数发生器的部分, 均提供了自定义随机数发生器的参数, 以回调函数方式实现, 函数类型为 `Callable[[int], bytes]`, 即生成指定长度的随机字节串.
 
 ```python
 def rnd_fn(n: int) -> bytes: ...
 ```
 
-如不传入随机数发生器, 则使用默认的系统相关随机数发生器, 在 Windows 下使用 `BCryptGenRandom`, 其余系统使用 `/dev/urandom` 实现, 其实现类似于 Python 标准库函数 `os.urandom`.
+如不传入随机数发生器, 则使用默认的系统相关随机数发生器, 在 Windows 下使用 `BCryptGenRandom`, 其余系统使用 `/dev/urandom` 实现, 其实现类似于 Python 标准库函数 [`os.urandom`](https://docs.python.org/3/library/os.html#os.urandom).
 
 具体实现见 [random.c](https://github.com/ww-rm/gmalglib/blob/main/src/gmalglib/core/random.c) 内 `OsRandomProc`.
```

### Comparing `gmalglib-0.5.1/include/gmalglib/bignum.h` & `gmalglib-0.5.2/include/gmalglib/bignum.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.1/include/gmalglib/random.h` & `gmalglib-0.5.2/include/gmalglib/random.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.1/include/gmalglib/sm2.h` & `gmalglib-0.5.2/include/gmalglib/sm2.h`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,17 @@
 extern "C" {
 #endif
 
 extern const uint8_t* const SM2_DEFAULT_UID;
 
 int SM2_IsSkValid(const uint8_t* sk);
 int SM2_IsPkValid(const uint8_t* pk, uint64_t pk_len);
-int SM2_GetPk(const uint8_t* sk, uint8_t* pk, int pc_mode);
+int SM2_IsKeyPair(const uint8_t* sk, const uint8_t* pk, uint64_t pk_len);
+int SM2_GetPk(const uint8_t* sk, int pc_mode, uint8_t* pk);
+int SM2_ConvertPk(const uint8_t* pk, uint64_t pk_len, int pc_mode, uint8_t* pk_converted);
 
 int SM2_Init(SM2* self, const uint8_t* sk, const uint8_t* pk, uint64_t pk_len, const uint8_t* uid, uint64_t uid_len, int pc_mode, RandomAlg* rand_alg);
 int SM2_GenerateKeyPair(SM2* self, uint8_t* sk, uint8_t* pk);
 int SM2_GetEntityInfo(SM2* self, uint8_t* entity_info);
 int SM2_SignDigest(SM2* self, const uint8_t* digest, uint8_t* signature);
 int SM2_VerifyDigest(SM2* self, const uint8_t* digest, const uint8_t* signature);
 int SM2_Sign(SM2* self, const uint8_t* msg, uint64_t msg_len, uint8_t* signature);
```

### Comparing `gmalglib-0.5.1/include/gmalglib/sm2curve.h` & `gmalglib-0.5.2/include/gmalglib/sm2curve.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.1/include/gmalglib/sm3.h` & `gmalglib-0.5.2/include/gmalglib/sm3.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.1/pyproject.toml` & `gmalglib-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.1/setup.py` & `gmalglib-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.1/src/gmalglib/core/bignum.c` & `gmalglib-0.5.2/src/gmalglib/core/bignum.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.1/src/gmalglib/core/random.c` & `gmalglib-0.5.2/src/gmalglib/core/random.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.1/src/gmalglib/core/sm2.c` & `gmalglib-0.5.2/src/gmalglib/core/sm2.c`

 * *Files 3% similar despite different names*

```diff
@@ -176,15 +176,33 @@
 
 int SM2_IsPkValid(const uint8_t* pk, uint64_t pk_len)
 {
     SM2JacobPointMont P = { 0 };
     return pk_len > 1 && SM2JacobPointMont_FromBytes(pk, pk_len, &P) == 0;
 }
 
-int SM2_GetPk(const uint8_t* sk, uint8_t* pk, int pc_mode)
+int SM2_IsKeyPair(const uint8_t* sk, const uint8_t* pk, uint64_t pk_len)
+{
+    SM2ModN sk_num = { 0 };
+    SM2JacobPointMont P = { 0 };
+    SM2JacobPointMont skG = { 0 };
+
+    UInt256_FromBytes(sk, &sk_num);
+    if (!_SM2_IsSkValid(&sk_num))
+        return 0;
+
+    if (pk_len <= 1 || SM2JacobPointMont_FromBytes(pk, pk_len, &P) != 0)
+        return 0;
+
+    SM2JacobPointMont_MulG(&sk_num, &skG);
+
+    return SM2JacobPointMont_IsEqual(&P, &skG);
+}
+
+int SM2_GetPk(const uint8_t* sk, int pc_mode, uint8_t* pk)
 {
     SM2ModN sk_num = { 0 };
     SM2JacobPointMont P = { 0 };
     UInt256_FromBytes(sk, &sk_num);
 
     if (!_SM2_IsSkValid(&sk_num))
         return SM2_ERR_INVALID_SK;
@@ -194,14 +212,27 @@
     if (pc_mode != SM2_PCMODE_COMPRESS && pc_mode != SM2_PCMODE_MIX)
         pc_mode = SM2_PCMODE_RAW;
 
     SM2JacobPointMont_ToBytes(&P, pc_mode, pk);
     return 0;
 }
 
+int SM2_ConvertPk(const uint8_t* pk, uint64_t pk_len, int pc_mode, uint8_t* pk_converted)
+{
+    SM2JacobPointMont P = { 0 };
+    if (pk_len <= 1 || SM2JacobPointMont_FromBytes(pk, pk_len, &P) != 0)
+        return SM2_ERR_INVALID_PK;
+
+    if (pc_mode != SM2_PCMODE_COMPRESS && pc_mode != SM2_PCMODE_MIX)
+        pc_mode = SM2_PCMODE_RAW;
+
+    SM2JacobPointMont_ToBytes(&P, pc_mode, pk_converted);
+    return 0;
+}
+
 static
 void _SM2_GetEntityInfo(const SM2JacobPointMont* pk, const uint8_t* uid, uint64_t uid_len, uint8_t* entity_info)
 {
     SM2Point P = { 0 };
     uint8_t buffer[SM2_PARAMS_LENGTH] = { 0 };
     SM3 sm3 = { 0 };
```

### Comparing `gmalglib-0.5.1/src/gmalglib/core/sm2curve.c` & `gmalglib-0.5.2/src/gmalglib/core/sm2curve.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.1/src/gmalglib/core/sm3.c` & `gmalglib-0.5.2/src/gmalglib/core/sm3.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.1/src/gmalglib/core/sm4.c` & `gmalglib-0.5.2/src/gmalglib/core/sm4.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.1/src/gmalglib/core/zuc.c` & `gmalglib-0.5.2/src/gmalglib/core/zuc.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.1/src/gmalglib/coremodule.c` & `gmalglib-0.5.2/src/gmalglib/coremodule.c`

 * *Files 8% similar despite different names*

```diff
@@ -578,48 +578,117 @@
     PyBuffer_Release(&py_buffer_pk);
 
     if (is_valid)
         Py_RETURN_TRUE;
     Py_RETURN_FALSE;
 }
 
+static PyObject* PySM2_is_keypair(PySM2Object* self, PyObject* args, PyObject* kwargs)
+{
+    char* keys[] = { "sk", "pk", NULL };
+    Py_buffer py_buffer_sk = { 0 };
+    Py_buffer py_buffer_pk = { 0 };
+
+    int is_pair = 0;
+
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*y*:is_keypair", keys, &py_buffer_sk, &py_buffer_pk))
+        return NULL;
+
+    if (py_buffer_sk.len != SM2_SK_LENGTH)
+    {
+        PyErr_SetString(PyExc_ValueError, "Incorrect secret key length.");
+        PyBuffer_Release(&py_buffer_sk);
+        PyBuffer_Release(&py_buffer_pk);
+        return NULL;
+    }
+    if (py_buffer_pk.len != SM2_PK_HALF_LENGTH && py_buffer_pk.len != SM2_PK_FULL_LENGTH)
+    {
+        PyErr_SetString(PyExc_ValueError, "Incorrect public key length.");
+        PyBuffer_Release(&py_buffer_sk);
+        PyBuffer_Release(&py_buffer_pk);
+        return NULL;
+    }
+
+    is_pair = SM2_IsKeyPair(py_buffer_sk.buf, py_buffer_pk.buf, py_buffer_pk.len);
+    PyBuffer_Release(&py_buffer_sk);
+    PyBuffer_Release(&py_buffer_pk);
+
+    if (is_pair)
+        Py_RETURN_TRUE;
+    Py_RETURN_FALSE;
+}
+
 static PyObject* PySM2_get_pk(PySM2Object* self, PyObject* args, PyObject* kwargs)
 {
     char* keys[] = { "sk", "pc_mode", NULL};
     Py_buffer py_buffer_sk = { 0 };
     int pc_mode = 0;
     uint8_t pk[SM2_PK_FULL_LENGTH] = { 0 };
 
     int sm2_ret = 0;
 
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*|$i:get_pk", keys, &py_buffer_sk, &pc_mode))
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*|i:get_pk", keys, &py_buffer_sk, &pc_mode))
         return NULL;
 
     if (py_buffer_sk.len != SM2_SK_LENGTH)
     {
         PyErr_SetString(PyExc_ValueError, "Incorrect secret key length.");
         PyBuffer_Release(&py_buffer_sk);
         return NULL;
     }
 
     if (pc_mode != SM2_PCMODE_COMPRESS && pc_mode != SM2_PCMODE_MIX)
         pc_mode = SM2_PCMODE_RAW;
 
-    sm2_ret = SM2_GetPk(py_buffer_sk.buf, pk, pc_mode);
+    sm2_ret = SM2_GetPk(py_buffer_sk.buf, pc_mode, pk);
     PyBuffer_Release(&py_buffer_sk);
 
     if (sm2_ret != 0)
     {
         PyErr_SetString(PyExc_ValueError, "Invalid secret key.");
         return NULL;
     }
 
     return PyBytes_FromStringAndSize((char*)pk, SM2_GET_PK_LENGTH(pc_mode));
 }
 
+static PyObject* PySM2_convert_pk(PySM2Object* self, PyObject* args, PyObject* kwargs)
+{
+    char* keys[] = { "pk", "pc_mode", NULL };
+    Py_buffer py_buffer_pk = { 0 };
+    int pc_mode = 0;
+    uint8_t pk[SM2_PK_FULL_LENGTH] = { 0 };
+
+    int sm2_ret = 0;
+
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*|i:convert_pk", keys, &py_buffer_pk, &pc_mode))
+        return NULL;
+
+    if (py_buffer_pk.len != SM2_PK_HALF_LENGTH && py_buffer_pk.len != SM2_PK_FULL_LENGTH)
+    {
+        PyErr_SetString(PyExc_ValueError, "Incorrect public key length.");
+        PyBuffer_Release(&py_buffer_pk);
+        return NULL;
+    }
+
+    if (pc_mode != SM2_PCMODE_COMPRESS && pc_mode != SM2_PCMODE_MIX)
+        pc_mode = SM2_PCMODE_RAW;
+
+    sm2_ret = SM2_ConvertPk(py_buffer_pk.buf, py_buffer_pk.len, pc_mode, pk);
+    PyBuffer_Release(&py_buffer_pk);
+
+    if (sm2_ret != 0)
+    {
+        PyErr_SetString(PyExc_ValueError, "Invalid public key.");
+        return NULL;
+    }
+
+    return PyBytes_FromStringAndSize((char*)pk, SM2_GET_PK_LENGTH(pc_mode));
+}
+
 static PyObject* PySM2_generate_keypair(PySM2Object* self, PyObject* Py_UNUSED(args))
 {
     uint8_t sk[SM2_SK_LENGTH] = { 0 };
     uint8_t pk[SM2_PK_FULL_LENGTH] = { 0 };
 
     if (SM2_GenerateKeyPair(&self->sm2, sk, pk) == SM2_ERR_RANDOM_FAILED)
     {
@@ -857,15 +926,17 @@
     PyBuffer_Release(&py_buffer_cipher);
     return ret;
 }
 
 static PyMethodDef py_methods_def_SM2[] = {
     {"is_sk_valid",         (PyCFunction)PySM2_is_sk_valid,         METH_VARARGS | METH_KEYWORDS | METH_STATIC,     PyDoc_STR("Check sk is valid.")},
     {"is_pk_valid",         (PyCFunction)PySM2_is_pk_valid,         METH_VARARGS | METH_KEYWORDS | METH_STATIC,     PyDoc_STR("Check pk is valid.")},
+    {"is_keypair",          (PyCFunction)PySM2_is_keypair,          METH_VARARGS | METH_KEYWORDS | METH_STATIC,     PyDoc_STR("Check if a valid keypair.")},
     {"get_pk",              (PyCFunction)PySM2_get_pk,              METH_VARARGS | METH_KEYWORDS | METH_STATIC,     PyDoc_STR("Get public key bytes.")},
+    {"convert_pk",          (PyCFunction)PySM2_convert_pk,          METH_VARARGS | METH_KEYWORDS | METH_STATIC,     PyDoc_STR("Convert public key bytes to other pc_mode.")},
     {"generate_keypair",    (PyCFunction)PySM2_generate_keypair,    METH_NOARGS,                                    PyDoc_STR("Generate key pair.")},
     {"get_entity_info",     (PyCFunction)PySM2_get_entity_info,     METH_NOARGS,                                    PyDoc_STR("Get entity info.")},
     {"sign_digest",         (PyCFunction)PySM2_sign_digest,         METH_VARARGS | METH_KEYWORDS,                   PyDoc_STR("Sign on digest.")},
     {"verify_digest",       (PyCFunction)PySM2_verify_digest,       METH_VARARGS | METH_KEYWORDS,                   PyDoc_STR("Verify on digest.")},
     {"sign",                (PyCFunction)PySM2_sign,                METH_VARARGS | METH_KEYWORDS,                   PyDoc_STR("Sign on full message.")},
     {"verify",              (PyCFunction)PySM2_verify,              METH_VARARGS | METH_KEYWORDS,                   PyDoc_STR("Verify on full message.")},
     {"encrypt",             (PyCFunction)PySM2_encrypt,             METH_VARARGS | METH_KEYWORDS,                   PyDoc_STR("Encrypt data.")},
```

### Comparing `gmalglib-0.5.1/src/gmalglib/sm2.pyi` & `gmalglib-0.5.2/src/gmalglib/sm2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -70,15 +70,23 @@
         """测试私钥是否合法."""
 
     @staticmethod
     def is_pk_valid(pk: bytes) -> bool:
         """测试公钥是否合法."""
 
     @staticmethod
-    def get_pk(sk: bytes) -> bytes:
+    def is_keypair(sk: bytes, pk: bytes) -> bool:
+        """检查是否是合法密钥对."""
+
+    @staticmethod
+    def get_pk(sk: bytes, pc_mode: int = SM2_PCMODE_RAW) -> bytes:
+        """由私钥得到公钥."""
+
+    @staticmethod
+    def convert_pk(pk: bytes, pc_mode: int = SM2_PCMODE_RAW) -> bytes:
         """由私钥得到公钥."""
 
     def __init__(
         self,
         sk: Optional[bytes] = None,
         pk: Optional[bytes] = None,
         uid: bytes = SM2_DEFAULT_UID,
```

### Comparing `gmalglib-0.5.1/src/gmalglib/sm3.pyi` & `gmalglib-0.5.2/src/gmalglib/sm3.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.1/src/gmalglib/wrapped.py` & `gmalglib-0.5.2/src/gmalglib/wrapped.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,18 +61,30 @@
 
 def sm2_is_pk_valid(pk: bytes) -> bool:
     """测试公钥是否合法."""
 
     return __sm2.SM2.is_pk_valid(pk)
 
 
-def sm2_get_pk(sk: bytes) -> bytes:
+def sm2_is_keypair(sk: bytes, pk: bytes) -> bool:
+    """检查是否是合法密钥对."""
+
+    return __sm2.SM2.is_keypair(sk, pk)
+
+
+def sm2_get_pk(sk: bytes, pc_mode: __T.Literal["raw", "compress", "mix"] = "raw") -> bytes:
+    """由私钥得到公钥."""
+
+    return __sm2.SM2.get_pk(sk, __sm2_pcmode[pc_mode])
+
+
+def sm2_convert_pk(pk: bytes, pc_mode: __T.Literal["raw", "compress", "mix"] = "raw") -> bytes:
     """由私钥得到公钥."""
 
-    return __sm2.SM2.get_pk(sk)
+    return __sm2.SM2.convert_pk(pk, __sm2_pcmode[pc_mode])
 
 
 def sm2_generate_keypair(pc_mode: __T.Literal["raw", "compress", "mix"] = "raw") -> __T.Tuple[bytes, bytes]:
     """生成密钥对.
 
     Returns:
         sk: 私钥.
```

### Comparing `gmalglib-0.5.1/src/gmalglib/zuc.pyi` & `gmalglib-0.5.2/src/gmalglib/zuc.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.1/src/gmalglib.egg-info/PKG-INFO` & `gmalglib-0.5.2/src/gmalglib.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python package implementing GM algorithms in C.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
@@ -15,25 +15,40 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gmalglib
 
 [![Unittest](https://github.com/ww-rm/gmalglib/actions/workflows/python-test.yml/badge.svg)](https://github.com/ww-rm/gmalglib/actions/workflows/python-test.yml)
 [![PyPI](https://github.com/ww-rm/gmalglib/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ww-rm/gmalglib/actions/workflows/python-publish.yml)
+[![docs](https://readthedocs.org/projects/gmalglib/badge/?version=latest)](https://gmalglib.readthedocs.io/zh-cn/latest/?badge=latest)
 
 Python extension library for GM (GuoMi) cryptographic algorithms, providing a set of fundamental cryptographic algorithms.
 
 Implemented in C language, encapsulated based on the native CPython interface, without dependencies on any third-party libraries.
 
 ## Installation
 
-```bat
+### Windows
+
+For `python3.8` and higher versions, you can directly install using `pip`.
+
+```bash
 pip install gmalglib
 ```
 
+Alternatively, refer to the source code installation for other platforms.
+
+### Other Platforms
+
+Visit the PyPI project file list [Download files](https://pypi.org/project/gmalglib/#files) page to download the source distribution package `gmalglib-x.y.z.tar.gz`, then proceed with the source code installation.
+
+```bash
+pip install gmalglib-x.y.z.tar.gz
+```
+
 ## Core Algorithms Implemented
 
 - SM2 Public Key Cryptograhpic Algorithm Based on Elliptic Curves
   - Sign/Verify
   - Encrypt/Decrypt
 - SM3 Cryptogrpahic Hash Algorithm
 - SM4 Block Cipher Algorithm
@@ -64,10 +79,10 @@
 
 For all sections involving random number generators, custom parameters for random number generation are provided, implemented in the form of callback functions. The function type is `Callable[[int], bytes]`, meaning it generates a byte string of a specified length.
 
 ```python
 def rnd_fn(n: int) -> bytes: ...
 ```
 
-If no random number generator is passed, the default system-related random number generator is used. On Windows, it utilizes `BCryptGenRandom`, while other systems use `/dev/urandom` for implementation, which is similar to the Python standard library function `os.urandom`.
+If no random number generator is passed, the default system-related random number generator is used. On Windows, it utilizes `BCryptGenRandom`, while other systems use `/dev/urandom` for implementation, which is similar to the Python standard library function [`os.urandom`](https://docs.python.org/3/library/os.html#os.urandom).
 
 For specific implementation details, refer to [random.c](https://github.com/ww-rm/gmalglib/blob/main/src/gmalglib/core/random.c) under the `OsRandomProc` function.
```

### Comparing `gmalglib-0.5.1/src/gmalglib.egg-info/SOURCES.txt` & `gmalglib-0.5.2/src/gmalglib.egg-info/SOURCES.txt`

 * *Files identical despite different names*


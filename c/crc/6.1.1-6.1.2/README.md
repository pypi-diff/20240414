# Comparing `tmp/crc-6.1.1.tar.gz` & `tmp/crc-6.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crc-6.1.1.tar", max compression
+gzip compressed data, was "crc-6.1.2.tar", max compression
```

## Comparing `crc-6.1.1.tar` & `crc-6.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1305 2024-02-10 11:01:58.827363 crc-6.1.1/LICENSE.txt
--rw-r--r--   0        0        0     4471 2024-02-10 11:01:58.831363 crc-6.1.1/README.md
--rw-r--r--   0        0        0     1751 2024-02-10 11:01:58.831363 crc-6.1.1/pyproject.toml
--rw-r--r--   0        0        0      437 2024-02-10 11:01:58.831363 crc-6.1.1/src/crc/__init__.py
--rw-r--r--   0        0        0      208 2024-02-10 11:01:58.831363 crc-6.1.1/src/crc/__main__.py
--rw-r--r--   0        0        0    16905 2024-02-10 11:01:58.831363 crc-6.1.1/src/crc/_crc.py
--rw-r--r--   0        0        0        0 2024-02-10 11:01:58.831363 crc-6.1.1/src/crc/py.typed
--rw-r--r--   0        0        0     5435 1970-01-01 00:00:00.000000 crc-6.1.1/setup.py
--rw-r--r--   0        0        0     5564 1970-01-01 00:00:00.000000 crc-6.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1305 2024-04-14 09:08:43.976723 crc-6.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     4471 2024-04-14 09:08:43.976723 crc-6.1.2/README.md
+-rw-r--r--   0        0        0     1779 2024-04-14 09:08:43.980723 crc-6.1.2/pyproject.toml
+-rw-r--r--   0        0        0      437 2024-04-14 09:08:43.980723 crc-6.1.2/src/crc/__init__.py
+-rw-r--r--   0        0        0      208 2024-04-14 09:08:43.980723 crc-6.1.2/src/crc/__main__.py
+-rw-r--r--   0        0        0    16895 2024-04-14 09:08:43.980723 crc-6.1.2/src/crc/_crc.py
+-rw-r--r--   0        0        0        0 2024-04-14 09:08:43.980723 crc-6.1.2/src/crc/py.typed
+-rw-r--r--   0        0        0     5435 1970-01-01 00:00:00.000000 crc-6.1.2/setup.py
+-rw-r--r--   0        0        0     5564 1970-01-01 00:00:00.000000 crc-6.1.2/PKG-INFO
```

### Comparing `crc-6.1.1/LICENSE.txt` & `crc-6.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crc-6.1.1/README.md` & `crc-6.1.2/README.md`

 * *Files identical despite different names*

### Comparing `crc-6.1.1/pyproject.toml` & `crc-6.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crc"
-version = "6.1.1"
+version = "6.1.2"
 description = "Library and CLI to calculate and verify all kinds of CRC checksums"
 packages = [
     { include = "crc", from = "src" },
 ]
 authors = ["Nicola Coretti <nico.coretti@gmail.com>"]
 maintainers = ["Nicola Coretti <nico.coretti@gmail.com>"]
 license = "BSD-2-Clause"
@@ -41,14 +41,15 @@
 mypy = ">=0.991"
 invoke = ">=2"
 mkdocs-autorefs = ">=0.4.1"
 mkdocstrings = ">=0.20.0"
 mkdocstrings-python = ">=0.8.2"
 pytkdocs = ">=0.16.1"
 pre-commit = "^3.1.1"
+mkdocs-gen-files = "^0.5.0"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.run]
```

### Comparing `crc-6.1.1/src/crc/_crc.py` & `crc-6.1.2/src/crc/_crc.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,17 +249,16 @@
             processed.
         """
 
     def digest(self) -> int:
         """
         See `AbstractRegister.digest`
         """
-        if self._config.reverse_output:
-            self.register = self.reverse()
-        return self.register ^ self._config.final_xor_value
+        value = self.reverse() if self._config.reverse_output else self.register
+        return value ^ self._config.final_xor_value
 
     def reverse(self) -> int:
         """
         See `AbstractRegister.digest`
         """
         index = 0
         reversed_value = 0
```

### Comparing `crc-6.1.1/setup.py` & `crc-6.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 entry_points = \
 {'console_scripts': ['crc = crc._crc:main']}
 
 setup_kwargs = {
     'name': 'crc',
-    'version': '6.1.1',
+    'version': '6.1.2',
     'description': 'Library and CLI to calculate and verify all kinds of CRC checksums',
     'long_description': '<h1 align="center">CRC</h1>\n<p align="center">\n\nCalculate CRC checksums, verify CRC checksum, predefined CRC configurations, custom CRC configurations\n</p>\n\n<p align="center">\n\n<a href="https://github.com/Nicoretti/crc/actions">\n    <img src="https://img.shields.io/github/checks-status/nicoretti/crc/master" alt="Checks Master">\n</a>\n<a href="https://coveralls.io/github/Nicoretti/crc">\n    <img src="https://img.shields.io/coverallsCoverage/github/Nicoretti/crc" alt="Coverage">\n</a>\n<a href="https://opensource.org/licenses/BSD-2-Clause">\n    <img src="https://img.shields.io/pypi/l/crc" alt="License">\n</a>\n<a href="https://pypi.org/project/crc/">\n    <img src="https://img.shields.io/pypi/dm/crc" alt="Downloads">\n</a>\n<a href="https://pypi.org/project/crc/">\n    <img src="https://img.shields.io/pypi/pyversions/crc" alt="Supported Python Versions">\n</a>\n<a href="https://pypi.org/project/crc/">\n    <img src="https://img.shields.io/pypi/v/crc" alt="PyPi Package">\n</a>\n</p>\n\n---\n* Documentation: [https://nicoretti.github.io/crc](https://nicoretti.github.io/crc)\n* Source Code: [https://github.com/Nicoretti/crc](https://github.com/Nicoretti/crc)\n---\n\n## Available CRC Configurations\nFor convenience various frequently used crc configurations ship with the library out of the box.\n\n| CRC8 | CRC16    | CRC32 | CRC64 |\n|------|----------|-------|-------|\n| CCITT | CCITT    | CRC32 | CRC64 |\n| AUTOSAR | GSM      | AUTOSAR | |\n| SAEJ1850 | PROFIBUS | BZIP2 | |\n| BLUETOOTH | MODBUS   | POSIX | |\n| MAXIM-DOW | IBM-3740 | | | |\n\nIf you find yourself in the position, where having a new configuration available out of the\nbox would be desirable, feel free to create a [PR](https://github.com/Nicoretti/crc/pulls) or file an [issue](https://github.com/Nicoretti/crc/issues).\n\n## Custom Configurations\n\nIf you want to create a custom configuration, you should have the following information available:\n\n🗒 Note:\n\n    This library currently only supports bit widths of full bytes 8, 16, 24, 32, ...\n\n* **width**\n* **polynom**\n* **init value**\n* **final xor value**\n* **reversed input**\n* **reversed output**\n\nIn case you only have a name of a specific crc configuration/algorithm and you are unsure what are the specific parameters\nof it, a look into this [crc-catalogue](http://reveng.sourceforge.net/crc-catalogue/all.htm) might help.\n\n\n## Requirements\n* [\\>= Python 3.8](https://www.python.org)\n\n## Installation\n\n```shell\npip install crc\n```\n\n## Examples\n\n### Create a Calculator\n\n#### Pre defined configuration\n\n```python\nfrom crc import Calculator, Crc8\n\ncalculator = Calculator(Crc8.CCITT)\n```\n#### Custom configuration\n\n```python\nfrom crc import Calculator, Configuration\n\nconfig = Configuration(\n    width=8,\n    polynomial=0x07,\n    init_value=0x00,\n    final_xor_value=0x00,\n    reverse_input=False,\n    reverse_output=False,\n)\n\ncalculator = Calculator(config)\n```\n\n### Calculate a checksum\n\n#### Standard\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator(Crc8.CCITT)\n\nassert expected == calculator.checksum(data)\n```\n\n#### Optimized for speed\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator(Crc8.CCITT, optimized=True)\n\nassert expected == calculator.checksum(data)\n```\n\n### Verify a checksum\n\n#### Standard\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator(Crc8.CCITT)\n\nassert calculator.verify(data, expected)\n```\n\n#### Optimized for speed\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator(Crc8.CCITT, optimized=True)\n\nassert calculator.verify(data, expected)\n```\n\n### Calculate a checksum with raw registers\n\n#### Register\n\n```python\nfrom crc import Crc8, Register\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\nregister = Register(Crc8.CCITT)\n\nregister.init()\nregister.update(data)\nassert expected == register.digest()\n```\n#### TableBasedRegister\n\n```python\nfrom crc import Crc8, TableBasedRegister\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\nregister = TableBasedRegister(Crc8.CCITT)\n\nregister.init()\nregister.update(data)\nassert expected == register.digest()\n```\n\nReferences & Resources\n-----------------------\n* [A Painless guide to crc error detection algorithms](http://www.zlib.net/crc_v3.txt)\n* [CRC-Catalogue](http://reveng.sourceforge.net/crc-catalogue/all.htm)\n',
     'author': 'Nicola Coretti',
     'author_email': 'nico.coretti@gmail.com',
     'maintainer': 'Nicola Coretti',
     'maintainer_email': 'nico.coretti@gmail.com',
     'url': 'https://github.com/Nicoretti/crc',
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['crc'] package_data = \ {'': ['*']} entry_points = \
 {'console_scripts': ['crc = crc._crc:main']} setup_kwargs = { 'name': 'crc',
-'version': '6.1.1', 'description': 'Library and CLI to calculate and verify all
+'version': '6.1.2', 'description': 'Library and CLI to calculate and verify all
 kinds of CRC checksums', 'long_description': '
                                ************ CCRRCC ************
 \n
        \n\nCalculate CRC checksums, verify CRC checksum, predefined CRC
                   configurations, custom CRC configurations\n
 \n\n
 \n\n_\_n_ _[_C_h_e_c_k_s_ _M_a_s_t_e_r_]_\_n\n_\_n_ _[_C_o_v_e_r_a_g_e_]_\_n\n_\_n_ _[_L_i_c_e_n_s_e_]_\_n\n_\_n_ _[_D_o_w_n_l_o_a_d_s_]_\_n\n_\_n
```

### Comparing `crc-6.1.1/PKG-INFO` & `crc-6.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crc
-Version: 6.1.1
+Version: 6.1.2
 Summary: Library and CLI to calculate and verify all kinds of CRC checksums
 Home-page: https://github.com/Nicoretti/crc
 License: BSD-2-Clause
 Keywords: CRC,CRC8,CRC16,CRC32,CRC64
 Author: Nicola Coretti
 Author-email: nico.coretti@gmail.com
 Maintainer: Nicola Coretti
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: crc Version: 6.1.1 Summary: Library and CLI to
+Metadata-Version: 2.1 Name: crc Version: 6.1.2 Summary: Library and CLI to
 calculate and verify all kinds of CRC checksums Home-page: https://github.com/
 Nicoretti/crc License: BSD-2-Clause Keywords: CRC,CRC8,CRC16,CRC32,CRC64
 Author: Nicola Coretti Author-email: nico.coretti@gmail.com Maintainer: Nicola
 Coretti Maintainer-email: nico.coretti@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```


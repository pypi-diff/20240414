# Comparing `tmp/pyproject-metadata-0.7.1.tar.gz` & `tmp/pyproject_metadata-0.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-metadata-0.7.1.tar", last modified: Mon Jan 30 19:32:14 2023, max compression
+gzip compressed data, was "pyproject_metadata-0.8.0rc1.tar", last modified: Sun Apr 14 04:17:49 2024, max compression
```

## Comparing `pyproject-metadata-0.7.1.tar` & `pyproject_metadata-0.8.0rc1.tar`

### file list

```diff
@@ -1,16 +1,26 @@
-drwxr-xr-x   0 anubis    (1000) users      (985)        0 2023-01-30 19:32:14.693050 pyproject-metadata-0.7.1/
--rw-r--r--   0 anubis    (1000) users      (985)     1113 2021-09-30 19:02:24.000000 pyproject-metadata-0.7.1/LICENSE
--rw-r--r--   0 anubis    (1000) users      (985)       36 2022-07-06 21:18:35.000000 pyproject-metadata-0.7.1/MANIFEST.in
--rw-r--r--   0 anubis    (1000) users      (985)     2610 2023-01-30 19:32:14.693050 pyproject-metadata-0.7.1/PKG-INFO
--rw-r--r--   0 anubis    (1000) users      (985)     1850 2022-10-31 00:30:40.000000 pyproject-metadata-0.7.1/README.md
--rw-r--r--   0 anubis    (1000) users      (985)      100 2021-09-30 19:02:24.000000 pyproject-metadata-0.7.1/pyproject.toml
-drwxr-xr-x   0 anubis    (1000) users      (985)        0 2023-01-30 19:32:14.693050 pyproject-metadata-0.7.1/pyproject_metadata/
--rw-r--r--   0 anubis    (1000) users      (985)    19787 2023-01-30 19:32:03.000000 pyproject-metadata-0.7.1/pyproject_metadata/__init__.py
--rw-r--r--   0 anubis    (1000) users      (985)        0 2022-07-06 21:18:35.000000 pyproject-metadata-0.7.1/pyproject_metadata/py.typed
-drwxr-xr-x   0 anubis    (1000) users      (985)        0 2023-01-30 19:32:14.693050 pyproject-metadata-0.7.1/pyproject_metadata.egg-info/
--rw-r--r--   0 anubis    (1000) users      (985)     2610 2023-01-30 19:32:14.000000 pyproject-metadata-0.7.1/pyproject_metadata.egg-info/PKG-INFO
--rw-r--r--   0 anubis    (1000) users      (985)      322 2023-01-30 19:32:14.000000 pyproject-metadata-0.7.1/pyproject_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 anubis    (1000) users      (985)        1 2023-01-30 19:32:14.000000 pyproject-metadata-0.7.1/pyproject_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 anubis    (1000) users      (985)      181 2023-01-30 19:32:14.000000 pyproject-metadata-0.7.1/pyproject_metadata.egg-info/requires.txt
--rw-r--r--   0 anubis    (1000) users      (985)       19 2023-01-30 19:32:14.000000 pyproject-metadata-0.7.1/pyproject_metadata.egg-info/top_level.txt
--rw-r--r--   0 anubis    (1000) users      (985)     1404 2023-01-30 19:32:14.693050 pyproject-metadata-0.7.1/setup.cfg
+-rw-r--r--   0        0        0     2198 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/CHANGELOG.rst
+-rw-r--r--   0        0        0     1113 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/LICENSE
+-rw-r--r--   0        0        0     1782 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/README.md
+lrwxr-xr-x   0        0        0        0 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/docs/changelog.rst -> ../CHANGELOG.rst
+-rw-r--r--   0        0        0     2299 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/docs/conf.py
+-rw-r--r--   0        0        0      846 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/docs/index.rst
+-rw-r--r--   0        0        0     2528 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    20762 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/pyproject_metadata/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/pyproject_metadata/py.typed
+-rw-r--r--   0        0        0        0 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0      724 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/dynamic-description/dynamic_description.py
+-rw-r--r--   0        0        0       90 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/dynamic-description/pyproject.toml
+-rw-r--r--   0        0        0       17 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/full-metadata/README.md
+-rw-r--r--   0        0        0        0 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/full-metadata/full_metadata.py
+-rw-r--r--   0        0        0     1204 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/full-metadata/pyproject.toml
+-rw-r--r--   0        0        0       19 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/full-metadata2/LICENSE
+-rw-r--r--   0        0        0       17 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/full-metadata2/README.rst
+-rw-r--r--   0        0        0        0 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/full-metadata2/full_metadata2.py
+-rw-r--r--   0        0        0     1196 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/full-metadata2/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/unknown-readme-type/README.just-made-this-up-now
+-rw-r--r--   0        0        0       97 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/unknown-readme-type/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/unknown-readme-type/unknown_readme_type.py
+-rw-r--r--   0        0        0     5899 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/test_rfc822.py
+-rw-r--r--   0        0        0    26273 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/test_standard_metadata.py
+-rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 pyproject_metadata-0.8.0rc1/PKG-INFO
```

### Comparing `pyproject-metadata-0.7.1/LICENSE` & `pyproject_metadata-0.8.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject-metadata-0.7.1/PKG-INFO` & `pyproject_metadata-0.8.0rc1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 Metadata-Version: 2.1
 Name: pyproject-metadata
-Version: 0.7.1
+Version: 0.8.0rc1
 Summary: PEP 621 metadata parsing
-Author: Filipe Laíns
-Author-email: lains@riseup.net
-License: MIT
-Project-URL: homepage, https://github.com/FFY00/python-pyproject-metadata
-Project-URL: changelog, https://pyproject-metadata.readthedocs.io/en/stable/changelog.html
+Author-email: Filipe Laíns <lains@riseup.net>
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: packaging>=19.0
+Requires-Dist: furo>=2023.9.10 ; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints>=1.10.0 ; extra == "docs"
+Requires-Dist: sphinx~=7.0 ; extra == "docs"
+Requires-Dist: pytest-cov[toml]>=2 ; extra == "test"
+Requires-Dist: pytest>=6.2.4 ; extra == "test"
+Requires-Dist: tomli>=1.0.0 ; extra == "test" and (python_version<"3.11")
+Project-URL: changelog, https://pep621.readthedocs.io/en/stable/changelog.html
+Project-URL: homepage, https://github.com/pypa/pyproject-metadata
 Provides-Extra: docs
-License-File: LICENSE
+Provides-Extra: test
 
 # pyproject-metadata
 
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/FFY00/python-pyproject-metadata/main.svg)](https://results.pre-commit.ci/latest/github/FFY00/python-pyproject-metadata/main)
-[![checks](https://github.com/FFY00/python-pyproject-metadata/actions/workflows/checks.yml/badge.svg)](https://github.com/FFY00/python-pyproject-metadata/actions/workflows/checks.yml)
-[![tests](https://github.com/FFY00/python-pyproject-metadata/actions/workflows/tests.yml/badge.svg)](https://github.com/FFY00/python-pyproject-metadata/actions/workflows/tests.yml)
-[![codecov](https://codecov.io/gh/FFY00/python-pyproject-metadata/branch/main/graph/badge.svg?token=9chBjS1lch)](https://codecov.io/gh/FFY00/python-pyproject-metadata)
-[![Documentation Status](https://readthedocs.org/projects/pyproject-metadata/badge/?version=latest)](https://pyproject-metadata.readthedocs.io/en/latest/?badge=latest)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/pypa/pyproject-metadata/main.svg)](https://results.pre-commit.ci/latest/github/pypa/pyproject-metadata/main)
+[![checks](https://github.com/pypa/pyproject-metadata/actions/workflows/checks.yml/badge.svg)](https://github.com/FFY00/python-pyproject-metadata/actions/workflows/checks.yml)
+[![tests](https://github.com/pypa/pyproject-metadata/actions/workflows/tests.yml/badge.svg)](https://github.com/pypa/pyproject-metadata/actions/workflows/tests.yml)
+[![codecov](https://codecov.io/gh/pypa/pyproject-metadata/branch/main/graph/badge.svg?token=9chBjS1lch)](https://codecov.io/gh/pypa/pyproject-metadata)
+[![Documentation Status](https://readthedocs.org/projects/pyproject-metadata/badge/?version=latest)](https://pep621.readthedocs.io/en/latest/?badge=latest)
 
 
 > Dataclass for PEP 621 metadata with support for [core metadata] generation
 
 This project does not implement the parsing of `pyproject.toml`
 containing PEP 621 metadata.
 
@@ -52,7 +59,8 @@
 
 pkg_info = metadata.as_rfc822()
 print(str(pkg_info))  # core metadata
 ```
 
 
 [core metadata]: https://packaging.python.org/specifications/core-metadata/
+
```

### Comparing `pyproject-metadata-0.7.1/README.md` & `pyproject_metadata-0.8.0rc1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pyproject-metadata
 
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/FFY00/python-pyproject-metadata/main.svg)](https://results.pre-commit.ci/latest/github/FFY00/python-pyproject-metadata/main)
-[![checks](https://github.com/FFY00/python-pyproject-metadata/actions/workflows/checks.yml/badge.svg)](https://github.com/FFY00/python-pyproject-metadata/actions/workflows/checks.yml)
-[![tests](https://github.com/FFY00/python-pyproject-metadata/actions/workflows/tests.yml/badge.svg)](https://github.com/FFY00/python-pyproject-metadata/actions/workflows/tests.yml)
-[![codecov](https://codecov.io/gh/FFY00/python-pyproject-metadata/branch/main/graph/badge.svg?token=9chBjS1lch)](https://codecov.io/gh/FFY00/python-pyproject-metadata)
-[![Documentation Status](https://readthedocs.org/projects/pyproject-metadata/badge/?version=latest)](https://pyproject-metadata.readthedocs.io/en/latest/?badge=latest)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/pypa/pyproject-metadata/main.svg)](https://results.pre-commit.ci/latest/github/pypa/pyproject-metadata/main)
+[![checks](https://github.com/pypa/pyproject-metadata/actions/workflows/checks.yml/badge.svg)](https://github.com/FFY00/python-pyproject-metadata/actions/workflows/checks.yml)
+[![tests](https://github.com/pypa/pyproject-metadata/actions/workflows/tests.yml/badge.svg)](https://github.com/pypa/pyproject-metadata/actions/workflows/tests.yml)
+[![codecov](https://codecov.io/gh/pypa/pyproject-metadata/branch/main/graph/badge.svg?token=9chBjS1lch)](https://codecov.io/gh/pypa/pyproject-metadata)
+[![Documentation Status](https://readthedocs.org/projects/pyproject-metadata/badge/?version=latest)](https://pep621.readthedocs.io/en/latest/?badge=latest)
 
 
 > Dataclass for PEP 621 metadata with support for [core metadata] generation
 
 This project does not implement the parsing of `pyproject.toml`
 containing PEP 621 metadata.
```

### Comparing `pyproject-metadata-0.7.1/pyproject_metadata/__init__.py` & `pyproject_metadata-0.8.0rc1/pyproject_metadata/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import collections
+import copy
 import dataclasses
+import email.utils
 import os
 import os.path
 import pathlib
-import re
 import typing
 
-from collections.abc import Mapping
-from typing import Any
+
+if typing.TYPE_CHECKING:
+    from collections.abc import Mapping
+    from typing import Any
+
+    from packaging.requirements import Requirement
 
 import packaging.markers
 import packaging.requirements
 import packaging.specifiers
+import packaging.utils
 import packaging.version
 
 
-__version__ = '0.7.1'
+__version__ = '0.8.0rc1'
+
+KNOWN_METADATA_VERSIONS = {'2.1', '2.2', '2.3'}
 
 
 class ConfigurationError(Exception):
     '''Error in the backend metadata.'''
     def __init__(self, msg: str, *, key: str | None = None):
         super().__init__(msg)
         self._key = key
 
     @property
     def key(self) -> str | None:  # pragma: no cover
         return self._key
 
 
-class RFC822Message():
+class RFC822Message:
     '''Python-flavored RFC 822 message implementation.'''
 
     def __init__(self) -> None:
         self.headers: collections.OrderedDict[str, list[str]] = collections.OrderedDict()
         self.body: str | None = None
 
     def __setitem__(self, name: str, value: str | None) -> None:
@@ -59,15 +67,15 @@
             text += '\n' + self.body
         return text
 
     def __bytes__(self) -> bytes:
         return str(self).encode()
 
 
-class DataFetcher():
+class DataFetcher:
     def __init__(self, data: Mapping[str, Any]) -> None:
         self._data = data
 
     def __contains__(self, key: Any) -> bool:
         if not isinstance(key, str):
             return False
         val = self._data
@@ -84,59 +92,44 @@
             val = val[part]
         return val
 
     def get_str(self, key: str) -> str | None:
         try:
             val = self.get(key)
             if not isinstance(val, str):
-                raise ConfigurationError(
-                    f'Field `{key}` has an invalid type, '
-                    f'expecting a string (got `{val}`)',
-                    key=key,
-                )
+                msg = f'Field "{key}" has an invalid type, expecting a string (got "{val}")'
+                raise ConfigurationError(msg, key=key)
             return val
         except KeyError:
             return None
 
     def get_list(self, key: str) -> list[str]:
         try:
             val = self.get(key)
             if not isinstance(val, list):
-                raise ConfigurationError(
-                    f'Field `{key}` has an invalid type, '
-                    f'expecting a list of strings (got `{val}`)',
-                    key=val,
-                )
+                msg = f'Field "{key}" has an invalid type, expecting a list of strings (got "{val}")'
+                raise ConfigurationError(msg, key=val)
             for item in val:
                 if not isinstance(item, str):
-                    raise ConfigurationError(
-                        f'Field `{key}` contains item with invalid type, '
-                        f'expecting a string (got `{item}`)',
-                        key=key,
-                    )
+                    msg = f'Field "{key}" contains item with invalid type, expecting a string (got "{item}")'
+                    raise ConfigurationError(msg, key=key)
             return val
         except KeyError:
             return []
 
     def get_dict(self, key: str) -> dict[str, str]:
         try:
             val = self.get(key)
             if not isinstance(val, dict):
-                raise ConfigurationError(
-                    f'Field `{key}` has an invalid type, '
-                    f'expecting a dictionary of strings (got `{val}`)',
-                    key=key,
-                )
+                msg = f'Field "{key}" has an invalid type, expecting a dictionary of strings (got "{val}")'
+                raise ConfigurationError(msg, key=key)
             for subkey, item in val.items():
                 if not isinstance(item, str):
-                    raise ConfigurationError(
-                        f'Field `{key}.{subkey}` has an invalid type, '
-                        f'expecting a string (got `{item}`)',
-                        key=f'{key}.{subkey}',
-                    )
+                    msg = f'Field "{key}.{subkey}" has an invalid type, expecting a string (got "{item}")'
+                    raise ConfigurationError(msg, key=f'{key}.{subkey}')
             return val
         except KeyError:
             return {}
 
     def get_people(self, key: str) -> list[tuple[str, str]]:
         try:
             val = self.get(key)
@@ -145,19 +138,19 @@
                 and all(isinstance(x, dict) for x in val)
                 and all(
                     isinstance(item, str)
                     for items in [_dict.values() for _dict in val]
                     for item in items
                 )
             ):
-                raise ConfigurationError(
-                    f'Field `{key}` has an invalid type, expecting a list of '
-                    f'dictionaries containing the `name` and/or `email` keys (got `{val}`)',
-                    key=key,
+                msg = (
+                    f'Field "{key}" has an invalid type, expecting a list of '
+                    f'dictionaries containing the "name" and/or "email" keys (got "{val}")'
                 )
+                raise ConfigurationError(msg, key=key)
             return [
                 (entry.get('name', 'Unknown'), entry.get('email'))
                 for entry in val
             ]
         except KeyError:
             return []
 
@@ -170,114 +163,140 @@
 class Readme(typing.NamedTuple):
     text: str
     file: pathlib.Path | None
     content_type: str
 
 
 @dataclasses.dataclass
-class StandardMetadata():
+class StandardMetadata:
     name: str
     version: packaging.version.Version | None = None
     description: str | None = None
     license: License | None = None
     readme: Readme | None = None
     requires_python: packaging.specifiers.SpecifierSet | None = None
-    dependencies: list[packaging.requirements.Requirement] = dataclasses.field(default_factory=list)
-    optional_dependencies: dict[str, list[packaging.requirements.Requirement]] = dataclasses.field(default_factory=dict)
+    dependencies: list[Requirement] = dataclasses.field(default_factory=list)
+    optional_dependencies: dict[str, list[Requirement]] = dataclasses.field(default_factory=dict)
     entrypoints: dict[str, dict[str, str]] = dataclasses.field(default_factory=dict)
     authors: list[tuple[str, str]] = dataclasses.field(default_factory=list)
     maintainers: list[tuple[str, str]] = dataclasses.field(default_factory=list)
     urls: dict[str, str] = dataclasses.field(default_factory=dict)
     classifiers: list[str] = dataclasses.field(default_factory=list)
     keywords: list[str] = dataclasses.field(default_factory=list)
     scripts: dict[str, str] = dataclasses.field(default_factory=dict)
     gui_scripts: dict[str, str] = dataclasses.field(default_factory=dict)
     dynamic: list[str] = dataclasses.field(default_factory=list)
 
-    def __post_init__(self) -> None:
-        self.name = re.sub(r'[-_.]+', '-', self.name).lower()
-        self._update_dynamic(self.version)
+    _metadata_version: str | None = None
+
+    @property
+    def metadata_version(self) -> str:
+        if self._metadata_version is None:
+            return '2.2' if self.dynamic else '2.1'
+        return self._metadata_version
+
+    @property
+    def canonical_name(self) -> str:
+        return packaging.utils.canonicalize_name(self.name)
 
     @classmethod
     def from_pyproject(
         cls,
         data: Mapping[str, Any],
         project_dir: str | os.PathLike[str] = os.path.curdir,
+        metadata_version: str | None = None,
     ) -> StandardMetadata:
         fetcher = DataFetcher(data)
         project_dir = pathlib.Path(project_dir)
 
         if 'project' not in fetcher:
-            raise ConfigurationError('Section `project` missing in pyproject.toml')
+            msg = 'Section "project" missing in pyproject.toml'
+            raise ConfigurationError(msg)
 
         dynamic = fetcher.get_list('project.dynamic')
         if 'name' in dynamic:
-            raise ConfigurationError('Unsupported field `name` in `project.dynamic`')
+            msg = 'Unsupported field "name" in "project.dynamic"'
+            raise ConfigurationError(msg)
 
         for field in dynamic:
             if field in data['project']:
-                raise ConfigurationError(
-                    f'Field `project.{field}` declared as dynamic in but is defined'
-                )
+                msg = f'Field "project.{field}" declared as dynamic in but is defined'
+                raise ConfigurationError(msg)
 
         name = fetcher.get_str('project.name')
         if not name:
-            raise ConfigurationError('Field `project.name` missing')
+            msg = 'Field "project.name" missing'
+            raise ConfigurationError(msg)
 
         version_string = fetcher.get_str('project.version')
         requires_python_string = fetcher.get_str('project.requires-python')
+        version = packaging.version.Version(version_string) if version_string else None
+
+        if version is None and 'version' not in dynamic:
+            msg = 'Field "project.version" missing and "version" not specified in "project.dynamic"'
+            raise ConfigurationError(msg)
+
+        # Description can't be multiline
+        description = fetcher.get_str('project.description')
+        if description and '\n' in description:
+            msg = 'The description must be a single line'
+            raise ConfigurationError(msg)
+
+        if metadata_version and metadata_version not in KNOWN_METADATA_VERSIONS:
+            msg = f'The metadata_version must be one of {KNOWN_METADATA_VERSIONS} or None (default)'
+            raise ConfigurationError(msg)
 
         return cls(
             name,
-            packaging.version.Version(version_string) if version_string else None,
-            fetcher.get_str('project.description'),
+            version,
+            description,
             cls._get_license(fetcher, project_dir),
             cls._get_readme(fetcher, project_dir),
             packaging.specifiers.SpecifierSet(requires_python_string) if requires_python_string else None,
             cls._get_dependencies(fetcher),
             cls._get_optional_dependencies(fetcher),
             cls._get_entrypoints(fetcher),
             fetcher.get_people('project.authors'),
             fetcher.get_people('project.maintainers'),
             fetcher.get_dict('project.urls'),
             fetcher.get_list('project.classifiers'),
             fetcher.get_list('project.keywords'),
             fetcher.get_dict('project.scripts'),
             fetcher.get_dict('project.gui-scripts'),
             dynamic,
+            metadata_version,
         )
 
     def _update_dynamic(self, value: Any) -> None:
         if value and 'version' in self.dynamic:
             self.dynamic.remove('version')
-        elif not value and 'version' not in self.dynamic:
-            self.dynamic.append('version')
 
     def __setattr__(self, name: str, value: Any) -> None:
         # update dynamic when version is set
         if name == 'version' and hasattr(self, 'dynamic'):
             self._update_dynamic(value)
         super().__setattr__(name, value)
 
     def as_rfc822(self) -> RFC822Message:
         message = RFC822Message()
         self.write_to_rfc822(message)
         return message
 
     def write_to_rfc822(self, message: RFC822Message) -> None:  # noqa: C901
-        message['Metadata-Version'] = '2.2' if self.dynamic else '2.1'
+        message['Metadata-Version'] = self.metadata_version
         message['Name'] = self.name
         if not self.version:
-            raise ConfigurationError('Missing version field')
+            msg = 'Missing version field'
+            raise ConfigurationError(msg)
         message['Version'] = str(self.version)
         # skip 'Platform'
         # skip 'Supported-Platform'
         if self.description:
             message['Summary'] = self.description
-        message['Keywords'] = ' '.join(self.keywords)
+        message['Keywords'] = ','.join(self.keywords)
         if 'homepage' in self.urls:
             message['Home-page'] = self.urls['homepage']
         # skip 'Download-URL'
         message['Author'] = self._name_list(self.authors)
         message['Author-Email'] = self._email_list(self.authors)
         message['Maintainer'] = self._name_list(self.maintainers)
         message['Maintainer-Email'] = self._email_list(self.maintainers)
@@ -291,84 +310,88 @@
         for name, url in self.urls.items():
             message['Project-URL'] = f'{name.capitalize()}, {url}'
         if self.requires_python:
             message['Requires-Python'] = str(self.requires_python)
         for dep in self.dependencies:
             message['Requires-Dist'] = str(dep)
         for extra, requirements in self.optional_dependencies.items():
-            message['Provides-Extra'] = extra
+            norm_extra = extra.replace('.', '-').replace('_', '-').lower()
+            message['Provides-Extra'] = norm_extra
             for requirement in requirements:
-                message['Requires-Dist'] = str(self._build_extra_req(extra, requirement))
+                message['Requires-Dist'] = str(self._build_extra_req(norm_extra, requirement))
         if self.readme:
             if self.readme.content_type:
                 message['Description-Content-Type'] = self.readme.content_type
             message.body = self.readme.text
         # Core Metadata 2.2
-        for field in self.dynamic:
-            if field in ('name', 'version'):
-                raise ConfigurationError(f'Field cannot be dynamic: {field}')
-            message['Dynamic'] = field
+        if self.metadata_version != '2.1':
+            for field in self.dynamic:
+                if field in ('name', 'version'):
+                    msg = f'Field cannot be dynamic: {field}'
+                    raise ConfigurationError(msg)
+                message['Dynamic'] = field
 
     def _name_list(self, people: list[tuple[str, str]]) -> str:
         return ', '.join(
             name
             for name, email_ in people
             if not email_
         )
 
     def _email_list(self, people: list[tuple[str, str]]) -> str:
-        return ', '.join([
-            '{}{}'.format(name, f' <{_email}>' if _email else '')
+        return ', '.join(
+            email.utils.formataddr((name, _email))
             for name, _email in people
             if _email
-        ])
+        )
 
     def _build_extra_req(
         self,
         extra: str,
-        requirement: packaging.requirements.Requirement,
-    ) -> packaging.requirements.Requirement:
-        if requirement.marker:  # append our extra to the marker
-            requirement.marker = packaging.markers.Marker(
-                str(requirement.marker) + f' and extra == "{extra}"'
-            )
-        else:  # add our extra marker
+        requirement: Requirement,
+    ) -> Requirement:
+        # append or add our extra marker
+        requirement = copy.copy(requirement)
+        if requirement.marker:
+            if 'or' in requirement.marker._markers:
+                requirement.marker = packaging.markers.Marker(
+                    f'({requirement.marker}) and extra == "{extra}"'
+                )
+            else:
+                requirement.marker = packaging.markers.Marker(
+                    f'{requirement.marker} and extra == "{extra}"'
+                )
+        else:
             requirement.marker = packaging.markers.Marker(f'extra == "{extra}"')
         return requirement
 
     @staticmethod
     def _get_license(fetcher: DataFetcher, project_dir: pathlib.Path) -> License | None:
         if 'project.license' not in fetcher:
             return None
 
         _license = fetcher.get_dict('project.license')
         for field in _license:
             if field not in ('file', 'text'):
-                raise ConfigurationError(
-                    f'Unexpected field `project.license.{field}`',
-                    key=f'project.license.{field}',
-                )
+                msg = f'Unexpected field "project.license.{field}"'
+                raise ConfigurationError(msg, key=f'project.license.{field}')
 
         file: pathlib.Path | None = None
         filename = fetcher.get_str('project.license.file')
         text = fetcher.get_str('project.license.text')
 
         if (filename and text) or (not filename and not text):
-            raise ConfigurationError(
-                f'Invalid `project.license` value, expecting either `file` or `text` (got `{_license}`)',
-                key='project.license',
-            )
+            msg = f'Invalid "project.license" value, expecting either "file" or "text" (got "{_license}")'
+            raise ConfigurationError(msg, key='project.license')
 
         if filename:
             file = project_dir.joinpath(filename)
             if not file.is_file():
-                raise ConfigurationError(
-                    f'License file not found (`{filename}`)',
-                    key='project.license.file',
-                )
+                msg = f'License file not found ("{filename}")'
+                raise ConfigurationError(msg, key='project.license.file')
             text = file.read_text(encoding='utf-8')
 
         assert text is not None
         return License(text, file)
 
     @staticmethod
     def _get_readme(fetcher: DataFetcher, project_dir: pathlib.Path) -> Readme | None:  # noqa: C901
@@ -386,130 +409,129 @@
             text = None
             filename = readme
             if filename.endswith('.md'):
                 content_type = 'text/markdown'
             elif filename.endswith('.rst'):
                 content_type = 'text/x-rst'
             else:
-                raise ConfigurationError(
-                    f'Could not infer content type for readme file `{filename}`',
-                    key='project.readme',
-                )
+                msg = f'Could not infer content type for readme file "{filename}"'
+                raise ConfigurationError(msg, key='project.readme')
         elif isinstance(readme, dict):
             # readme is a dict containing either 'file' or 'text', and content-type
             for field in readme:
                 if field not in ('content-type', 'file', 'text'):
-                    raise ConfigurationError(
-                        f'Unexpected field `project.readme.{field}`',
-                        key=f'project.readme.{field}',
-                    )
+                    msg = f'Unexpected field "project.readme.{field}"'
+                    raise ConfigurationError(msg, key=f'project.readme.{field}')
             content_type = fetcher.get_str('project.readme.content-type')
             filename = fetcher.get_str('project.readme.file')
             text = fetcher.get_str('project.readme.text')
             if (filename and text) or (not filename and not text):
-                raise ConfigurationError(
-                    f'Invalid `project.readme` value, expecting either `file` or `text` (got `{readme}`)',
-                    key='project.license',
-                )
+                msg = f'Invalid "project.readme" value, expecting either "file" or "text" (got "{readme}")'
+                raise ConfigurationError(msg, key='project.readme')
             if not content_type:
-                raise ConfigurationError(
-                    'Field `project.readme.content-type` missing',
-                    key='project.readme.content-type',
-                )
+                msg = 'Field "project.readme.content-type" missing'
+                raise ConfigurationError(msg, key='project.readme.content-type')
         else:
-            raise ConfigurationError(
-                f'Field `project.readme` has an invalid type, expecting either, '
-                f'a string or dictionary of strings (got `{readme}`)',
-                key='project.readme',
+            msg = (
+                f'Field "project.readme" has an invalid type, expecting either, '
+                f'a string or dictionary of strings (got "{readme}")'
             )
+            raise ConfigurationError(msg, key='project.readme')
 
         if filename:
             file = project_dir.joinpath(filename)
             if not file.is_file():
-                raise ConfigurationError(
-                    f'Readme file not found (`{filename}`)',
-                    key='project.license.file',
-                )
+                msg = f'Readme file not found ("{filename}")'
+                raise ConfigurationError(msg, key='project.readme.file')
             text = file.read_text(encoding='utf-8')
 
         assert text is not None
         return Readme(text, file, content_type)
 
     @staticmethod
-    def _get_dependencies(fetcher: DataFetcher) -> list[packaging.requirements.Requirement]:
+    def _get_dependencies(fetcher: DataFetcher) -> list[Requirement]:
         try:
             requirement_strings = fetcher.get_list('project.dependencies')
         except KeyError:
             return []
 
-        requirements: list[packaging.requirements.Requirement] = []
+        requirements: list[Requirement] = []
         for req in requirement_strings:
             try:
                 requirements.append(packaging.requirements.Requirement(req))
             except packaging.requirements.InvalidRequirement as e:
-                raise ConfigurationError(
-                    'Field `project.dependencies` contains an invalid PEP 508 '
-                    f'requirement string `{req}` (`{str(e)}`)'
+                msg = (
+                    'Field "project.dependencies" contains an invalid PEP 508 '
+                    f'requirement string "{req}" ("{e}")'
                 )
+                raise ConfigurationError(msg) from None
         return requirements
 
     @staticmethod
-    def _get_optional_dependencies(fetcher: DataFetcher) -> dict[str, list[packaging.requirements.Requirement]]:
+    def _get_optional_dependencies(fetcher: DataFetcher) -> dict[str, list[Requirement]]:
         try:
             val = fetcher.get('project.optional-dependencies')
         except KeyError:
             return {}
 
-        requirements_dict: collections.defaultdict[str, list[packaging.requirements.Requirement]] = collections.defaultdict(list)
+        requirements_dict: dict[str, list[Requirement]] = {}
         if not isinstance(val, dict):
-            raise ConfigurationError(
-                'Field `project.optional-dependencies` has an invalid type, expecting a '
-                f'dictionary of PEP 508 requirement strings (got `{val}`)'
+            msg = (
+                'Field "project.optional-dependencies" has an invalid type, expecting a '
+                f'dictionary of PEP 508 requirement strings (got "{val}")'
             )
+            raise ConfigurationError(msg)
         for extra, requirements in val.copy().items():
             assert isinstance(extra, str)
             if not isinstance(requirements, list):
-                raise ConfigurationError(
-                    f'Field `project.optional-dependencies.{extra}` has an invalid type, expecting a '
-                    f'dictionary PEP 508 requirement strings (got `{requirements}`)'
-                )
-            for i, req in enumerate(requirements):
+                msg = (
+                    f'Field "project.optional-dependencies.{extra}" has an invalid type, expecting a '
+                    f'dictionary PEP 508 requirement strings (got "{requirements}")'
+                )
+                raise ConfigurationError(msg)
+            requirements_dict[extra] = []
+            for req in requirements:
                 if not isinstance(req, str):
-                    raise ConfigurationError(
-                        f'Field `project.optional-dependencies.{extra}` has an invalid type, '
-                        f'expecting a PEP 508 requirement string (got `{req}`)'
+                    msg = (
+                        f'Field "project.optional-dependencies.{extra}" has an invalid type, '
+                        f'expecting a PEP 508 requirement string (got "{req}")'
                     )
+                    raise ConfigurationError(msg)
                 try:
                     requirements_dict[extra].append(packaging.requirements.Requirement(req))
                 except packaging.requirements.InvalidRequirement as e:
-                    raise ConfigurationError(
-                        f'Field `project.optional-dependencies.{extra}` contains '
-                        f'an invalid PEP 508 requirement string `{req}` (`{str(e)}`)'
+                    msg = (
+                        f'Field "project.optional-dependencies.{extra}" contains '
+                        f'an invalid PEP 508 requirement string "{req}" ("{e}")'
                     )
+                    raise ConfigurationError(msg) from None
         return dict(requirements_dict)
 
     @staticmethod
     def _get_entrypoints(fetcher: DataFetcher) -> dict[str, dict[str, str]]:
         try:
             val = fetcher.get('project.entry-points')
         except KeyError:
             return {}
         if not isinstance(val, dict):
-            raise ConfigurationError(
-                'Field `project.entry-points` has an invalid type, expecting a '
-                f'dictionary of entrypoint sections (got `{val}`)'
+            msg = (
+                'Field "project.entry-points" has an invalid type, expecting a '
+                f'dictionary of entrypoint sections (got "{val}")'
             )
+            raise ConfigurationError(msg)
         for section, entrypoints in val.items():
             assert isinstance(section, str)
             if not isinstance(entrypoints, dict):
-                raise ConfigurationError(
-                    f'Field `project.entry-points.{section}` has an invalid type, expecting a '
-                    f'dictionary of entrypoints (got `{entrypoints}`)'
+                msg = (
+                    f'Field "project.entry-points.{section}" has an invalid type, expecting a '
+                    f'dictionary of entrypoints (got "{entrypoints}")'
                 )
+                raise ConfigurationError(msg)
             for name, entrypoint in entrypoints.items():
                 assert isinstance(name, str)
                 if not isinstance(entrypoint, str):
-                    raise ConfigurationError(
-                        f'Field `project.entry-points.{section}.{name}` has an invalid type, '
-                        f'expecting a string (got `{entrypoint}`)'
+                    msg = (
+                        f'Field "project.entry-points.{section}.{name}" has an invalid type, '
+                        f'expecting a string (got "{entrypoint}")'
                     )
+                    raise ConfigurationError(msg)
         return val
```


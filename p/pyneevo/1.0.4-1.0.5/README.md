# Comparing `tmp/pyneevo-1.0.4.tar.gz` & `tmp/pyneevo-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneevo-1.0.4.tar", last modified: Sun Jan  8 15:08:02 2023, max compression
+gzip compressed data, was "pyneevo-1.0.5.tar", last modified: Sun Apr 14 21:41:11 2024, max compression
```

## Comparing `pyneevo-1.0.4.tar` & `pyneevo-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-01-08 15:08:02.471482 pyneevo-1.0.4/
--rw-r--r--   0 david     (1000) david     (1000)     1068 2022-12-19 00:18:04.000000 pyneevo-1.0.4/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)       54 2022-12-19 04:13:01.000000 pyneevo-1.0.4/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)      381 2023-01-08 15:08:02.471482 pyneevo-1.0.4/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)        9 2022-12-19 00:18:04.000000 pyneevo-1.0.4/README.md
--rw-rw-r--   0 david     (1000) david     (1000)      103 2022-12-19 04:11:24.000000 pyneevo-1.0.4/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)       79 2023-01-08 15:08:02.471482 pyneevo-1.0.4/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)      883 2023-01-08 15:07:20.000000 pyneevo-1.0.4/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-01-08 15:08:02.471482 pyneevo-1.0.4/src/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-01-08 15:08:02.471482 pyneevo-1.0.4/src/pyneevo/
--rw-rw-r--   0 david     (1000) david     (1000)       91 2022-12-19 03:31:38.000000 pyneevo-1.0.4/src/pyneevo/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3800 2023-01-08 15:05:49.000000 pyneevo-1.0.4/src/pyneevo/api.py
--rw-rw-r--   0 david     (1000) david     (1000)      401 2022-12-19 17:16:58.000000 pyneevo-1.0.4/src/pyneevo/errors.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-01-08 15:08:02.471482 pyneevo-1.0.4/src/pyneevo/tank/
--rw-rw-r--   0 david     (1000) david     (1000)     3258 2023-01-08 14:27:53.000000 pyneevo-1.0.4/src/pyneevo/tank/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-01-08 15:08:02.471482 pyneevo-1.0.4/src/pyneevo.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)      381 2023-01-08 15:08:02.000000 pyneevo-1.0.4/src/pyneevo.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      331 2023-01-08 15:08:02.000000 pyneevo-1.0.4/src/pyneevo.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-01-08 15:08:02.000000 pyneevo-1.0.4/src/pyneevo.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)        8 2023-01-08 15:08:02.000000 pyneevo-1.0.4/src/pyneevo.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)        8 2023-01-08 15:08:02.000000 pyneevo-1.0.4/src/pyneevo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:41:11.385230 pyneevo-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-14 21:41:07.000000 pyneevo-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-14 21:41:07.000000 pyneevo-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-14 21:41:11.385230 pyneevo-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 21:41:07.000000 pyneevo-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-14 21:41:07.000000 pyneevo-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-14 21:41:11.385230 pyneevo-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-14 21:41:07.000000 pyneevo-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:41:11.381230 pyneevo-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:41:11.381230 pyneevo-1.0.5/src/pyneevo/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-14 21:41:07.000000 pyneevo-1.0.5/src/pyneevo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-14 21:41:07.000000 pyneevo-1.0.5/src/pyneevo/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-14 21:41:07.000000 pyneevo-1.0.5/src/pyneevo/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:41:11.381230 pyneevo-1.0.5/src/pyneevo/tank/
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-14 21:41:07.000000 pyneevo-1.0.5/src/pyneevo/tank/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:41:11.381230 pyneevo-1.0.5/src/pyneevo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-14 21:41:11.000000 pyneevo-1.0.5/src/pyneevo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-14 21:41:11.000000 pyneevo-1.0.5/src/pyneevo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:41:11.000000 pyneevo-1.0.5/src/pyneevo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 21:41:11.000000 pyneevo-1.0.5/src/pyneevo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 21:41:11.000000 pyneevo-1.0.5/src/pyneevo.egg-info/top_level.txt
```

### Comparing `pyneevo-1.0.4/LICENSE` & `pyneevo-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneevo-1.0.4/setup.py` & `pyneevo-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text(encoding="utf-8")
 
 # This call to setup() does all the work
 setup(
     name="pyneevo",
-    version="1.0.4",
+    version="1.0.5",
     author="davidflypei",
     description="Python library for interacting with the Neevo API",
     long_description=README,
     long_description_content_type="text/markdown",
     package_dir={"": "src"},
     packages=find_packages(where="src", exclude=("tests", "tests.*", "*.tests.*", ".tests", "dist")),
     install_requires=["aiohttp"],
```

### Comparing `pyneevo-1.0.4/src/pyneevo/api.py` & `pyneevo-1.0.5/src/pyneevo/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
             raise err
         finally:
             await _session.close()
             return responsejson
 
     # Get Tanks
     async def _get_tanks(self) -> None:
+        _session = ClientSession()
         tanks = await self.GetAllDisplayPropaneDevices()
         for _tank in tanks:
             _tank_obj = Tank(_tank, self)
             self._tanks[_tank.get('Id')] = _tank_obj
 
     async def get_tanks_info(self) -> Dict:
         if not self._tanks:
```

### Comparing `pyneevo-1.0.4/src/pyneevo/tank/__init__.py` & `pyneevo-1.0.5/src/pyneevo/tank/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -76,21 +76,21 @@
 
     @property
     def serial_number(self) -> str:
         """Return the serial number of the tank."""
         return self._tank_data['SerialNumber']
 
     @property
-    def tank_capacity(self) -> str:
-        """Return the serial number of the tank."""
-        return self._tank_data['TankCapacity']
+    def last_pressure_unit(self) -> str:
+        """Return the last pressure unit of the tank."""
+        return self.pressure_unit(self)
 
     @property
-    def tank_last_pressure(self) -> str:
+    def last_pressure(self) -> str:
         """Return the last pressure unit of the tank."""
         return self._tank_data['TankLastPressure']
 
     @property
-    def tank_last_pressure_unit(self) -> str:
-        """Return the last pressure unit of the tank."""
+    def pressure_unit(self) -> str:
+        """Return the pressure unit of the tank."""
         return self._tank_data['TankPressureDisplayUnitSymbol']
```


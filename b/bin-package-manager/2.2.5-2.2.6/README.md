# Comparing `tmp/bin_package_manager-2.2.5.tar.gz` & `tmp/bin_package_manager-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bin_package_manager-2.2.5.tar", max compression
+gzip compressed data, was "bin_package_manager-2.2.6.tar", max compression
```

## Comparing `bin_package_manager-2.2.5.tar` & `bin_package_manager-2.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1066 2024-02-03 15:14:27.236806 bin_package_manager-2.2.5/LICENSE
--rw-r--r--   0        0        0     3907 2024-04-12 17:44:29.537756 bin_package_manager-2.2.5/README.md
--rw-r--r--   0        0        0      211 2024-04-12 12:39:24.674496 bin_package_manager-2.2.5/bpm/__init__.py
--rw-r--r--   0        0        0       61 2024-02-14 06:21:44.497403 bin_package_manager-2.2.5/bpm/__main__.py
--rw-r--r--   0        0        0     4119 2024-04-12 12:39:24.674496 bin_package_manager-2.2.5/bpm/cli.py
--rw-r--r--   0        0        0     6946 2024-04-12 12:39:24.674496 bin_package_manager-2.2.5/bpm/command.py
--rw-r--r--   0        0        0    17654 2024-04-12 12:39:24.674496 bin_package_manager-2.2.5/bpm/install/__init__.py
--rw-r--r--   0        0        0     4103 2024-02-19 11:56:44.850635 bin_package_manager-2.2.5/bpm/lib/windowspathadder.py
--rw-r--r--   0        0        0    12254 2024-04-12 17:42:26.398806 bin_package_manager-2.2.5/bpm/search.py
--rw-r--r--   0        0        0     4449 2024-04-12 12:39:24.674496 bin_package_manager-2.2.5/bpm/storage.py
--rw-r--r--   0        0        0     3913 2024-04-12 17:41:05.452840 bin_package_manager-2.2.5/bpm/utils/__init__.py
--rw-r--r--   0        0        0      526 2024-04-12 12:39:24.674496 bin_package_manager-2.2.5/bpm/utils/constants.py
--rw-r--r--   0        0        0      988 2024-02-21 10:21:37.512797 bin_package_manager-2.2.5/bpm/utils/exceptions.py
--rw-r--r--   0        0        0     1003 2024-04-12 17:43:02.785161 bin_package_manager-2.2.5/pyproject.toml
--rw-r--r--   0        0        0     4819 1970-01-01 00:00:00.000000 bin_package_manager-2.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-02-03 15:14:27.236806 bin_package_manager-2.2.6/LICENSE
+-rw-r--r--   0        0        0     3907 2024-04-12 17:44:29.537756 bin_package_manager-2.2.6/README.md
+-rw-r--r--   0        0        0      211 2024-04-12 12:39:24.674496 bin_package_manager-2.2.6/bpm/__init__.py
+-rw-r--r--   0        0        0       61 2024-02-14 06:21:44.497403 bin_package_manager-2.2.6/bpm/__main__.py
+-rw-r--r--   0        0        0     4138 2024-04-14 10:57:29.327187 bin_package_manager-2.2.6/bpm/cli.py
+-rw-r--r--   0        0        0     7005 2024-04-14 11:16:00.299639 bin_package_manager-2.2.6/bpm/command.py
+-rw-r--r--   0        0        0    18498 2024-04-14 11:40:21.759536 bin_package_manager-2.2.6/bpm/install/__init__.py
+-rw-r--r--   0        0        0     4103 2024-02-19 11:56:44.850635 bin_package_manager-2.2.6/bpm/lib/windowspathadder.py
+-rw-r--r--   0        0        0    12270 2024-04-14 11:18:11.259006 bin_package_manager-2.2.6/bpm/search.py
+-rw-r--r--   0        0        0     4449 2024-04-12 12:39:24.674496 bin_package_manager-2.2.6/bpm/storage.py
+-rw-r--r--   0        0        0     3913 2024-04-12 17:41:05.452840 bin_package_manager-2.2.6/bpm/utils/__init__.py
+-rw-r--r--   0        0        0      526 2024-04-12 12:39:24.674496 bin_package_manager-2.2.6/bpm/utils/constants.py
+-rw-r--r--   0        0        0      988 2024-02-21 10:21:37.512797 bin_package_manager-2.2.6/bpm/utils/exceptions.py
+-rw-r--r--   0        0        0     1003 2024-04-14 11:47:17.921734 bin_package_manager-2.2.6/pyproject.toml
+-rw-r--r--   0        0        0     4819 1970-01-01 00:00:00.000000 bin_package_manager-2.2.6/PKG-INFO
```

### Comparing `bin_package_manager-2.2.5/LICENSE` & `bin_package_manager-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bin_package_manager-2.2.5/README.md` & `bin_package_manager-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `bin_package_manager-2.2.5/bpm/cli.py` & `bin_package_manager-2.2.6/bpm/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     metavar="Archive",
     help="install from local archive.",
 )
 install_parser.add_argument(
     "-q",
     "--quiet",
     action="store_true",
-    help="not ask, install the best match repo.",
+    help="not ask, install the best match repo, show less messages",
 )
 install_parser.add_argument(
     "--one-bin",
     action="store_true",
     help="install given binary only. Use package name as binary name by default.",
 )
 # github api not support info pre releases. https://docs.github.com/en/rest/releases/releases?apiVersion=2022-11-28#get-the-latest-release
```

### Comparing `bin_package_manager-2.2.5/bpm/command.py` & `bin_package_manager-2.2.6/bpm/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
         raise e
 
 
 def cli_install(args):
     if args.interactive and args.quiet:
         log.error("Cannot use both --interactive and --quiet.")
         exit(1)
+    if args.quiet:
+        log.getLogger().setLevel(log.WARNING)
     if args.dry_run:
         set_dry_run()
     else:
         check_root()
     if args.local and len(args.packages) > 1:
         log.error(
             "Cannot install multiple packages from local. Please install them separately."
@@ -84,21 +86,21 @@
             log.error(f"Failed on searching `{package}`: {e}")
             trace()
             exit(1)
 
         # install
         try:
             download_and_install(args, repo)
-            log.info(f"Successfully installed `{repo.name}`.")
+            print(f"Successfully installed `{repo.name}`.")
             if WINDOWS:
                 bins = copy(repo.file_list)
                 bins = filter(lambda x: x.endswith(".lnk"), bins)
                 bins = map(lambda x: Path(x).stem, bins)
                 bins = map(lambda x: f"`{x}`", bins)
-                log.info(
+                print(
                     f"You can press `Win+r`, enter {', '.join(bins)} to start software, or execute in cmd."
                 )
             if not args.dry_run:
                 repo_group.insert_repo(repo)
         except Exception as e:
             log.error(f"Failed to install `{repo.name}`: {e}")
             trace()
```

### Comparing `bin_package_manager-2.2.5/bpm/install/__init__.py` & `bin_package_manager-2.2.6/bpm/install/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,32 +232,35 @@
         pbar.close()
         log.warning("Keyboard Cancelled")
         exit(1)
 
 
 def install_on_linux(
     path: Path,
-    # how about using multiple candidate bin_names : list[str] ?
+    # TODO: how about using multiple candidate bin_names : list[str] ?
     bin_name: str,
     one_bin: bool = False,
     rename: bool = True,
     recorder: Optional[list[str]] = None,
-    pkgdst=Path("/usr"),
+    pkgdst=Path("/"),
 ):
     """
     Install files to a linux system.
     1. Single binary
     2. System structure-like
     3. completions
+    4. services
 
     `path`: The "main path" dir of files to be installed.
     """
     assert LINUX, "Not a linux system"
     pkgdst = Path(pkgdst)
 
+    log.debug(f"install_on_linux() with params: {locals()}")
+
     def install_to(_from: Path, _to: Path, mode: Optional[int] = None):
         """
         install file to a folder.
         """
         install(
             _from,
             _to / _from.name,
@@ -267,70 +270,90 @@
         )
 
     def install_bin(p: Path):
         """Install binary file."""
         if hasattr(install_bin, "called"):
             log.debug(f"already installed {p.name}")
             return
-        install_to(p, pkgdst / "bin", mode=0o755)
+        install_to(p, pkgdst / "usr/bin", mode=0o755)
         install_bin.called = True
 
+    def install_service(p: Path):
+        """Install service file."""
+        install_to(p, pkgdst / "usr/lib/systemd/system/", mode=0o644)
+
     def install_completions(path: Path):
         """Install completions from a dir."""
         log.debug(f"installing completions from {path}")
         if not path.is_dir():
             log.warning(f"trying to install {path} as completions: not a directory")
             return
         with suppress(FileNotFoundError):
             for file in path.rglob("*.fish"):
                 # $fish_complete_path
-                install_to(file, pkgdst / "share/fish/vendor_completions.d", mode=0o644)
+                install_to(
+                    file, pkgdst / "usr/share/fish/vendor_completions.d", mode=0o644
+                )
         with suppress(FileNotFoundError):
             for file in path.rglob("*.bash"):
                 install_to(
-                    file, pkgdst / "share/bash-completion/completions", mode=0o644
+                    file, pkgdst / "usr/share/bash-completion/completions", mode=0o644
                 )
         with suppress(FileNotFoundError):
             for file in path.rglob("_*"):
                 if "zsh" in file.read_text():
-                    install_to(file, pkgdst / "share/zsh/site-functions", mode=0o644)
+                    install_to(
+                        file, pkgdst / "usr/share/zsh/site-functions", mode=0o644
+                    )
 
     first_layer: list[Path] = list(path.glob("*"))
     assert first_layer, f"{path} is empty"
 
     # 1. only install one bin
     if one_bin or len(first_layer) == 1:
-        bin = next(path.glob("*" if len(first_layer) == 1 else bin_name))
-        first_layer.remove(bin)
-        install_bin(bin)
-        if one_bin:
-            return
+        # if there is only one file (not dir), assert it's a binary file, whatever the name it is.
+        if len(first_layer) == 1 and first_layer[0].is_file():
+            bin = first_layer[0]
+        else:
+            bin = next(path.rglob(bin_name))
+        if bin is not None and bin.is_file():
+            log.debug(f"judge out bin: selected {bin}")
+            install_bin(bin)
+            bin.unlink()
+            if one_bin:
+                return
 
-    for file in first_layer:
+    for file in path.glob("*"):
         # 2. merge all files to coordinate position
-        if file.name == "lib":
-            merge_dir(file, pkgdst / "lib", rename=rename, recorder=recorder)
+        if file.name == "usr":
+            merge_dir(file, pkgdst / "usr", rename=rename, recorder=recorder)
+        elif file.name == "lib":
+            merge_dir(file, pkgdst / "usr/lib", rename=rename, recorder=recorder)
         elif file.name == "include":
-            merge_dir(file, pkgdst / "include", rename=rename, recorder=recorder)
+            merge_dir(file, pkgdst / "usr/include", rename=rename, recorder=recorder)
         elif file.name == "share":
-            merge_dir(file, pkgdst / "share", rename=rename, recorder=recorder)
+            merge_dir(file, pkgdst / "usr/share", rename=rename, recorder=recorder)
         elif file.name == "bin":
-            merge_dir(file, pkgdst / "bin", rename=rename, recorder=recorder)
+            merge_dir(file, pkgdst / "usr/bin", rename=rename, recorder=recorder)
         elif file.name == "man":
-            merge_dir(file, pkgdst / "share/man", rename=rename, recorder=recorder)
+            merge_dir(file, pkgdst / "usr/share/man", rename=rename, recorder=recorder)
         # 3. deal with other circumstance.
         else:
             name = file.name
             if name.startswith("complet"):
                 install_completions(file)
             elif name == bin_name and file.is_file():
                 install_bin(file)
             else:
                 log.debug(f"cannot match {name}.")
 
+    # 4 install service file
+    for file in path.rglob("*.service"):
+        install_service(file)
+
     # check binary
     if not any(map(lambda x: x.startswith("/usr/bin"), recorder)):
         log.warning("No binary file found, please check the release package.")
 
 
 def install_on_windows(
     repo: RepoHandler,
@@ -528,22 +551,22 @@
             fish_completion.mkdir(parents=True, exist_ok=True)
             bash_completion.mkdir(parents=True, exist_ok=True)
             zsh_completion.mkdir(parents=True, exist_ok=True)
             main = download_and_extract(
                 "https://github.com/eza-community/eza/releases/download/v0.17.2/eza_x86_64-unknown-linux-musl.tar.gz",
                 src,
             )
-            install_on_linux(main, "eza", pkgdst=usr)
+            install_on_linux(main, "eza", pkgdst=dst)
             self.assertTrue((bin / "eza").exists())
 
             main = download_and_extract(
                 "https://github.com/BurntSushi/ripgrep/releases/download/14.1.0/ripgrep-14.1.0-x86_64-unknown-linux-musl.tar.gz",
                 src,
             )
-            install_on_linux(main, "rg", pkgdst=usr)
+            install_on_linux(main, "rg", pkgdst=dst)
             for i in usr.rglob("*"):
                 log.debug(i) if i.is_file() else None
             self.assertTrue((bin / "rg").exists())
             self.assertTrue((fish_completion / "rg.fish").exists())
 
 
 if __name__ == "__main__":
```

### Comparing `bin_package_manager-2.2.5/bpm/lib/windowspathadder.py` & `bin_package_manager-2.2.6/bpm/lib/windowspathadder.py`

 * *Files identical despite different names*

### Comparing `bin_package_manager-2.2.5/bpm/search.py` & `bin_package_manager-2.2.6/bpm/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,16 +106,17 @@
 @functools.lru_cache()
 def platform_map() -> list:
     return [platform.system()]
 
 
 @functools.lru_cache()
 def architecture_map():
-    if platform.machine() == "AMD64":
-        return ["x86_64", "amd64"]
+    pair1 = ["x86_64", "amd64"]
+    if platform.machine() in pair1:
+        return pair1
     else:
         return [platform.machine()]
 
 
 class RepoHandler:
     def __init__(self, name: str, **kwargs):
         self.name = name
```

### Comparing `bin_package_manager-2.2.5/bpm/storage.py` & `bin_package_manager-2.2.6/bpm/storage.py`

 * *Files identical despite different names*

### Comparing `bin_package_manager-2.2.5/bpm/utils/__init__.py` & `bin_package_manager-2.2.6/bpm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bin_package_manager-2.2.5/bpm/utils/constants.py` & `bin_package_manager-2.2.6/bpm/utils/constants.py`

 * *Files identical despite different names*

### Comparing `bin_package_manager-2.2.5/bpm/utils/exceptions.py` & `bin_package_manager-2.2.6/bpm/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `bin_package_manager-2.2.5/pyproject.toml` & `bin_package_manager-2.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bin-package-manager"
-version = "2.2.5"
+version = "2.2.6"
 description = "Bin package manager, a package manager based on Github release"
 authors = ["lxl66566 <lxl66566@gmail.com>"]
 license = "MIT"
 readme = ["README.md"]
 keywords = ["binary", "packaging", "release"]
 repository = "https://github.com/lxl66566/bpm"
 homepage = "https://github.com/lxl66566/bpm"
```

### Comparing `bin_package_manager-2.2.5/PKG-INFO` & `bin_package_manager-2.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bin-package-manager
-Version: 2.2.5
+Version: 2.2.6
 Summary: Bin package manager, a package manager based on Github release
 Home-page: https://github.com/lxl66566/bpm
 License: MIT
 Keywords: binary,packaging,release
 Author: lxl66566
 Author-email: lxl66566@gmail.com
 Requires-Python: >=3.9,<4.0
```


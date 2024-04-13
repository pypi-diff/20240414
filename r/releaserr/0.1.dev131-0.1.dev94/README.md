# Comparing `tmp/releaserr-0.1.dev131.tar.gz` & `tmp/releaserr-0.1.dev94.tar.gz`

## Comparing `releaserr-0.1.dev131.tar` & `releaserr-0.1.dev94.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/.git_archival.txt
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/.gitattributes
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/CONTRIBUTING.md
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/noxfile.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/ruff.toml
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/.builds/main.yml
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/.reuse/dep5
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/__init__.py
--rwxr-xr-x   0        0        0    13538 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/__main__.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/cli_utils.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/config.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/copr.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/py.typed
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/scd.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/subprocess_util.py
--rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/toml.py
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/version.py
--rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/new/__init__.py
--rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/new/files.py
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/new/sourcehut.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/new/data/CONTRIBUTING.md.j2
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/new/data/NEWS.md.j2
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/new/data/NEWS_FRAGMENT.md.j2
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/new/data/README.md.j2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/new/data/__init__.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/new/data/app.spec.j2
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/new/data/blankmod.py.j2
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/new/data/builds-main.yml.j2
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/new/data/builds-mockbuild.yml.j2
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/new/data/copr-Makefile.j2
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/new/data/empty.j2
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/new/data/gitignore.j2
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/new/data/init.py.j2
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/new/data/library.spec.j2
--rw-r--r--   0        0        0     6277 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/new/data/noxfile.py.j2
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/new/data/pyproject.toml.j2
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/new/data/ruff.toml.j2
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/releaserr/new/data/test-placeholder.py.j2
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/.gitignore
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/README.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/pyproject.toml
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/LICENSES/MIT.txt
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/LICENSES/Unlicense.txt
--rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 releaserr-0.1.dev131/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/.gitattributes
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/noxfile.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/ruff.toml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/.builds/main.yml
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/.reuse/dep5
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/__init__.py
+-rwxr-xr-x   0        0        0    12269 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/__main__.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/cli_utils.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/config.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/copr.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/py.typed
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/scd.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/subprocess_util.py
+-rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/toml.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/version.py
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/new/__init__.py
+-rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/new/files.py
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/new/sourcehut.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/new/data/CONTRIBUTING.md.j2
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/new/data/FRAG.md.j2
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/new/data/NEWS.md.j2
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/new/data/README.md.j2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/new/data/__init__.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/new/data/app.spec.j2
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/new/data/blankmod.py.j2
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/new/data/builds-main.yml.j2
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/new/data/builds-mockbuild.yml.j2
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/new/data/copr-Makefile.j2
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/new/data/empty.j2
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/new/data/gitignore.j2
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/new/data/init.py.j2
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/new/data/library.spec.j2
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/new/data/noxfile.py.j2
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/new/data/pyproject.toml.j2
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/new/data/ruff.toml.j2
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/releaserr/new/data/test-placeholder.py.j2
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/.gitignore
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/README.md
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/pyproject.toml
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/LICENSES/Unlicense.txt
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 releaserr-0.1.dev94/PKG-INFO
```

### Comparing `releaserr-0.1.dev131/CONTRIBUTING.md` & `releaserr-0.1.dev94/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `releaserr-0.1.dev131/noxfile.py` & `releaserr-0.1.dev94/noxfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright (C) 2023 Maxwell G <maxwell@gtmx.me>
 # SPDX-License-Identifier: MIT
 from __future__ import annotations
 
-import os
 from pathlib import Path
 
 import nox
 
 LINT_FILES = ("releaserr/", "noxfile.py")
 LINT_SESSIONS = ("formatters", "codeqa", "typing")
 nox.options.sessions = (*LINT_SESSIONS, "integration")
@@ -34,39 +33,31 @@
 
 @nox.session
 def lint(session: nox.Session) -> None:
     for target in LINT_SESSIONS:
         session.notify(target)
 
 
-def _temp_repo(session: nox.Session) -> None:
-    session.run("git", "init", "--initial-branch=main", ".", external=True)
-    session.run("git", "add", ".", external=True)
-    session.run("git", "commit", "--no-gpg-sign", "-m", "init", external=True)
-
-
 @nox.session
 def integration(session: nox.Session) -> None:
     session.install(".", "nox", "reuse")
 
     tmp = session.create_tmp()
     project = Path(tmp, "testproj").resolve()
     session.run("rm", "-rf", str(project), external=True)
     with session.chdir(tmp):
         session.run(
             "releaserr", "new", "files", str(project), "--description=test project"
         )
     with session.chdir(project):
-        _temp_repo(session)
         session.run("nox", *session.posargs, env={"CI": "1"})
 
 
 @nox.session
 def publish(session: nox.Session) -> None:
     """
     Publish the current git snapshot to PyPI
     """
     session.install(".", "build", "twine")
     session.run("releaserr", "check-remote")
-    isolated = [] if "BUILD_SUBMITTER" in os.environ else ["--isolated"]
-    session.run("releaserr", "build", *isolated)
+    session.run("releaserr", "build", "--isolated")
     session.run("releaserr", "upload")
```

### Comparing `releaserr-0.1.dev131/releaserr/__main__.py` & `releaserr-0.1.dev94/releaserr/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,17 +70,14 @@
                 if frag_lines[0] != line:
                     lines.extend((*frag_lines, "\n"))
                 needs_append = False
             lines.append(line)
         if needs_append:
             lines.extend(("\n", *frag_lines))
         fp.seek(0)
-        # Ensure file ends with newline
-        if not lines[-1].endswith("\n"):
-            lines[-1] += "\n"
         fp.writelines(lines)
         fp.truncate()
     return frag_heading, raw_frag_lines
 
 
 def format_git_msg(project: str, version: str, raw_frag_lines: List[str]) -> List[str]:
     lines: list[str] = [f"{project} {version}\n", "\n"]
@@ -106,67 +103,50 @@
     tag = "v" + version
     tags = git(["tag", "--list"], capture_output=True).stdout.splitlines()
     if tag in tags:
         err(f"{tag} is already tagged")
         raise typer.Exit(1)
 
 
-def get_fragment_filename() -> Path:
-    for path in (Path("NEWS_FRAGMENT.md"), Path("FRAG.md")):
-        if path.is_file():
-            return path
-    err("NEWS_FRAGMENT.md does not exist!")
-    raise typer.Exit(1)
-
-
 @APP.command()
 def clog(
     *,
     version: str,
     git_msg_file: Path = Path("GIT_MSG"),
-    frag: Optional[Path] = None,
+    frag: Path = Path("FRAG.md"),
     output: Path = Path("NEWS.md"),
     project: str = Path.cwd().name,
     commit: bool = False,
     tag: bool = False,
-    ensure_clean_: bool = typer.Option(True, "--ensure-clean/--no-ensure-clean"),
-    v_prefix: bool = True,
 ) -> None:
-    """
-    Append changlog entries to a properly formatted NEWS.md file, and
-    optionally, create a git commit and tag
-    """
-    frag = frag or get_fragment_filename()
-    tag_name = "v" + version if v_prefix else version
     if tag:
         commit = True
     _, lines = add_frag(frag, output, version)
     with git_msg_file.open("w") as fp:
         fp.writelines(format_git_msg(project, version, lines))
     if tag or commit:
         git(["add", "NEWS.md"])
         git(["commit", "-S", "-m", f"Release {version}"])
     if tag:
-        if ensure_clean_:
-            ensure_clean()
+        ensure_clean()
         edit(filename=str(git_msg_file))
         if not git_msg_file.read_text().strip():
             err("Exiting...")
             raise typer.Exit(1)
-        git(["tag", "-s", "-F", git_msg_file, tag_name])
+        git(["tag", "-s", "-F", git_msg_file, f"v{version}"])
 
 
 class BuildBackend(TyperChoices):
     FLIT_CORE = "flit_core"
     HATCHLING = "hatchling"
     GENERIC = "generic"
 
 
 BUILD_COMMANDS: dict[BuildBackend, tuple["StrPath", ...]] = {
-    BuildBackend.FLIT_CORE: ("flit", "build", "--use-vcs"),
+    BuildBackend.FLIT_CORE: ("flit", "build"),
     BuildBackend.HATCHLING: ("hatch", "build"),
     BuildBackend.GENERIC: ("python", "-m", "build"),
 }
 
 
 @contextlib.contextmanager
 def chdir(directory: "StrPath") -> Iterator[Path]:
@@ -213,22 +193,18 @@
     backend: BuildBackend = BuildBackend.GENERIC,
     sign: bool = typer.Option(False, "-s", "--sign"),
     identity: Optional[str] = typer.Option(None, "-i", "--identity"),
     isolated: bool = typer.Option(
         False, "--isolated", help="Whether to build in an isolated directory"
     ),
     args: List[str] = typer.Option([], "-A", "--arg"),
-    ensure_clean_: bool = typer.Option(True, "--ensure-clean/--no-ensure-clean"),
-    dist_dir: Path = typer.Option(Path("dist/"), "--dist-dir", "-o", file_okay=False),
-    twine_check: bool = typer.Option(True, help="Whether to check dist with twine"),
 ) -> None:
-    if ensure_clean_:
-        ensure_clean()
+    ensure_clean()
 
-    if dist_dir.is_dir():
+    if Path("dist").is_dir():
         msg("Removing dist/")
         shutil.rmtree("dist/", True)
 
     if sign and not identity:
         identity = git(["config", "user.email"], capture_output=True).stdout.strip()
 
     build_command = (*BUILD_COMMANDS[backend], *args)
@@ -243,44 +219,37 @@
             sign_artifacts(artifacts, identity)
         if old is not None:
             shutil.copytree("dist/", old / "dist")
 
     for path in Path("dist").iterdir():
         CONSOLE.print(f"[blue]Output:[/blue] {path}")
 
-    if twine_check:
-        run(["twine", "check", "--strict", *artifacts])
+    run(["twine", "check", "--strict", *artifacts])
 
 
-@APP.command(name="upload")
-@APP.command(name="publish", help="Alias for upload")
+@APP.command()
 def upload(
     *,
     args: List[str] = typer.Option([], "-A", "--arg"),
-    dist_dir: Path = typer.Option(Path("dist/"), "--dist-dir", "-o", file_okay=False),
 ):
     """
     Upload Python distributions to PyPI
     """
-    args = args.copy()
+    dist = Path("dist")
     artifacts: list[Path] = []
     for patt in "*.tar.gz", "*.whl":
-        matches = list(dist_dir.glob(patt))
+        matches = list(dist.glob(patt))
         if len(matches) != 1:
             err("Did not find expected wheel and sdist")
             raise typer.Exit(1)
         artifacts.append(matches[0])
     for artifact in artifacts:
         CONSOLE.print(f"[blue]Found artifact:[/blue] {artifact}")
 
-    fargs: list[str] = []
-    if not sys.stdout.isatty():
-        fargs.append("--no-color")
-        args.insert(0, "--disable-progress-bar")
-    run(["twine", *fargs, "upload", *args, *artifacts])
+    run(["twine", "upload", *args, *artifacts])
 
 
 _SOURCE_ENUM: TypeAlias = TyperChoices(  # type: ignore
     "_SOURCE_ENUM",
     list(VERSION_SOURCES),
 )
 
@@ -442,15 +411,18 @@
     with contextlib.suppress(OSError):  # noqa: SIM117
         with open("pyproject.toml", "rb") as fp:
             data = load_toml(fp)
     tool_config: MutableMapping[str, Any] = data.get("tool", {}).get("releaserr", {})
     project_config: MutableMapping[str, Any] = data.get("project", {})
 
     if not name:
-        name = project_config["name"] if "name" in project_config else Path.cwd().name
+        if "name" in project_config:
+            name = project_config["name"]
+        else:
+            name = Path.cwd().name
 
     context.obj = CLIContext(
         cast(str, name),
         dict(project_config),
         dict(tool_config),
         ReleaserrConfig.read_config(),
     )
```

### Comparing `releaserr-0.1.dev131/releaserr/cli_utils.py` & `releaserr-0.1.dev94/releaserr/cli_utils.py`

 * *Files identical despite different names*

### Comparing `releaserr-0.1.dev131/releaserr/config.py` & `releaserr-0.1.dev94/releaserr/config.py`

 * *Files identical despite different names*

### Comparing `releaserr-0.1.dev131/releaserr/copr.py` & `releaserr-0.1.dev94/releaserr/copr.py`

 * *Files identical despite different names*

### Comparing `releaserr-0.1.dev131/releaserr/scd.py` & `releaserr-0.1.dev94/releaserr/scd.py`

 * *Files identical despite different names*

### Comparing `releaserr-0.1.dev131/releaserr/subprocess_util.py` & `releaserr-0.1.dev94/releaserr/subprocess_util.py`

 * *Files identical despite different names*

### Comparing `releaserr-0.1.dev131/releaserr/toml.py` & `releaserr-0.1.dev94/releaserr/toml.py`

 * *Files identical despite different names*

### Comparing `releaserr-0.1.dev131/releaserr/version.py` & `releaserr-0.1.dev94/releaserr/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,26 +56,24 @@
     PATTERN = re.compile(
         r'(?i)^(__version__|VERSION) *= *([\'"])v?(?P<version>.+?)\2',
         flags=re.MULTILINE,
     )
     version_file: Path
 
     def __post_init__(self) -> None:
-        project_name = self.project_name.replace("-", "_")
         version_file: Path | None = None
         if "version-file" in self.config:
             version_file = Path(self.config["version-file"])
         else:
             for path in (
-                Path("src", project_name, "__init__.py"),
-                Path(project_name, "__init__.py"),
+                Path("src", self.project_name, "__init__.py"),
+                Path(self.project_name, "__init__.py"),
             ):
                 if path.exists():
                     version_file = path
-                    break
         if not version_file:
             err("Failed to find version file!")
             raise Exit(1)
 
         self.version_file: Path = version_file
         self.changed_files = (self.version_file,)
```

### Comparing `releaserr-0.1.dev131/releaserr/new/__init__.py` & `releaserr-0.1.dev94/releaserr/new/__init__.py`

 * *Files identical despite different names*

### Comparing `releaserr-0.1.dev131/releaserr/new/files.py` & `releaserr-0.1.dev94/releaserr/new/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     Path(".builds/main.yml"): "builds-main.yml.j2",
     Path(".builds/mockbuild.yml"): "builds-mockbuild.yml.j2",
     Path(".builds/mockbuild-f37.yml"): "builds-mockbuild.yml.j2",
     Path(".builds/mockbuild-epel9.yml"): "builds-mockbuild.yml.j2",
     Path(".copr/Makefile"): "copr-Makefile.j2",
     Path(".gitignore"): "gitignore.j2",
     Path("CONTRIBUTING.md"): "CONTRIBUTING.md.j2",
-    Path("NEWS_FRAGMENT.md"): "NEWS_FRAGMENT.md.j2",
+    Path("FRAG.md"): "FRAG.md.j2",
     Path("NEWS.md"): "NEWS.md.j2",
     Path("README.md"): "README.md.j2",
     Path("ruff.toml"): "ruff.toml.j2",
     Path("pyproject.toml"): "pyproject.toml.j2",
     Path("noxfile.py"): "noxfile.py.j2",
     Path("tests/__init__.py"): "blankmod.py.j2",
 }
@@ -75,18 +75,14 @@
     name: str
     description: str
     path: Path
     build_backend: BUILD_BACKENDS
     license_id: str
     specfile_template: Optional[SPECFILE_TEMPLATES]
 
-    @property
-    def unname(self) -> str:
-        return self.name.replace("-", "_")
-
 
 def get_license_headers(config: FilesConfig, dt: DT) -> list[str]:
     # REUSE-IgnoreStart
     return [
         f"Copyright (C) {dt.year} Maxwell G <maxwell@gtmx.me>",
         f"SPDX-License-Identifier: {config.license_id}",
     ]
```

### Comparing `releaserr-0.1.dev131/releaserr/new/sourcehut.py` & `releaserr-0.1.dev94/releaserr/new/sourcehut.py`

 * *Files identical despite different names*

### Comparing `releaserr-0.1.dev131/releaserr/new/data/CONTRIBUTING.md.j2` & `releaserr-0.1.dev94/releaserr/new/data/CONTRIBUTING.md.j2`

 * *Files identical despite different names*

### Comparing `releaserr-0.1.dev131/releaserr/new/data/README.md.j2` & `releaserr-0.1.dev94/releaserr/new/data/README.md.j2`

 * *Files identical despite different names*

### Comparing `releaserr-0.1.dev131/releaserr/new/data/app.spec.j2` & `releaserr-0.1.dev94/releaserr/new/data/app.spec.j2`

 * *Files identical despite different names*

### Comparing `releaserr-0.1.dev131/releaserr/new/data/builds-main.yml.j2` & `releaserr-0.1.dev94/releaserr/new/data/builds-main.yml.j2`

 * *Files identical despite different names*

### Comparing `releaserr-0.1.dev131/releaserr/new/data/builds-mockbuild.yml.j2` & `releaserr-0.1.dev94/releaserr/new/data/builds-mockbuild.yml.j2`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 {% endfor %}
 ---
 
 image: fedora/latest
 packages:
   - mock
   - mock-core-configs
-  - nox
   - rpm-build
   - rpmdevtools
   - rpmlint
 sources:
   - "https://git.sr.ht/~gotmax23/{{ config.name }}"
 artifacts:
   - {{ config.name }}/results_{{ config.name }}.tar.gz
```

### Comparing `releaserr-0.1.dev131/releaserr/new/data/library.spec.j2` & `releaserr-0.1.dev94/releaserr/new/data/library.spec.j2`

 * *Files identical despite different names*

### Comparing `releaserr-0.1.dev131/releaserr/new/data/noxfile.py.j2` & `releaserr-0.1.dev94/releaserr/new/data/noxfile.py.j2`

 * *Files 4% similar despite different names*

```diff
@@ -21,26 +21,24 @@
 
 PROJECT = "{{ config.name.replace("-", "_") }}"
 {% if config.specfile_template %}
 SPECFILE = "{{ config.specfile_template.package_name(config.name) }}.spec"
 {% endif %}
 LINT_SESSIONS = ("formatters", "codeqa", "typing")
 LINT_FILES = (f"src/{PROJECT}", "tests/", "noxfile.py")
+RELEASERR = "releaserr[all] @ git+https://git.sr.ht/~gotmax23/releaserr"
+# RELEASERR = "-e../releaserr[all]"
 
-nox.options.sessions = ("lint", "covtest")
+nox.options.sessions = (*LINT_SESSIONS, "test")
 
 
 # Helpers
 
 
 def install(session: nox.Session, *args, editable=False, **kwargs):
-    # nox --no-venv
-    if isinstance(session.virtualenv, nox.virtualenv.PassthroughEnv):
-        session.warn(f"No venv. Skipping installation of {args}")
-        return
     if editable and ALLOW_EDITABLE:
         args = ("-e", *args)
     session.install(*args, **kwargs)
 
 
 def git(session: nox.Session, *args, **kwargs):
     return session.run("git", *args, **kwargs, external=True)
@@ -63,41 +61,31 @@
     session.run("pytest", *session.posargs, env=env)
 
 
 @nox.session
 def coverage(session: nox.Session):
     install(session, "coverage[toml]")
     session.run("coverage", "combine", "--keep", *iglob(".nox/test*/tmp/.coverage"))
-    session.run("coverage", "xml")
     session.run("coverage", "html")
     session.run("coverage", "report", "--fail-under=95")
 
 
-@nox.session()
-def covtest(session: nox.Session):
-    session.run("rm", "-f", *iglob(".nox/*/tmp/.coverage*"), external=True)
-    test_sessions = (f"test-{v}" for v in test.python)  # type: ignore[attr-defined]
-    for target in test_sessions:
-        session.notify(target, ["--cov"])
-    session.notify("coverage")
-
-
 @nox.session(venv_backend="none")
 def lint(session: nox.Session):
     """
     Run formatters, codeqa, and typing sessions
     """
     for notify in LINT_SESSIONS:
         session.notify(notify)
 
 
 @nox.session
 def codeqa(session: nox.Session):
     install(session, ".[codeqa]")
-    session.run("ruff", "check", *session.posargs, *LINT_FILES)
+    session.run("ruff", *session.posargs, *LINT_FILES)
     session.run("reuse", "lint")
 
 
 @nox.session
 def formatters(session: nox.Session):
     install(session, ".[formatters]")
     posargs = session.posargs
@@ -114,17 +102,17 @@
 
 
 @nox.session
 def bump(session: nox.Session):
     version = session.posargs[0]
 
 {% if config.build_backend.value == "flit_core" %}
-    install(session, "releaserr", "flit", "fclogr")
+    install(session, RELEASERR, "flit", "fclogr")
 {% else %}
-    install(session, "releaserr", "fclogr")
+    install(session, RELEASERR, "fclogr")
 {% endif %}
     session.run("releaserr", "--version")
 
     session.run("releaserr", "check-tag", version)
     session.run("releaserr", "ensure-clean")
     session.run("releaserr", "set-version", "-s", "file", version)
 
@@ -155,15 +143,15 @@
     session.run("releaserr", "build", "--sign", "--backend", "generic", "--isolated")
 {% endif %}
 
 
 @nox.session
 def publish(session: nox.Session):
     # Setup
-    install(session, "releaserr")
+    install(session, RELEASERR)
     session.run("releaserr", "--version")
 
     session.run("releaserr", "ensure-clean")
 
     # Upload to PyPI
     session.run("releaserr", "upload")
 
@@ -194,15 +182,15 @@
     session.run("copr-cli", "build", "--nowait", f"gotmax23/{PROJECT}", str(dest))
 
 
 @nox.session
 def srpm(session: nox.Session, posargs=None):
     install(session, "fclogr")
     posargs = posargs or session.posargs
-    session.run("python3", "-m", "fclogr", "--debug", "dev-srpm", *posargs, SPECFILE)
+    session.run("fclogr", "--debug", "dev-srpm", *posargs, SPECFILE)
 
 
 @nox.session
 def mockbuild(session: nox.Session):
     tmp = Path(session.create_tmp())
     srpm(session, ("-o", tmp, "--keep"))
     margs = [
@@ -215,12 +203,11 @@
     ]
     if not session.interactive:
         margs.append("--verbose")
     session.run(*margs, external=True)
 {% endif %}
 
 
-@nox.session
 def releaserr(session: nox.Session):
-    session.install("releaserr")
+    session.install(RELEASERR)
     session.run("releaserr", *session.posargs)
```

### Comparing `releaserr-0.1.dev131/releaserr/new/data/pyproject.toml.j2` & `releaserr-0.1.dev94/releaserr/new/data/pyproject.toml.j2`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 ]
 dependencies = [
 ]
 requires-python = ">=3.8"
 
 [project.optional-dependencies]
 codeqa = [
-    "ruff>=0.2.0",
+    "ruff",
     "reuse",
 ]
 formatters = [
     "black",
     "isort",
 ]
 typing = [
```

### Comparing `releaserr-0.1.dev131/releaserr/new/data/ruff.toml.j2` & `releaserr-0.1.dev94/releaserr/new/data/ruff.toml.j2`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,18 @@
 {% for header in license_headers %}
 # {{ header }}
 {% endfor %}
 
-src = [
-    "src",
-    "tests",
-]
-
-[lint]
 select = [
     "A",    # flake8-builtins
     "ARG",  # unused-arguments
     "B",    # flake8-bugbear
-    "DTZ",  # flake8-datetimez
     "E",    # pycodestyle errors
     "F",    # pyflakes
-    "PERF", # Perflint
     "PL",   # pylint
-    "RUF",  # Ruff's own rules
     "SIM",  # flake8-simplify
     "W",    # pycodestyle warnings
 ]
 ignore = [
     # function-call-in-default-argument
     # There's nothing wrong with calling a function that returns an immutable
     # object
@@ -32,22 +23,19 @@
     # Allow overwriting loop variable
     "PLW2901",
     # Magic value used in comparison
     # This is a good rule, but the checker is a bit overzealous.
     "PLR2004",
     # Too many arguments to function call
     "PLR0913",
-    # collection-literal-concatenation
-    # Sometimes, this is more elegant, and mypy already complains when we're
-    # doing something illegal
-    "RUF005",
-    # try-except-in-loop
-    # This is common when, for example, you want to ignore errors and move to
-    # the next loop iteration
-    "PERF203",
 ]
 
-[lint.extend-per-file-ignores]
+src = [
+    "src",
+    "tests",
+]
+
+[extend-per-file-ignores]
 "tests/*" = ["ARG"]
 {#
 # vim: ft=toml.jinja2:
 #}
```

### Comparing `releaserr-0.1.dev131/README.md` & `releaserr-0.1.dev94/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 Copyright (C) 2023 Maxwell G <maxwell@gtmx.me
 SPDX-License-Identifier: MIT
 -->
 
 # releaserr
 
 [![builds.sr.ht status](https://builds.sr.ht/~gotmax23/releaserr/commits/main.svg)](https://builds.sr.ht/~gotmax23/releaserr/commits/main?)
-[![PyPI - Version](https://img.shields.io/pypi/v/releaserr?logo=pypi&label=releaserr%20on%20PyPI&color=blue)](https://pypi.org/project/releaserr/)
 
-Simple, purpose-built release manager for @gotmax23's projects
+Collections, frozen mappings, and more
 
 ## Links
 
 - [releaserr project hub](https://sr.ht/~gotmax23/releaserr)
 - [releaserr git.sr.ht repo](https://git.sr.ht/~gotmax23/releaserr)
 - [releaserr tracker](https://todo.sr.ht/~gotmax23/releaserr)
 - [releaserr mailing list][archives] ([~gotmax/releaserr@lists.sr.ht][mailto])
```

### Comparing `releaserr-0.1.dev131/pyproject.toml` & `releaserr-0.1.dev94/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     "copr",
     "requests_gssapi",
 ]
 
 # Development
 
 codeqa = [
-    "ruff>=0.2.0",
+    "ruff",
     "reuse",
 ]
 formatters = [
     "black",
     "isort",
 ]
 typing = [
```

### Comparing `releaserr-0.1.dev131/LICENSES/MIT.txt` & `releaserr-0.1.dev94/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `releaserr-0.1.dev131/LICENSES/Unlicense.txt` & `releaserr-0.1.dev94/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `releaserr-0.1.dev131/PKG-INFO` & `releaserr-0.1.dev94/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: releaserr
-Version: 0.1.dev131
+Version: 0.1.dev94
 Summary: Simple, purpose-built release manager for @gotmax23's projects
 Author-email: Maxwell G <maxwell@gtmx.me>
 License-Expression: MIT AND Unlicense
 License-File: LICENSES/MIT.txt
 License-File: LICENSES/Unlicense.txt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -23,15 +23,15 @@
 Requires-Dist: typing-extensions
 Provides-Extra: all
 Requires-Dist: build; extra == 'all'
 Requires-Dist: tomlkit; extra == 'all'
 Requires-Dist: twine; extra == 'all'
 Provides-Extra: codeqa
 Requires-Dist: reuse; extra == 'codeqa'
-Requires-Dist: ruff>=0.2.0; extra == 'codeqa'
+Requires-Dist: ruff; extra == 'codeqa'
 Provides-Extra: copr
 Requires-Dist: copr; extra == 'copr'
 Requires-Dist: requests-gssapi; extra == 'copr'
 Provides-Extra: dev
 Requires-Dist: releaserr[all]; extra == 'dev'
 Requires-Dist: releaserr[codeqa]; extra == 'dev'
 Requires-Dist: releaserr[formatters]; extra == 'dev'
@@ -52,17 +52,16 @@
 Copyright (C) 2023 Maxwell G <maxwell@gtmx.me
 SPDX-License-Identifier: MIT
 -->
 
 # releaserr
 
 [![builds.sr.ht status](https://builds.sr.ht/~gotmax23/releaserr/commits/main.svg)](https://builds.sr.ht/~gotmax23/releaserr/commits/main?)
-[![PyPI - Version](https://img.shields.io/pypi/v/releaserr?logo=pypi&label=releaserr%20on%20PyPI&color=blue)](https://pypi.org/project/releaserr/)
 
-Simple, purpose-built release manager for @gotmax23's projects
+Collections, frozen mappings, and more
 
 ## Links
 
 - [releaserr project hub](https://sr.ht/~gotmax23/releaserr)
 - [releaserr git.sr.ht repo](https://git.sr.ht/~gotmax23/releaserr)
 - [releaserr tracker](https://todo.sr.ht/~gotmax23/releaserr)
 - [releaserr mailing list][archives] ([~gotmax/releaserr@lists.sr.ht][mailto])
```


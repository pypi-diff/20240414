# Comparing `tmp/dbrownell_DevTools-0.8.1-py3-none-any.whl.zip` & `tmp/dbrownell_DevTools-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8533 bytes, number of entries: 10
--rw-r--r--  2.0 unx     1707 b- defN 24-Feb-14 18:45 dbrownell_DevTools/BuildActivities.py
--rw-r--r--  2.0 unx     7460 b- defN 24-Feb-14 18:45 dbrownell_DevTools/PythonBuildActivities.py
--rw-r--r--  2.0 unx      326 b- defN 24-Feb-14 18:45 dbrownell_DevTools/__init__.py
--rw-r--r--  2.0 unx    12444 b- defN 24-Feb-14 18:45 dbrownell_DevTools/RepoBuildTools/Python.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-14 18:45 dbrownell_DevTools/RepoBuildTools/__init__.py
--rw-r--r--  2.0 unx     1071 b- defN 24-Feb-14 18:45 dbrownell_DevTools-0.8.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     2739 b- defN 24-Feb-14 18:45 dbrownell_DevTools-0.8.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-14 18:45 dbrownell_DevTools-0.8.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 24-Feb-14 18:45 dbrownell_DevTools-0.8.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      925 b- defN 24-Feb-14 18:45 dbrownell_DevTools-0.8.1.dist-info/RECORD
-10 files, 26783 bytes uncompressed, 6919 bytes compressed:  74.2%
+Zip file size: 10961 bytes, number of entries: 10
+-rw-r--r--  2.0 unx    11959 b- defN 24-Feb-16 15:36 dbrownell_DevTools/BuildActivities.py
+-rw-r--r--  2.0 unx     7460 b- defN 24-Feb-16 15:36 dbrownell_DevTools/PythonBuildActivities.py
+-rw-r--r--  2.0 unx      326 b- defN 24-Feb-16 15:36 dbrownell_DevTools/__init__.py
+-rw-r--r--  2.0 unx    14577 b- defN 24-Feb-16 15:36 dbrownell_DevTools/RepoBuildTools/Python.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-16 15:36 dbrownell_DevTools/RepoBuildTools/__init__.py
+-rw-r--r--  2.0 unx     1071 b- defN 24-Feb-16 15:36 dbrownell_DevTools-0.9.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2739 b- defN 24-Feb-16 15:36 dbrownell_DevTools-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Feb-16 15:36 dbrownell_DevTools-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-Feb-16 15:36 dbrownell_DevTools-0.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      926 b- defN 24-Feb-16 15:36 dbrownell_DevTools-0.9.0.dist-info/RECORD
+10 files, 39169 bytes uncompressed, 9347 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: dbrownell_DevTools/RepoBuildTools/Python.py
 Comment: 
 
 Filename: dbrownell_DevTools/RepoBuildTools/__init__.py
 Comment: 
 
-Filename: dbrownell_DevTools-0.8.1.dist-info/LICENSE.txt
+Filename: dbrownell_DevTools-0.9.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dbrownell_DevTools-0.8.1.dist-info/METADATA
+Filename: dbrownell_DevTools-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: dbrownell_DevTools-0.8.1.dist-info/WHEEL
+Filename: dbrownell_DevTools-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: dbrownell_DevTools-0.8.1.dist-info/top_level.txt
+Filename: dbrownell_DevTools-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dbrownell_DevTools-0.8.1.dist-info/RECORD
+Filename: dbrownell_DevTools-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dbrownell_DevTools/BuildActivities.py

```diff
@@ -9,20 +9,30 @@
 # |
 # |  Copyright David Brownell 2024
 # |  Distributed under the MIT License.
 # |
 # ----------------------------------------------------------------------
 """Functionality often invoked as part of a build process"""
 
+import os
+import textwrap
+import uuid
+
+from contextlib import contextmanager
+from datetime import datetime
 from pathlib import Path
-from typing import Callable, Optional
+from typing import Callable, Generator, Optional, Protocol
 
 from AutoGitSemVer.Lib import GetSemanticVersion  # type: ignore [import-untyped]
+from dbrownell_Common.ContextlibEx import ExitStack  # type: ignore [import-untyped]
+from dbrownell_Common import PathEx  # type: ignore [import-untyped]
 from dbrownell_Common.Streams.DoneManager import DoneManager  # type: ignore[import-untyped]
+from dbrownell_Common import SubprocessEx  # type: ignore [import-untyped]
 from semantic_version import Version as SemVer  # type: ignore [import-untyped]
+import git
 
 
 # ----------------------------------------------------------------------
 def UpdateVersion(
     dm: DoneManager,
     source_root: Path,
     version_filename: Path,
@@ -44,7 +54,333 @@
         with version_filename.open("r") as f:
             content = f.read()
 
         content = version_replacement_func(content, semantic_version)
 
         with version_filename.open("w") as f:
             f.write(content)
+
+
+# ----------------------------------------------------------------------
+class CreateBaseImageFunc(Protocol):
+    """Callback passed to CreateDockerImage."""
+
+    def __call__(
+        self,
+        dm: DoneManager,
+    ) -> Generator[str, None, None]:
+        """\
+        Creates a base image to use as the foundation for the docker image.
+
+        Returns (image_name, True if the docker image should be deleted)
+        """
+        ...  # pragma: no cover
+
+
+def CreateDockerImage(
+    dm: DoneManager,
+    repo_root: Path,
+    create_base_image_func: Optional[CreateBaseImageFunc] = None,
+    bootstrap_args: str = "--package",
+    name_suffix: Optional[str] = None,  # Decorates the docker image name and output file
+) -> None:
+    create_base_image_func = create_base_image_func or _CreateDefaultBaseImage  # type: ignore
+    name_suffix = name_suffix or ""
+
+    # Extract the repo name
+    repo_name: Optional[str] = None
+
+    with dm.Nested(
+        "Extracting repository info...",
+        lambda: repo_name or "<Error>",
+    ):
+        repo = git.Repo(repo_root)
+
+        repo_name = repo.remotes.origin.url.split(".git")[0].split("/")[-1]
+
+    # Create the base image
+    with create_base_image_func(dm) as base_image_name:  # type: ignore
+        if dm.result != 0:
+            return
+
+        with _CreateDockerContainer(dm, repo_root, bootstrap_args, base_image_name) as container_id:
+            if dm.result != 0:
+                return
+
+            with _SaveTemporaryImage(dm, container_id) as temporary_image_id:
+                if dm.result != 0:
+                    return
+
+                with _CreateFinalImage(
+                    dm,
+                    name_suffix,
+                    repo_name,
+                    temporary_image_id,
+                ) as final_image_id:
+                    if dm.result != 0:
+                        return
+
+                    _ExtractImage(
+                        dm,
+                        repo_root,
+                        name_suffix,
+                        final_image_id,
+                    )
+
+
+# ----------------------------------------------------------------------
+def StreamCommand(
+    dm: DoneManager,
+    header: str,
+    command_line: str,
+    *suffix_funcs,
+    cwd: Optional[Path] = None,
+) -> None:
+    with dm.Nested(
+        header,
+        list(suffix_funcs),
+        suffix="\n",
+    ) as this_dm:
+        this_dm.WriteVerbose("Command Line: {}\n\n".format(command_line))
+
+        with this_dm.YieldStream() as stream:
+            this_dm.result = SubprocessEx.Stream(
+                command_line,
+                stream,
+                cwd=cwd,
+            )
+
+
+# ----------------------------------------------------------------------
+# ----------------------------------------------------------------------
+# ----------------------------------------------------------------------
+@contextmanager
+def _CreateDefaultBaseImage(
+    dm: DoneManager,
+) -> Generator[str, None, None]:
+    unique_id = str(uuid.uuid4()).replace("-", "")
+
+    docker_filename = Path(f"{unique_id}.dockerfile")
+
+    with dm.Nested("Creating base image Dockerfile..."):
+        with docker_filename.open("w") as f:
+            f.write(
+                textwrap.dedent(
+                    """\
+                    FROM ubuntu:latest
+
+                    RUN apt-get update \
+                     && apt-get install -y \
+                            build-essential \
+                            curl \
+                            git \
+                     && apt-get clean \
+                     && rm -rf /var/lib/apt/lists/*
+
+                    SHELL ["/bin/bash", "-c"]
+                    """,
+                ),
+            )
+
+    with ExitStack(docker_filename.unlink):
+        StreamCommand(
+            dm,
+            "Building base image...",
+            f"docker build --tag {unique_id} --file {docker_filename.name} .",
+        )
+
+        if dm.result != 0:
+            yield ""
+            return
+
+        with ExitStack(
+            lambda: StreamCommand(
+                dm,
+                "Deleting base image...",
+                f"docker image rm {unique_id}",
+            ),
+        ):
+            yield unique_id
+
+
+# ----------------------------------------------------------------------
+@contextmanager
+def _CreateDockerContainer(
+    dm: DoneManager,
+    repo_root: Path,
+    bootstrap_args: str,
+    base_image_name: str,
+) -> Generator[str, None, None]:
+    unique_id = str(uuid.uuid4()).replace("-", "")
+
+    script_filename = repo_root / f"{unique_id}.sh"
+
+    with dm.Nested("Creating initialization script..."):
+        with script_filename.open("w", newline="\n") as f:
+            f.write(
+                textwrap.dedent(
+                    f"""\
+                    #!/bin/bash
+
+                    git clone /local code
+
+                    cd code
+                    ./Bootstrap.sh {bootstrap_args}
+
+                    echo "source /code/Activate.sh" >> /etc/bash.bashrc
+
+                    . ./Activate.sh
+                    pip cache purge
+                    micromamba clean --all --force-pkgs-dirs --quiet --trash --yes
+                    """,
+                ),
+            )
+
+        script_filename.chmod(0o755)
+
+    with ExitStack(script_filename.unlink):
+        # Run docker and invoke the initialization script
+        StreamCommand(
+            dm,
+            "Creating the temporary container...",
+            f'docker run --name {unique_id} --volume "{repo_root}:/local" {base_image_name} /local/{script_filename.name}',
+        )
+
+        if dm.result != 0:
+            yield ""
+            return
+
+    with ExitStack(
+        lambda: StreamCommand(
+            dm,
+            "Deleting the temporary container...",
+            f"docker container rm {unique_id}",
+        ),
+    ):
+        yield unique_id
+
+
+# ----------------------------------------------------------------------
+@contextmanager
+def _SaveTemporaryImage(
+    dm: DoneManager,
+    container_id: str,
+) -> Generator[str, None, None]:
+    unique_id = str(uuid.uuid4()).replace("-", "")
+
+    StreamCommand(
+        dm,
+        "Saving temporary image...",
+        f"docker commit {container_id} {unique_id}",
+    )
+
+    if dm.result != 0:
+        yield ""
+        return
+
+    with ExitStack(
+        lambda: StreamCommand(
+            dm,
+            "Deleting temporary image...",
+            f"docker image rm {unique_id}",
+        ),
+    ):
+        yield unique_id
+
+
+# ----------------------------------------------------------------------
+@contextmanager
+def _CreateFinalImage(
+    dm: DoneManager,
+    name_suffix: str,
+    repo_name: str,
+    temporary_image_id: str,
+) -> Generator[str, None, None]:
+    now = datetime.now()
+    image_name = f"{repo_name}{name_suffix}-{now.year:04d}.{now.month:02d}.{now.day:02d}-{now.hour:02d}.{now.minute:02d}.{now.second:02d}".lower()
+
+    docker_filename = Path(f"{image_name}.dockerfile")
+
+    with dm.Nested("Creating final Dockerfile..."):
+        with docker_filename.open("w") as f:
+            f.write(
+                textwrap.dedent(
+                    f"""\
+                    FROM {temporary_image_id}
+
+                    WORKDIR /code
+
+                    ENTRYPOINT ["/bin/bash", "--login"]
+                    """,
+                ),
+            )
+
+    with ExitStack(docker_filename.unlink):
+        StreamCommand(
+            dm,
+            "Building final image...",
+            f"docker build --tag {image_name} --file {docker_filename.name} .",
+        )
+
+        if dm.result != 0:
+            yield ""
+            return
+
+        with ExitStack(
+            lambda: StreamCommand(
+                dm,
+                "Deleting final image...",
+                f"docker image rm {image_name}",
+            ),
+        ):
+            yield image_name
+
+
+# ----------------------------------------------------------------------
+def _ExtractImage(
+    dm: DoneManager,
+    repo_root: Path,
+    name_suffix: str,
+    final_image_id: str,
+) -> None:
+    if os.name == "nt":
+        compressed_filename = repo_root / f"docker_image{name_suffix}.tar"
+
+        # ----------------------------------------------------------------------
+        def Postprocess():
+            with ExitStack(compressed_filename.unlink):
+                # Zip the tarball
+                final_filename = compressed_filename.with_suffix(".tar.zip")
+
+                if final_filename.is_file():
+                    with dm.Nested("Removing previous compressed docker image..."):
+                        final_filename.unlink()
+
+                StreamCommand(
+                    dm,
+                    "Compressing docker image...",
+                    f'PowerShell -Command "Compress-Archive -Path {compressed_filename} -DestinationPath {final_filename}"',
+                    lambda: PathEx.GetSizeDisplay(final_filename),
+                )
+
+        # ----------------------------------------------------------------------
+
+        postprocess_func = Postprocess
+    else:
+        compressed_filename = repo_root / f"docker_image{name_suffix}.tar.gz"
+        postprocess_func = lambda *args, **kwargs: None
+
+    if compressed_filename.is_file():
+        with dm.Nested("Removing previous docker image..."):
+            compressed_filename.unlink()
+
+    StreamCommand(
+        dm,
+        "Saving docker image...",
+        f'docker save --output "{compressed_filename}" {final_image_id}',
+        lambda: PathEx.GetSizeDisplay(compressed_filename),
+    )
+
+    if dm.result != 0:
+        return
+
+    postprocess_func()
```

## dbrownell_DevTools/__init__.py

```diff
@@ -1,6 +1,6 @@
 # pylint: disable=missing-module-docstring,invalid-name
 
 # Note that this value will be overwritten by calls to `python ../../Build.py UpdateVersion` based
 # on changes observed in the git repository. The default value below will be used until the value
 # here is explicitly updated as part of a commit.
-__version__ = "0.8.1"
+__version__ = "0.9.0"
```

## dbrownell_DevTools/RepoBuildTools/Python.py

```diff
@@ -39,15 +39,15 @@
 
 # ----------------------------------------------------------------------
 # |
 # |  Public Functions
 # |
 # ----------------------------------------------------------------------
 def BlackFuncFactory(
-    source_root: Path,
+    repo_root: Path,  # given /src/<package_name>, repo_root is /
     app: typer.Typer,
 ) -> Callable:
     # ----------------------------------------------------------------------
     @app.command("black", no_args_is_help=False)
     def Black(
         format: Annotated[  # pylint: disable=redefined-builtin
             bool,
@@ -62,26 +62,26 @@
         """Runs black on the python code."""
 
         with DoneManager.CreateCommandLine(
             flags=DoneManagerFlags.Create(verbose=verbose, debug=debug),
         ) as dm:
             PythonBuildActivities.Black(
                 dm,
-                source_root,
+                repo_root,
                 format_sources=format,
             )
 
     # ----------------------------------------------------------------------
 
     return Black
 
 
 # ----------------------------------------------------------------------
 def PylintFuncFactory(
-    source_root: Path,
+    package_root: Path,  # given /src/<package_name>, package_root is /src/<package_name>
     app: typer.Typer,
     default_min_score: float = 9.5,
 ) -> Callable:
     # ----------------------------------------------------------------------
     @app.command("pylint", no_args_is_help=False)
     def Pylint(
         min_score: Annotated[
@@ -99,26 +99,26 @@
         """Runs pylint on the python code."""
 
         with DoneManager.CreateCommandLine(
             flags=DoneManagerFlags.Create(verbose=verbose, debug=debug),
         ) as dm:
             PythonBuildActivities.Pylint(
                 dm,
-                source_root,
+                package_root,
                 min_score,
             )
 
     # ----------------------------------------------------------------------
 
     return Pylint
 
 
 # ----------------------------------------------------------------------
 def PytestFuncFactory(
-    test_root: Path,
+    test_root: Path,  # given /src/<package_name> and /tests, test_root is /tests
     cov_name: str,
     app: typer.Typer,
     default_min_coverage: float = 95.0,
 ) -> Callable:
     # ----------------------------------------------------------------------
     @app.command("pytest", no_args_is_help=False)
     def Pytest(
@@ -155,15 +155,15 @@
     # ----------------------------------------------------------------------
 
     return Pytest
 
 
 # ----------------------------------------------------------------------
 def UpdateVersionFuncFactory(
-    source_root: Path,
+    source_root: Path,  # given /src/<package_name>, source_root is /src
     init_filename: Path,
     app: typer.Typer,
 ) -> Callable:
     assert source_root.is_dir(), source_root
     assert init_filename.is_file(), init_filename
     assert PathEx.IsDescendant(init_filename, source_root), (init_filename, source_root)
 
@@ -203,15 +203,15 @@
     # ----------------------------------------------------------------------
 
     return UpdateVersion
 
 
 # ----------------------------------------------------------------------
 def PackageFuncFactory(
-    source_root: Path,
+    repo_root: Path,  # given /src/<package_name>, repo_root is /
     app: typer.Typer,
 ) -> Callable:
     # ----------------------------------------------------------------------
     @app.command("package", no_args_is_help=False)
     def Package(
         additional_args: Annotated[
             Optional[str],
@@ -223,26 +223,26 @@
         """Builds the python package."""
 
         with DoneManager.CreateCommandLine(
             flags=DoneManagerFlags.Create(verbose=verbose, debug=debug),
         ) as dm:
             PythonBuildActivities.Package(
                 dm,
-                source_root,
+                repo_root,
                 additional_args,
             )
 
     # ----------------------------------------------------------------------
 
     return Package
 
 
 # ----------------------------------------------------------------------
 def PublishFuncFactory(
-    source_root: Path,
+    repo_root: Path,  # given /src/<package_name>, repo_root is /
     app: typer.Typer,
 ) -> Callable:
     # ----------------------------------------------------------------------
     @app.command("publish", no_args_is_help=False)
     def Publish(
         pypi_api_token: Annotated[
             str,
@@ -260,27 +260,27 @@
         """Publishes the python package."""
 
         with DoneManager.CreateCommandLine(
             flags=DoneManagerFlags.Create(verbose=verbose, debug=debug),
         ) as dm:
             PythonBuildActivities.Publish(
                 dm,
-                source_root,
+                repo_root,
                 pypi_api_token,
                 production=production,
             )
 
     # ----------------------------------------------------------------------
 
     return Publish
 
 
 # ----------------------------------------------------------------------
 def BuildBinaryFuncFactory(
-    source_root: Path,
+    repo_root: Path,  # given /src/<package_name>, repo_root is /
     build_filename: Path,
     app: typer.Typer,
 ) -> Callable:
     # ----------------------------------------------------------------------
     @app.command("build_binary", no_args_is_help=False)
     def BuildBinary(
         verbose: Annotated[bool, _verbose_typer_option] = False,
@@ -290,25 +290,25 @@
 
         with DoneManager.CreateCommandLine(
             flags=DoneManagerFlags.Create(verbose=verbose, debug=debug),
         ) as dm:
             PythonBuildActivities.BuildBinary(
                 dm,
                 build_filename,
-                source_root / "build",
+                repo_root / "build",
             )
 
     # ----------------------------------------------------------------------
 
     return BuildBinary
 
 
 # ----------------------------------------------------------------------
 def BuildBinariesFuncFactory(
-    source_root: Path,
+    repo_root: Path,  # given /src/<package_name>, repo_root is /
     build_filenames: dict[str, Path],
     app: typer.Typer,
 ) -> Callable:
     # Create an enumeration of the build names
     enum_type = Enum("BuildNames", {item: item for item in build_filenames})  # type: ignore
 
     # ----------------------------------------------------------------------
@@ -334,16 +334,63 @@
                 with dm.Nested(
                     "Building '{}' ({} of {})...".format(build_name, index + 1, len(binary_names)),
                     suffix="\n",
                 ) as this_dm:
                     PythonBuildActivities.BuildBinary(
                         this_dm,
                         build_filename,
-                        source_root / "build" / build_name,
+                        repo_root / "build" / build_name,
                     )
 
-                    if this_dm.result != 0:
-                        return
-
     # ----------------------------------------------------------------------
 
     return BuildBinaries
+
+
+# ----------------------------------------------------------------------
+def CreateDockerImageFuncFactory(
+    repo_root: Path,  # Given /src/<package_name>, repo_root is /
+    app: typer.Typer,
+    create_base_image_func: Optional[BuildActivities.CreateBaseImageFunc] = None,
+    default_bootstrap_args: str = "--package",
+) -> Callable:
+    # ----------------------------------------------------------------------
+    @app.command("create_docker_image", no_args_is_help=False)
+    def CreateDockerImage(
+        name_suffix: Annotated[
+            Optional[str],
+            typer.Option(
+                "--name-suffix",
+                help="Suffix to apply to the generated image name",
+            ),
+        ] = None,
+        bootstrap_args: Annotated[
+            Optional[str],
+            typer.Option(
+                "--bootstrap-args",
+                help="Additional arguments passed to the bootstrap command.",
+            ),
+        ] = None,
+        verbose: Annotated[bool, _verbose_typer_option] = False,
+        debug: Annotated[bool, _debug_typer_option] = False,
+    ) -> None:
+        """Creates a docker image for the repository."""
+
+        with DoneManager.CreateCommandLine(
+            flags=DoneManagerFlags.Create(verbose=verbose, debug=debug),
+        ) as dm:
+            final_bootstrap_args = default_bootstrap_args
+
+            if bootstrap_args:
+                final_bootstrap_args += f" {bootstrap_args}"
+
+            BuildActivities.CreateDockerImage(
+                dm,
+                repo_root,
+                create_base_image_func,
+                final_bootstrap_args,
+                name_suffix or None,
+            )
+
+    # ----------------------------------------------------------------------
+
+    return CreateDockerImage
```

## Comparing `dbrownell_DevTools-0.8.1.dist-info/LICENSE.txt` & `dbrownell_DevTools-0.9.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `dbrownell_DevTools-0.8.1.dist-info/METADATA` & `dbrownell_DevTools-0.9.0.dist-info/METADATA`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbrownell_DevTools
-Version: 0.8.1
+Version: 0.9.0
 Summary: Foundation for various development tools.
 Author-email: David Brownell <db@DavidBrownell.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/davidbrownell/dbrownell_DevTools
 Project-URL: Documentation, https://github.com/davidbrownell/dbrownell_DevTools
 Project-URL: Repository, https://github.com/davidbrownell/dbrownell_DevTools
 Classifier: Development Status :: 4 - Beta
```

## Comparing `dbrownell_DevTools-0.8.1.dist-info/RECORD` & `dbrownell_DevTools-0.9.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-dbrownell_DevTools/BuildActivities.py,sha256=fRkAswTK6ww8D0loAo6Me00GCxtdT_RXo0e-cv6s1tk,1707
+dbrownell_DevTools/BuildActivities.py,sha256=EHYvRL1-CZrInOzVeVfUg-quZMhCnZ10aRZz2QbHwg4,11959
 dbrownell_DevTools/PythonBuildActivities.py,sha256=ZdA-fOUV3Kyd-cJBAOkoMBru_tWRek-4GgzVrKFdO28,7460
-dbrownell_DevTools/__init__.py,sha256=-UmTaP23HDOCQSf900WMvL4m9_7lZjbsJiuR7RFPa28,326
-dbrownell_DevTools/RepoBuildTools/Python.py,sha256=7cbdxQcWEfA1tTnOIqjqCD2-rbRuBWoaTsGJMAvya48,12444
+dbrownell_DevTools/__init__.py,sha256=-9tGWXGlEs_AgRfK-WvkfWVaa1AW7QKztCrnXZW1jK4,326
+dbrownell_DevTools/RepoBuildTools/Python.py,sha256=rB3LaReYZdJIEIQDJPRm4jiU8HBiBgrZhjGo8MVO9YQ,14577
 dbrownell_DevTools/RepoBuildTools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dbrownell_DevTools-0.8.1.dist-info/LICENSE.txt,sha256=6ycKI8SWG920Saey4PGi5YUVLX0C_8hfqJr7Q0sqGI8,1071
-dbrownell_DevTools-0.8.1.dist-info/METADATA,sha256=B_tVCMgtThyxVkQdJ2MAV4Ft1TL2uCOVLaUlOqMuczo,2739
-dbrownell_DevTools-0.8.1.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-dbrownell_DevTools-0.8.1.dist-info/top_level.txt,sha256=QjTAbRmAb0uclURJ_LCxogyut0QQrri6Q2NPDZ8JKGU,19
-dbrownell_DevTools-0.8.1.dist-info/RECORD,,
+dbrownell_DevTools-0.9.0.dist-info/LICENSE.txt,sha256=6ycKI8SWG920Saey4PGi5YUVLX0C_8hfqJr7Q0sqGI8,1071
+dbrownell_DevTools-0.9.0.dist-info/METADATA,sha256=_oeU7EOJTqJIOYjpN65fnUX4QffgFl73ZVwbzBpDZU8,2739
+dbrownell_DevTools-0.9.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+dbrownell_DevTools-0.9.0.dist-info/top_level.txt,sha256=QjTAbRmAb0uclURJ_LCxogyut0QQrri6Q2NPDZ8JKGU,19
+dbrownell_DevTools-0.9.0.dist-info/RECORD,,
```


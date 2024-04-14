# Comparing `tmp/betatester-0.0.0.tar.gz` & `tmp/betatester-0.0.1.tar.gz`

## Comparing `betatester-0.0.0.tar` & `betatester-0.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 betatester-0.0.0/src/betatester/__init__.py
--rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 betatester-0.0.0/src/betatester/betatester_types.py
--rw-r--r--   0        0        0     6294 2020-02-02 00:00:00.000000 betatester-0.0.0/src/betatester/cli.py
--rw-r--r--   0        0        0    30139 2020-02-02 00:00:00.000000 betatester-0.0.0/src/betatester/execution.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 betatester-0.0.0/src/betatester/model.py
--rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 betatester-0.0.0/src/betatester/prompts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 betatester-0.0.0/src/betatester/file/__init__.py
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 betatester-0.0.0/src/betatester/file/local.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 betatester-0.0.0/.gitignore
--rw-r--r--   0        0        0    10932 2020-02-02 00:00:00.000000 betatester-0.0.0/LICENSE
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 betatester-0.0.0/README.md
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 betatester-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     5576 2020-02-02 00:00:00.000000 betatester-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 betatester-0.0.1/src/betatester/__init__.py
+-rw-r--r--   0        0        0     7252 2020-02-02 00:00:00.000000 betatester-0.0.1/src/betatester/betatester_types.py
+-rw-r--r--   0        0        0     6615 2020-02-02 00:00:00.000000 betatester-0.0.1/src/betatester/cli.py
+-rw-r--r--   0        0        0    29848 2020-02-02 00:00:00.000000 betatester-0.0.1/src/betatester/execution.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 betatester-0.0.1/src/betatester/model.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 betatester-0.0.1/src/betatester/prompts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 betatester-0.0.1/src/betatester/file/__init__.py
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 betatester-0.0.1/src/betatester/file/local.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 betatester-0.0.1/.gitignore
+-rw-r--r--   0        0        0    10932 2020-02-02 00:00:00.000000 betatester-0.0.1/LICENSE
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 betatester-0.0.1/README.md
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 betatester-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 betatester-0.0.1/PKG-INFO
```

### Comparing `betatester-0.0.0/src/betatester/betatester_types.py` & `betatester-0.0.1/src/betatester/betatester_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 from abc import abstractmethod
 from enum import Enum
 from typing import Literal, Optional, Union, cast
 from uuid import UUID
 
-from pydantic import BaseModel, model_serializer
+from pydantic import BaseModel, field_serializer, model_serializer
 
 
 class SpecialInstruction(str, Enum):
     WAIT = "WAIT"
     DONE = "DONE"
 
 
@@ -221,21 +221,27 @@
         return output
 
 
 ScrapeEvent = Union[Action, SpecialInstruction]
 
 
 class ScrapeSpec(BaseModel):
+    original_scrape_id: UUID
     url: str
+    high_level_goal: str
     scrape_events: list[ScrapeEvent]
     variables: ScrapeVariables
     files: ScrapeFiles
     viewport_width: int
     viewport_height: int
 
+    @field_serializer("original_scrape_id", when_used="always")
+    def serialize_original_scrape_id(original_scrape_id: UUID) -> str:  # type: ignore
+        return str(original_scrape_id)
+
 
 class ExecutorMessage(BaseModel):
     step_id: Optional[UUID] = None
     scrape_page_view_count: Optional[int] = None
     scrape_action_count: Optional[int] = None
     next_step: Optional[str] = None
     action: Optional[Action] = None
@@ -263,22 +269,14 @@
         raise NotImplementedError()
 
     @abstractmethod
     async def save_trace(self, scrape_id: UUID, tmp_trace_path: str) -> str:
         raise NotImplementedError()
 
     @abstractmethod
-    async def save_scrape_spec(self, scrape_id: UUID, spec: ScrapeSpec) -> str:
-        raise NotImplementedError()
-
-    @abstractmethod
-    async def load_scrape_spec(self, path: str) -> ScrapeSpec:
-        raise NotImplementedError()
-
-    @abstractmethod
     def img_path(self, scrape_id: UUID, step_id: UUID) -> str:
         raise NotImplementedError()
 
     @abstractmethod
     def trace_path(self, scrape_id: UUID) -> str:
         raise NotImplementedError()
```

### Comparing `betatester-0.0.0/src/betatester/cli.py` & `betatester-0.0.1/src/betatester/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,41 +49,50 @@
 
         return LocalFileClient(save_path)
     else:
         raise ValueError(f"Invalid file provider: {file_client}")
 
 
 def _run_scraper(scraper: Union[ScrapeAiExecutor, ScrapeSpecExecutor]):
+    output = None
     try:
-        asyncio.run(scraper.run())
+        output = asyncio.run(scraper.run())
         print()
         print("Test [bold green]completed[/bold green] successfully!")
     except Exception as e:
         print()
         print(f"Test [bold red]failed[/bold red] with error: {e}")
 
+    return output
+
 
 @app.command("start_ai", no_args_is_help=True)
 def start_ai(
     url: Annotated[str, typer.Option(help="URL to test")],
     high_level_goal: Annotated[
         str,
         typer.Option(help="High level goal to accomplish at url"),
     ],
     max_page_views: Annotated[
-        Optional[int],
-        typer.Option(help="Max page views to take across the entire test"),
+        int,
+        typer.Option(
+            help="Max page views to take across the entire test. Set to 0 for no limit."
+        ),
     ] = 10,
     max_total_actions: Annotated[
-        Optional[int],
-        typer.Option(help="Max total actions to take across the entire test"),
+        int,
+        typer.Option(
+            help="Max total actions to take across the entire test. Set to 0 for no limit."
+        ),
     ] = 20,
     max_action_attempts_per_step: Annotated[
-        Optional[int],
-        typer.Option(help="Max actions to take on a single page"),
+        int,
+        typer.Option(
+            help="Max actions to take on a single page. Set to 0 for no limit."
+        ),
     ] = 5,
     viewport_width: Annotated[
         int, typer.Option(help="Viewport width in pixels")
     ] = 1280,
     viewport_height: Annotated[
         int, typer.Option(help="Viewport height in pixels")
     ] = 720,
@@ -151,26 +160,30 @@
         files=files_loaded,
         openai_api_key=openai_api_key,
         file_client=file_client,
         save_playwright_trace=save_playwright_trace,
         headless=not view_browser,
     )
 
-    _run_scraper(scraper)
+    output = _run_scraper(scraper)
+    if output is not None:
+        return output
 
 
 @app.command("start_spec", no_args_is_help=True)
 def start_spec(
-    spec_path: Annotated[str, typer.Option(help="path to the spec file")],
+    spec_path: Annotated[
+        str, typer.Option(help="path to the local spec .json file")
+    ],
     file_client_type: Annotated[
-        FileClientType,
+        Optional[FileClientType],
         typer.Option(
-            help="The file client will be used to load the spec file and persist files (e.g. screenshots) generated by the test. Make sure to provide the relevant credentials in the FILE_CLIENT_CONFIG environment variable",
+            help="Provide a file client if you want to persist files generated by the test, if you do provide a client, make sure to provide the relevant credentials in the FILE_CLIENT_CONFIG environment variable",
         ),
-    ],
+    ] = None,
     save_playwright_trace: Annotated[
         bool,
         typer.Option(
             help="Save Playwright trace, must provide a file client to use. See https://playwright.dev/python/docs/trace-viewer-intro for more information",
         ),
     ] = False,
     view_browser: Annotated[
@@ -178,16 +191,21 @@
         typer.Option(
             help="Opens up the browser in headful mode to view the test in action",
         ),
     ] = False,
 ):
     _setup_logging()
 
-    file_client = _create_file_client(file_client_type)
-    spec = asyncio.run(file_client.load_scrape_spec(spec_path))
+    if file_client_type is None:
+        file_client = None
+    else:
+        file_client = _create_file_client(file_client_type)
+
+    with open(spec_path, "r") as f:
+        spec = json.load(f)
 
     scraper = ScrapeSpecExecutor(
         scrape_spec=spec,
         file_client=file_client,
         save_playwright_trace=save_playwright_trace,
         headless=not view_browser,
     )
```

### Comparing `betatester-0.0.0/src/betatester/execution.py` & `betatester-0.0.1/src/betatester/execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import base64
 import json
 import logging
 import re
 import tempfile
 from abc import abstractmethod
-from typing import Any, Optional, Union, cast
+from typing import Any, Generic, Optional, TypeVar, Union, cast
 from uuid import UUID, uuid4
 
 import httpx
 from bs4 import BeautifulSoup, Tag
 from playwright.async_api import (
     Page,
     TimeoutError,
@@ -151,31 +151,36 @@
         )
 
     def publish(self, message: ExecutorMessage) -> None:
         for queue in self.subscriptions:
             queue.put_nowait(message)
 
 
-class _ScrapeExecutorBase:
+T = TypeVar("T")
+
+
+class _ScrapeExecutorBase(Generic[T]):
     def __init__(
         self,
         url: str,
+        high_level_goal: str,
         viewport_width: int,
         viewport_height: int,
         file_client: Optional[FileClient] = None,
         scrape_id: Optional[UUID] = None,
         save_playwright_trace: bool = False,
         headless: bool = True,
     ) -> None:
         if file_client is None and save_playwright_trace:
             raise ValueError(
                 "file_client must be provided when save_playwright_trace is True"
             )
         self.scrape_id = scrape_id or uuid4()
         self.url = url
+        self.high_level_goal = high_level_goal
         self.file_client = file_client
         self.viewport = ViewportSize(
             width=viewport_width, height=viewport_height
         )
 
         self.headless = headless
         self.save_playwright_trace = save_playwright_trace
@@ -183,18 +188,18 @@
     @abstractmethod
     async def _execute(self, page: Page) -> None:
         pass
 
     async def _run_start_callback(self) -> None:
         pass
 
-    async def _run_end_callback(self) -> None:
-        pass
+    async def _run_end_callback(self) -> Optional[T]:
+        return None
 
-    async def run(self) -> None:
+    async def run(self) -> Optional[T]:
         """
         Runs the test until the high level goal is completed or it errors out
         """
 
         logger.info("Starting to test %s", self.url)
         logger.info("===============================================")
         async with async_playwright() as p:
@@ -225,32 +230,34 @@
                         logger.info("Saved trace to %s", save_path)
                     trace_tempdir.cleanup()
 
                 # cleanup playwright
                 await context.close()
                 await browser.close()
 
-                await self._run_end_callback()
+                return_value = await self._run_end_callback()
 
         logger.info("Test %s completed", self.url)
         logger.info(
             "=============================================================="
         )
 
+        return return_value
+
 
 class ScrapeStepAiExecutor(_AiExecutorBase):
     def __init__(
         self,
         high_level_goal: str,
         previous_steps: list[str],
         page: Page,
         variables: ScrapeVariables,
         files: ScrapeFiles,
         openai_api_key: str,
-        max_action_attempts: Optional[int] = 5,
+        max_action_attempts: int = 5,
         scrape_id: Optional[UUID] = None,
         step_id: Optional[UUID] = None,
         file_client: Optional[FileClient] = None,
         http_client: Optional[httpx.AsyncClient] = None,
         subscriptions: Optional[set[asyncio.Queue[ExecutorMessage]]] = None,
     ) -> None:
         """
@@ -272,15 +279,15 @@
         Args:
             high_level_goal (str): High level goal to accomplish at the URL
             previous_steps (list[str]): Previous steps taken in the test
             page (Page): Playwright page object
             variables (ScrapeVariables): Variables to use in the scrape, e.g. for filling in a username and password to log in
             files (ScrapeFiles): Files to use in the scrape, e.g. for uploading some data as part of the goal
             openai_api_key (str): OpenAI API key, see https://platform.openai.com/api-keys
-            max_action_attempts (Optional[int], optional): Max actions to take on a single page. Defaults to 5.
+            max_action_attempts (int): Max actions to take on a single page. Set to 0 for no limit. Defaults to 5.
             scrape_id (Optional[UUID], optional): Scrape ID. Defaults to None.
             step_id (Optional[UUID], optional): Step ID. Defaults to None.
             file_client (Optional[FileClient], optional): File client to use for saving images, html, and traces. Defaults to None.
             http_client (Optional[httpx.AsyncClient], optional): Http client to use for making requests, pass one through to reuse across tests. Defaults to None.
             subscriptions (Optional[set[asyncio.Queue[ExecutorMessage]], optional): Subscriptions that will receive messages from the executor as it progresses. Defaults to None.
         """
         super().__init__(subscriptions)
@@ -481,15 +488,15 @@
                             content="The locator resolved to more than one element, try to use `role` and `name` instead",
                         )
                     )
                 else:
                     raise e
 
             if (
-                self.max_action_attempts is not None
+                self.max_action_attempts > 0
                 and self.actions_count >= self.max_action_attempts
             ):
                 logger.warning(
                     "Max action attempts (%s) reached",
                     self.max_action_attempts,
                 )
                 return None, self.actions_count
@@ -519,23 +526,23 @@
             )
         finally:
             if self.http_client is None:
                 await http_client.aclose()
         return next_instruction, action, action_count
 
 
-class ScrapeAiExecutor(_AiExecutorBase, _ScrapeExecutorBase):
+class ScrapeAiExecutor(_AiExecutorBase, _ScrapeExecutorBase[ScrapeSpec]):
     def __init__(
         self,
         url: str,
         high_level_goal: str,
         openai_api_key: str,
-        max_page_views: Optional[int] = 10,
-        max_total_actions: Optional[int] = 20,
-        max_action_attempts_per_step: Optional[int] = 5,
+        max_page_views: int = 10,
+        max_total_actions: int = 20,
+        max_action_attempts_per_step: int = 5,
         viewport_width: int = 1280,
         viewport_height: int = 720,
         variables: Optional[ScrapeVariables] = None,
         files: Optional[ScrapeFiles] = None,
         scrape_id: Optional[UUID] = None,
         file_client: Optional[FileClient] = None,
         save_playwright_trace: bool = False,
@@ -549,47 +556,47 @@
         Examples:
             ```python
             scrape_executor = ScrapeAiExecutor(
                 url="https://google.com",
                 high_level_goal="Find images of cats",
                 openai_api_key="...",
             )
-            await scrape_executor.run()
+            scrape_spec = await scrape_executor.run()
             ```
 
         Args:
             url (str): URL to test
             high_level_goal (str): High level goal to accomplish at the URL
             openai_api_key (str): OpenAI API key, see https://platform.openai.com/api-keys
-            max_page_views (Optional[int], optional): Max page views to take across the entire test. Defaults to 10.
-            max_total_actions (Optional[int], optional): Max total actions to take across the entire test. Defaults to 20.
-            max_action_attempts_per_step (Optional[int], optional): Max actions to take on a single page. Defaults to 5.
+            max_page_views (int): Max page views to take across the entire test. Set to 0 for no limit. Defaults to 10.
+            max_total_actions (int): Max total actions to take across the entire test. Set to 0 for no limit. Defaults to 20.
+            max_action_attempts_per_step (int): Max actions to take on a single page. Set to 0 for no limit Defaults to 5.
             viewport_width (int, optional): Viewport width in pixels. Defaults to 1280.
             viewport_height (int, optional): Viewport height in pixels. Defaults to 720.
             variables (Optional[ScrapeVariables], optional): Variables to use in the scrape, e.g. for filling in a username and password to log in. Defaults to None.
             files (Optional[ScrapeFiles], optional): Files to use in the scrape, e.g. for uploading some data as part of the goal. Defaults to None.
             scrape_id (Optional[UUID], optional): Scrape ID. Defaults to None.
             file_client (Optional[FileClient], optional): File client to use for saving images, html, and traces. Defaults to None.
             save_playwright_trace (bool, optional): Whether to save the playwright trace, see https://playwright.dev/python/docs/trace-viewer-intro for more information. You must provide a file_client to use this option. Defaults to False.
             http_client (Optional[httpx.AsyncClient], optional): Http client to use for making requests, pass one through to reuse across tests. Defaults to None.
             subscriptions (Optional[set[asyncio.Queue[ExecutorMessage]], optional): Subscriptions that will receive messages from the executor as it progresses. Defaults to None.
             headless (bool, optional): Whether to run the browser in headless mode, if False a chromium browswer will display the actions of the test in real time. Defaults to True.
         """
         _ScrapeExecutorBase.__init__(
             self,
             url=url,
+            high_level_goal=high_level_goal,
             viewport_width=viewport_width,
             viewport_height=viewport_height,
             file_client=file_client,
             scrape_id=scrape_id,
             save_playwright_trace=save_playwright_trace,
             headless=headless,
         )
         _AiExecutorBase.__init__(self, subscriptions=subscriptions)
-        self.high_level_goal = high_level_goal
         self._openai_api_key = openai_api_key
         self.max_page_views = max_page_views
         self.max_total_actions = max_total_actions
         self.max_action_attempts_per_step = max_action_attempts_per_step
         self.variables = variables or {}
         self.files = files or {}
 
@@ -603,42 +610,32 @@
 
         self.scrape_events: list[ScrapeEvent] = []
 
     async def _run_start_callback(self) -> None:
         if self.http_client is None:
             self.http_client = httpx.AsyncClient()
 
-    async def _run_end_callback(self) -> None:
-        # save scrape spec
-        if self.file_client is not None:
-            spec = ScrapeSpec(
-                url=self.url,
-                scrape_events=self.scrape_events,
-                variables=self.variables,
-                files=self.files,
-                viewport_height=self.viewport["height"],
-                viewport_width=self.viewport["width"],
-            )
-            spec_save_path = await self.file_client.save_scrape_spec(
-                self.scrape_id, spec
-            )
-            logger.info(
-                "Saved scrape spec to %s",
-                spec_save_path,
-            )
-
-        # cleanup model client
-        if self.close_http_client and self.http_client is not None:
-            await self.http_client.aclose()
+    async def _run_end_callback(self) -> ScrapeSpec:
+        spec = ScrapeSpec(
+            original_scrape_id=self.scrape_id,
+            url=self.url,
+            high_level_goal=self.high_level_goal,
+            scrape_events=self.scrape_events,
+            variables=self.variables,
+            files=self.files,
+            viewport_height=self.viewport["height"],
+            viewport_width=self.viewport["width"],
+        )
+        return spec
 
     @property
-    def max_action_attempts(self) -> Optional[int]:
-        max_action_attempts = None
-        if self.max_action_attempts_per_step is not None:
-            if self.max_total_actions is not None:
+    def max_action_attempts(self) -> int:
+        max_action_attempts = 0
+        if self.max_action_attempts_per_step > 0:
+            if self.max_total_actions > 0:
                 max_action_attempts = min(
                     self.max_action_attempts_per_step,
                     self.max_total_actions - self.scrape_action_count,
                 )
             else:
                 max_action_attempts = self.max_action_attempts_per_step
 
@@ -708,50 +705,46 @@
 
             # end test if high level goal is completed
             if next_instruction_fmt == SpecialInstruction.DONE:
                 break
 
             # check if max total actions reached
             if (
-                self.max_total_actions is not None
+                self.max_total_actions > 0
                 and self.scrape_action_count >= self.max_total_actions
             ):
                 raise MaxTotalActionsReachedException(
                     f"Max total actions ({self.scrape_action_count}) reached"
                 )
 
             # check if max page views reached
             if (
-                self.max_page_views is not None
+                self.max_page_views > 0
                 and self.scrape_page_view_count >= self.max_page_views
             ):
                 raise MaxPageViewsReachedException(
                     f"Max page views ({self.scrape_page_view_count}) reached"
                 )
 
 
-class ScrapeSpecExecutor(_ScrapeExecutorBase):
+class ScrapeSpecExecutor(_ScrapeExecutorBase[None]):
     def __init__(
         self,
         scrape_spec: ScrapeSpec,
         scrape_id: Optional[UUID] = None,
         file_client: Optional[FileClient] = None,
         save_playwright_trace: bool = False,
         headless: bool = True,
     ) -> None:
         """
         Executes a test on a given URL from a previously saved scrape spec
 
         Examples:
             ```python
             from betatester import ScrapeSpecExecutor
-            from betatester.file.local import LocalFileClient
-
-            file_client = LocalFileClient("...")
-            scrape_spec = file_client.load_scrape_spec("/path/to/scrape_spec.json")
 
             scrape_spec_executor = ScrapeSpecExecutor(
                 scrape_spec=scrape_spec,
             )
             await scrape_spec_executor.run()
             ```
 
@@ -761,21 +754,23 @@
             file_client (Optional[FileClient], optional): File client to use for saving images, html, and traces. Defaults to None.
             save_playwright_trace (bool, optional): Whether to save the playwright trace, see https://playwright.dev/python/docs/trace-viewer-int for more information. You must provide a file_client to use this option. Defaults to False.
             headless (bool, optional): Whether to run the browser in headless mode, if False a chromium browswer will display the actions of the test in real time. Defaults to True.
         """
         _ScrapeExecutorBase.__init__(
             self,
             url=scrape_spec.url,
+            high_level_goal=scrape_spec.high_level_goal,
             viewport_width=scrape_spec.viewport_width,
             viewport_height=scrape_spec.viewport_height,
             file_client=file_client,
             scrape_id=scrape_id,
             save_playwright_trace=save_playwright_trace,
             headless=headless,
         )
+        self.original_scrape_id = scrape_spec.original_scrape_id
         self.scrape_events = scrape_spec.scrape_events
         self.variables = scrape_spec.variables
         self.files = scrape_spec.files
 
     async def _execute(self, page: Page) -> None:
         await page.goto(self.url)
         logger.info("Navigated to %s", self.url)
```

### Comparing `betatester-0.0.0/src/betatester/model.py` & `betatester-0.0.1/src/betatester/model.py`

 * *Files identical despite different names*

### Comparing `betatester-0.0.0/src/betatester/prompts.py` & `betatester-0.0.1/src/betatester/prompts.py`

 * *Files identical despite different names*

### Comparing `betatester-0.0.0/src/betatester/file/local.py` & `betatester-0.0.1/src/betatester/file/local.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from uuid import UUID
 
 import aiofiles
 
-from ..betatester_types import FileClient, HtmlType, ScrapeSpec
+from ..betatester_types import FileClient, HtmlType
 
 
 class LocalFileClient(FileClient):
     def __init__(self, save_path: str):
         self.save_path = save_path
 
     def _create_imgs_path(
@@ -82,23 +82,12 @@
     ) -> str:
         path = self._create_html_path(scrape_id, step_id, html_type)
         async with aiofiles.open(path, "w") as f_out:
             await f_out.write(html)
 
         return path
 
-    async def save_scrape_spec(self, scrape_id: UUID, spec: ScrapeSpec) -> str:
-        path = self._create_representation_path(scrape_id)
-        async with aiofiles.open(path, "w") as f_out:
-            await f_out.write(spec.model_dump_json())
-
-        return path
-
-    async def load_scrape_spec(self, path: str) -> ScrapeSpec:
-        async with aiofiles.open(path, "r") as f:
-            return ScrapeSpec.model_validate_json(await f.read())
-
     def img_path(self, scrape_id: UUID, step_id: UUID) -> str:
         return self._create_imgs_path(scrape_id, step_id)
 
     def trace_path(self, scrape_id: UUID) -> str:
         return self._create_traces_path(scrape_id)
```

### Comparing `betatester-0.0.0/LICENSE` & `betatester-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `betatester-0.0.0/README.md` & `betatester-0.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -33,35 +33,27 @@
 
 ### Usage
 
 Run the test using LLMs. See the docstring [here](./src/betatester/execution.py#L559) for more information on the avaiable parameters.
 
 ```python
 from betatester import ScrapeAiExecutor
-from betatester.file.local import LocalFileClient
-
-file_client = LocalFileClient("./app-data/")
 
 scrape_executor = ScrapeAiExecutor(
     url="https://google.com",
     high_level_goal="Find images of cats",
     openai_api_key="...",
-    file_client=file_client,
 )
-await scrape_executor.run()
+scrape_spec = await scrape_executor.run()
 ```
 
 Run the test using a scrape spec (with no LLM calls) generated from a previous LLM run. See the docstring [here](./src/betatester/execution.py#L758) for more information on the avaiable parameters.
 
 ```python
 from betatester import ScrapeSpecExecutor
-from betatester.file.local import LocalFileClient
-
-file_client = LocalFileClient("./app-data/")
-scrape_spec = await file_client.load_scrape_spec("/path/to/scrape_spec.json")
 
 scrape_spec_executor = ScrapeSpecExecutor(
     scrape_spec=scrape_spec,
 )
 await scrape_spec_executor.run()
 ```
 
@@ -84,21 +76,21 @@
 3. Make sure to retrieve an [your OpenAI API key](https://platform.openai.com/docs/quickstart/account-setup) if you have not already done so and set it as an environment variable `OPENAI_API_KEY`.
 
 ### Usage
 
 Run the test using LLMs. Use `betatester start_ai --help` for more information on the avaiable parameters.
 
 ```bash
-FILE_CLIENT_CONFIG='{"save_path": "./app-data/"}' betatester start_ai --url "https://google.com" --high-level-goal "Find images of cats" --file-client-type "local"
+betatester start_ai --url "https://google.com" --high-level-goal "Find images of cats"  > "/path/to/scrape_spec.json"
 ```
 
 Run the test using a scrape spec (with no LLM calls) generated from a previous LLM run. Use `betatester start_spec --help` for more information on the avaiable parameters.
 
 ```bash
-FILE_CLIENT_CONFIG='{"save_path": "./app-data/"}' betatester start_spec --scrape-spec-path "/path/to/scrape_spec.json" --file-client-type "local"
+betatester start_spec --scrape-spec-path "/path/to/scrape_spec.json"
 ```
 
 ## Extensions
 
 ### File
 
 AutoTransform provides a file extension that allows you to store your files in the storage provider of your choice. To use the file extension, you will need to provide the following environment variables:
```

### Comparing `betatester-0.0.0/pyproject.toml` & `betatester-0.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "betatester"
-version = "0.0.0"
+version = "0.0.1"
 authors = [
   { name="Ihsaan Patel" },
 ]
 description = "A package for automatically testing the UX / UI of a website."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `betatester-0.0.0/PKG-INFO` & `betatester-0.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: betatester
-Version: 0.0.0
+Version: 0.0.1
 Summary: A package for automatically testing the UX / UI of a website.
 Project-URL: Homepage, https://github.com/pateli18/betatester
 Project-URL: Issues, https://github.com/pateli18/betatester/issues
 Author: Ihsaan Patel
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -56,35 +56,27 @@
 
 ### Usage
 
 Run the test using LLMs. See the docstring [here](./src/betatester/execution.py#L559) for more information on the avaiable parameters.
 
 ```python
 from betatester import ScrapeAiExecutor
-from betatester.file.local import LocalFileClient
-
-file_client = LocalFileClient("./app-data/")
 
 scrape_executor = ScrapeAiExecutor(
     url="https://google.com",
     high_level_goal="Find images of cats",
     openai_api_key="...",
-    file_client=file_client,
 )
-await scrape_executor.run()
+scrape_spec = await scrape_executor.run()
 ```
 
 Run the test using a scrape spec (with no LLM calls) generated from a previous LLM run. See the docstring [here](./src/betatester/execution.py#L758) for more information on the avaiable parameters.
 
 ```python
 from betatester import ScrapeSpecExecutor
-from betatester.file.local import LocalFileClient
-
-file_client = LocalFileClient("./app-data/")
-scrape_spec = await file_client.load_scrape_spec("/path/to/scrape_spec.json")
 
 scrape_spec_executor = ScrapeSpecExecutor(
     scrape_spec=scrape_spec,
 )
 await scrape_spec_executor.run()
 ```
 
@@ -107,21 +99,21 @@
 3. Make sure to retrieve an [your OpenAI API key](https://platform.openai.com/docs/quickstart/account-setup) if you have not already done so and set it as an environment variable `OPENAI_API_KEY`.
 
 ### Usage
 
 Run the test using LLMs. Use `betatester start_ai --help` for more information on the avaiable parameters.
 
 ```bash
-FILE_CLIENT_CONFIG='{"save_path": "./app-data/"}' betatester start_ai --url "https://google.com" --high-level-goal "Find images of cats" --file-client-type "local"
+betatester start_ai --url "https://google.com" --high-level-goal "Find images of cats"  > "/path/to/scrape_spec.json"
 ```
 
 Run the test using a scrape spec (with no LLM calls) generated from a previous LLM run. Use `betatester start_spec --help` for more information on the avaiable parameters.
 
 ```bash
-FILE_CLIENT_CONFIG='{"save_path": "./app-data/"}' betatester start_spec --scrape-spec-path "/path/to/scrape_spec.json" --file-client-type "local"
+betatester start_spec --scrape-spec-path "/path/to/scrape_spec.json"
 ```
 
 ## Extensions
 
 ### File
 
 AutoTransform provides a file extension that allows you to store your files in the storage provider of your choice. To use the file extension, you will need to provide the following environment variables:
```


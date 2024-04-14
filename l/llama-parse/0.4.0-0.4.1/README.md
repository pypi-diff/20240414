# Comparing `tmp/llama_parse-0.4.0.tar.gz` & `tmp/llama_parse-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_parse-0.4.0.tar", max compression
+gzip compressed data, was "llama_parse-0.4.1.tar", max compression
```

## Comparing `llama_parse-0.4.0.tar` & `llama_parse-0.4.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-01-31 18:33:52.872404 llama_parse-0.4.0/LICENSE
--rw-r--r--   0        0        0     2809 2024-03-13 14:58:09.813098 llama_parse-0.4.0/README.md
--rw-r--r--   0        0        0       91 2024-02-02 19:51:20.620573 llama_parse-0.4.0/llama_parse/__init__.py
--rw-r--r--   0        0        0    13128 2024-03-21 16:50:38.370713 llama_parse-0.4.0/llama_parse/base.py
--rw-r--r--   0        0        0      482 2024-03-21 16:51:58.925230 llama_parse-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3350 1970-01-01 00:00:00.000000 llama_parse-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-14 19:10:02.541219 llama_parse-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2858 2024-04-14 19:10:02.541219 llama_parse-0.4.1/README.md
+-rw-r--r--   0        0        0       92 2024-04-14 19:10:02.557219 llama_parse-0.4.1/llama_parse/__init__.py
+-rw-r--r--   0        0        0    15192 2024-04-14 19:10:02.557219 llama_parse-0.4.1/llama_parse/base.py
+-rw-r--r--   0        0        0      483 2024-04-14 19:10:02.561219 llama_parse-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3451 1970-01-01 00:00:00.000000 llama_parse-0.4.1/PKG-INFO
```

### Comparing `llama_parse-0.4.0/LICENSE` & `llama_parse-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_parse-0.4.0/README.md` & `llama_parse-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # LlamaParse
 
 LlamaParse is an API created by LlamaIndex to efficiently parse and represent files for efficient retrieval and context augmentation using LlamaIndex frameworks.
 
 LlamaParse directly integrates with [LlamaIndex](https://github.com/run-llama/llama_index).
 
-
 Free plan is up to 1000 pages a day. Paid plan is free 7k pages per week + 0.3c per additional page.
 
 ## Getting Started
 
-First, login and get an api-key from `https://cloud.llamaindex.ai`.
+First, login and get an api-key from [**https://cloud.llamaindex.ai ↗**](https://cloud.llamaindex.ai).
 
 Then, make sure you have the latest LlamaIndex version installed.
 
 **NOTE:** If you are upgrading from v0.9.X, we recommend following our [migration guide](https://pretty-sodium-5e0.notion.site/v0-10-0-Migration-Guide-6ede431dcb8841b09ea171e7f133bd77), as well as uninstalling your previous version first.
 
 ```
 pip uninstall llama-index  # run this if upgrading from v0.9.x or older
@@ -24,24 +23,25 @@
 
 `pip install llama-parse`
 
 Now you can run the following to parse your first PDF file:
 
 ```python
 import nest_asyncio
+
 nest_asyncio.apply()
 
 from llama_parse import LlamaParse
 
 parser = LlamaParse(
     api_key="llx-...",  # can also be set in your env as LLAMA_CLOUD_API_KEY
     result_type="markdown",  # "markdown" and "text" are available
-    num_workers=4, # if multiple files passed, split in `num_workers` API calls
+    num_workers=4,  # if multiple files passed, split in `num_workers` API calls
     verbose=True,
-    language="en" # Optionaly you can define a language, default=en
+    language="en",  # Optionally you can define a language, default=en
 )
 
 # sync
 documents = parser.load_data("./my_file.pdf")
 
 # sync batch
 documents = parser.load_data(["./my_file1.pdf", "./my_file2.pdf"])
@@ -55,27 +55,30 @@
 
 ## Using with `SimpleDirectoryReader`
 
 You can also integrate the parser as the default PDF loader in `SimpleDirectoryReader`:
 
 ```python
 import nest_asyncio
+
 nest_asyncio.apply()
 
 from llama_parse import LlamaParse
 from llama_index.core import SimpleDirectoryReader
 
 parser = LlamaParse(
     api_key="llx-...",  # can also be set in your env as LLAMA_CLOUD_API_KEY
     result_type="markdown",  # "markdown" and "text" are available
-    verbose=True
+    verbose=True,
 )
 
 file_extractor = {".pdf": parser}
-documents = SimpleDirectoryReader("./data", file_extractor=file_extractor).load_data()
+documents = SimpleDirectoryReader(
+    "./data", file_extractor=file_extractor
+).load_data()
 ```
 
 Full documentation for `SimpleDirectoryReader` can be found on the [LlamaIndex Documentation](https://docs.llamaindex.ai/en/stable/module_guides/loading/simpledirectoryreader.html).
 
 ## Examples
 
 Several end-to-end indexing examples can be found in the examples folder
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `llama_parse-0.4.0/llama_parse/base.py` & `llama_parse-0.4.1/llama_parse/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,20 +13,23 @@
 from llama_index.core.readers.base import BasePydanticReader
 from llama_index.core.schema import Document
 
 
 nest_asyncio_err = "cannot be called from a running event loop"
 nest_asyncio_msg = "The event loop is already running. Add `import nest_asyncio; nest_asyncio.apply()` to your code to fix this issue."
 
+
 class ResultType(str, Enum):
     """The result type for the parser."""
+
     TXT = "text"
     MD = "markdown"
     JSON = "json"
 
+
 class Language(str, Enum):
     BAZA = "abq"
     ADYGHE = "ady"
     AFRIKAANS = "af"
     ANGIKA = "ang"
     ARABIC = "ar"
     ASSAMESE = "as"
@@ -99,15 +102,15 @@
     TABASSARAN = "tab"
     TELUGU = "te"
     THAI = "th"
     TAJIK = "tjk"
     TAGALOG = "tl"
     TURKISH = "tr"
     UYGHUR = "ug"
-    UKRANIAN = "uk"
+    UKRAINIAN = "uk"
     URDU = "ur"
     UZBEK = "uz"
     VIETNAMESE = "vi"
 
 
 SUPPORTED_FILE_TYPES = [
     ".pdf",
@@ -120,56 +123,46 @@
     ".dotm",
     # Rich text format
     ".rtf",
     # Microsoft Works
     ".wps",
     # Word Perfect
     ".wpd",
-
     # Open Office
     ".sxw",
-    ".stw", 
+    ".stw",
     ".sxg",
-
     # Apple
     ".pages",
-
     # Mac Write
     ".mw",
     ".mcw",
-
-
     # Unified Office Format text
     ".uot",
     ".uof",
     ".uos",
     ".uop",
-
     # Microsoft powerpoints
     ".ppt",
     ".pptx",
     ".pot",
     ".pptm",
     ".potx",
     ".potm",
-
-
     # Apple keynote
     ".key",
-
     # Open Office Presentations
     ".odp",
     ".odg",
     ".otp",
     ".fopd",
-    ".sxi", 
+    ".sxi",
     ".sti",
-    
     # ebook
-    ".epub"
+    ".epub",
 ]
 
 
 class LlamaParse(BasePydanticReader):
     """A smart-parser for files."""
 
     api_key: str = Field(default="", description="The API key for the LlamaParse API.")
@@ -179,56 +172,65 @@
     )
     result_type: ResultType = Field(
         default=ResultType.TXT, description="The result type for the parser."
     )
     num_workers: int = Field(
         default=4,
         gt=0,
-        lt=10, 
-        description="The number of workers to use sending API requests for parsing."
+        lt=10,
+        description="The number of workers to use sending API requests for parsing.",
     )
     check_interval: int = Field(
         default=1,
         description="The interval in seconds to check if the parsing is done.",
     )
     max_timeout: int = Field(
         default=2000,
         description="The maximum timeout in seconds to wait for the parsing to finish.",
     )
     verbose: bool = Field(
         default=True, description="Whether to print the progress of the parsing."
     )
-    language: Language  = Field(
-         default=Language.ENGLISH, description="The language of the text to parse."
+    show_progress: bool = Field(
+        default=True, description="Show progress when parsing multiple files."
+    )
+    language: Language = Field(
+        default=Language.ENGLISH, description="The language of the text to parse."
     )
     parsing_instruction: Optional[str] = Field(
-        default="",
-        description="The parsing instruction for the parser."
+        default="", description="The parsing instruction for the parser."
+    )
+    ignore_errors: bool = Field(
+        default=True,
+        description="Whether or not to ignore and skip errors raised during parsing.",
     )
 
     @validator("api_key", pre=True, always=True)
     def validate_api_key(cls, v: str) -> str:
         """Validate the API key."""
         if not v:
             import os
+
             api_key = os.getenv("LLAMA_CLOUD_API_KEY", None)
             if api_key is None:
                 raise ValueError("The API key is required.")
             return api_key
-        
+
         return v
-    
+
     @validator("base_url", pre=True, always=True)
     def validate_base_url(cls, v: str) -> str:
         """Validate the base URL."""
         url = os.getenv("LLAMA_CLOUD_BASE_URL", None)
         return url or v or DEFAULT_BASE_URL
 
     # upload a document and get back a job_id
-    async def _create_job(self, file_path: str, extra_info: Optional[dict] = None) -> str:
+    async def _create_job(
+        self, file_path: str, extra_info: Optional[dict] = None
+    ) -> str:
         file_path = str(file_path)
         file_ext = os.path.splitext(file_path)[1]
         if file_ext not in SUPPORTED_FILE_TYPES:
             raise Exception(
                 f"Currently, only the following file types are supported: {SUPPORTED_FILE_TYPES}\n"
                 f"Current file type: {file_ext}"
             )
@@ -242,169 +244,237 @@
         with open(file_path, "rb") as f:
             mime_type = mimetypes.guess_type(file_path)[0]
             files = {"file": (f.name, f, mime_type)}
 
             # send the request, start job
             url = f"{self.base_url}/api/parsing/upload"
             async with httpx.AsyncClient(timeout=self.max_timeout) as client:
-                response = await client.post(url, files=files, headers=headers, data={"language": self.language.value, "parsing_instruction": self.parsing_instruction})
+                response = await client.post(
+                    url,
+                    files=files,
+                    headers=headers,
+                    data={
+                        "language": self.language.value,
+                        "parsing_instruction": self.parsing_instruction,
+                    },
+                )
                 if not response.is_success:
                     raise Exception(f"Failed to parse the file: {response.text}")
 
         # check the status of the job, return when done
         job_id = response.json()["id"]
         return job_id
 
-    async def _get_job_result(self, job_id: str, result_type: str) -> dict:
+    async def _get_job_result(
+        self, job_id: str, result_type: str, verbose: bool = False
+    ) -> dict:
         result_url = f"{self.base_url}/api/parsing/job/{job_id}/result/{result_type}"
+        status_url = f"{self.base_url}/api/parsing/job/{job_id}"
         headers = {"Authorization": f"Bearer {self.api_key}"}
 
         start = time.time()
         tries = 0
         while True:
             await asyncio.sleep(self.check_interval)
-            async with httpx.AsyncClient(timeout=self.max_timeout) as client: 
-                tries += 1   
-                
-                result = await client.get(result_url, headers=headers)
+            async with httpx.AsyncClient(timeout=self.max_timeout) as client:
+                tries += 1
+
+                result = await client.get(status_url, headers=headers)
 
-                if result.status_code == 404:
+                if result.status_code != 200:
                     end = time.time()
                     if end - start > self.max_timeout:
-                        raise Exception(
-                            f"Timeout while parsing the file: {job_id}"
-                        )
-                    if self.verbose and tries % 10 == 0:
+                        raise Exception(f"Timeout while parsing the file: {job_id}")
+                    if verbose and tries % 10 == 0:
                         print(".", end="", flush=True)
+
+                    await asyncio.sleep(self.check_interval)
+
                     continue
 
-                if result.status_code == 400:
-                    detail = result.json().get("detail", "Unknown error")
-                    raise Exception(f"Failed to parse the file: {detail}")
+                # Allowed values "PENDING", "SUCCESS", "ERROR", "CANCELED"
+                status = result.json()["status"]
+                if status == "SUCCESS":
+                    parsed_result = await client.get(result_url, headers=headers)
+                    return parsed_result.json()
+                elif status == "PENDING":
+                    end = time.time()
+                    if end - start > self.max_timeout:
+                        raise Exception(f"Timeout while parsing the file: {job_id}")
+                    if verbose and tries % 10 == 0:
+                        print(".", end="", flush=True)
 
-                return result.json()
+                    await asyncio.sleep(self.check_interval)
 
-    async def _aload_data(self, file_path: str, extra_info: Optional[dict] = None) -> List[Document]:
+                    continue
+                else:
+                    raise Exception(
+                        f"Failed to parse the file: {job_id}, status: {status}"
+                    )
+
+    async def _aload_data(
+        self, file_path: str, extra_info: Optional[dict] = None, verbose: bool = False
+    ) -> List[Document]:
         """Load data from the input path."""
         try:
             job_id = await self._create_job(file_path, extra_info=extra_info)
-            if self.verbose:
+            if verbose:
                 print("Started parsing the file under job_id %s" % job_id)
-            
-            result = await self._get_job_result(job_id, self.result_type.value)
+
+            result = await self._get_job_result(
+                job_id, self.result_type.value, verbose=verbose
+            )
 
             return [
                 Document(
                     text=result[self.result_type.value],
                     metadata=extra_info or {},
                 )
             ]
-          
+
         except Exception as e:
             print(f"Error while parsing the file '{file_path}':", e)
-            raise e
-            return []
-    
+            if self.ignore_errors:
+                return []
+            else:
+                raise e
 
-    async def aload_data(self, file_path: Union[List[str], str], extra_info: Optional[dict] = None) -> List[Document]:
+    async def aload_data(
+        self, file_path: Union[List[str], str], extra_info: Optional[dict] = None
+    ) -> List[Document]:
         """Load data from the input path."""
         if isinstance(file_path, (str, Path)):
-            return await self._aload_data(file_path, extra_info=extra_info)
+            return await self._aload_data(
+                file_path, extra_info=extra_info, verbose=self.verbose
+            )
         elif isinstance(file_path, list):
-            jobs = [self._aload_data(f, extra_info=extra_info) for f in file_path]
+            jobs = [
+                self._aload_data(
+                    f,
+                    extra_info=extra_info,
+                    verbose=self.verbose and not self.show_progress,
+                )
+                for f in file_path
+            ]
             try:
-                results = await run_jobs(jobs, workers=self.num_workers)
-                
+                results = await run_jobs(
+                    jobs,
+                    workers=self.num_workers,
+                    desc="Parsing files",
+                    show_progress=self.show_progress,
+                )
+
                 # return flattened results
                 return [item for sublist in results for item in sublist]
             except RuntimeError as e:
                 if nest_asyncio_err in str(e):
                     raise RuntimeError(nest_asyncio_msg)
                 else:
                     raise e
         else:
-            raise ValueError("The input file_path must be a string or a list of strings.")
+            raise ValueError(
+                "The input file_path must be a string or a list of strings."
+            )
 
-    def load_data(self, file_path: Union[List[str], str], extra_info: Optional[dict] = None) -> List[Document]:
+    def load_data(
+        self, file_path: Union[List[str], str], extra_info: Optional[dict] = None
+    ) -> List[Document]:
         """Load data from the input path."""
         try:
             return asyncio.run(self.aload_data(file_path, extra_info))
         except RuntimeError as e:
             if nest_asyncio_err in str(e):
                 raise RuntimeError(nest_asyncio_msg)
             else:
                 raise e
-    
 
-    async def _aget_json(self, file_path: str, extra_info: Optional[dict] = None) -> List[dict]:
+    async def _aget_json(
+        self, file_path: str, extra_info: Optional[dict] = None
+    ) -> List[dict]:
         """Load data from the input path."""
         try:
             job_id = await self._create_job(file_path, extra_info=extra_info)
             if self.verbose:
                 print("Started parsing the file under job_id %s" % job_id)
-            
+
             result = await self._get_job_result(job_id, "json")
             result["job_id"] = job_id
             result["file_path"] = file_path
             return [result]
-          
+
         except Exception as e:
             print(f"Error while parsing the file '{file_path}':", e)
-            raise e
-        
-    
+            if self.ignore_errors:
+                return []
+            else:
+                raise e
 
-    async def aget_json(self, file_path: Union[List[str], str], extra_info: Optional[dict] = None) -> List[dict]:
+    async def aget_json(
+        self, file_path: Union[List[str], str], extra_info: Optional[dict] = None
+    ) -> List[dict]:
         """Load data from the input path."""
         if isinstance(file_path, (str, Path)):
             return await self._aget_json(file_path, extra_info=extra_info)
         elif isinstance(file_path, list):
             jobs = [self._aget_json(f, extra_info=extra_info) for f in file_path]
             try:
-                results = await run_jobs(jobs, workers=self.num_workers)
-                
+                results = await run_jobs(
+                    jobs,
+                    workers=self.num_workers,
+                    desc="Parsing files",
+                    show_progress=self.show_progress,
+                )
+
                 # return flattened results
                 return [item for sublist in results for item in sublist]
             except RuntimeError as e:
                 if nest_asyncio_err in str(e):
                     raise RuntimeError(nest_asyncio_msg)
                 else:
                     raise e
         else:
-            raise ValueError("The input file_path must be a string or a list of strings.")
-
+            raise ValueError(
+                "The input file_path must be a string or a list of strings."
+            )
 
-    def get_json_result(self, file_path: Union[List[str], str], extra_info: Optional[dict] = None) -> List[dict]:
+    def get_json_result(
+        self, file_path: Union[List[str], str], extra_info: Optional[dict] = None
+    ) -> List[dict]:
         """Parse the input path."""
         try:
             return asyncio.run(self.aget_json(file_path, extra_info))
         except RuntimeError as e:
             if nest_asyncio_err in str(e):
                 raise RuntimeError(nest_asyncio_msg)
             else:
                 raise e
-            
-    def get_images(self, json_result: list[dict], download_path: str) -> List[dict]:
+
+    def get_images(self, json_result: List[dict], download_path: str) -> List[dict]:
         """Download images from the parsed result."""
         headers = {"Authorization": f"Bearer {self.api_key}"}
         try:
             images = []
             for result in json_result:
                 job_id = result["job_id"]
                 for page in result["pages"]:
                     if self.verbose:
                         print(f"> Image for page {page['page']}: {page['images']}")
                     for image in page["images"]:
                         image_name = image["name"]
-                        image_path = os.path.join(download_path, f"{job_id}-{image_name}")
-                        image["path"]=image_path
-                        image["job_id"]=job_id
-                        image["original_pdf_path"]=result["file_path"]
-                        image["page_number"]=page["page"]
+                        image_path = os.path.join(
+                            download_path, f"{job_id}-{image_name}"
+                        )
+                        image["path"] = image_path
+                        image["job_id"] = job_id
+                        image["original_pdf_path"] = result["file_path"]
+                        image["page_number"] = page["page"]
                         with open(image_path, "wb") as f:
                             image_url = f"{self.base_url}/api/parsing/job/{job_id}/result/image/{image_name}"
                             f.write(httpx.get(image_url, headers=headers).content)
                         images.append(image)
             return images
         except Exception as e:
-            print(f"Error while downloading images from the parsed result:", e)
-            return []
+            print("Error while downloading images from the parsed result:", e)
+            if self.ignore_errors:
+                return []
+            else:
+                raise e
```

### Comparing `llama_parse-0.4.0/PKG-INFO` & `llama_parse-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: llama-parse
-Version: 0.4.0
+Version: 0.4.1
 Summary: Parse files into RAG-Optimized formats.
 License: MIT
 Author: Logan Markewich
 Author-email: logan@llamaindex.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: llama-index-core (>=0.10.7)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: llama-index-core (>=0.10.29)
 Description-Content-Type: text/markdown
 
 # LlamaParse
 
 LlamaParse is an API created by LlamaIndex to efficiently parse and represent files for efficient retrieval and context augmentation using LlamaIndex frameworks.
 
 LlamaParse directly integrates with [LlamaIndex](https://github.com/run-llama/llama_index).
 
-
 Free plan is up to 1000 pages a day. Paid plan is free 7k pages per week + 0.3c per additional page.
 
 ## Getting Started
 
-First, login and get an api-key from `https://cloud.llamaindex.ai`.
+First, login and get an api-key from [**https://cloud.llamaindex.ai ↗**](https://cloud.llamaindex.ai).
 
 Then, make sure you have the latest LlamaIndex version installed.
 
 **NOTE:** If you are upgrading from v0.9.X, we recommend following our [migration guide](https://pretty-sodium-5e0.notion.site/v0-10-0-Migration-Guide-6ede431dcb8841b09ea171e7f133bd77), as well as uninstalling your previous version first.
 
 ```
 pip uninstall llama-index  # run this if upgrading from v0.9.x or older
@@ -40,24 +40,25 @@
 
 `pip install llama-parse`
 
 Now you can run the following to parse your first PDF file:
 
 ```python
 import nest_asyncio
+
 nest_asyncio.apply()
 
 from llama_parse import LlamaParse
 
 parser = LlamaParse(
     api_key="llx-...",  # can also be set in your env as LLAMA_CLOUD_API_KEY
     result_type="markdown",  # "markdown" and "text" are available
-    num_workers=4, # if multiple files passed, split in `num_workers` API calls
+    num_workers=4,  # if multiple files passed, split in `num_workers` API calls
     verbose=True,
-    language="en" # Optionaly you can define a language, default=en
+    language="en",  # Optionally you can define a language, default=en
 )
 
 # sync
 documents = parser.load_data("./my_file.pdf")
 
 # sync batch
 documents = parser.load_data(["./my_file1.pdf", "./my_file2.pdf"])
@@ -71,27 +72,30 @@
 
 ## Using with `SimpleDirectoryReader`
 
 You can also integrate the parser as the default PDF loader in `SimpleDirectoryReader`:
 
 ```python
 import nest_asyncio
+
 nest_asyncio.apply()
 
 from llama_parse import LlamaParse
 from llama_index.core import SimpleDirectoryReader
 
 parser = LlamaParse(
     api_key="llx-...",  # can also be set in your env as LLAMA_CLOUD_API_KEY
     result_type="markdown",  # "markdown" and "text" are available
-    verbose=True
+    verbose=True,
 )
 
 file_extractor = {".pdf": parser}
-documents = SimpleDirectoryReader("./data", file_extractor=file_extractor).load_data()
+documents = SimpleDirectoryReader(
+    "./data", file_extractor=file_extractor
+).load_data()
 ```
 
 Full documentation for `SimpleDirectoryReader` can be found on the [LlamaIndex Documentation](https://docs.llamaindex.ai/en/stable/module_guides/loading/simpledirectoryreader.html).
 
 ## Examples
 
 Several end-to-end indexing examples can be found in the examples folder
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


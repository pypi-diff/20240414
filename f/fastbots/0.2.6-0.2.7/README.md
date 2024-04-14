# Comparing `tmp/fastbots-0.2.6.tar.gz` & `tmp/fastbots-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastbots-0.2.6.tar", max compression
+gzip compressed data, was "fastbots-0.2.7.tar", max compression
```

## Comparing `fastbots-0.2.6.tar` & `fastbots-0.2.7.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    11343 2023-11-16 19:08:50.352039 fastbots-0.2.6/LICENSE
--rw-r--r--   0        0        0    16549 2024-01-05 14:28:26.436502 fastbots-0.2.6/README.md
--rw-r--r--   0        0        0      765 2023-12-23 16:02:21.582428 fastbots-0.2.6/fastbots/__init__.py
--rw-r--r--   0        0        0    15329 2023-12-23 16:05:32.704323 fastbots-0.2.6/fastbots/bot.py
--rw-r--r--   0        0        0     4119 2023-12-22 20:37:44.309447 fastbots-0.2.6/fastbots/chrome_bot.py
--rw-r--r--   0        0        0     4539 2024-01-05 14:36:20.435937 fastbots-0.2.6/fastbots/config.py
--rw-r--r--   0        0        0     3348 2023-12-22 20:37:44.309447 fastbots-0.2.6/fastbots/exceptions.py
--rw-r--r--   0        0        0     5049 2023-12-22 20:37:44.309447 fastbots-0.2.6/fastbots/firefox_bot.py
--rw-r--r--   0        0        0      755 2023-12-22 20:37:44.309447 fastbots-0.2.6/fastbots/logger.py
--rw-r--r--   0        0        0     4675 2023-12-22 20:37:44.309447 fastbots-0.2.6/fastbots/page.py
--rw-r--r--   0        0        0      364 2023-12-22 20:37:44.309447 fastbots-0.2.6/fastbots/payload.py
--rw-r--r--   0        0        0     5107 2023-12-22 20:37:44.309447 fastbots-0.2.6/fastbots/task.py
--rw-r--r--   0        0        0      724 2024-01-05 14:34:42.351082 fastbots-0.2.6/pyproject.toml
--rw-r--r--   0        0        0    17314 1970-01-01 00:00:00.000000 fastbots-0.2.6/PKG-INFO
+-rwxr-xr-x   0        0        0    11343 2023-11-16 19:08:50.352039 fastbots-0.2.7/LICENSE
+-rwxr-xr-x   0        0        0    18771 2024-04-14 20:32:40.781492 fastbots-0.2.7/README.md
+-rwxr-xr-x   0        0        0      870 2024-04-14 20:20:04.614926 fastbots-0.2.7/fastbots/__init__.py
+-rwxr-xr-x   0        0        0    15329 2023-12-23 16:05:32.704323 fastbots-0.2.7/fastbots/bot.py
+-rwxr-xr-x   0        0        0     4119 2023-12-22 20:37:44.309447 fastbots-0.2.7/fastbots/chrome_bot.py
+-rwxr-xr-x   0        0        0     4636 2024-04-14 18:40:53.986816 fastbots-0.2.7/fastbots/config.py
+-rwxr-xr-x   0        0        0     3348 2023-12-22 20:37:44.309447 fastbots-0.2.7/fastbots/exceptions.py
+-rwxr-xr-x   0        0        0     5049 2023-12-22 20:37:44.309447 fastbots-0.2.7/fastbots/firefox_bot.py
+-rwxr-xr-x   0        0        0     5463 2024-04-14 20:25:00.459822 fastbots-0.2.7/fastbots/llm_extractor.py
+-rwxr-xr-x   0        0        0      755 2023-12-22 20:37:44.309447 fastbots-0.2.7/fastbots/logger.py
+-rwxr-xr-x   0        0        0     4675 2023-12-22 20:37:44.309447 fastbots-0.2.7/fastbots/page.py
+-rwxr-xr-x   0        0        0      364 2023-12-22 20:37:44.309447 fastbots-0.2.7/fastbots/payload.py
+-rwxr-xr-x   0        0        0     5107 2023-12-22 20:37:44.309447 fastbots-0.2.7/fastbots/task.py
+-rwxr-xr-x   0        0        0      774 2024-04-14 20:33:55.739645 fastbots-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0    19628 1970-01-01 00:00:00.000000 fastbots-0.2.7/PKG-INFO
```

### Comparing `fastbots-0.2.6/LICENSE` & `fastbots-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fastbots-0.2.6/README.md` & `fastbots-0.2.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # fastbots
 
 [Fastbots](https://ubertidavide.github.io/fastbots/) is a simple library designed for rapid bot and scraper development using Selenium and the POM (Page Object Model) design.  
-It enhances productivity by allowing developers to focus solely on scraping, reducing boilerplate code, and eliminating the need for direct driver management-related code, thanks to browser-independent settings.  
+It enhances productivity by allowing developers to focus solely on scraping automatically using AI, reducing boilerplate code, and eliminating the need for direct driver management-related code, thanks to browser-independent settings.  
 Even if site locators change, this library doesn't require modifications to the code; adjustments can be made solely in the configuration.
 
 fastbots is also fully compatible with all selenium functions, refer to [selenium official documentation](https://www.selenium.dev/documentation/webdriver/elements/interactions/) for more details.
 
 ## Installation
 
 The installation process is straightforward using pip from the PyPI repository.
@@ -110,18 +110,50 @@
     def on_success(self, payload: Payload):
         logging.info(f'SUCCESS {payload.downloads}')
 
     # Method executed on bot failure
     def on_failure(self, payload: Payload):
         logging.info(f'FAILED {payload.output_data}')
 
+# Rapresentation of the data needed to extract from the HTML page.
+class InformationModel(BaseModel):
+    images_url: List[str] = Field(description="Images URL present in the page")
+    product_url: List[str] = Field(description="Product URL present in the page")
+    categories_names: List[str] = Field(description="Categories name present in the page")
+
+# Define a TestLLMTask class, which is a subclass of the Task class
+class TestLLMTask(Task):
+
+    # Main task code to be executed when running the script
+    def run(self, bot: Bot) -> bool:
+        # Log information about the current action
+        logging.info('DO THINGS')
+
+        # leverage the ai capabilities to automatically extract data from html (no need locators an manual data extraction)
+        extracted_data: str = LLMExtractor(bot=bot, pydantic_model=InformationModel).extract_data(locator_name='page_content_locator')
+
+        # set the extracted data as my output
+        bot.payload.output_data['information_model'] = extracted_data
+        
+        # For default, the task will succeed
+        return True
+
+    # Method executed on bot success, with its payload
+    def on_success(self, payload: Payload):
+        logging.info(f'SUCCESS {payload.downloads}')
+    
+    # Method executed on bot failure
+    def on_failure(self, payload: Payload):
+        logging.info(f'FAILED {payload.output_data}')
+
 # Check if the script is executed as the main program
 if __name__ == '__main__':
     # Start the above TestTask
-    TestTask()()
+    TestLLMTask()()
+    #TestTask()()
 ```
 
 **Attention**: This framework is flexible, you could also use only the Task class and the selenium's related functions inside the run method without using the POM (Page Object Model) or develop specific pages flow depending on your needs.
 
 ### Locators File
 
 In the locators configuration file `locators.ini`, all required locator configurations are defined.  
@@ -137,14 +169,29 @@
 
 [search_page] #*_page first page_name parameter, with it's related locators
 search_locator=(By.ID, "twotabsearchtextbox")
 product_locator=(By.XPATH, '//*[@id="search"]/div[1]/div[1]/div/span[1]/div[1]/div[2]')
 
 [product_page]#*_page second page_name parameter, with it's related locators
 name_locator=(By.ID, "title")
+
+[llm_extractor] # used by the llm extractor to get only a piecie of HTML because llm have a text limit
+page_content_locator=(By.ID, 'pageContent')
+```
+
+## AI Enanched
+It provides the LLMExtractor utility that leverage the language models LLM to automatically extract, parse and validate data from html pages and convert it into a json formatted string.  
+Remember to declare your data representation through a Pydantic class and the `llm_extractor` section in `locators.ini` with it's locator used as entry point to get the HTML as the the above example.
+Under the hood now uses [OpenAI ChatGPT3.5](https://openai.com/blog/chatgpt).  
+Specify your API Key in the settings, using the [OpenAI Page](https://platform.openai.com/api-keys).  
+
+```ini
+# settings.ini
+[settings]
+OPENAI_API_KEY="my-api-key"
 ```
 
 ## Settings
 
 ### Browser and Drivers 
 
 For default configuration, the selected browser is Firefox, but it could be changed from the `settings.ini` file:
```

### Comparing `fastbots-0.2.6/fastbots/__init__.py` & `fastbots-0.2.7/fastbots/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,11 +6,14 @@
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.common.alert import Alert
 from selenium.common.exceptions import TimeoutException, NoSuchElementException, ElementNotInteractableException, StaleElementReferenceException, ElementClickInterceptedException
 
 import capsolver
 
+from langchain_core.pydantic_v1 import BaseModel, Field
+
 from fastbots.bot import Bot
 from fastbots.page import Page
 from fastbots.task import Task
 from fastbots.payload import Payload
+from fastbots.llm_extractor import LLMExtractor
```

### Comparing `fastbots-0.2.6/fastbots/bot.py` & `fastbots-0.2.7/fastbots/bot.py`

 * *Files identical despite different names*

### Comparing `fastbots-0.2.6/fastbots/chrome_bot.py` & `fastbots-0.2.7/fastbots/chrome_bot.py`

 * *Files identical despite different names*

### Comparing `fastbots-0.2.6/fastbots/config.py` & `fastbots-0.2.7/fastbots/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,8 +103,11 @@
 # Specify all the url in scope for the capture, using a comma separated list (nothing by default)
 SELENIUM_IN_SCOPE_CAPTURE: str = config('SELENIUM_IN_SCOPE_CAPTURE', default=None, cast=str)
 
 # Enable Har capture (disabbled by default)
 SELENIUM_ENABLE_HAR_CAPTURE: bool = config('SELENIUM_ENABLE_HAR_CAPTURE', default=False, cast=bool)
 
 # Capsolver CHAPTCHA resolver service
-CAPSOLVER_API_KEY: str = config('CAPSOLVER_API_KEY', default=None, cast=str)
+CAPSOLVER_API_KEY: str = config('CAPSOLVER_API_KEY', default=None, cast=str)
+
+# OpenAI service for llm
+OPENAI_API_KEY: str = config('OPENAI_API_KEY', default=None, cast=str)
```

### Comparing `fastbots-0.2.6/fastbots/exceptions.py` & `fastbots-0.2.7/fastbots/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastbots-0.2.6/fastbots/firefox_bot.py` & `fastbots-0.2.7/fastbots/firefox_bot.py`

 * *Files identical despite different names*

### Comparing `fastbots-0.2.6/fastbots/logger.py` & `fastbots-0.2.7/fastbots/logger.py`

 * *Files identical despite different names*

### Comparing `fastbots-0.2.6/fastbots/page.py` & `fastbots-0.2.7/fastbots/page.py`

 * *Files identical despite different names*

### Comparing `fastbots-0.2.6/fastbots/task.py` & `fastbots-0.2.7/fastbots/task.py`

 * *Files identical despite different names*

### Comparing `fastbots-0.2.6/pyproject.toml` & `fastbots-0.2.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [tool.poetry]
 name = "fastbots"
-version = "0.2.6"
+version = "0.2.7"
 description = "A simple library designed for rapid bot and scraper development using Selenium and the POM (Page Object Model) design."
 authors = ["Uberti Davide <24529587+ubertidavide@users.noreply.github.com>"]
 license = "LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 selenium = "^4.15.2"
 python-decouple = "^3.8"
 tenacity = "^8.2.3"
 selenium-wire = "^5.1.0"
 capsolver = "^1.0.7"
+langchain = "^0.1.16"
+langchain-openai = "^0.1.3"
 
 [tool.poetry.group.dev.dependencies]
 setuptools = "^68.2.2"
 pytest = "^7.4.3"
 pytest-mock = "^3.12.0"
 mkdocstrings = {extras = ["python"], version = "^0.24.0"}
 mkdocs = "^1.5.3"
```

### Comparing `fastbots-0.2.6/PKG-INFO` & `fastbots-0.2.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: fastbots
-Version: 0.2.6
+Version: 0.2.7
 Summary: A simple library designed for rapid bot and scraper development using Selenium and the POM (Page Object Model) design.
 License: LICENSE
 Author: Uberti Davide
 Author-email: 24529587+ubertidavide@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: capsolver (>=1.0.7,<2.0.0)
+Requires-Dist: langchain (>=0.1.16,<0.2.0)
+Requires-Dist: langchain-openai (>=0.1.3,<0.2.0)
 Requires-Dist: python-decouple (>=3.8,<4.0)
 Requires-Dist: selenium (>=4.15.2,<5.0.0)
 Requires-Dist: selenium-wire (>=5.1.0,<6.0.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Description-Content-Type: text/markdown
 
 # fastbots
 
 [Fastbots](https://ubertidavide.github.io/fastbots/) is a simple library designed for rapid bot and scraper development using Selenium and the POM (Page Object Model) design.  
-It enhances productivity by allowing developers to focus solely on scraping, reducing boilerplate code, and eliminating the need for direct driver management-related code, thanks to browser-independent settings.  
+It enhances productivity by allowing developers to focus solely on scraping automatically using AI, reducing boilerplate code, and eliminating the need for direct driver management-related code, thanks to browser-independent settings.  
 Even if site locators change, this library doesn't require modifications to the code; adjustments can be made solely in the configuration.
 
 fastbots is also fully compatible with all selenium functions, refer to [selenium official documentation](https://www.selenium.dev/documentation/webdriver/elements/interactions/) for more details.
 
 ## Installation
 
 The installation process is straightforward using pip from the PyPI repository.
@@ -129,18 +131,50 @@
     def on_success(self, payload: Payload):
         logging.info(f'SUCCESS {payload.downloads}')
 
     # Method executed on bot failure
     def on_failure(self, payload: Payload):
         logging.info(f'FAILED {payload.output_data}')
 
+# Rapresentation of the data needed to extract from the HTML page.
+class InformationModel(BaseModel):
+    images_url: List[str] = Field(description="Images URL present in the page")
+    product_url: List[str] = Field(description="Product URL present in the page")
+    categories_names: List[str] = Field(description="Categories name present in the page")
+
+# Define a TestLLMTask class, which is a subclass of the Task class
+class TestLLMTask(Task):
+
+    # Main task code to be executed when running the script
+    def run(self, bot: Bot) -> bool:
+        # Log information about the current action
+        logging.info('DO THINGS')
+
+        # leverage the ai capabilities to automatically extract data from html (no need locators an manual data extraction)
+        extracted_data: str = LLMExtractor(bot=bot, pydantic_model=InformationModel).extract_data(locator_name='page_content_locator')
+
+        # set the extracted data as my output
+        bot.payload.output_data['information_model'] = extracted_data
+        
+        # For default, the task will succeed
+        return True
+
+    # Method executed on bot success, with its payload
+    def on_success(self, payload: Payload):
+        logging.info(f'SUCCESS {payload.downloads}')
+    
+    # Method executed on bot failure
+    def on_failure(self, payload: Payload):
+        logging.info(f'FAILED {payload.output_data}')
+
 # Check if the script is executed as the main program
 if __name__ == '__main__':
     # Start the above TestTask
-    TestTask()()
+    TestLLMTask()()
+    #TestTask()()
 ```
 
 **Attention**: This framework is flexible, you could also use only the Task class and the selenium's related functions inside the run method without using the POM (Page Object Model) or develop specific pages flow depending on your needs.
 
 ### Locators File
 
 In the locators configuration file `locators.ini`, all required locator configurations are defined.  
@@ -156,14 +190,29 @@
 
 [search_page] #*_page first page_name parameter, with it's related locators
 search_locator=(By.ID, "twotabsearchtextbox")
 product_locator=(By.XPATH, '//*[@id="search"]/div[1]/div[1]/div/span[1]/div[1]/div[2]')
 
 [product_page]#*_page second page_name parameter, with it's related locators
 name_locator=(By.ID, "title")
+
+[llm_extractor] # used by the llm extractor to get only a piecie of HTML because llm have a text limit
+page_content_locator=(By.ID, 'pageContent')
+```
+
+## AI Enanched
+It provides the LLMExtractor utility that leverage the language models LLM to automatically extract, parse and validate data from html pages and convert it into a json formatted string.  
+Remember to declare your data representation through a Pydantic class and the `llm_extractor` section in `locators.ini` with it's locator used as entry point to get the HTML as the the above example.
+Under the hood now uses [OpenAI ChatGPT3.5](https://openai.com/blog/chatgpt).  
+Specify your API Key in the settings, using the [OpenAI Page](https://platform.openai.com/api-keys).  
+
+```ini
+# settings.ini
+[settings]
+OPENAI_API_KEY="my-api-key"
 ```
 
 ## Settings
 
 ### Browser and Drivers 
 
 For default configuration, the selected browser is Firefox, but it could be changed from the `settings.ini` file:
```


# Comparing `tmp/gtsystem-0.0.8.tar.gz` & `tmp/gtsystem-0.0.9.tar.gz`

## Comparing `gtsystem-0.0.8.tar` & `gtsystem-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtsystem-0.0.8/gtsystem/__init__.py
--rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 gtsystem-0.0.8/gtsystem/bedrock.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 gtsystem-0.0.8/gtsystem/benchmark.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 gtsystem-0.0.8/gtsystem/instrument.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 gtsystem-0.0.8/gtsystem/ollama.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 gtsystem-0.0.8/gtsystem/openai.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 gtsystem-0.0.8/gtsystem/openai_master.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 gtsystem-0.0.8/gtsystem/render.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 gtsystem-0.0.8/gtsystem/tasks.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 gtsystem-0.0.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gtsystem-0.0.8/LICENSE
--rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 gtsystem-0.0.8/README.md
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 gtsystem-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 gtsystem-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtsystem-0.0.9/gtsystem/__init__.py
+-rw-r--r--   0        0        0     5532 2020-02-02 00:00:00.000000 gtsystem-0.0.9/gtsystem/bedrock.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 gtsystem-0.0.9/gtsystem/benchmark.py
+-rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 gtsystem-0.0.9/gtsystem/instrument.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 gtsystem-0.0.9/gtsystem/ollama.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 gtsystem-0.0.9/gtsystem/openai.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 gtsystem-0.0.9/gtsystem/openai_master.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 gtsystem-0.0.9/gtsystem/render.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 gtsystem-0.0.9/gtsystem/tasks.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 gtsystem-0.0.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gtsystem-0.0.9/LICENSE
+-rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 gtsystem-0.0.9/README.md
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 gtsystem-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     7880 2020-02-02 00:00:00.000000 gtsystem-0.0.9/PKG-INFO
```

### Comparing `gtsystem-0.0.8/gtsystem/bedrock.py` & `gtsystem-0.0.9/gtsystem/bedrock.py`

 * *Files 11% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 def list_models(vendor):
     if BEDROCK is None:
         init()
     listModels = BEDROCK.list_foundation_models(byProvider=vendor)
     print("\n".join(list(map(lambda x: f"{x['modelName']} : { x['modelId'] }", listModels['modelSummaries']))))
 
 @metrics.track
-def claude_text(system='', prompt='', temperature=0.0, topP=1.0, tokens=512, model='anthropic.claude-v2:1'):
+def claude_text(prompt, system='', temperature=0.0, topP=1.0, tokens=512, model='anthropic.claude-v2:1'):
 
     decorated_prompt = f'Human: {(system + " " + prompt).strip()}\n\nAssistant:\n'
     body = json.dumps({"prompt": decorated_prompt, 
                        "temperature": temperature,
                        "top_p": topP,
                        "max_tokens_to_sample": tokens})
     modelId = model
@@ -112,15 +112,15 @@
                      \nhttps://docs.aws.amazon.com/IAM/latest/UserGuide/troubleshoot_access-denied.html\
                      \nhttps://docs.aws.amazon.com/bedrock/latest/userguide/security-iam.html\x1b[0m\n")
     
         else:
             raise error
 
 @metrics.track        
-def llama_text(system='', prompt='', temperature=0.0, topP=1.0, tokens=512, model='meta.llama2-70b-chat-v1'):
+def llama_text(prompt, system='', temperature=0.0, topP=1.0, tokens=512, model='meta.llama2-70b-chat-v1'):
 
     if system != '':
         decorated_prompt = f'<<SYS>>{system}<</SYS>>\n[INST]User:{prompt}[/INST]\nAssistant:'
     else:
         decorated_prompt = prompt
 
     body = json.dumps({ 
@@ -153,7 +153,15 @@
                     \nTo troubeshoot this issue please refer to the following resources.\
                      \nhttps://docs.aws.amazon.com/IAM/latest/UserGuide/troubleshoot_access-denied.html\
                      \nhttps://docs.aws.amazon.com/bedrock/latest/userguide/security-iam.html\x1b[0m\n")
     
         else:
             raise error
 
+def text(prompt, system='', temperature=0.0, topP=1.0, tokens=512, model='llama2'):
+    match model:
+        case 'claude':
+            return claude_text(prompt, system, temperature, topP, model='anthropic.claude-v2:1')
+        case 'llama2':
+            return llama_text(prompt, system, temperature, topP, model='meta.llama2-70b-chat-v1')
+        case _:
+            return 'Please specify a valid model name'
```

### Comparing `gtsystem-0.0.8/gtsystem/benchmark.py` & `gtsystem-0.0.9/gtsystem/benchmark.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 from .openai_master import gpt_master
 
-def accuracy(system='', prompt='', result=''):
-    openai_system = """You are evaluating the accuracy of an LLM response. You will be given a system prompt and/or a user prompt, and response from an LLM and you will evaluate the response accuracy as a percentage to second decimal relative to your own response to the same system and/or user prompt. If you can evaluate the accuracy, you will  only respond with the response accuracy number. If you are not able to evaluate the accuracy, you will respond with the reason why you cannot evaluate the response."""
-    openai_prompt = f"""Evaluate the accuracy of the following LLM response based on the given System and/or User prompt:
+def accuracy(prompt, system='', result=''):
+    openai_system = """You are evaluating the accuracy of an LLM response. 
+    You will be given a system prompt and/or a user prompt, and response from an LLM and 
+    you will evaluate the response accuracy as a percentage to second decimal relative to 
+    your own response to the same system and/or user prompt. You will only respond with 
+    the response accuracy number. If you are not able to evaluate 
+    the accuracy, you will respond with 'Cannot Evaluate Accuracy'."""
+    openai_prompt = f"""Evaluate the accuracy of the following LLM response based on the 
+    given System and/or User prompt:
     System: {system} 
     User: {prompt}
     Response: {result}"""
 
-    accuracy = gpt_master(system=openai_system, prompt=openai_prompt)
+    accuracy = gpt_master(prompt=openai_prompt, system=openai_system)
     return accuracy
```

### Comparing `gtsystem-0.0.8/gtsystem/openai_master.py` & `gtsystem-0.0.9/gtsystem/openai_master.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from openai import OpenAI
 OPENAI = None
 
 def init():
     global OPENAI
     OPENAI = OpenAI()
 
-def gpt_master(system='', prompt='', temperature=0.0, topP=1, tokens=64, model="gpt-4-turbo-preview"):
+def gpt_master(prompt, system='', temperature=0.0, topP=1, tokens=64, model="gpt-4-0125-preview"):
     if OPENAI is None:
         init()
 
     response = OPENAI.chat.completions.create(
     model=model,
     messages=[
         {
```

### Comparing `gtsystem-0.0.8/gtsystem/render.py` & `gtsystem-0.0.9/gtsystem/render.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 def img(url):
     return Image(url=url)
 
 def df(df):
     # Set display options for max column width
     pd.set_option('display.max_colwidth', None)
+    pd.set_option('display.precision', 2)
 
     # Define CSS to hide the index and apply other styles
     styles = [
         dict(selector="th", props=[("font-size", "10pt"), ("text-align", "left")]),
         dict(selector="td", props=[
                                 ("text-align", "left"),
                                 ("word-wrap", "break-word"),
```

### Comparing `gtsystem-0.0.8/gtsystem/tasks.py` & `gtsystem-0.0.9/gtsystem/tasks.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 TASKS = None
 
 def get(task = ''):
     system = TASKS[TASKS['Task'] == task]['System'].values[0]
     prompt = TASKS[TASKS['Task'] == task]['Prompt'].values[0]
     temperature = float(TASKS[TASKS['Task'] == task]['Temperature'].values[0])
     topP = float(TASKS[TASKS['Task'] == task]['TopP'].values[0])
-    return system, prompt, temperature, topP
+    return prompt, system, temperature, topP
 
 def list(start=1, end=5):
     return TASKS.iloc[start:end]
 
 def find(task='', type='', prompt='', source=''):
     if type != '':
         df = TASKS[TASKS['Task Types'].str.contains(type, case=False)]
```

### Comparing `gtsystem-0.0.8/.gitignore` & `gtsystem-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `gtsystem-0.0.8/LICENSE` & `gtsystem-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gtsystem-0.0.8/README.md` & `gtsystem-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 3. **Load evaluation tasks from Excel:** Try `03-tasks.ipynb` for automating evaluation tasks - find, list, load prompts by task, including optimal parameter values for temperature and TopP.
 
 4. **Instrument speed and size (cost) of response:** Reuse `04-instrument.ipynb` for instrumenting and comparing multiple models across latency and size of response.
 
 4. **Benchmark quality of response:** Use `05-benchmark.ipynb` for automated benchmarking quality of responses from models like Llama and Claude using GPT-4 as an LLM evaluator.
 
-5. **Run models on your laptop:** Get `06-ollama.ipynb` to run models like Mistral, Llama, and Llava locally on your laptop and compare models hosted on Cloud or proprietary model APIs.
+5. **Run models on your laptop:** Get `06-ollama.ipynb` to run models like Mistral, Llama, and CodeLlama locally on your laptop and compare models hosted on Cloud or proprietary model APIs.
 
 ## Installing Dependencies
 
 You can install following dependencies to work with `gtsystem` based on your needs. Start with our `requirements.txt` or create your own. Then run `pip install -r requirements.txt` within your environment.
 
 ```
 # GenAI Techne System
```

### Comparing `gtsystem-0.0.8/pyproject.toml` & `gtsystem-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gtsystem"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="GenAI Techne", email="team@genaitechne.com" },
 ]
 description = "GenAI Techne System (gtsystem) is a low code Python package for crafting GenAI applications quickly"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `gtsystem-0.0.8/PKG-INFO` & `gtsystem-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtsystem
-Version: 0.0.8
+Version: 0.0.9
 Summary: GenAI Techne System (gtsystem) is a low code Python package for crafting GenAI applications quickly
 Project-URL: Homepage, https://github.com/GenaiTechne/gtsystem
 Project-URL: Issues, https://github.com/GenaiTechne/gtsystem/issues
 Author-email: GenAI Techne <team@genaitechne.com>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Jupyter
@@ -68,15 +68,15 @@
 
 3. **Load evaluation tasks from Excel:** Try `03-tasks.ipynb` for automating evaluation tasks - find, list, load prompts by task, including optimal parameter values for temperature and TopP.
 
 4. **Instrument speed and size (cost) of response:** Reuse `04-instrument.ipynb` for instrumenting and comparing multiple models across latency and size of response.
 
 4. **Benchmark quality of response:** Use `05-benchmark.ipynb` for automated benchmarking quality of responses from models like Llama and Claude using GPT-4 as an LLM evaluator.
 
-5. **Run models on your laptop:** Get `06-ollama.ipynb` to run models like Mistral, Llama, and Llava locally on your laptop and compare models hosted on Cloud or proprietary model APIs.
+5. **Run models on your laptop:** Get `06-ollama.ipynb` to run models like Mistral, Llama, and CodeLlama locally on your laptop and compare models hosted on Cloud or proprietary model APIs.
 
 ## Installing Dependencies
 
 You can install following dependencies to work with `gtsystem` based on your needs. Start with our `requirements.txt` or create your own. Then run `pip install -r requirements.txt` within your environment.
 
 ```
 # GenAI Techne System
```


# Comparing `tmp/ragtime-0.0.26.tar.gz` & `tmp/ragtime-0.0.27.tar.gz`

## Comparing `ragtime-0.0.26.tar` & `ragtime-0.0.27.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 ragtime-0.0.26/CONTRIBUTING.md
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ragtime-0.0.26/deploy/deploy.py
--rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 ragtime-0.0.26/img/Ragtime_logo.png
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/__init__.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/api.py
--rw-r--r--   0        0        0     8850 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/config.py
--rw-r--r--   0        0        0    19120 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/expe.py
--rw-r--r--   0        0        0    38773 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/generators.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/base_folder/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/base_folder/LICENSE
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/base_folder/README.md
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/base_folder/classes.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/base_folder/main.py
--rw-r--r--   0        0        0    15410 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/base_folder/res/html_templates/basic_template.jinja
--rw-r--r--   0        0        0    91060 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx
--rw-r--r--   0        0        0    31095 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/base_folder/res/spreadsheet_templates/basic_template.xlsx
--rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx
--rw-r--r--   0        0        0    33387 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/base_folder/res/spreadsheet_templates/spreadsheet_rich_template.xlsx
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 ragtime-0.0.26/tests/main.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 ragtime-0.0.26/tests/test_quest.json
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ragtime-0.0.26/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 ragtime-0.0.26/LICENSE
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 ragtime-0.0.26/README.md
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 ragtime-0.0.26/pyproject.toml
--rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 ragtime-0.0.26/PKG-INFO
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 ragtime-0.0.27/CONTRIBUTING.md
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ragtime-0.0.27/deploy/deploy.py
+-rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 ragtime-0.0.27/img/Ragtime_logo.png
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ragtime-0.0.27/src/ragtime/__init__.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 ragtime-0.0.27/src/ragtime/api.py
+-rw-r--r--   0        0        0     8850 2020-02-02 00:00:00.000000 ragtime-0.0.27/src/ragtime/config.py
+-rw-r--r--   0        0        0    19120 2020-02-02 00:00:00.000000 ragtime-0.0.27/src/ragtime/expe.py
+-rw-r--r--   0        0        0    38966 2020-02-02 00:00:00.000000 ragtime-0.0.27/src/ragtime/generators.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 ragtime-0.0.27/src/ragtime/base_folder/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragtime-0.0.27/src/ragtime/base_folder/LICENSE
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ragtime-0.0.27/src/ragtime/base_folder/README.md
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 ragtime-0.0.27/src/ragtime/base_folder/classes.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 ragtime-0.0.27/src/ragtime/base_folder/main.py
+-rw-r--r--   0        0        0    15410 2020-02-02 00:00:00.000000 ragtime-0.0.27/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx
+-rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 ragtime-0.0.27/src/ragtime/base_folder/res/html_templates/basic_template.jinja
+-rw-r--r--   0        0        0    91060 2020-02-02 00:00:00.000000 ragtime-0.0.27/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx
+-rw-r--r--   0        0        0    31095 2020-02-02 00:00:00.000000 ragtime-0.0.27/src/ragtime/base_folder/res/spreadsheet_templates/basic_template.xlsx
+-rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 ragtime-0.0.27/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx
+-rw-r--r--   0        0        0    33387 2020-02-02 00:00:00.000000 ragtime-0.0.27/src/ragtime/base_folder/res/spreadsheet_templates/spreadsheet_rich_template.xlsx
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 ragtime-0.0.27/tests/main.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 ragtime-0.0.27/tests/test_quest.json
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ragtime-0.0.27/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 ragtime-0.0.27/LICENSE
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 ragtime-0.0.27/README.md
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 ragtime-0.0.27/pyproject.toml
+-rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 ragtime-0.0.27/PKG-INFO
```

### Comparing `ragtime-0.0.26/img/Ragtime_logo.png` & `ragtime-0.0.27/img/Ragtime_logo.png`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.26/src/ragtime/__init__.py` & `ragtime-0.0.27/src/ragtime/__init__.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.26/src/ragtime/api.py` & `ragtime-0.0.27/src/ragtime/api.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.26/src/ragtime/config.py` & `ragtime-0.0.27/src/ragtime/config.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.26/src/ragtime/expe.py` & `ragtime-0.0.27/src/ragtime/expe.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.26/src/ragtime/generators.py` & `ragtime-0.0.27/src/ragtime/generators.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Optional
 from ragtime.expe import Answer, Answers, Chunks, Eval, Expe, Fact, Facts, LLMAnswer, Question, RagtimeBase, QA, Prompt, WithLLMAnswer
 from litellm import completion_cost, completion
 from ragtime.config import RagtimeException, logger, div0
 import re
 
 import litellm
+litellm.telemetry = False
 
 #################################
 ## CONSTANTS
 #################################
 UNKOWN_LLM:str = "unkown LLM (manual ?)"
 
 #################################
@@ -243,22 +244,24 @@
         answer:str = cur_obj.llm_answer.text if cur_obj.llm_answer.text != "[]" else ""
         answer = answer.replace('(FAIT ', '(') # removes the word FAIT before the fact number as it is sometimes generated in the answer
         # get the set of facts numbers from answer
         facts_in_answer:set[int] = set([int(s) for s in ','.join(re.findall('\([\d+,+\s+]+\)',answer)).replace('(','').replace(')','').split(',') if s])
         # get the numbers in the true facts
         true_facts:set[int] = set([int(s.text[0] if s.text[1] == '.' else s.text[:2]) for s in qa.facts if s])
         true_facts_in_answer:set[int] = facts_in_answer & true_facts
+        true_facts_not_in_answer:set[int] = true_facts - true_facts_in_answer
         # get the number of hallucinations (?)
         nb_false_facts_in_answer:int = len(re.findall("\(\?\)", answer))
         # compute metrics
         precision:float = div0(len(true_facts_in_answer), len(facts_in_answer)+nb_false_facts_in_answer)
         recall:float = div0(len(true_facts_in_answer), len(true_facts))
         cur_obj.meta["precision"] = precision
         cur_obj.meta["recall"] = recall
         cur_obj.meta["hallus"] = nb_false_facts_in_answer
+        cur_obj.meta["missing"] = ', '.join(list(true_facts_not_in_answer))
         cur_obj.meta["facts_in_ans"] = str(sorted(facts_in_answer))
         cur_obj.auto = div0(2*precision*recall, precision+recall)
         cur_obj.text = answer
 
 class PptrSimpleEvalFR(Prompter):
     def get_prompt(self, answer:Answer, facts:Facts) -> Prompt:
         result:Prompt = Prompt()
@@ -486,14 +489,15 @@
                 self.gen_for_qa(qa=qa, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms)
                 logger.info(f'End question "{qa.question.text}"')
                 if save_every and (num_q % save_every == 0): expe.save_to_json()
         except Exception as e:
             logger.exception(f"Exception caught - saving what has been done so far:\n{e}")
             expe.save_temp(name=f"Stopped_at_{num_q}_of_{nb_q}_")
             return False
+        
         return True
 
     def write_chunks(self, qa:QA):
         """Write chunks in the current qa if a Retriever has been given when creating the object. Ignore otherwise"""
         raise NotImplementedError('Must implement this if you want to use it!')
     
     @abstractmethod
```

### Comparing `ragtime-0.0.26/src/ragtime/base_folder/.gitignore` & `ragtime-0.0.27/src/ragtime/base_folder/.gitignore`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.26/src/ragtime/base_folder/LICENSE` & `ragtime-0.0.27/src/ragtime/base_folder/LICENSE`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.26/src/ragtime/base_folder/classes.py` & `ragtime-0.0.27/src/ragtime/base_folder/classes.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.26/src/ragtime/base_folder/main.py` & `ragtime-0.0.27/src/ragtime/base_folder/main.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.26/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx` & `ragtime-0.0.27/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.26/src/ragtime/base_folder/res/html_templates/basic_template.jinja` & `ragtime-0.0.27/src/ragtime/base_folder/res/html_templates/basic_template.jinja`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.26/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx` & `ragtime-0.0.27/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.26/src/ragtime/base_folder/res/spreadsheet_templates/basic_template.xlsx` & `ragtime-0.0.27/src/ragtime/base_folder/res/spreadsheet_templates/basic_template.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.26/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx` & `ragtime-0.0.27/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.26/src/ragtime/base_folder/res/spreadsheet_templates/spreadsheet_rich_template.xlsx` & `ragtime-0.0.27/src/ragtime/base_folder/res/spreadsheet_templates/spreadsheet_rich_template.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.26/tests/main.py` & `ragtime-0.0.27/tests/main.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.26/tests/test_quest.json` & `ragtime-0.0.27/tests/test_quest.json`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.26/.gitignore` & `ragtime-0.0.27/.gitignore`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.26/LICENSE` & `ragtime-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.26/README.md` & `ragtime-0.0.27/README.md`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.26/pyproject.toml` & `ragtime-0.0.27/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ragtime"
-version = "0.0.26"
+version = "0.0.27"
 
 authors = [
   { name="Gilles Moyse", email="gilles@recital.ai" },
 ]
 maintainers = [
   { name="reciTAL", email="ragtime@recital.ai" },
 ]
```

### Comparing `ragtime-0.0.26/PKG-INFO` & `ragtime-0.0.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragtime
-Version: 0.0.26
+Version: 0.0.27
 Summary: Ragtime 🎹 is an LLMOps framework to automatically evaluate Retrieval Augmented Generation (RAG) systems and compare different RAGs / LLMs
 Project-URL: Homepage, https://github.com/recitalAI/ragtime-package
 Project-URL: Issues, https://github.com/recitalAI/ragtime-package/issues
 Author-email: Gilles Moyse <gilles@recital.ai>
 Maintainer-email: reciTAL <ragtime@recital.ai>
 License: MIT License
```


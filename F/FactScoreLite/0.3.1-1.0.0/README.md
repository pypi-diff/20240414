# Comparing `tmp/FactScoreLite-0.3.1.tar.gz` & `tmp/factscorelite-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FactScoreLite-0.3.1.tar", last modified: Thu Apr  4 23:57:40 2024, max compression
+gzip compressed data, was "factscorelite-1.0.0.tar", last modified: Sat Apr 13 23:42:24 2024, max compression
```

## Comparing `FactScoreLite-0.3.1.tar` & `factscorelite-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:57:40.320932 FactScoreLite-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:57:40.316932 FactScoreLite-0.3.1/FactScoreLite/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-04 23:57:36.000000 FactScoreLite-0.3.1/FactScoreLite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-04 23:57:36.000000 FactScoreLite-0.3.1/FactScoreLite/atomic_facts.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 23:57:36.000000 FactScoreLite-0.3.1/FactScoreLite/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:57:40.316932 FactScoreLite-0.3.1/FactScoreLite/data/
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-04-04 23:57:36.000000 FactScoreLite-0.3.1/FactScoreLite/data/demons.json
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-04 23:57:36.000000 FactScoreLite-0.3.1/FactScoreLite/data/demons_generation_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-04 23:57:36.000000 FactScoreLite-0.3.1/FactScoreLite/fact_scorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-04 23:57:36.000000 FactScoreLite-0.3.1/FactScoreLite/openai_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:57:40.320932 FactScoreLite-0.3.1/FactScoreLite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-04 23:57:40.000000 FactScoreLite-0.3.1/FactScoreLite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-04 23:57:40.000000 FactScoreLite-0.3.1/FactScoreLite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:57:40.000000 FactScoreLite-0.3.1/FactScoreLite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 23:57:40.000000 FactScoreLite-0.3.1/FactScoreLite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-04 23:57:40.000000 FactScoreLite-0.3.1/FactScoreLite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-04 23:57:36.000000 FactScoreLite-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-04 23:57:40.320932 FactScoreLite-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-04 23:57:36.000000 FactScoreLite-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-04 23:57:40.320932 FactScoreLite-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 23:57:36.000000 FactScoreLite-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:57:40.316932 FactScoreLite-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:57:36.000000 FactScoreLite-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-04 23:57:36.000000 FactScoreLite-0.3.1/tests/test_atomic_facts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11274 2024-04-04 23:57:36.000000 FactScoreLite-0.3.1/tests/test_openai_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-04 23:57:36.000000 FactScoreLite-0.3.1/tests/test_scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:42:24.926438 factscorelite-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:42:24.922438 factscorelite-1.0.0/FactScoreLite/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-13 23:42:21.000000 factscorelite-1.0.0/FactScoreLite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-13 23:42:21.000000 factscorelite-1.0.0/FactScoreLite/atomic_facts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-13 23:42:21.000000 factscorelite-1.0.0/FactScoreLite/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:42:24.922438 factscorelite-1.0.0/FactScoreLite/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-04-13 23:42:21.000000 factscorelite-1.0.0/FactScoreLite/data/demons.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-13 23:42:21.000000 factscorelite-1.0.0/FactScoreLite/data/demons_generation_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-13 23:42:21.000000 factscorelite-1.0.0/FactScoreLite/fact_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-13 23:42:21.000000 factscorelite-1.0.0/FactScoreLite/factscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-13 23:42:21.000000 factscorelite-1.0.0/FactScoreLite/openai_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-13 23:42:21.000000 factscorelite-1.0.0/FactScoreLite/state_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:42:24.926438 factscorelite-1.0.0/FactScoreLite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-13 23:42:24.000000 factscorelite-1.0.0/FactScoreLite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-13 23:42:24.000000 factscorelite-1.0.0/FactScoreLite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 23:42:24.000000 factscorelite-1.0.0/FactScoreLite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-13 23:42:24.000000 factscorelite-1.0.0/FactScoreLite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-13 23:42:24.000000 factscorelite-1.0.0/FactScoreLite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-13 23:42:21.000000 factscorelite-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-13 23:42:24.926438 factscorelite-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-13 23:42:21.000000 factscorelite-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-13 23:42:24.926438 factscorelite-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 23:42:21.000000 factscorelite-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:42:24.926438 factscorelite-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 23:42:21.000000 factscorelite-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-13 23:42:21.000000 factscorelite-1.0.0/tests/test_atomic_facts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-13 23:42:21.000000 factscorelite-1.0.0/tests/test_fact_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-13 23:42:21.000000 factscorelite-1.0.0/tests/test_factscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11274 2024-04-13 23:42:21.000000 factscorelite-1.0.0/tests/test_openai_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-13 23:42:21.000000 factscorelite-1.0.0/tests/test_state_handler.py
```

### Comparing `FactScoreLite-0.3.1/FactScoreLite/atomic_facts.py` & `factscorelite-1.0.0/FactScoreLite/atomic_facts.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
         Returns:
             list: A list of atomic facts extracted from the sentence.
         """
         atoms = None
         instructions = self.get_instructions()
 
-        prompt = instructions + f"Sentence: {sent}\nIndependent Facts:"
+        prompt = instructions + f"Sentence:\n{sent}\nIndependent Facts:"
 
         output = self.openai_agent.generate(prompt)
         atoms = self.gpt_output_to_sentences(output)
 
         return atoms
 
     def gpt_output_to_sentences(self, text: str) -> list:
```

### Comparing `FactScoreLite-0.3.1/FactScoreLite/data/demons.json` & `factscorelite-1.0.0/FactScoreLite/data/demons.json`

 * *Files identical despite different names*

### Comparing `FactScoreLite-0.3.1/FactScoreLite/data/demons_generation_prompt.txt` & `factscorelite-1.0.0/FactScoreLite/data/demons_generation_prompt.txt`

 * *Files identical despite different names*

### Comparing `FactScoreLite-0.3.1/FactScoreLite/fact_scorer.py` & `factscorelite-1.0.0/FactScoreLite/fact_scorer.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 
 
 class FactScorer:
     def __init__(self):
         # To interact with OpenAI APIs
         self.openai_agent = OpenAIAgent()
 
-    def get_score(self, atomic_facts: list, knowledge_source: str) -> list:
+    def get_score(self, facts: list, knowledge_source: str) -> list:
         """
         Calculates the score of each atomic fact based on the knowledge source.
         The score is caclulated by using the OpenAI API.
 
         Args:
-            atomic_facts (list): A list of atomic facts to be scored.
+            facts (list): A list of atomic  to be scored.
             knowledge_source (str): The knowledge source to be used for scoring.
 
         Returns:
             list: A list of dictionaries containing the atomic fact and its score.
         """
 
         decisions = []
 
-        for atom in atomic_facts:
+        for atom in facts:
             atom = atom.strip()
 
             # Prompt that will be sent to GPT
             prompt = "Answer the question based on the given context.\n\n"
             prompt += f"Context:\n{knowledge_source}"
 
             if not prompt[-1] in string.punctuation:
@@ -62,10 +62,12 @@
                             "cannot",
                             "unknown",
                             "information",
                         ]
                     ]
                 )
 
-            decisions.append({atom: is_supported})
+            decisions.append(
+                {"fact": atom, "is_supported": is_supported, "output": output}
+            )
 
         return decisions
```

### Comparing `FactScoreLite-0.3.1/FactScoreLite/openai_agent.py` & `factscorelite-1.0.0/FactScoreLite/openai_agent.py`

 * *Files identical despite different names*

### Comparing `FactScoreLite-0.3.1/FactScoreLite.egg-info/SOURCES.txt` & `factscorelite-1.0.0/FactScoreLite.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 README.md
 setup.cfg
 setup.py
 FactScoreLite/__init__.py
 FactScoreLite/atomic_facts.py
 FactScoreLite/configs.py
 FactScoreLite/fact_scorer.py
+FactScoreLite/factscore.py
 FactScoreLite/openai_agent.py
+FactScoreLite/state_handler.py
 FactScoreLite.egg-info/PKG-INFO
 FactScoreLite.egg-info/SOURCES.txt
 FactScoreLite.egg-info/dependency_links.txt
 FactScoreLite.egg-info/requires.txt
 FactScoreLite.egg-info/top_level.txt
 FactScoreLite/data/demons.json
 FactScoreLite/data/demons_generation_prompt.txt
 tests/__init__.py
 tests/test_atomic_facts.py
+tests/test_fact_scorer.py
+tests/test_factscore.py
 tests/test_openai_agent.py
-tests/test_scorer.py
+tests/test_state_handler.py
```

### Comparing `FactScoreLite-0.3.1/LICENSE` & `factscorelite-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FactScoreLite-0.3.1/tests/test_atomic_facts.py` & `factscorelite-1.0.0/tests/test_atomic_facts.py`

 * *Files identical despite different names*

### Comparing `FactScoreLite-0.3.1/tests/test_openai_agent.py` & `factscorelite-1.0.0/tests/test_openai_agent.py`

 * *Files identical despite different names*

### Comparing `FactScoreLite-0.3.1/tests/test_scorer.py` & `factscorelite-1.0.0/tests/test_fact_scorer.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 )
 def test_get_score_response_interpretation(
     fact_scorer, mock_openai_agent, response, expected
 ):
     mock_openai_agent.generate.return_value = response
     result = fact_scorer.get_score(["Fact 1"], "Knowledge source")
     assert result == [
-        {"Fact 1": expected}
+        {"fact": "Fact 1", "is_supported": expected, "output": response}
     ], f"Expected decision to be {expected} for response '{response}'."
 
 
 def test_error_handling_when_openai_agent_fails(fact_scorer, mock_openai_agent):
     mock_openai_agent.generate.side_effect = Exception("Network error")
     with pytest.raises(Exception):
         fact_scorer.get_score(["Fact 1"], "Knowledge source")
```


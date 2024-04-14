# Comparing `tmp/statecraft-0.2.0.tar.gz` & `tmp/statecraft-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statecraft-0.2.0.tar", max compression
+gzip compressed data, was "statecraft-0.3.0.tar", max compression
```

## Comparing `statecraft-0.2.0.tar` & `statecraft-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11358 2024-04-03 11:02:42.934332 statecraft-0.2.0/LICENSE
--rw-r--r--   0        0        0     3125 2024-04-06 21:45:35.753326 statecraft-0.2.0/README.md
--rw-r--r--   0        0        0      993 2024-04-08 09:40:25.775390 statecraft-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      236 2024-04-03 10:36:07.499173 statecraft-0.2.0/statecraft/__init__.py
--rw-r--r--   0        0        0      849 2024-03-27 00:09:23.511207 statecraft-0.2.0/statecraft/_setup.py
--rw-r--r--   0        0        0     1816 2024-04-07 23:03:02.330960 statecraft-0.2.0/statecraft/cache.py
--rw-r--r--   0        0        0     4513 2024-04-07 23:03:02.332394 statecraft-0.2.0/statecraft/client.py
--rw-r--r--   0        0        0    16342 2024-04-07 23:03:02.334208 statecraft-0.2.0/statecraft/core.py
--rw-r--r--   0        0        0      287 2024-03-26 13:46:51.357963 statecraft-0.2.0/statecraft/metadata.py
--rw-r--r--   0        0        0      417 2024-04-07 23:03:02.340045 statecraft-0.2.0/statecraft/models.py
--rw-r--r--   0        0        0     1682 2024-04-03 10:35:22.202552 statecraft-0.2.0/statecraft/states_list.py
--rw-r--r--   0        0        0      195 2024-03-27 00:03:59.367245 statecraft-0.2.0/statecraft/user_attributes.py
--rw-r--r--   0        0        0      838 2024-04-07 23:03:02.340438 statecraft-0.2.0/statecraft/utils.py
--rw-r--r--   0        0        0     4370 1970-01-01 00:00:00.000000 statecraft-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-14 01:03:08.654304 statecraft-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3125 2024-04-14 01:03:08.654304 statecraft-0.3.0/README.md
+-rw-r--r--   0        0        0     1041 2024-04-14 01:03:08.654304 statecraft-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      236 2024-04-14 01:03:08.654304 statecraft-0.3.0/statecraft/__init__.py
+-rw-r--r--   0        0        0      849 2024-04-14 01:03:08.654304 statecraft-0.3.0/statecraft/_setup.py
+-rw-r--r--   0        0        0     2389 2024-04-14 01:03:08.654304 statecraft-0.3.0/statecraft/cache.py
+-rw-r--r--   0        0        0     4513 2024-04-14 01:03:08.654304 statecraft-0.3.0/statecraft/client.py
+-rw-r--r--   0        0        0    18710 2024-04-14 01:03:08.654304 statecraft-0.3.0/statecraft/core.py
+-rw-r--r--   0        0        0      818 2024-04-14 01:03:08.654304 statecraft-0.3.0/statecraft/metadata.py
+-rw-r--r--   0        0        0      417 2024-04-14 01:03:08.658304 statecraft-0.3.0/statecraft/models.py
+-rw-r--r--   0        0        0     1682 2024-04-14 01:03:08.658304 statecraft-0.3.0/statecraft/states_list.py
+-rw-r--r--   0        0        0      195 2024-04-14 01:03:08.658304 statecraft-0.3.0/statecraft/user_attributes.py
+-rw-r--r--   0        0        0      838 2024-04-14 01:03:08.658304 statecraft-0.3.0/statecraft/utils.py
+-rw-r--r--   0        0        0     4367 1970-01-01 00:00:00.000000 statecraft-0.3.0/PKG-INFO
```

### Comparing `statecraft-0.2.0/LICENSE` & `statecraft-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `statecraft-0.2.0/README.md` & `statecraft-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `statecraft-0.2.0/pyproject.toml` & `statecraft-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "statecraft"
-version = "0.2.0"
+version = "0.3.0"
 description = "Store, manage and remix states for SSMs and other Stateful models"
 authors = ["koayon <koayon@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "statecraft"}]
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -24,18 +24,19 @@
 
 [tool.poetry.dependencies]
 einops= "^0.6.1"
 pydantic = "^2.5.3"
 python = "^3.8"
 python-dotenv = "^0.19.1"
 Requests = "^2.31.0"
-torch = "^2.1.2"
 transformers = "^4.39.3"
 typer = "^0.7.0"
 accelerate = "^0.29.1"
+torch = "^2.2.2"
+# causal-conv1d = "^1.2.0"
+# mamba-ssm = "^1.2.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
-pylint = "^2.17.4"
-setuptools = "^67.7.2"
-poetry = "^1.8.2"
+pylint = ">=2.17.4,<4.0.0"
+setuptools = "^67.7.2,<70.0.0"
```

### Comparing `statecraft-0.2.0/statecraft/_setup.py` & `statecraft-0.3.0/statecraft/_setup.py`

 * *Files identical despite different names*

### Comparing `statecraft-0.2.0/statecraft/cache.py` & `statecraft-0.3.0/statecraft/cache.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import torch as t
 from transformers.models.mamba.modeling_mamba import MambaCache as HFMambaCache
 from transformers.models.mamba.modeling_mamba import MambaConfig
 
 
 class MambaCache(HFMambaCache):
     def to(self, device):
-        mamba_cache = copy.deepcopy(self)
+        mamba_cache = copy.copy(self)
 
         ssm_states = {
             layer_num: layer_cache.to(device)
             for layer_num, layer_cache in mamba_cache.ssm_states.items()
         }
 
         conv_states = {
@@ -21,18 +21,40 @@
         }
 
         mamba_cache.ssm_states = ssm_states
         mamba_cache.conv_states = conv_states
 
         return mamba_cache
 
+    def to_dtype(self, dtype):
+        mamba_cache = copy.copy(self)
+
+        ssm_states = {
+            layer_num: layer_cache.to(dtype)
+            for layer_num, layer_cache in mamba_cache.ssm_states.items()
+        }
+
+        conv_states = {
+            layer_num: layer_cache.to(dtype)
+            for layer_num, layer_cache in mamba_cache.conv_states.items()
+        }
+
+        mamba_cache.ssm_states = ssm_states
+        mamba_cache.conv_states = conv_states
+
+        return mamba_cache
+
     @property
     def device(self):
         return self.ssm_states[0].device
 
+    # @property
+    # def dtype(self):
+    #     return self.ssm_states[0].dtype
+
     # def __iadd__(self, other: "MambaCache"):
     #     for layer_num, layer_cache in self.ssm_states.items():
     #         layer_cache += other.ssm_states[layer_num]
     #     for layer_num, layer_cache in self.conv_states.items():
     #         layer_cache += other.conv_states[layer_num]
     #     return self
```

### Comparing `statecraft-0.2.0/statecraft/client.py` & `statecraft-0.3.0/statecraft/client.py`

 * *Files identical despite different names*

### Comparing `statecraft-0.2.0/statecraft/core.py` & `statecraft-0.3.0/statecraft/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import io
 import json
+import math
 import os
 from pathlib import Path
 from typing import Any, Optional, Union
 
 import torch as t
 from einops import einsum
+from tqdm import tqdm
 from transformers import AutoTokenizer, MambaForCausalLM, PreTrainedModel
 from transformers.generation.utils import GenerateOutput
 from transformers.models.mamba.modeling_mamba import MambaCache as HFMambaCache
 from transformers.models.mamba.modeling_mamba import MambaCausalLMOutput
 
 from statecraft.cache import MambaCache
 from statecraft.client import client
@@ -41,15 +43,15 @@
 
     is_local = os.path.isdir(base_path)
     if not is_local:
         raise CantFindLocalStateError(
             "Path to saved state must be a directory which exists on the system"
         )
 
-    state = t.load(os.path.join(base_path, "state.pt"))
+    state = t.load(os.path.join(base_path, "state.pt"), map_location=default_device())
 
     with open(os.path.join(base_path, "metadata.json"), "r") as json_file:
         metadata_dict: dict[str, Any] = json.load(json_file)
 
     for key in ("state_name", "model_name", "prompt"):
         if key not in metadata_dict:
             raise CorruptedMetadataError(f"Metadata must contain key: {key}")
@@ -139,16 +141,22 @@
         **kwargs,
     ) -> Union[t.LongTensor, GenerateOutput]:
         if cache_params is None:
             cache_params = self.initial_state
         if reset_sequence_offset:
             cache_params = self._reset_state_offset(cache_params)
 
+        cache_params = cache_params.to_dtype(self.model.dtype)
+
         out = self.model.generate(
-            input_ids=input_ids, max_length=max_length, cache_params=cache_params, **kwargs
+            input_ids=input_ids,
+            max_length=max_length,
+            cache_params=cache_params,
+            use_cache=True,
+            **kwargs,
         )
 
         return out
 
     @classmethod
     def from_pretrained(
         cls,
@@ -164,30 +172,92 @@
             initial_state = cls._load_state(model_name, initial_state_name)
         else:
             initial_state = None
 
         stateful_model = cls(
             model=model, initial_state=initial_state, model_name=model_name, device=device
         )
-        return stateful_model
+        return stateful_model.to(device)  # type: ignore
 
     def build_state(
         self,
+        state_name: str,
+        prompt: str,
+        description: Optional[str] = None,
+        tags: Optional[list[str]] = None,
+        cache_params: Optional[MambaCache] = None,
+        model_name: Optional[str] = None,
+        prompt_reference: Optional[str] = None,
+        chunk_size: int = 256,
+    ) -> tuple[MambaCache, SSMStateMetadata]:
+        # Check if model_name is provided
+        model_name = model_name or self.model_name
+        if model_name is None:
+            raise ValueError("Model name must be provided.")
+
+        tokeniser = AutoTokenizer.from_pretrained(model_name)
+        tokenised_ids: t.Tensor = tokeniser(prompt, return_tensors="pt")["input_ids"]  # type: ignore
+
+        print("Tokenised ids shape: ", tokenised_ids.shape)
+
+        # TODO: Chunk tokenization
+
+        cache_params = cache_params or MambaCache(
+            config=self.model.config, batch_size=1, device=self.initial_state.device
+        )
+
+        batch, seq_len = tokenised_ids.shape
+        num_chunks = math.ceil(seq_len / chunk_size)
+        for i in tqdm(range(0, seq_len, chunk_size)):
+            # print(f"chunk {i//chunk_size}/{num_chunks} of {num_chunks}")
+
+            chunk = tokenised_ids[:, i : i + chunk_size].to(self.device)
+
+            cache_params = self._build_state(
+                input_ids=chunk.to(self.device),
+                cache_params=cache_params.to(self.device),
+                model_name=model_name,
+            )
+
+            # Move the tensors back to CPU and delete them
+            chunk = chunk.to("cpu")
+            del chunk
+
+            # Clear the GPU cache
+            t.cuda.empty_cache()
+
+        metadata = SSMStateMetadata(
+            state_name=state_name,
+            prompt=prompt_reference or prompt,
+            model_name=model_name,
+            description=description,
+            keywords=tags,
+        )
+
+        return cache_params, metadata
+
+    def _build_state(
+        self,
         input_ids: t.Tensor,
         cache_params: Optional[MambaCache] = None,
         model_name: Optional[str] = None,
     ) -> MambaCache:
         # Check if model_name is provided
         if model_name is None and self.model_name is None:
             raise ValueError("Model name must be provided.")
         elif model_name is None:
             model_name = self.model_name
         assert model_name is not None
 
-        out: MambaCausalLMOutput = self.forward(input_ids=input_ids, cache_params=cache_params)
+        # print("about to forward")
+        with t.no_grad():
+            out: MambaCausalLMOutput = self.forward(
+                input_ids=input_ids, cache_params=cache_params
+            )
+
         assert out.cache_params is not None
 
         mamba_cache = MambaCache.from_hf_cache(
             hf_cache=out.cache_params, model_name=model_name
         )
         return mamba_cache
 
@@ -327,34 +397,37 @@
         self.update_state(state)
 
     def update_state(self, state: MambaCache) -> None:
         self.initial_state = state
 
     def reset_state(self) -> None:
         device = self.initial_state.device
-        self.initial_state = MambaCache(config=self.model.config, batch_size=1, device=device)
+        dtype = self.initial_state.dtype
+        self.initial_state = MambaCache(
+            config=self.model.config, batch_size=1, device=device, dtype=dtype
+        )
 
     # HELPER METHODS
 
     @classmethod
     def _save_state_binaries(
         cls,
         state_bytes: bytes,
         model_name_path: str,
         state_name_path: str,
         cache_dir: Optional[str] = None,
     ) -> None:
         cache_dir = cls._get_default_cache_dir() if cache_dir is None else cache_dir
         base_path = os.path.join(cache_dir, model_name_path, state_name_path)
 
-        os.makedirs(base_path, exist_ok=False)
+        os.makedirs(base_path, exist_ok=True)
 
         byte_stream = io.BytesIO(state_bytes)
         try:
-            state = t.load(byte_stream)
+            state = t.load(byte_stream, map_location=default_device())
         except Exception as e:
             raise IOError(
                 f"Failed to parse downloaded state from bytes.",
             )
 
         state_path = os.path.join(base_path, "state.pt")
         t.save(state, state_path)
```

### Comparing `statecraft-0.2.0/statecraft/states_list.py` & `statecraft-0.3.0/statecraft/states_list.py`

 * *Files identical despite different names*

### Comparing `statecraft-0.2.0/statecraft/utils.py` & `statecraft-0.3.0/statecraft/utils.py`

 * *Files identical despite different names*

### Comparing `statecraft-0.2.0/PKG-INFO` & `statecraft-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statecraft
-Version: 0.2.0
+Version: 0.3.0
 Summary: Store, manage and remix states for SSMs and other Stateful models
 License: Apache-2.0
 Author: koayon
 Author-email: koayon@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -12,22 +12,22 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
 Requires-Dist: Requests (>=2.31.0,<3.0.0)
 Requires-Dist: accelerate (>=0.29.1,<0.30.0)
 Requires-Dist: einops (>=0.6.1,<0.7.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: python-dotenv (>=0.19.1,<0.20.0)
-Requires-Dist: torch (>=2.1.2,<3.0.0)
+Requires-Dist: torch (>=2.2.2,<3.0.0)
 Requires-Dist: transformers (>=4.39.3,<5.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Project-URL: Repository, https://github.com/koayon/statecraft.git
 Description-Content-Type: text/markdown
 
 # 🪄 Statecraft -  Load, store and remix states for SSMs, Mamba and Stateful models
```


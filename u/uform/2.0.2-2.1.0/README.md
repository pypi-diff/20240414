# Comparing `tmp/uform-2.0.2.tar.gz` & `tmp/uform-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uform-2.0.2.tar", last modified: Thu Mar 28 20:44:08 2024, max compression
+gzip compressed data, was "uform-2.1.0.tar", last modified: Sun Apr 14 00:51:21 2024, max compression
```

## Comparing `uform-2.0.2.tar` & `uform-2.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:44:08.527103 uform-2.0.2/
--rwxr-xr-x   0 runner    (1001) docker     (127)    11357 2024-03-28 20:44:04.000000 uform-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    27269 2024-03-28 20:44:08.527103 uform-2.0.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    25346 2024-03-28 20:44:04.000000 uform-2.0.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2656 2024-03-28 20:44:04.000000 uform-2.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:44:08.523103 uform-2.0.2/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:44:08.523103 uform-2.0.2/python/uform/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1963 2024-03-28 20:44:04.000000 uform-2.0.2/python/uform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-03-28 20:44:04.000000 uform-2.0.2/python/uform/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-03-28 20:44:04.000000 uform-2.0.2/python/uform/gen_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-03-28 20:44:04.000000 uform-2.0.2/python/uform/numpy_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-03-28 20:44:04.000000 uform-2.0.2/python/uform/onnx_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-03-28 20:44:04.000000 uform-2.0.2/python/uform/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    15465 2024-03-28 20:44:04.000000 uform-2.0.2/python/uform/torch_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-03-28 20:44:04.000000 uform-2.0.2/python/uform/torch_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:44:08.527103 uform-2.0.2/python/uform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27269 2024-03-28 20:44:08.000000 uform-2.0.2/python/uform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-28 20:44:08.000000 uform-2.0.2/python/uform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 20:44:08.000000 uform-2.0.2/python/uform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-28 20:44:08.000000 uform-2.0.2/python/uform.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-28 20:44:08.000000 uform-2.0.2/python/uform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-28 20:44:08.000000 uform-2.0.2/python/uform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 20:44:08.527103 uform-2.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:51:21.702597 uform-2.1.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11357 2024-04-14 00:51:14.000000 uform-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    27269 2024-04-14 00:51:21.698597 uform-2.1.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25346 2024-04-14 00:51:14.000000 uform-2.1.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2656 2024-04-14 00:51:14.000000 uform-2.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:51:21.694597 uform-2.1.0/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:51:21.698597 uform-2.1.0/python/uform/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1963 2024-04-14 00:51:14.000000 uform-2.1.0/python/uform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-14 00:51:14.000000 uform-2.1.0/python/uform/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-04-14 00:51:14.000000 uform-2.1.0/python/uform/gen_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-14 00:51:14.000000 uform-2.1.0/python/uform/numpy_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-04-14 00:51:14.000000 uform-2.1.0/python/uform/onnx_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-14 00:51:14.000000 uform-2.1.0/python/uform/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-04-14 00:51:14.000000 uform-2.1.0/python/uform/torch_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-14 00:51:14.000000 uform-2.1.0/python/uform/torch_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:51:21.698597 uform-2.1.0/python/uform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27269 2024-04-14 00:51:21.000000 uform-2.1.0/python/uform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-14 00:51:21.000000 uform-2.1.0/python/uform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 00:51:21.000000 uform-2.1.0/python/uform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-14 00:51:21.000000 uform-2.1.0/python/uform.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-14 00:51:21.000000 uform-2.1.0/python/uform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 00:51:21.000000 uform-2.1.0/python/uform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 00:51:21.702597 uform-2.1.0/setup.cfg
```

### Comparing `uform-2.0.2/LICENSE` & `uform-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uform-2.0.2/PKG-INFO` & `uform-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uform
-Version: 2.0.2
+Version: 2.1.0
 Summary: Pocket-Sized Multimodal AI for Content Understanding and Generation
 Author-email: Ash Vardanian <ash.vardanian@unum.cloud>, Mikhail Kim <mike.kim@unum.cloud>, Vladimir Orshulevich <vladimir.orshulevich@unum.cloud>
 Maintainer-email: Unum Cloud <info@unum.cloud>
 Project-URL: Homepage, https://github.com/unum-cloud/uform
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: Chinese (Simplified)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: uform Version: 2.0.2 Summary: Pocket-Sized
+Metadata-Version: 2.1 Name: uform Version: 2.1.0 Summary: Pocket-Sized
 Multimodal AI for Content Understanding and Generation Author-email: Ash
 Vardanian
 unum.cloud>, Mikhail Kim
 unum.cloud>, Vladimir Orshulevich
 unum.cloud> Maintainer-email: Unum Cloud
 unum.cloud> Project-URL: Homepage, https://github.com/unum-cloud/uform
 Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
```

### Comparing `uform-2.0.2/README.md` & `uform-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `uform-2.0.2/pyproject.toml` & `uform-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 description = "Pocket-Sized Multimodal AI for Content Understanding and Generation"
 maintainers = [
     {email = "info@unum.cloud", name = "Unum Cloud"},
 ]
 name = "uform"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "2.0.2"
+version = "2.1.0"
 
 [project.scripts]
 uform-chat = "uform.chat:main"
 
 [project.optional-dependencies]
 torch = ["torch>=1.13.1", "torchvision", "transformers>=4.36.2"]
 onnx = ["onnx>=1.15.0", "onnxruntime>=1.17.1", "numpy"]
```

### Comparing `uform-2.0.2/python/uform/__init__.py` & `uform-2.1.0/python/uform/__init__.py`

 * *Files identical despite different names*

### Comparing `uform-2.0.2/python/uform/chat.py` & `uform-2.1.0/python/uform/chat.py`

 * *Files identical despite different names*

### Comparing `uform-2.0.2/python/uform/gen_model.py` & `uform-2.1.0/python/uform/gen_model.py`

 * *Files identical despite different names*

### Comparing `uform-2.0.2/python/uform/numpy_preprocessor.py` & `uform-2.1.0/python/uform/numpy_preprocessor.py`

 * *Files 17% similar despite different names*

```diff
@@ -85,10 +85,13 @@
 
         left = (width - self._image_size) / 2
         top = (height - self._image_size) / 2
         right = (width + self._image_size) / 2
         bottom = (height + self._image_size) / 2
 
         image = image.convert("RGB").crop((left, top, right, bottom))
+        # At this point `image` is a PIL Image with RGB channels.
+        # If you convert it to `np.ndarray` it will have shape (H, W, C) where C is the number of channels.
         image = (np.array(image).astype(np.float32) / 255.0 - self.image_mean) / self.image_std
 
+        # To make it compatible with PyTorch, we need to transpose the image to (C, H, W).
         return np.transpose(image, (2, 0, 1))
```

### Comparing `uform-2.0.2/python/uform/onnx_models.py` & `uform-2.1.0/python/uform/onnx_models.py`

 * *Files identical despite different names*

### Comparing `uform-2.0.2/python/uform/preprocessing.py` & `uform-2.1.0/python/uform/preprocessing.py`

 * *Files identical despite different names*

### Comparing `uform-2.0.2/python/uform/torch_models.py` & `uform-2.1.0/python/uform/torch_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -203,14 +203,15 @@
         self.embedding_projection = nn.Linear(self.dim, self.embedding_dim, bias=False)
         self.matching_head = nn.Linear(self.dim, 1 if self.head_one_neuron else 2)
 
         if self.context_dim != self.dim:
             self.context_projection = nn.Linear(self.context_dim, self.dim, bias=False)
         else:
             self.context_projection = nn.Identity()
+        self.return_features = False
 
     def forward_features(self, x: Tensor, attn_mask: Tensor) -> Tensor:
         x = self.embed_text(x)
         attn_mask = self.get_attention_mask(attn_mask, x.dtype)
 
         for block in self.blocks:
             if not block.cross_attention:
@@ -263,18 +264,35 @@
         return self.position_ids[:, : x.shape[1]]
 
     def embed_text(self, x: Tensor) -> Tensor:
         positional_embedding = self.position_embeddings(self.get_position_ids(x))
         x = self.word_embeddings(x) + positional_embedding
         return self.dropout(self.layer_norm(x))
 
-    def forward(self, x: dict) -> Tensor:
-        features = self.forward_features(x["input_ids"], x["attention_mask"])
-        embeddings = self.forward_embedding(features, x["attention_mask"])
-        return features, embeddings
+    def forward(
+        self,
+        x: Union[Tensor, dict],
+        attention_mask: Optional[Tensor] = None,
+        return_features: Optional[bool] = None,
+    ) -> Tensor:
+        if isinstance(x, dict):
+            assert attention_mask is None, "If `x` is a dictionary, then `attention_mask` should be None"
+            attention_mask = x["attention_mask"]
+            x = x["input_ids"]
+        elif attention_mask is None:
+            # If no attention mask is provided - create one with all ones
+            attention_mask = torch.ones_like(x)
+
+        features = self.forward_features(x, attention_mask)
+        embeddings = self.forward_embedding(features, attention_mask)
+
+        return_features = return_features if return_features is not None else self.return_features
+        if return_features:
+            return features, embeddings
+        return embeddings
 
 
 @dataclass(eq=False)
 class VisualEncoder(nn.Module):
     dim: int
     patch_size: int
     image_size: int
@@ -297,14 +315,15 @@
 
         self.blocks = nn.Sequential(
             *[VisualEncoderBlock(self.dim, self.num_heads) for _ in range(self.num_layers)],
         )
 
         self.norm = nn.LayerNorm(self.dim, eps=1e-6)
         self.embedding_projection = nn.Linear(self.dim, self.embedding_dim, bias=False)
+        self.return_features = False
 
     def forward_features(self, x: Tensor) -> Tensor:
         x = self.patch_embed(x).flatten(start_dim=2).transpose(2, 1)
         x = x + self.pos_embed
 
         special_tokens = [self.cls_token.expand(x.shape[0], -1, -1)]
 
@@ -321,18 +340,21 @@
         if self.pooling == "cls":
             x = x[:, 0]
         else:
             x = x.mean(dim=1)
 
         return self.embedding_projection(x)
 
-    def forward(self, x: Tensor) -> Tensor:
+    def forward(self, x: Tensor, return_features: Optional[bool] = None) -> Tensor:
         features = self.forward_features(x)
         embeddings = self.forward_embedding(features)
-        return features, embeddings
+        return_features = return_features if return_features is not None else self.return_features
+        if return_features:
+            return features, embeddings
+        return embeddings
 
 
 class VLM(nn.Module):
     """
     Vision-Language Model for Multimodal embeddings.
     """
 
@@ -426,15 +448,15 @@
             )
 
         embeddings = self.text_encoder.forward_multimodal(
             text_features,
             attention_mask if attention_mask is not None else text["attention_mask"],
             image_features,
         )
-        
+
         if return_scores:
             return self.get_matching_scores(embeddings), embeddings
 
         return embeddings
 
     def get_matching_scores(self, embeddings: Tensor) -> Tensor:
         """Computes the probability that there is a match between images and texts based on their multimodal embeddings
```

### Comparing `uform-2.0.2/python/uform/torch_preprocessor.py` & `uform-2.1.0/python/uform/torch_preprocessor.py`

 * *Files identical despite different names*

### Comparing `uform-2.0.2/python/uform.egg-info/PKG-INFO` & `uform-2.1.0/python/uform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uform
-Version: 2.0.2
+Version: 2.1.0
 Summary: Pocket-Sized Multimodal AI for Content Understanding and Generation
 Author-email: Ash Vardanian <ash.vardanian@unum.cloud>, Mikhail Kim <mike.kim@unum.cloud>, Vladimir Orshulevich <vladimir.orshulevich@unum.cloud>
 Maintainer-email: Unum Cloud <info@unum.cloud>
 Project-URL: Homepage, https://github.com/unum-cloud/uform
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: Chinese (Simplified)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: uform Version: 2.0.2 Summary: Pocket-Sized
+Metadata-Version: 2.1 Name: uform Version: 2.1.0 Summary: Pocket-Sized
 Multimodal AI for Content Understanding and Generation Author-email: Ash
 Vardanian
 unum.cloud>, Mikhail Kim
 unum.cloud>, Vladimir Orshulevich
 unum.cloud> Maintainer-email: Unum Cloud
 unum.cloud> Project-URL: Homepage, https://github.com/unum-cloud/uform
 Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
```


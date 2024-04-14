# Comparing `tmp/substrate-120240405.0.3.tar.gz` & `tmp/substrate-120240411.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrate-120240405.0.3.tar", max compression
+gzip compressed data, was "substrate-120240411.0.4.tar", max compression
```

## Comparing `substrate-120240405.0.3.tar` & `substrate-120240411.0.4.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-120240405.0.3/LICENSE
--rw-r--r--   0        0        0       45 2024-03-19 21:55:57.200047 substrate-120240405.0.3/README.md
--rw-r--r--   0        0        0     2023 2024-04-05 17:53:46.736693 substrate-120240405.0.3/pyproject.toml
--rw-r--r--   0        0        0       17 2024-04-05 15:54:24.000000 substrate-120240405.0.3/substrate/GEN_VERSION
--rw-r--r--   0        0        0     1982 2024-04-05 15:55:06.000000 substrate-120240405.0.3/substrate/__init__.py
--rw-r--r--   0        0        0     5645 2024-04-05 17:52:12.432835 substrate-120240405.0.3/substrate/_client.py
--rw-r--r--   0        0        0       30 2024-03-13 14:46:31.829473 substrate-120240405.0.3/substrate/_version.py
--rw-r--r--   0        0        0        1 2024-04-05 17:45:52.679181 substrate-120240405.0.3/substrate/core/__init__.py
--rw-r--r--   0        0        0       27 2024-04-05 17:45:52.679078 substrate-120240405.0.3/substrate/core/_version.py
--rw-r--r--   0        0        0     2200 2024-04-05 17:45:52.679407 substrate-120240405.0.3/substrate/core/base_future.py
--rw-r--r--   0        0        0        0 2024-04-05 17:45:52.679662 substrate-120240405.0.3/substrate/core/client/__init__.py
--rw-r--r--   0        0        0     1750 2024-04-05 17:45:52.679764 substrate-120240405.0.3/substrate/core/client/find_futures_client.py
--rw-r--r--   0        0        0     2620 2024-04-05 17:45:52.679873 substrate-120240405.0.3/substrate/core/client/future.py
--rw-r--r--   0        0        0     1212 2024-04-05 17:45:52.679592 substrate-120240405.0.3/substrate/core/client/graph.py
--rw-r--r--   0        0        0     1149 2024-04-05 17:45:52.679293 substrate-120240405.0.3/substrate/core/coregraph.py
--rw-r--r--   0        0        0     1960 2024-04-05 17:45:52.678464 substrate-120240405.0.3/substrate/core/corenode.py
--rw-r--r--   0        0        0      894 2024-04-05 17:45:52.678318 substrate-120240405.0.3/substrate/core/id_generator.py
--rw-r--r--   0        0        0    36616 2024-04-05 17:45:52.678693 substrate-120240405.0.3/substrate/core/models.py
--rw-r--r--   0        0        0     1405 2024-04-05 17:45:52.678152 substrate-120240405.0.3/substrate/core/sb.py
--rw-r--r--   0        0        0    31518 2024-04-05 15:54:13.000000 substrate-120240405.0.3/substrate/dataclass_models.py
--rw-r--r--   0        0        0    41860 2024-04-05 15:54:13.000000 substrate-120240405.0.3/substrate/future_dataclass_models.py
--rw-r--r--   0        0        0    57918 2024-04-05 15:55:06.000000 substrate-120240405.0.3/substrate/nodes.py
--rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-120240405.0.3/substrate/py.typed
--rw-r--r--   0        0        0     1647 2024-04-05 17:52:32.972614 substrate-120240405.0.3/substrate/substrate.py
--rw-r--r--   0        0        0    34044 2024-04-05 15:54:13.000000 substrate-120240405.0.3/substrate/typeddict_models.py
--rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 substrate-120240405.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-120240411.0.4/LICENSE
+-rw-r--r--   0        0        0       45 2024-03-19 21:55:57.200047 substrate-120240411.0.4/README.md
+-rw-r--r--   0        0        0     2023 2024-04-14 21:13:22.652063 substrate-120240411.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 19:17:25.000000 substrate-120240411.0.4/substrate/.keep
+-rw-r--r--   0        0        0       17 2024-04-14 20:21:27.000000 substrate-120240411.0.4/substrate/GEN_VERSION
+-rw-r--r--   0        0        0     2048 2024-04-14 20:21:28.000000 substrate-120240411.0.4/substrate/__init__.py
+-rw-r--r--   0        0        0     5645 2024-04-05 17:52:12.432835 substrate-120240411.0.4/substrate/_client.py
+-rw-r--r--   0        0        0       30 2024-03-13 14:46:31.829473 substrate-120240411.0.4/substrate/_version.py
+-rw-r--r--   0        0        0        1 2024-04-14 21:12:46.459958 substrate-120240411.0.4/substrate/core/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-14 21:12:46.459837 substrate-120240411.0.4/substrate/core/_version.py
+-rw-r--r--   0        0        0     1535 2024-04-14 21:12:46.460219 substrate-120240411.0.4/substrate/core/base_future.py
+-rw-r--r--   0        0        0        0 2024-04-14 21:12:46.460602 substrate-120240411.0.4/substrate/core/client/__init__.py
+-rw-r--r--   0        0        0     1750 2024-04-14 21:12:46.460706 substrate-120240411.0.4/substrate/core/client/find_futures_client.py
+-rw-r--r--   0        0        0     2697 2024-04-14 21:12:46.460832 substrate-120240411.0.4/substrate/core/client/future.py
+-rw-r--r--   0        0        0     1212 2024-04-14 21:12:46.460537 substrate-120240411.0.4/substrate/core/client/graph.py
+-rw-r--r--   0        0        0     1149 2024-04-14 21:12:46.460085 substrate-120240411.0.4/substrate/core/coregraph.py
+-rw-r--r--   0        0        0     1989 2024-04-14 21:12:46.459382 substrate-120240411.0.4/substrate/core/corenode.py
+-rw-r--r--   0        0        0     1227 2024-04-14 21:12:46.460350 substrate-120240411.0.4/substrate/core/future_directive.py
+-rw-r--r--   0        0        0      894 2024-04-14 21:12:46.459221 substrate-120240411.0.4/substrate/core/id_generator.py
+-rw-r--r--   0        0        0    37511 2024-04-14 21:12:46.459592 substrate-120240411.0.4/substrate/core/models.py
+-rw-r--r--   0        0        0     2332 2024-04-14 21:12:46.459081 substrate-120240411.0.4/substrate/core/sb.py
+-rw-r--r--   0        0        0    31945 2024-04-14 20:21:25.000000 substrate-120240411.0.4/substrate/dataclass_models.py
+-rw-r--r--   0        0        0    42701 2024-04-14 20:21:27.000000 substrate-120240411.0.4/substrate/future_dataclass_models.py
+-rw-r--r--   0        0        0    59500 2024-04-14 20:21:28.000000 substrate-120240411.0.4/substrate/nodes.py
+-rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-120240411.0.4/substrate/py.typed
+-rw-r--r--   0        0        0     1647 2024-04-05 21:20:49.456063 substrate-120240411.0.4/substrate/substrate.py
+-rw-r--r--   0        0        0    34991 2024-04-14 20:21:24.000000 substrate-120240411.0.4/substrate/typeddict_models.py
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 substrate-120240411.0.4/PKG-INFO
```

### Comparing `substrate-120240405.0.3/LICENSE` & `substrate-120240411.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `substrate-120240405.0.3/pyproject.toml` & `substrate-120240411.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "substrate"
-version = "120240405.0.3"
+version = "120240411.0.4"
 description = "Substrate Python SDK"
 readme = "README.md"
 authors = [ "vprtwn <ben@substrate.run>", "liamgriffiths <liam@substrate.run>",]
 [[tool.poetry.packages]]
 include = "substrate"
 
 [tool.pyright]
```

### Comparing `substrate-120240405.0.3/substrate/__init__.py` & `substrate-120240411.0.4/substrate/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 ꩜ Substrate Python SDK
 
-20240405.20240405
+20240411.20240414
 """
 
 from .nodes import (
     CLIP,
     XTTSV2,
     JinaV2,
     BigLaMa,
@@ -39,14 +39,15 @@
     StableDiffusionXL,
     GenerateTextVision,
     MultiGenerateImage,
     GenerativeEditImage,
     MultiGenerativeEditImage,
     StableDiffusionXLInpaint,
     StableDiffusionXLIPAdapter,
+    StableDiffusionXLLightning,
     StableDiffusionXLControlNet,
 )
 from .core.sb import sb
 from ._version import __version__
 from .substrate import Substrate, AsyncSubstrate, SubstrateResponse
 
 __all__ = [
@@ -63,28 +64,29 @@
     "Mistral7BInstruct",
     "Firellava13B",
     "GenerateImage",
     "MultiGenerateImage",
     "GenerativeEditImage",
     "MultiGenerativeEditImage",
     "StableDiffusionXL",
+    "StableDiffusionXLLightning",
     "StableDiffusionXLInpaint",
-    "StableDiffusionXLIPAdapter",
     "StableDiffusionXLControlNet",
+    "StableDiffusionXLIPAdapter",
+    "TranscribeMedia",
+    "GenerateSpeech",
+    "XTTSV2",
+    "RemoveBackground",
     "FillMask",
-    "BigLaMa",
     "UpscaleImage",
-    "RealESRGAN",
-    "RemoveBackground",
-    "DISISNet",
     "SegmentUnderPoint",
+    "DISISNet",
+    "BigLaMa",
+    "RealESRGAN",
     "SegmentAnything",
-    "TranscribeMedia",
-    "GenerateSpeech",
-    "XTTSV2",
     "EmbedText",
     "MultiEmbedText",
     "EmbedImage",
     "MultiEmbedImage",
     "JinaV2",
     "CLIP",
     "CreateVectorStore",
```

### Comparing `substrate-120240405.0.3/substrate/_client.py` & `substrate-120240411.0.4/substrate/_client.py`

 * *Files identical despite different names*

### Comparing `substrate-120240405.0.3/substrate/core/client/find_futures_client.py` & `substrate-120240411.0.4/substrate/core/client/find_futures_client.py`

 * *Files identical despite different names*

### Comparing `substrate-120240405.0.3/substrate/core/client/future.py` & `substrate-120240411.0.4/substrate/core/client/future.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 """
 CORE ꩜ SUBSTRATE
 """
-from typing import (
-    Union,
-    Optional,
-)
+from typing import Union, TypeVar, Optional
 
 import networkx as nx
 
-from ..base_future import (
-    Directive,
-    TraceType,
-    BaseFuture,
-    TraceDirective,
-    TraceOperation,
-)
+from ..base_future import BaseFuture
+from ..future_directive import TraceType, TraceDirective, TraceOperation
 
+T = TypeVar("T", bound="BaseDirective")
 
-class Future(BaseFuture):
+
+class Future(BaseFuture[T]):
     def __init__(
         self,
-        directive: Directive,
+        directive: T,
         FG: Optional["nx.DiGraph[Future]"] = None,
         **kwargs,
     ):
         super().__init__(directive, **kwargs)
+        self.directive = directive
         self.FutureG = FG if FG is not None else nx.DiGraph()
 
 
-class TracedFuture(Future):
+class TracedFuture(Future[TraceDirective]):
     """
     You can think of this as a logical handle to a future result. This means that you can access attributes or items
     from it as if it were a resolved instance. If you use a traced future as an argument to other nodes, it will
     implicitly create an execution dependency graph. This enables you to define an inter-related graph of computations
     without worrying about the actual execution order.
 
     TracedFutures can create one or many future computation paths. To originate one, use Node.future. The same node
```

### Comparing `substrate-120240405.0.3/substrate/core/client/graph.py` & `substrate-120240411.0.4/substrate/core/client/graph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240405.0.3/substrate/core/coregraph.py` & `substrate-120240411.0.4/substrate/core/coregraph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240405.0.3/substrate/core/corenode.py` & `substrate-120240411.0.4/substrate/core/corenode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 CORE ꩜ SUBSTRATE
 """
 from typing import List, Optional
 
 import networkx as nx
 
-from .base_future import BaseFuture, TraceDirective
+from .base_future import BaseFuture
 from .id_generator import IDGenerator
 from .client.future import TracedFuture
+from .future_directive import TraceDirective
 from .client.find_futures_client import find_futures_client
 
 
 class CoreNode:
     def __init__(self, **attr):
         self.node = self.__class__.__name__
         self.args = attr
```

### Comparing `substrate-120240405.0.3/substrate/core/id_generator.py` & `substrate-120240411.0.4/substrate/core/id_generator.py`

 * *Files identical despite different names*

### Comparing `substrate-120240405.0.3/substrate/core/models.py` & `substrate-120240411.0.4/substrate/core/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,33 +21,37 @@
     """
     The type of error returned.
     """
     message: str
     """
     A message providing more details about the error.
     """
+    request_id: Optional[str] = None
+    """
+    A unique identifier for the request.
+    """
 
 
 class GenerateTextIn(BaseModel):
     class Config:
         extra = Extra.allow
 
     prompt: str
     """
     Input prompt.
     """
-    temperature: Annotated[Optional[int], Field(ge=1, le=10)] = 4
+    temperature: Annotated[float, Field(ge=0.0, le=1.0)] = 0.4
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
-    node: Optional[Literal["Mistral7BInstruct"]] = "Mistral7BInstruct"
+    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
 class GenerateTextOut(BaseModel):
     class Config:
@@ -67,23 +71,23 @@
     """
     Input prompt.
     """
     json_schema: Dict[str, Any]
     """
     JSON schema to guide `json_object` response.
     """
-    temperature: Annotated[Optional[int], Field(ge=1, le=10)] = 4
+    temperature: Annotated[float, Field(ge=0.0, le=1.0)] = 0.4
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
-    node: Optional[Literal["Mistral7BInstruct"]] = "Mistral7BInstruct"
+    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
 class GenerateJSONOut(BaseModel):
     class Config:
@@ -99,93 +103,99 @@
     class Config:
         extra = Extra.allow
 
     prompt: str
     """
     Input prompt.
     """
-    num_choices: int
+    num_choices: Annotated[int, Field(ge=1, le=8)]
     """
     Number of choices to generate.
     """
-    temperature: Annotated[Optional[int], Field(ge=1, le=10)] = 4
+    temperature: Annotated[float, Field(ge=0.0, le=1.0)] = 0.4
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
-    node: Optional[Literal["Mistral7BInstruct"]] = "Mistral7BInstruct"
+    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
 class MultiGenerateTextOut(BaseModel):
     class Config:
         extra = Extra.allow
 
     choices: List[GenerateTextOut]
+    """
+    Response choices.
+    """
 
 
 class MultiGenerateJSONIn(BaseModel):
     class Config:
         extra = Extra.allow
 
     prompt: str
     """
     Input prompt.
     """
     json_schema: Dict[str, Any]
     """
     JSON schema to guide `json_object` response.
     """
-    num_choices: int
+    num_choices: Annotated[int, Field(ge=1, le=8)]
     """
     Number of choices to generate.
     """
-    temperature: Annotated[Optional[int], Field(ge=1, le=10)] = 4
+    temperature: Annotated[float, Field(ge=0.0, le=1.0)] = 0.4
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
-    node: Optional[Literal["Mistral7BInstruct"]] = "Mistral7BInstruct"
+    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
 class MultiGenerateJSONOut(BaseModel):
     class Config:
         extra = Extra.allow
 
     choices: List[GenerateJSONOut]
+    """
+    Response choices.
+    """
 
 
 class Mistral7BInstructIn(BaseModel):
     class Config:
         extra = Extra.allow
 
     prompt: str
     """
     Input prompt.
     """
-    num_choices: int
+    num_choices: Annotated[int, Field(ge=1, le=8)]
     """
     Number of choices to generate.
     """
     json_schema: Optional[Dict[str, Any]] = None
     """
     JSON schema to guide response.
     """
-    temperature: Annotated[Optional[float], Field(ge=0.0, le=2.0)] = None
+    temperature: Annotated[Optional[float], Field(ge=0.0, le=1.0)] = None
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
@@ -206,37 +216,36 @@
 
 
 class Mistral7BInstructOut(BaseModel):
     class Config:
         extra = Extra.allow
 
     choices: List[Mistral7BInstructChoice]
+    """
+    Response choices.
+    """
 
 
 class GenerateTextVisionIn(BaseModel):
     class Config:
         extra = Extra.allow
 
     prompt: str
     """
     Text prompt.
     """
     image_uris: List[str]
     """
     Image prompts.
     """
-    temperature: Annotated[Optional[int], Field(ge=1, le=10)] = 4
-    """
-    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
-    """
-    max_tokens: Optional[int] = 800
+    max_tokens: int = 800
     """
     Maximum number of tokens to generate.
     """
-    node: Optional[Literal["Firellava13B"]] = "Firellava13B"
+    node: Literal["Firellava13B"] = "Firellava13B"
     """
     Selected node.
     """
 
 
 class GenerateTextVisionOut(BaseModel):
     class Config:
@@ -256,19 +265,15 @@
     """
     Text prompt.
     """
     image_uris: List[str]
     """
     Image prompts.
     """
-    temperature: Annotated[Optional[float], Field(ge=0.0)] = None
-    """
-    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
-    """
-    max_tokens: Optional[int] = 800
+    max_tokens: int = 800
     """
     Maximum number of tokens to generate.
     """
 
 
 class Firellava13BOut(BaseModel):
     class Config:
@@ -288,15 +293,15 @@
     """
     Text prompt.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["StableDiffusionXL"]] = "StableDiffusionXL"
+    node: Literal["StableDiffusionXL"] = "StableDiffusionXL"
     """
     Selected node.
     """
 
 
 class GenerateImageOut(BaseModel):
     class Config:
@@ -312,72 +317,75 @@
     class Config:
         extra = Extra.allow
 
     prompt: str
     """
     Text prompt.
     """
-    num_images: int
+    num_images: Annotated[int, Field(ge=1, le=8)]
     """
     Number of images to generate.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["StableDiffusionXL"]] = "StableDiffusionXL"
+    node: Literal["StableDiffusionXL"] = "StableDiffusionXL"
     """
     Selected node.
     """
 
 
 class MultiGenerateImageOut(BaseModel):
     class Config:
         extra = Extra.allow
 
     outputs: List[GenerateImageOut]
+    """
+    Generated images.
+    """
 
 
 class StableDiffusionXLIn(BaseModel):
     class Config:
         extra = Extra.allow
 
     prompt: str
     """
     Text prompt.
     """
     negative_prompt: Optional[str] = None
     """
     Negative input prompt.
     """
-    steps: Optional[int] = None
+    steps: Annotated[int, Field(ge=0, le=150)] = 30
     """
     Number of diffusion steps.
     """
-    num_images: Optional[int] = None
+    num_images: Annotated[int, Field(ge=1, le=8)]
     """
     Number of images to generate.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    height: Optional[int] = None
+    height: Annotated[int, Field(ge=640, le=1536)] = 1024
     """
     Height of output image, in pixels.
     """
-    width: Optional[int] = None
+    width: Annotated[int, Field(ge=640, le=1536)] = 1024
     """
     Width of output image, in pixels.
     """
-    seeds: Optional[int] = None
+    seeds: Optional[List[int]] = None
     """
     Seeds for deterministic generation. Default is a random seed.
     """
-    guidance_scale: Annotated[Optional[float], Field(ge=0.0)] = 5
+    guidance_scale: Annotated[float, Field(ge=0.0, le=30.0)] = 7
     """
     Higher values adhere to the text prompt more strongly, typically at the expense of image quality.
     """
 
 
 class StableDiffusionImage(BaseModel):
     class Config:
@@ -394,29 +402,76 @@
 
 
 class StableDiffusionXLOut(BaseModel):
     class Config:
         extra = Extra.allow
 
     outputs: List[StableDiffusionImage]
+    """
+    Generated images.
+    """
+
+
+class StableDiffusionXLLightningIn(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    prompt: str
+    """
+    Text prompt.
+    """
+    negative_prompt: Optional[str] = None
+    """
+    Negative input prompt.
+    """
+    num_images: Annotated[int, Field(ge=1, le=8)] = 1
+    """
+    Number of images to generate.
+    """
+    store: Optional[str] = None
+    """
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    """
+    height: Optional[int] = None
+    """
+    Height of output image, in pixels.
+    """
+    width: Optional[int] = None
+    """
+    Width of output image, in pixels.
+    """
+    seeds: Optional[List[int]] = None
+    """
+    Seeds for deterministic generation. Default is a random seed.
+    """
+
+
+class StableDiffusionXLLightningOut(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    outputs: List[StableDiffusionImage]
+    """
+    Generated images.
+    """
 
 
 class StableDiffusionXLIPAdapterIn(BaseModel):
     class Config:
         extra = Extra.allow
 
     prompt: str
     """
     Text prompt.
     """
     image_prompt_uri: Optional[str] = None
     """
     Image prompt.
     """
-    num_images: int
+    num_images: Annotated[int, Field(ge=1, le=8)]
     """
     Number of images to generate.
     """
     ip_adapter_scale: Annotated[Optional[float], Field(ge=0.0)] = None
     """
     Controls the influence of the image prompt on the generated output.
     """
@@ -443,14 +498,17 @@
 
 
 class StableDiffusionXLIPAdapterOut(BaseModel):
     class Config:
         extra = Extra.allow
 
     outputs: List[StableDiffusionImage]
+    """
+    Generated images.
+    """
 
 
 class StableDiffusionXLControlNetIn(BaseModel):
     class Config:
         extra = Extra.allow
 
     image_uri: str
@@ -461,19 +519,19 @@
     """
     Strategy to control generation using the input image.
     """
     prompt: str
     """
     Text prompt.
     """
-    num_images: int
+    num_images: Annotated[int, Field(ge=1, le=8)]
     """
     Number of images to generate.
     """
-    output_resolution: Optional[int] = 1024
+    output_resolution: int = 1024
     """
     Resolution of the output image, in pixels.
     """
     negative_prompt: Optional[str] = None
     """
     Negative input prompt.
     """
@@ -492,14 +550,17 @@
 
 
 class StableDiffusionXLControlNetOut(BaseModel):
     class Config:
         extra = Extra.allow
 
     outputs: List[StableDiffusionImage]
+    """
+    Generated images.
+    """
 
 
 class GenerativeEditImageIn(BaseModel):
     class Config:
         extra = Extra.allow
 
     image_uri: str
@@ -514,15 +575,15 @@
     """
     Mask image that controls which pixels are inpainted. If unset, the entire image is edited (image-to-image).
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["StableDiffusionXLInpaint"]] = "StableDiffusionXLInpaint"
+    node: Literal["StableDiffusionXLInpaint"] = "StableDiffusionXLInpaint"
     """
     Selected node.
     """
 
 
 class GenerativeEditImageOut(BaseModel):
     class Config:
@@ -546,33 +607,36 @@
     """
     Text prompt.
     """
     mask_image_uri: Optional[str] = None
     """
     Mask image that controls which pixels are edited (inpainting). If unset, the entire image is edited (image-to-image).
     """
-    num_images: int
+    num_images: Annotated[int, Field(ge=1, le=8)]
     """
     Number of images to generate.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["StableDiffusionXLInpaint"]] = "StableDiffusionXLInpaint"
+    node: Literal["StableDiffusionXLInpaint"] = "StableDiffusionXLInpaint"
     """
     Selected node.
     """
 
 
 class MultiGenerativeEditImageOut(BaseModel):
     class Config:
         extra = Extra.allow
 
     outputs: List[GenerativeEditImageOut]
+    """
+    Generated images.
+    """
 
 
 class StableDiffusionXLInpaintIn(BaseModel):
     class Config:
         extra = Extra.allow
 
     image_uri: str
@@ -583,45 +647,48 @@
     """
     Text prompt.
     """
     mask_image_uri: Optional[str] = None
     """
     Mask image that controls which pixels are edited (inpainting). If unset, the entire image is edited (image-to-image).
     """
-    num_images: int
+    num_images: Annotated[int, Field(ge=1, le=8)]
     """
     Number of images to generate.
     """
-    output_resolution: Optional[int] = 1024
+    output_resolution: int = 1024
     """
     Resolution of the output image, in pixels.
     """
     negative_prompt: Optional[str] = None
     """
     Negative input prompt.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    strength: Annotated[Optional[float], Field(ge=0.0)] = 0.5
+    strength: Annotated[float, Field(ge=0.0, le=1.0)] = 1
     """
     Controls the strength of the generation process.
     """
     seeds: Optional[List[int]] = None
     """
     Random noise seeds. Default is random seeds for each generation.
     """
 
 
 class StableDiffusionXLInpaintOut(BaseModel):
     class Config:
         extra = Extra.allow
 
     outputs: List[StableDiffusionImage]
+    """
+    Generated images.
+    """
 
 
 class BoundingBox(BaseModel):
     class Config:
         extra = Extra.allow
 
     x1: float
@@ -668,15 +735,15 @@
     """
     Mask image that controls which pixels are inpainted.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["BigLaMa"]] = "BigLaMa"
+    node: Literal["BigLaMa"] = "BigLaMa"
     """
     Selected node.
     """
 
 
 class FillMaskOut(BaseModel):
     class Config:
@@ -720,27 +787,27 @@
     class Config:
         extra = Extra.allow
 
     image_uri: str
     """
     Input image.
     """
-    return_mask: Optional[bool] = None
+    return_mask: bool = False
     """
     Return a mask image instead of the original content.
     """
     background_color: Optional[str] = None
     """
     Hex value background color. Transparent if unset.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["DISISNet"]] = "DISISNet"
+    node: Literal["DISISNet"] = "DISISNet"
     """
     Selected node.
     """
 
 
 class RemoveBackgroundOut(BaseModel):
     class Config:
@@ -756,22 +823,14 @@
     class Config:
         extra = Extra.allow
 
     image_uri: str
     """
     Input image.
     """
-    return_mask: Optional[bool] = None
-    """
-    Return a mask image instead of the original content.
-    """
-    background_color: Optional[str] = None
-    """
-    Hex value background color. Transparent if unset.
-    """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 class DISISNetOut(BaseModel):
@@ -792,15 +851,15 @@
     """
     Input image.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["RealESRGAN"]] = "RealESRGAN"
+    node: Literal["RealESRGAN"] = "RealESRGAN"
     """
     Selected node.
     """
 
 
 class UpscaleImageOut(BaseModel):
     class Config:
@@ -816,18 +875,14 @@
     class Config:
         extra = Extra.allow
 
     image_uri: str
     """
     Input image.
     """
-    model: Optional[Literal["real-esrgan-x4"]] = "real-esrgan-x4"
-    """
-    Selected model.
-    """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 class RealESRGANOut(BaseModel):
@@ -852,15 +907,15 @@
     """
     Point prompt.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["SegmentAnything"]] = "SegmentAnything"
+    node: Literal["SegmentAnything"] = "SegmentAnything"
     """
     Selected node.
     """
 
 
 class SegmentUnderPointOut(BaseModel):
     class Config:
@@ -912,31 +967,31 @@
     """
     Input audio.
     """
     prompt: Optional[str] = None
     """
     Prompt to guide model on the content and context of input audio.
     """
-    language: Optional[str] = "en"
+    language: str = "en"
     """
     Language of input audio in [ISO-639-1](https://en.wikipedia.org/wiki/List_of_ISO_639_language_codes) format.
     """
-    segment: Optional[bool] = False
+    segment: bool = False
     """
     Segment the text into sentences with approximate timestamps.
     """
-    align: Optional[bool] = False
+    align: bool = False
     """
     Align transcription to produce more accurate sentence-level timestamps and word-level timestamps. An array of word segments will be included in each sentence segment.
     """
-    diarize: Optional[bool] = False
+    diarize: bool = False
     """
     Identify speakers for each segment. Speaker IDs will be included in each segment.
     """
-    suggest_chapters: Optional[bool] = False
+    suggest_chapters: bool = False
     """
     Suggest automatic chapter markers.
     """
 
 
 class TranscribedWord(BaseModel):
     class Config:
@@ -1026,15 +1081,15 @@
     """
     Input text.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the audio data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["XTTSV2"]] = "XTTSV2"
+    node: Literal["XTTSV2"] = "XTTSV2"
     """
     Selected node.
     """
 
 
 class GenerateSpeechOut(BaseModel):
     class Config:
@@ -1054,15 +1109,15 @@
     """
     Input text.
     """
     audio_uri: Optional[str] = None
     """
     Reference audio used to synthesize the speaker. If unset, a default speaker voice will be used.
     """
-    language: Optional[str] = "en"
+    language: str = "en"
     """
     Language of input text. Supported languages: `en, de, fr, es, it, pt, pl, zh, ar, cs, ru, nl, tr, hu, ko`.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the audio data will be returned as a base64-encoded string.
     """
@@ -1116,15 +1171,15 @@
     """
     Choose keys from `metadata` to embed with text.
     """
     doc_id: Optional[str] = None
     """
     Vector store document ID. Ignored if `store` is unset.
     """
-    node: Optional[Literal["JinaV2", "CLIP"]] = "JinaV2"
+    node: Literal["JinaV2", "CLIP"] = "JinaV2"
     """
     Selected node.
     """
 
 
 class EmbedTextOut(BaseModel):
     class Config:
@@ -1166,15 +1221,15 @@
     """
     [Vector store](/docs/vector-stores) identifier.
     """
     embedded_metadata_keys: Optional[List[str]] = None
     """
     Choose keys from `metadata` to embed with text.
     """
-    node: Optional[Literal["JinaV2", "CLIP"]] = "JinaV2"
+    node: Literal["JinaV2", "CLIP"] = "JinaV2"
     """
     Selected node.
     """
 
 
 class MultiEmbedTextOut(BaseModel):
     class Config:
@@ -1226,15 +1281,15 @@
     """
     [Vector store](/docs/vector-stores) identifier.
     """
     doc_id: Optional[str] = None
     """
     Vector store document ID. Ignored if `store` is unset.
     """
-    node: Optional[Literal["CLIP"]] = "CLIP"
+    node: Literal["CLIP"] = "CLIP"
     """
     Selected node.
     """
 
 
 class EmbedImageOut(BaseModel):
     class Config:
@@ -1290,15 +1345,15 @@
     """
     Items to embed.
     """
     store: Optional[str] = None
     """
     [Vector store](/docs/vector-stores) identifier.
     """
-    node: Optional[Literal["CLIP"]] = "CLIP"
+    node: Literal["CLIP"] = "CLIP"
     """
     Selected node.
     """
 
 
 class MultiEmbedImageOut(BaseModel):
     class Config:
@@ -1346,23 +1401,23 @@
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model
     """
-    m: Annotated[Optional[int], Field(ge=1, le=64)] = 16
+    m: Annotated[int, Field(ge=1, le=64)] = 16
     """
     The max number of connections per layer for the index.
     """
-    ef_construction: Annotated[Optional[int], Field(ge=1, le=128)] = 64
+    ef_construction: Annotated[int, Field(ge=1, le=128)] = 64
     """
     The size of the dynamic candidate list for constructing the index graph.
     """
-    metric: Optional[Literal["cosine", "l2", "inner"]] = "inner"
+    metric: Literal["cosine", "l2", "inner"] = "inner"
     """
     The distance metric to construct the index with.
     """
 
 
 class CreateVectorStoreOut(BaseModel):
     class Config:
@@ -1583,34 +1638,38 @@
     """
     Vector to use for the query.
     """
     query_strings: Optional[List[str]] = None
     """
     Texts to embed and use for the query.
     """
-    top_k: Annotated[Optional[int], Field(ge=1, le=1000)] = 10
+    top_k: Annotated[int, Field(ge=1, le=1000)] = 10
     """
     Number of results to return.
     """
-    ef_search: Annotated[Optional[int], Field(ge=1, le=1000)] = 40
+    ef_search: Annotated[int, Field(ge=1, le=1000)] = 40
     """
     The size of the dynamic candidate list for searching the index graph.
     """
-    include_values: Optional[bool] = False
+    include_values: bool = False
     """
     Include the values of the vectors in the response.
     """
-    include_metadata: Optional[bool] = False
+    include_metadata: bool = False
     """
     Include the metadata of the vectors in the response.
     """
     filters: Optional[Dict[str, Any]] = None
     """
     Filter metadata by key-value pairs.
     """
+    metric: Optional[Literal["cosine", "l2", "inner"]] = None
+    """
+    The distance metric used for the query. Defaults to the distance metric the vector store was created with.
+    """
 
 
 class VectorStoreQueryResult(BaseModel):
     class Config:
         extra = Extra.allow
 
     id: str
```

### Comparing `substrate-120240405.0.3/substrate/core/sb.py` & `substrate-120240411.0.4/substrate/core/sb.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 """
 CORE ꩜ SUBSTRATE
 """
-from typing import Union
+from typing import Any, Union
 
-from .base_future import Concatable, ConcatDirective
 from .client.future import Future
+from .future_directive import (
+    JQDirective,
+    JQTargetType,
+    ConcatDirective,
+    JQDirectiveTarget,
+    ConcatDirectiveItem,
+)
 
 StringConcatable = Union[str, None, Future]
+JQCompatible = Union[Future, JQTargetType]
 
 
 class sb:
     """
     Utilities for working with future references.
     """
 
@@ -26,21 +33,34 @@
         else:
             concat_args = []
             futures = []
             for arg in args:
                 is_future = isinstance(arg, Future)
                 if is_future:
                     futures.append(arg)
-                concat_args.append(
-                    Concatable(
-                        future_id=arg.id if is_future else None,
-                        # if arg is None and not a future, use ""
-                        val=arg or "" if not is_future else None,
-                    )
-                )
+                future_id = arg.id if is_future else None
+                # if arg is None and not a future, use ""
+                val = arg or "" if not is_future else None
+                concat_args.append(ConcatDirectiveItem(future_id=future_id, val=val))
 
-            directive = ConcatDirective(type="string-concat", items=concat_args)
-            os = Future(directive=directive)
+            directive = ConcatDirective(items=concat_args)
+            result = Future(directive=directive)
             # draw edges from the concat op to all of its child futures
             for f in futures:
-                os.FutureG.add_edge(f, os)
-            return os  # type: ignore
+                result.FutureG.add_edge(f, result)
+            return result  # type: ignore
+
+    @classmethod
+    def jq(cls, target: JQCompatible, query: str) -> Any:
+        """
+        Given a target and a query, returns a future reference to the result of the jq query.
+        :param target: any future-compatible object, this can be another future, or a real value
+        :param query: jq query string, e.g. ".foo.bar"
+        :return: a future reference to the result of the jq query applied to the target
+        """
+        future_id = target.id if isinstance(target, Future) else None
+        val = target if not isinstance(target, Future) else None
+        directive = JQDirective(target=JQDirectiveTarget(future_id=future_id, val=val), query=query)
+        result = Future(directive=directive)
+        if isinstance(target, Future):
+            result.FutureG.add_edge(target, result)
+        return result  # type: ignore
```

### Comparing `substrate-120240405.0.3/substrate/dataclass_models.py` & `substrate-120240411.0.4/substrate/dataclass_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,31 +18,35 @@
     """
     The type of error returned.
     """
     message: str
     """
     A message providing more details about the error.
     """
+    request_id: Optional[str] = None
+    """
+    A unique identifier for the request.
+    """
 
 
 @dataclass
 class GenerateTextIn:
     prompt: str
     """
     Input prompt.
     """
-    temperature: Optional[int] = 4
+    temperature: float = 0.4
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
-    node: Optional[Literal["Mistral7BInstruct"]] = "Mistral7BInstruct"
+    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
 @dataclass
 class GenerateTextOut:
@@ -58,23 +62,23 @@
     """
     Input prompt.
     """
     json_schema: Dict[str, Any]
     """
     JSON schema to guide `json_object` response.
     """
-    temperature: Optional[int] = 4
+    temperature: float = 0.4
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
-    node: Optional[Literal["Mistral7BInstruct"]] = "Mistral7BInstruct"
+    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
 @dataclass
 class GenerateJSONOut:
@@ -90,31 +94,34 @@
     """
     Input prompt.
     """
     num_choices: int
     """
     Number of choices to generate.
     """
-    temperature: Optional[int] = 4
+    temperature: float = 0.4
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
-    node: Optional[Literal["Mistral7BInstruct"]] = "Mistral7BInstruct"
+    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
 @dataclass
 class MultiGenerateTextOut:
     choices: List[GenerateTextOut]
+    """
+    Response choices.
+    """
 
 
 @dataclass
 class MultiGenerateJSONIn:
     prompt: str
     """
     Input prompt.
@@ -123,31 +130,34 @@
     """
     JSON schema to guide `json_object` response.
     """
     num_choices: int
     """
     Number of choices to generate.
     """
-    temperature: Optional[int] = 4
+    temperature: float = 0.4
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
-    node: Optional[Literal["Mistral7BInstruct"]] = "Mistral7BInstruct"
+    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
 @dataclass
 class MultiGenerateJSONOut:
     choices: List[GenerateJSONOut]
+    """
+    Response choices.
+    """
 
 
 @dataclass
 class Mistral7BInstructIn:
     prompt: str
     """
     Input prompt.
@@ -181,35 +191,34 @@
     JSON response, if `json_schema` was provided.
     """
 
 
 @dataclass
 class Mistral7BInstructOut:
     choices: List[Mistral7BInstructChoice]
+    """
+    Response choices.
+    """
 
 
 @dataclass
 class GenerateTextVisionIn:
     prompt: str
     """
     Text prompt.
     """
     image_uris: List[str]
     """
     Image prompts.
     """
-    temperature: Optional[int] = 4
-    """
-    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
-    """
-    max_tokens: Optional[int] = 800
+    max_tokens: int = 800
     """
     Maximum number of tokens to generate.
     """
-    node: Optional[Literal["Firellava13B"]] = "Firellava13B"
+    node: Literal["Firellava13B"] = "Firellava13B"
     """
     Selected node.
     """
 
 
 @dataclass
 class GenerateTextVisionOut:
@@ -225,19 +234,15 @@
     """
     Text prompt.
     """
     image_uris: List[str]
     """
     Image prompts.
     """
-    temperature: Optional[float] = None
-    """
-    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
-    """
-    max_tokens: Optional[int] = 800
+    max_tokens: int = 800
     """
     Maximum number of tokens to generate.
     """
 
 
 @dataclass
 class Firellava13BOut:
@@ -253,15 +258,15 @@
     """
     Text prompt.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["StableDiffusionXL"]] = "StableDiffusionXL"
+    node: Literal["StableDiffusionXL"] = "StableDiffusionXL"
     """
     Selected node.
     """
 
 
 @dataclass
 class GenerateImageOut:
@@ -281,60 +286,63 @@
     """
     Number of images to generate.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["StableDiffusionXL"]] = "StableDiffusionXL"
+    node: Literal["StableDiffusionXL"] = "StableDiffusionXL"
     """
     Selected node.
     """
 
 
 @dataclass
 class MultiGenerateImageOut:
     outputs: List[GenerateImageOut]
+    """
+    Generated images.
+    """
 
 
 @dataclass
 class StableDiffusionXLIn:
     prompt: str
     """
     Text prompt.
     """
+    num_images: int
+    """
+    Number of images to generate.
+    """
     negative_prompt: Optional[str] = None
     """
     Negative input prompt.
     """
-    steps: Optional[int] = None
+    steps: int = 30
     """
     Number of diffusion steps.
     """
-    num_images: Optional[int] = None
-    """
-    Number of images to generate.
-    """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    height: Optional[int] = None
+    height: int = 1024
     """
     Height of output image, in pixels.
     """
-    width: Optional[int] = None
+    width: int = 1024
     """
     Width of output image, in pixels.
     """
-    seeds: Optional[int] = None
+    seeds: Optional[List[int]] = None
     """
     Seeds for deterministic generation. Default is a random seed.
     """
-    guidance_scale: Optional[float] = 5
+    guidance_scale: float = 7
     """
     Higher values adhere to the text prompt more strongly, typically at the expense of image quality.
     """
 
 
 @dataclass
 class StableDiffusionImage:
@@ -347,14 +355,57 @@
     The random noise seed used for generation.
     """
 
 
 @dataclass
 class StableDiffusionXLOut:
     outputs: List[StableDiffusionImage]
+    """
+    Generated images.
+    """
+
+
+@dataclass
+class StableDiffusionXLLightningIn:
+    prompt: str
+    """
+    Text prompt.
+    """
+    negative_prompt: Optional[str] = None
+    """
+    Negative input prompt.
+    """
+    num_images: int = 1
+    """
+    Number of images to generate.
+    """
+    store: Optional[str] = None
+    """
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    """
+    height: Optional[int] = None
+    """
+    Height of output image, in pixels.
+    """
+    width: Optional[int] = None
+    """
+    Width of output image, in pixels.
+    """
+    seeds: Optional[List[int]] = None
+    """
+    Seeds for deterministic generation. Default is a random seed.
+    """
+
+
+@dataclass
+class StableDiffusionXLLightningOut:
+    outputs: List[StableDiffusionImage]
+    """
+    Generated images.
+    """
 
 
 @dataclass
 class StableDiffusionXLIPAdapterIn:
     prompt: str
     """
     Text prompt.
@@ -392,14 +443,17 @@
     Random noise seeds. Default is random seeds for each generation.
     """
 
 
 @dataclass
 class StableDiffusionXLIPAdapterOut:
     outputs: List[StableDiffusionImage]
+    """
+    Generated images.
+    """
 
 
 @dataclass
 class StableDiffusionXLControlNetIn:
     image_uri: str
     """
     Input image.
@@ -412,15 +466,15 @@
     """
     Text prompt.
     """
     num_images: int
     """
     Number of images to generate.
     """
-    output_resolution: Optional[int] = 1024
+    output_resolution: int = 1024
     """
     Resolution of the output image, in pixels.
     """
     negative_prompt: Optional[str] = None
     """
     Negative input prompt.
     """
@@ -437,14 +491,17 @@
     Random noise seeds. Default is random seeds for each generation.
     """
 
 
 @dataclass
 class StableDiffusionXLControlNetOut:
     outputs: List[StableDiffusionImage]
+    """
+    Generated images.
+    """
 
 
 @dataclass
 class GenerativeEditImageIn:
     image_uri: str
     """
     Original image.
@@ -457,15 +514,15 @@
     """
     Mask image that controls which pixels are inpainted. If unset, the entire image is edited (image-to-image).
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["StableDiffusionXLInpaint"]] = "StableDiffusionXLInpaint"
+    node: Literal["StableDiffusionXLInpaint"] = "StableDiffusionXLInpaint"
     """
     Selected node.
     """
 
 
 @dataclass
 class GenerativeEditImageOut:
@@ -493,23 +550,26 @@
     """
     Mask image that controls which pixels are edited (inpainting). If unset, the entire image is edited (image-to-image).
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["StableDiffusionXLInpaint"]] = "StableDiffusionXLInpaint"
+    node: Literal["StableDiffusionXLInpaint"] = "StableDiffusionXLInpaint"
     """
     Selected node.
     """
 
 
 @dataclass
 class MultiGenerativeEditImageOut:
     outputs: List[GenerativeEditImageOut]
+    """
+    Generated images.
+    """
 
 
 @dataclass
 class StableDiffusionXLInpaintIn:
     image_uri: str
     """
     Original image.
@@ -522,39 +582,42 @@
     """
     Number of images to generate.
     """
     mask_image_uri: Optional[str] = None
     """
     Mask image that controls which pixels are edited (inpainting). If unset, the entire image is edited (image-to-image).
     """
-    output_resolution: Optional[int] = 1024
+    output_resolution: int = 1024
     """
     Resolution of the output image, in pixels.
     """
     negative_prompt: Optional[str] = None
     """
     Negative input prompt.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    strength: Optional[float] = 0.5
+    strength: float = 1
     """
     Controls the strength of the generation process.
     """
     seeds: Optional[List[int]] = None
     """
     Random noise seeds. Default is random seeds for each generation.
     """
 
 
 @dataclass
 class StableDiffusionXLInpaintOut:
     outputs: List[StableDiffusionImage]
+    """
+    Generated images.
+    """
 
 
 @dataclass
 class BoundingBox:
     x1: float
     """
     Top left corner x.
@@ -595,15 +658,15 @@
     """
     Mask image that controls which pixels are inpainted.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["BigLaMa"]] = "BigLaMa"
+    node: Literal["BigLaMa"] = "BigLaMa"
     """
     Selected node.
     """
 
 
 @dataclass
 class FillMaskOut:
@@ -639,27 +702,27 @@
 
 @dataclass
 class RemoveBackgroundIn:
     image_uri: str
     """
     Input image.
     """
-    return_mask: Optional[bool] = None
+    return_mask: bool = False
     """
     Return a mask image instead of the original content.
     """
     background_color: Optional[str] = None
     """
     Hex value background color. Transparent if unset.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["DISISNet"]] = "DISISNet"
+    node: Literal["DISISNet"] = "DISISNet"
     """
     Selected node.
     """
 
 
 @dataclass
 class RemoveBackgroundOut:
@@ -671,22 +734,14 @@
 
 @dataclass
 class DISISNetIn:
     image_uri: str
     """
     Input image.
     """
-    return_mask: Optional[bool] = None
-    """
-    Return a mask image instead of the original content.
-    """
-    background_color: Optional[str] = None
-    """
-    Hex value background color. Transparent if unset.
-    """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
@@ -703,15 +758,15 @@
     """
     Input image.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["RealESRGAN"]] = "RealESRGAN"
+    node: Literal["RealESRGAN"] = "RealESRGAN"
     """
     Selected node.
     """
 
 
 @dataclass
 class UpscaleImageOut:
@@ -723,18 +778,14 @@
 
 @dataclass
 class RealESRGANIn:
     image_uri: str
     """
     Input image.
     """
-    model: Optional[Literal["real-esrgan-x4"]] = "real-esrgan-x4"
-    """
-    Selected model.
-    """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
@@ -755,15 +806,15 @@
     """
     Point prompt.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["SegmentAnything"]] = "SegmentAnything"
+    node: Literal["SegmentAnything"] = "SegmentAnything"
     """
     Selected node.
     """
 
 
 @dataclass
 class SegmentUnderPointOut:
@@ -807,31 +858,31 @@
     """
     Input audio.
     """
     prompt: Optional[str] = None
     """
     Prompt to guide model on the content and context of input audio.
     """
-    language: Optional[str] = "en"
+    language: str = "en"
     """
     Language of input audio in [ISO-639-1](https://en.wikipedia.org/wiki/List_of_ISO_639_language_codes) format.
     """
-    segment: Optional[bool] = False
+    segment: bool = False
     """
     Segment the text into sentences with approximate timestamps.
     """
-    align: Optional[bool] = False
+    align: bool = False
     """
     Align transcription to produce more accurate sentence-level timestamps and word-level timestamps. An array of word segments will be included in each sentence segment.
     """
-    diarize: Optional[bool] = False
+    diarize: bool = False
     """
     Identify speakers for each segment. Speaker IDs will be included in each segment.
     """
-    suggest_chapters: Optional[bool] = False
+    suggest_chapters: bool = False
     """
     Suggest automatic chapter markers.
     """
 
 
 @dataclass
 class TranscribedWord:
@@ -911,15 +962,15 @@
     """
     Input text.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the audio data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["XTTSV2"]] = "XTTSV2"
+    node: Literal["XTTSV2"] = "XTTSV2"
     """
     Selected node.
     """
 
 
 @dataclass
 class GenerateSpeechOut:
@@ -935,15 +986,15 @@
     """
     Input text.
     """
     audio_uri: Optional[str] = None
     """
     Reference audio used to synthesize the speaker. If unset, a default speaker voice will be used.
     """
-    language: Optional[str] = "en"
+    language: str = "en"
     """
     Language of input text. Supported languages: `en, de, fr, es, it, pt, pl, zh, ar, cs, ru, nl, tr, hu, ko`.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the audio data will be returned as a base64-encoded string.
     """
@@ -991,15 +1042,15 @@
     """
     Choose keys from `metadata` to embed with text.
     """
     doc_id: Optional[str] = None
     """
     Vector store document ID. Ignored if `store` is unset.
     """
-    node: Optional[Literal["JinaV2", "CLIP"]] = "JinaV2"
+    node: Literal["JinaV2", "CLIP"] = "JinaV2"
     """
     Selected node.
     """
 
 
 @dataclass
 class EmbedTextOut:
@@ -1035,15 +1086,15 @@
     """
     [Vector store](/docs/vector-stores) identifier.
     """
     embedded_metadata_keys: Optional[List[str]] = None
     """
     Choose keys from `metadata` to embed with text.
     """
-    node: Optional[Literal["JinaV2", "CLIP"]] = "JinaV2"
+    node: Literal["JinaV2", "CLIP"] = "JinaV2"
     """
     Selected node.
     """
 
 
 @dataclass
 class MultiEmbedTextOut:
@@ -1087,15 +1138,15 @@
     """
     [Vector store](/docs/vector-stores) identifier.
     """
     doc_id: Optional[str] = None
     """
     Vector store document ID. Ignored if `store` is unset.
     """
-    node: Optional[Literal["CLIP"]] = "CLIP"
+    node: Literal["CLIP"] = "CLIP"
     """
     Selected node.
     """
 
 
 @dataclass
 class EmbedImageOut:
@@ -1143,15 +1194,15 @@
     """
     Items to embed.
     """
     store: Optional[str] = None
     """
     [Vector store](/docs/vector-stores) identifier.
     """
-    node: Optional[Literal["CLIP"]] = "CLIP"
+    node: Literal["CLIP"] = "CLIP"
     """
     Selected node.
     """
 
 
 @dataclass
 class MultiEmbedImageOut:
@@ -1191,23 +1242,23 @@
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model
     """
-    m: Optional[int] = 16
+    m: int = 16
     """
     The max number of connections per layer for the index.
     """
-    ef_construction: Optional[int] = 64
+    ef_construction: int = 64
     """
     The size of the dynamic candidate list for constructing the index graph.
     """
-    metric: Optional[Literal["cosine", "l2", "inner"]] = "inner"
+    metric: Literal["cosine", "l2", "inner"] = "inner"
     """
     The distance metric to construct the index with.
     """
 
 
 @dataclass
 class CreateVectorStoreOut:
@@ -1400,34 +1451,38 @@
     """
     Vector to use for the query.
     """
     query_strings: Optional[List[str]] = None
     """
     Texts to embed and use for the query.
     """
-    top_k: Optional[int] = 10
+    top_k: int = 10
     """
     Number of results to return.
     """
-    ef_search: Optional[int] = 40
+    ef_search: int = 40
     """
     The size of the dynamic candidate list for searching the index graph.
     """
-    include_values: Optional[bool] = False
+    include_values: bool = False
     """
     Include the values of the vectors in the response.
     """
-    include_metadata: Optional[bool] = False
+    include_metadata: bool = False
     """
     Include the metadata of the vectors in the response.
     """
     filters: Optional[Dict[str, Any]] = None
     """
     Filter metadata by key-value pairs.
     """
+    metric: Optional[Literal["cosine", "l2", "inner"]] = None
+    """
+    The distance metric used for the query. Defaults to the distance metric the vector store was created with.
+    """
 
 
 @dataclass
 class VectorStoreQueryResult:
     id: str
     """
     Document ID.
```

### Comparing `substrate-120240405.0.3/substrate/future_dataclass_models.py` & `substrate-120240411.0.4/substrate/future_dataclass_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,38 +24,43 @@
     The type of error returned.
     """
     message: str
     """
     (Future reference)
     A message providing more details about the error.
     """
+    request_id: Optional[str] = None
+    """
+    (Future reference)
+    A unique identifier for the request.
+    """
 
 
 @dataclass
 class FutureGenerateTextIn:
     """
     (Future reference)
     """
 
     prompt: str
     """
     (Future reference)
     Input prompt.
     """
-    temperature: Optional[int] = 4
+    temperature: float = 0.4
     """
     (Future reference)
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     (Future reference)
     Maximum number of tokens to generate.
     """
-    node: Optional[Literal["Mistral7BInstruct"]] = "Mistral7BInstruct"
+    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
@@ -83,25 +88,25 @@
     Input prompt.
     """
     json_schema: Dict[str, Any]
     """
     (Future reference)
     JSON schema to guide `json_object` response.
     """
-    temperature: Optional[int] = 4
+    temperature: float = 0.4
     """
     (Future reference)
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     (Future reference)
     Maximum number of tokens to generate.
     """
-    node: Optional[Literal["Mistral7BInstruct"]] = "Mistral7BInstruct"
+    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
@@ -129,38 +134,42 @@
     Input prompt.
     """
     num_choices: int
     """
     (Future reference)
     Number of choices to generate.
     """
-    temperature: Optional[int] = 4
+    temperature: float = 0.4
     """
     (Future reference)
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     (Future reference)
     Maximum number of tokens to generate.
     """
-    node: Optional[Literal["Mistral7BInstruct"]] = "Mistral7BInstruct"
+    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
 class FutureMultiGenerateTextOut:
     """
     (Future reference)
     """
 
     choices: List[FutureGenerateTextOut]
+    """
+    (Future reference)
+    Response choices.
+    """
 
 
 @dataclass
 class FutureMultiGenerateJSONIn:
     """
     (Future reference)
     """
@@ -176,38 +185,42 @@
     JSON schema to guide `json_object` response.
     """
     num_choices: int
     """
     (Future reference)
     Number of choices to generate.
     """
-    temperature: Optional[int] = 4
+    temperature: float = 0.4
     """
     (Future reference)
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     (Future reference)
     Maximum number of tokens to generate.
     """
-    node: Optional[Literal["Mistral7BInstruct"]] = "Mistral7BInstruct"
+    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
 class FutureMultiGenerateJSONOut:
     """
     (Future reference)
     """
 
     choices: List[FutureGenerateJSONOut]
+    """
+    (Future reference)
+    Response choices.
+    """
 
 
 @dataclass
 class FutureMistral7BInstructIn:
     """
     (Future reference)
     """
@@ -260,14 +273,18 @@
 @dataclass
 class FutureMistral7BInstructOut:
     """
     (Future reference)
     """
 
     choices: List[Mistral7BInstructChoice]
+    """
+    (Future reference)
+    Response choices.
+    """
 
 
 @dataclass
 class FutureGenerateTextVisionIn:
     """
     (Future reference)
     """
@@ -278,25 +295,20 @@
     Text prompt.
     """
     image_uris: List[str]
     """
     (Future reference)
     Image prompts.
     """
-    temperature: Optional[int] = 4
-    """
-    (Future reference)
-    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
-    """
-    max_tokens: Optional[int] = 800
+    max_tokens: int = 800
     """
     (Future reference)
     Maximum number of tokens to generate.
     """
-    node: Optional[Literal["Firellava13B"]] = "Firellava13B"
+    node: Literal["Firellava13B"] = "Firellava13B"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
@@ -324,20 +336,15 @@
     Text prompt.
     """
     image_uris: List[str]
     """
     (Future reference)
     Image prompts.
     """
-    temperature: Optional[float] = None
-    """
-    (Future reference)
-    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
-    """
-    max_tokens: Optional[int] = 800
+    max_tokens: int = 800
     """
     (Future reference)
     Maximum number of tokens to generate.
     """
 
 
 @dataclass
@@ -365,15 +372,15 @@
     Text prompt.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["StableDiffusionXL"]] = "StableDiffusionXL"
+    node: Literal["StableDiffusionXL"] = "StableDiffusionXL"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
@@ -406,77 +413,81 @@
     Number of images to generate.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["StableDiffusionXL"]] = "StableDiffusionXL"
+    node: Literal["StableDiffusionXL"] = "StableDiffusionXL"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
 class FutureMultiGenerateImageOut:
     """
     (Future reference)
     """
 
     outputs: List[FutureGenerateImageOut]
+    """
+    (Future reference)
+    Generated images.
+    """
 
 
 @dataclass
 class FutureStableDiffusionXLIn:
     """
     (Future reference)
     """
 
     prompt: str
     """
     (Future reference)
     Text prompt.
     """
-    negative_prompt: Optional[str] = None
+    num_images: int
     """
     (Future reference)
-    Negative input prompt.
+    Number of images to generate.
     """
-    steps: Optional[int] = None
+    negative_prompt: Optional[str] = None
     """
     (Future reference)
-    Number of diffusion steps.
+    Negative input prompt.
     """
-    num_images: Optional[int] = None
+    steps: int = 30
     """
     (Future reference)
-    Number of images to generate.
+    Number of diffusion steps.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    height: Optional[int] = None
+    height: int = 1024
     """
     (Future reference)
     Height of output image, in pixels.
     """
-    width: Optional[int] = None
+    width: int = 1024
     """
     (Future reference)
     Width of output image, in pixels.
     """
-    seeds: Optional[int] = None
+    seeds: Optional[List[int]] = None
     """
     (Future reference)
     Seeds for deterministic generation. Default is a random seed.
     """
-    guidance_scale: Optional[float] = 5
+    guidance_scale: float = 7
     """
     (Future reference)
     Higher values adhere to the text prompt more strongly, typically at the expense of image quality.
     """
 
 
 @dataclass
@@ -500,14 +511,74 @@
 @dataclass
 class FutureStableDiffusionXLOut:
     """
     (Future reference)
     """
 
     outputs: List[StableDiffusionImage]
+    """
+    (Future reference)
+    Generated images.
+    """
+
+
+@dataclass
+class FutureStableDiffusionXLLightningIn:
+    """
+    (Future reference)
+    """
+
+    prompt: str
+    """
+    (Future reference)
+    Text prompt.
+    """
+    negative_prompt: Optional[str] = None
+    """
+    (Future reference)
+    Negative input prompt.
+    """
+    num_images: int = 1
+    """
+    (Future reference)
+    Number of images to generate.
+    """
+    store: Optional[str] = None
+    """
+    (Future reference)
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    """
+    height: Optional[int] = None
+    """
+    (Future reference)
+    Height of output image, in pixels.
+    """
+    width: Optional[int] = None
+    """
+    (Future reference)
+    Width of output image, in pixels.
+    """
+    seeds: Optional[List[int]] = None
+    """
+    (Future reference)
+    Seeds for deterministic generation. Default is a random seed.
+    """
+
+
+@dataclass
+class FutureStableDiffusionXLLightningOut:
+    """
+    (Future reference)
+    """
+
+    outputs: List[StableDiffusionImage]
+    """
+    (Future reference)
+    Generated images.
+    """
 
 
 @dataclass
 class FutureStableDiffusionXLIPAdapterIn:
     """
     (Future reference)
     """
@@ -562,14 +633,18 @@
 @dataclass
 class FutureStableDiffusionXLIPAdapterOut:
     """
     (Future reference)
     """
 
     outputs: List[StableDiffusionImage]
+    """
+    (Future reference)
+    Generated images.
+    """
 
 
 @dataclass
 class FutureStableDiffusionXLControlNetIn:
     """
     (Future reference)
     """
@@ -590,15 +665,15 @@
     Text prompt.
     """
     num_images: int
     """
     (Future reference)
     Number of images to generate.
     """
-    output_resolution: Optional[int] = 1024
+    output_resolution: int = 1024
     """
     (Future reference)
     Resolution of the output image, in pixels.
     """
     negative_prompt: Optional[str] = None
     """
     (Future reference)
@@ -624,14 +699,18 @@
 @dataclass
 class FutureStableDiffusionXLControlNetOut:
     """
     (Future reference)
     """
 
     outputs: List[StableDiffusionImage]
+    """
+    (Future reference)
+    Generated images.
+    """
 
 
 @dataclass
 class FutureGenerativeEditImageIn:
     """
     (Future reference)
     """
@@ -652,15 +731,15 @@
     Mask image that controls which pixels are inpainted. If unset, the entire image is edited (image-to-image).
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["StableDiffusionXLInpaint"]] = "StableDiffusionXLInpaint"
+    node: Literal["StableDiffusionXLInpaint"] = "StableDiffusionXLInpaint"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
@@ -703,28 +782,32 @@
     Mask image that controls which pixels are edited (inpainting). If unset, the entire image is edited (image-to-image).
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["StableDiffusionXLInpaint"]] = "StableDiffusionXLInpaint"
+    node: Literal["StableDiffusionXLInpaint"] = "StableDiffusionXLInpaint"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
 class FutureMultiGenerativeEditImageOut:
     """
     (Future reference)
     """
 
     outputs: List[FutureGenerativeEditImageOut]
+    """
+    (Future reference)
+    Generated images.
+    """
 
 
 @dataclass
 class FutureStableDiffusionXLInpaintIn:
     """
     (Future reference)
     """
@@ -745,30 +828,30 @@
     Number of images to generate.
     """
     mask_image_uri: Optional[str] = None
     """
     (Future reference)
     Mask image that controls which pixels are edited (inpainting). If unset, the entire image is edited (image-to-image).
     """
-    output_resolution: Optional[int] = 1024
+    output_resolution: int = 1024
     """
     (Future reference)
     Resolution of the output image, in pixels.
     """
     negative_prompt: Optional[str] = None
     """
     (Future reference)
     Negative input prompt.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    strength: Optional[float] = 0.5
+    strength: float = 1
     """
     (Future reference)
     Controls the strength of the generation process.
     """
     seeds: Optional[List[int]] = None
     """
     (Future reference)
@@ -779,14 +862,18 @@
 @dataclass
 class FutureStableDiffusionXLInpaintOut:
     """
     (Future reference)
     """
 
     outputs: List[StableDiffusionImage]
+    """
+    (Future reference)
+    Generated images.
+    """
 
 
 @dataclass
 class BoundingBox:
     """
     (Future reference)
     """
@@ -848,15 +935,15 @@
     Mask image that controls which pixels are inpainted.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["BigLaMa"]] = "BigLaMa"
+    node: Literal["BigLaMa"] = "BigLaMa"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
@@ -915,30 +1002,30 @@
     """
 
     image_uri: str
     """
     (Future reference)
     Input image.
     """
-    return_mask: Optional[bool] = None
+    return_mask: bool = False
     """
     (Future reference)
     Return a mask image instead of the original content.
     """
     background_color: Optional[str] = None
     """
     (Future reference)
     Hex value background color. Transparent if unset.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["DISISNet"]] = "DISISNet"
+    node: Literal["DISISNet"] = "DISISNet"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
@@ -961,24 +1048,14 @@
     """
 
     image_uri: str
     """
     (Future reference)
     Input image.
     """
-    return_mask: Optional[bool] = None
-    """
-    (Future reference)
-    Return a mask image instead of the original content.
-    """
-    background_color: Optional[str] = None
-    """
-    (Future reference)
-    Hex value background color. Transparent if unset.
-    """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
@@ -1007,15 +1084,15 @@
     Input image.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["RealESRGAN"]] = "RealESRGAN"
+    node: Literal["RealESRGAN"] = "RealESRGAN"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
@@ -1038,19 +1115,14 @@
     """
 
     image_uri: str
     """
     (Future reference)
     Input image.
     """
-    model: Optional[Literal["real-esrgan-x4"]] = "real-esrgan-x4"
-    """
-    (Future reference)
-    Selected model.
-    """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
@@ -1084,15 +1156,15 @@
     Point prompt.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["SegmentAnything"]] = "SegmentAnything"
+    node: Literal["SegmentAnything"] = "SegmentAnything"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
@@ -1161,35 +1233,35 @@
     Input audio.
     """
     prompt: Optional[str] = None
     """
     (Future reference)
     Prompt to guide model on the content and context of input audio.
     """
-    language: Optional[str] = "en"
+    language: str = "en"
     """
     (Future reference)
     Language of input audio in [ISO-639-1](https://en.wikipedia.org/wiki/List_of_ISO_639_language_codes) format.
     """
-    segment: Optional[bool] = False
+    segment: bool = False
     """
     (Future reference)
     Segment the text into sentences with approximate timestamps.
     """
-    align: Optional[bool] = False
+    align: bool = False
     """
     (Future reference)
     Align transcription to produce more accurate sentence-level timestamps and word-level timestamps. An array of word segments will be included in each sentence segment.
     """
-    diarize: Optional[bool] = False
+    diarize: bool = False
     """
     (Future reference)
     Identify speakers for each segment. Speaker IDs will be included in each segment.
     """
-    suggest_chapters: Optional[bool] = False
+    suggest_chapters: bool = False
     """
     (Future reference)
     Suggest automatic chapter markers.
     """
 
 
 @dataclass
@@ -1306,15 +1378,15 @@
     Input text.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the audio data will be returned as a base64-encoded string.
     """
-    node: Optional[Literal["XTTSV2"]] = "XTTSV2"
+    node: Literal["XTTSV2"] = "XTTSV2"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
@@ -1342,15 +1414,15 @@
     Input text.
     """
     audio_uri: Optional[str] = None
     """
     (Future reference)
     Reference audio used to synthesize the speaker. If unset, a default speaker voice will be used.
     """
-    language: Optional[str] = "en"
+    language: str = "en"
     """
     (Future reference)
     Language of input text. Supported languages: `en, de, fr, es, it, pt, pl, zh, ar, cs, ru, nl, tr, hu, ko`.
     """
     store: Optional[str] = None
     """
     (Future reference)
@@ -1421,15 +1493,15 @@
     Choose keys from `metadata` to embed with text.
     """
     doc_id: Optional[str] = None
     """
     (Future reference)
     Vector store document ID. Ignored if `store` is unset.
     """
-    node: Optional[Literal["JinaV2", "CLIP"]] = "JinaV2"
+    node: Literal["JinaV2", "CLIP"] = "JinaV2"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
@@ -1485,15 +1557,15 @@
     [Vector store](/docs/vector-stores) identifier.
     """
     embedded_metadata_keys: Optional[List[str]] = None
     """
     (Future reference)
     Choose keys from `metadata` to embed with text.
     """
-    node: Optional[Literal["JinaV2", "CLIP"]] = "JinaV2"
+    node: Literal["JinaV2", "CLIP"] = "JinaV2"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
@@ -1562,15 +1634,15 @@
     [Vector store](/docs/vector-stores) identifier.
     """
     doc_id: Optional[str] = None
     """
     (Future reference)
     Vector store document ID. Ignored if `store` is unset.
     """
-    node: Optional[Literal["CLIP"]] = "CLIP"
+    node: Literal["CLIP"] = "CLIP"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
@@ -1644,15 +1716,15 @@
     Items to embed.
     """
     store: Optional[str] = None
     """
     (Future reference)
     [Vector store](/docs/vector-stores) identifier.
     """
-    node: Optional[Literal["CLIP"]] = "CLIP"
+    node: Literal["CLIP"] = "CLIP"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
@@ -1716,25 +1788,25 @@
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     (Future reference)
     Selected embedding model
     """
-    m: Optional[int] = 16
+    m: int = 16
     """
     (Future reference)
     The max number of connections per layer for the index.
     """
-    ef_construction: Optional[int] = 64
+    ef_construction: int = 64
     """
     (Future reference)
     The size of the dynamic candidate list for constructing the index graph.
     """
-    metric: Optional[Literal["cosine", "l2", "inner"]] = "inner"
+    metric: Literal["cosine", "l2", "inner"] = "inner"
     """
     (Future reference)
     The distance metric to construct the index with.
     """
 
 
 @dataclass
@@ -2015,39 +2087,44 @@
     Vector to use for the query.
     """
     query_strings: Optional[List[str]] = None
     """
     (Future reference)
     Texts to embed and use for the query.
     """
-    top_k: Optional[int] = 10
+    top_k: int = 10
     """
     (Future reference)
     Number of results to return.
     """
-    ef_search: Optional[int] = 40
+    ef_search: int = 40
     """
     (Future reference)
     The size of the dynamic candidate list for searching the index graph.
     """
-    include_values: Optional[bool] = False
+    include_values: bool = False
     """
     (Future reference)
     Include the values of the vectors in the response.
     """
-    include_metadata: Optional[bool] = False
+    include_metadata: bool = False
     """
     (Future reference)
     Include the metadata of the vectors in the response.
     """
     filters: Optional[Dict[str, Any]] = None
     """
     (Future reference)
     Filter metadata by key-value pairs.
     """
+    metric: Optional[Literal["cosine", "l2", "inner"]] = None
+    """
+    (Future reference)
+    The distance metric used for the query. Defaults to the distance metric the vector store was created with.
+    """
 
 
 @dataclass
 class VectorStoreQueryResult:
     """
     (Future reference)
     """
```

### Comparing `substrate-120240405.0.3/substrate/nodes.py` & `substrate-120240411.0.4/substrate/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 ꩜ Substrate
 @GENERATED FILE
-20240405.20240405
+20240411.20240414
 """
 
 from .substrate import SubstrateResponse
 from .core.corenode import CoreNode
 from .dataclass_models import (
     CLIPOut,
     JinaV2Out,
@@ -41,14 +41,15 @@
     StableDiffusionXLOut,
     GenerateTextVisionOut,
     MultiGenerateImageOut,
     GenerativeEditImageOut,
     MultiGenerativeEditImageOut,
     StableDiffusionXLInpaintOut,
     StableDiffusionXLIPAdapterOut,
+    StableDiffusionXLLightningOut,
     StableDiffusionXLControlNetOut,
 )
 from .typeddict_models import (
     CLIPIn,
     JinaV2In,
     XTTSV2In,
     BigLaMaIn,
@@ -82,14 +83,15 @@
     StableDiffusionXLIn,
     GenerateTextVisionIn,
     MultiGenerateImageIn,
     GenerativeEditImageIn,
     MultiGenerativeEditImageIn,
     StableDiffusionXLInpaintIn,
     StableDiffusionXLIPAdapterIn,
+    StableDiffusionXLLightningIn,
     StableDiffusionXLControlNetIn,
 )
 from .future_dataclass_models import (
     FutureCLIPOut,
     FutureJinaV2Out,
     FutureXTTSV2Out,
     FutureBigLaMaOut,
@@ -123,14 +125,15 @@
     FutureStableDiffusionXLOut,
     FutureGenerateTextVisionOut,
     FutureMultiGenerateImageOut,
     FutureGenerativeEditImageOut,
     FutureMultiGenerativeEditImageOut,
     FutureStableDiffusionXLInpaintOut,
     FutureStableDiffusionXLIPAdapterOut,
+    FutureStableDiffusionXLLightningOut,
     FutureStableDiffusionXLControlNetOut,
 )
 
 
 class GenerateText(CoreNode):
     """
     Generate text using a language model.
@@ -324,15 +327,15 @@
     Generate text with image input.
 
     https://substrate.run/library#GenerateTextVision
     """
 
     def __init__(self, args: GenerateTextVisionIn):
         """
-        Input arguments: `prompt`, `image_uris`, `temperature` (optional), `max_tokens` (optional), `node` (optional)
+        Input arguments: `prompt`, `image_uris`, `max_tokens` (optional), `node` (optional)
 
         Output fields: `future.text`
 
         https://substrate.run/library#GenerateTextVision
         """
         super().__init__(**args)
         self.node = "GenerateTextVision"
@@ -418,15 +421,15 @@
     Generate text with image input using [FireLLaVA 13B](https://fireworks.ai/blog/firellava-the-first-commercially-permissive-oss-llava-model).
 
     https://substrate.run/library#Firellava13B
     """
 
     def __init__(self, args: Firellava13BIn):
         """
-        Input arguments: `prompt`, `image_uris`, `temperature` (optional), `max_tokens` (optional)
+        Input arguments: `prompt`, `image_uris`, `max_tokens` (optional)
 
         Output fields: `future.text`
 
         https://substrate.run/library#Firellava13B
         """
         super().__init__(**args)
         self.node = "Firellava13B"
@@ -653,15 +656,15 @@
     Generate an image using [Stable Diffusion XL](https://arxiv.org/abs/2307.01952).
 
     https://substrate.run/library#StableDiffusionXL
     """
 
     def __init__(self, args: StableDiffusionXLIn):
         """
-        Input arguments: `prompt`, `negative_prompt` (optional), `steps` (optional), `num_images` (optional), `store` (optional), `height` (optional), `width` (optional), `seeds` (optional), `guidance_scale` (optional)
+        Input arguments: `prompt`, `negative_prompt` (optional), `steps` (optional), `num_images`, `store` (optional), `height` (optional), `width` (optional), `seeds` (optional), `guidance_scale` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXL
         """
         super().__init__(**args)
         self.node = "StableDiffusionXL"
@@ -691,104 +694,104 @@
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXL
         """
         return super().future  # type: ignore
 
 
-class StableDiffusionXLInpaint(CoreNode):
+class StableDiffusionXLLightning(CoreNode):
     """
-    Edit an image using [Stable Diffusion XL](https://arxiv.org/abs/2307.01952). Supports inpainting (edit part of the image with a mask) and image-to-image (edit the full image).
+    Generate an image using [Stable Diffusion XL Lightning](https://arxiv.org/abs/2402.13929).
 
-    https://substrate.run/library#StableDiffusionXLInpaint
+    https://substrate.run/library#StableDiffusionXLLightning
     """
 
-    def __init__(self, args: StableDiffusionXLInpaintIn):
+    def __init__(self, args: StableDiffusionXLLightningIn):
         """
-        Input arguments: `image_uri`, `prompt`, `mask_image_uri` (optional), `num_images`, `output_resolution` (optional), `negative_prompt` (optional), `store` (optional), `strength` (optional), `seeds` (optional)
+        Input arguments: `prompt`, `negative_prompt` (optional), `num_images` (optional), `store` (optional), `height` (optional), `width` (optional), `seeds` (optional)
 
         Output fields: `future.outputs`
 
-        https://substrate.run/library#StableDiffusionXLInpaint
+        https://substrate.run/library#StableDiffusionXLLightning
         """
         super().__init__(**args)
-        self.node = "StableDiffusionXLInpaint"
+        self.node = "StableDiffusionXLLightning"
 
-    def output(self, response: SubstrateResponse) -> StableDiffusionXLInpaintOut:
+    def output(self, response: SubstrateResponse) -> StableDiffusionXLLightningOut:
         """
         Retrieve this node's output from a response.
 
         Output fields: `future.outputs`
 
-        https://substrate.run/library#StableDiffusionXLInpaint
+        https://substrate.run/library#StableDiffusionXLLightning
         """
-        klass = StableDiffusionXLInpaintOut
+        klass = StableDiffusionXLLightningOut
         json = response.api_response.json
         if json and json.get("data"):
             data = json["data"]
             node_id = self.id
             if data.get(self.id):
                 return klass(**data[self.id])
         raise ValueError(f"Node {self.id} not found in response")
 
     @property
-    def future(self) -> FutureStableDiffusionXLInpaintOut:  # type: ignore
+    def future(self) -> FutureStableDiffusionXLLightningOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.outputs`
 
-        https://substrate.run/library#StableDiffusionXLInpaint
+        https://substrate.run/library#StableDiffusionXLLightning
         """
         return super().future  # type: ignore
 
 
-class StableDiffusionXLIPAdapter(CoreNode):
+class StableDiffusionXLInpaint(CoreNode):
     """
-    Generate an image with an image prompt, using Stable Diffusion XL with [IP-Adapter](https://arxiv.org/abs/2308.06721).
+    Edit an image using [Stable Diffusion XL](https://arxiv.org/abs/2307.01952). Supports inpainting (edit part of the image with a mask) and image-to-image (edit the full image).
 
-    https://substrate.run/library#StableDiffusionXLIPAdapter
+    https://substrate.run/library#StableDiffusionXLInpaint
     """
 
-    def __init__(self, args: StableDiffusionXLIPAdapterIn):
+    def __init__(self, args: StableDiffusionXLInpaintIn):
         """
-        Input arguments: `prompt`, `image_prompt_uri` (optional), `num_images`, `ip_adapter_scale` (optional), `negative_prompt` (optional), `store` (optional), `width` (optional), `height` (optional), `seeds` (optional)
+        Input arguments: `image_uri`, `prompt`, `mask_image_uri` (optional), `num_images`, `output_resolution` (optional), `negative_prompt` (optional), `store` (optional), `strength` (optional), `seeds` (optional)
 
         Output fields: `future.outputs`
 
-        https://substrate.run/library#StableDiffusionXLIPAdapter
+        https://substrate.run/library#StableDiffusionXLInpaint
         """
         super().__init__(**args)
-        self.node = "StableDiffusionXLIPAdapter"
+        self.node = "StableDiffusionXLInpaint"
 
-    def output(self, response: SubstrateResponse) -> StableDiffusionXLIPAdapterOut:
+    def output(self, response: SubstrateResponse) -> StableDiffusionXLInpaintOut:
         """
         Retrieve this node's output from a response.
 
         Output fields: `future.outputs`
 
-        https://substrate.run/library#StableDiffusionXLIPAdapter
+        https://substrate.run/library#StableDiffusionXLInpaint
         """
-        klass = StableDiffusionXLIPAdapterOut
+        klass = StableDiffusionXLInpaintOut
         json = response.api_response.json
         if json and json.get("data"):
             data = json["data"]
             node_id = self.id
             if data.get(self.id):
                 return klass(**data[self.id])
         raise ValueError(f"Node {self.id} not found in response")
 
     @property
-    def future(self) -> FutureStableDiffusionXLIPAdapterOut:  # type: ignore
+    def future(self) -> FutureStableDiffusionXLInpaintOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.outputs`
 
-        https://substrate.run/library#StableDiffusionXLIPAdapter
+        https://substrate.run/library#StableDiffusionXLInpaint
         """
         return super().future  # type: ignore
 
 
 class StableDiffusionXLControlNet(CoreNode):
     """
     Generate an image with generation structured by an input image, using Stable Diffusion XL with [ControlNet](https://arxiv.org/abs/2302.05543).
@@ -832,198 +835,198 @@
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXLControlNet
         """
         return super().future  # type: ignore
 
 
-class FillMask(CoreNode):
+class StableDiffusionXLIPAdapter(CoreNode):
     """
-    Fill (inpaint) part of an image, e.g. to 'remove' an object.
+    Generate an image with an image prompt, using Stable Diffusion XL with [IP-Adapter](https://arxiv.org/abs/2308.06721).
 
-    https://substrate.run/library#FillMask
+    https://substrate.run/library#StableDiffusionXLIPAdapter
     """
 
-    def __init__(self, args: FillMaskIn):
+    def __init__(self, args: StableDiffusionXLIPAdapterIn):
         """
-        Input arguments: `image_uri`, `mask_image_uri`, `store` (optional), `node` (optional)
+        Input arguments: `prompt`, `image_prompt_uri` (optional), `num_images`, `ip_adapter_scale` (optional), `negative_prompt` (optional), `store` (optional), `width` (optional), `height` (optional), `seeds` (optional)
 
-        Output fields: `future.image_uri`
+        Output fields: `future.outputs`
 
-        https://substrate.run/library#FillMask
+        https://substrate.run/library#StableDiffusionXLIPAdapter
         """
         super().__init__(**args)
-        self.node = "FillMask"
+        self.node = "StableDiffusionXLIPAdapter"
 
-    def output(self, response: SubstrateResponse) -> FillMaskOut:
+    def output(self, response: SubstrateResponse) -> StableDiffusionXLIPAdapterOut:
         """
         Retrieve this node's output from a response.
 
-        Output fields: `future.image_uri`
+        Output fields: `future.outputs`
 
-        https://substrate.run/library#FillMask
+        https://substrate.run/library#StableDiffusionXLIPAdapter
         """
-        klass = FillMaskOut
+        klass = StableDiffusionXLIPAdapterOut
         json = response.api_response.json
         if json and json.get("data"):
             data = json["data"]
             node_id = self.id
             if data.get(self.id):
                 return klass(**data[self.id])
         raise ValueError(f"Node {self.id} not found in response")
 
     @property
-    def future(self) -> FutureFillMaskOut:  # type: ignore
+    def future(self) -> FutureStableDiffusionXLIPAdapterOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.image_uri`
+        Output fields: `future.outputs`
 
-        https://substrate.run/library#FillMask
+        https://substrate.run/library#StableDiffusionXLIPAdapter
         """
         return super().future  # type: ignore
 
 
-class BigLaMa(CoreNode):
+class TranscribeMedia(CoreNode):
     """
-    Inpaint a mask using [LaMa](https://github.com/advimman/lama).
+    Transcribe speech in an audio or video file.
 
-    https://substrate.run/library#BigLaMa
+    https://substrate.run/library#TranscribeMedia
     """
 
-    def __init__(self, args: BigLaMaIn):
+    def __init__(self, args: TranscribeMediaIn):
         """
-        Input arguments: `image_uri`, `mask_image_uri`, `store` (optional)
+        Input arguments: `audio_uri`, `prompt` (optional), `language` (optional), `segment` (optional), `align` (optional), `diarize` (optional), `suggest_chapters` (optional)
 
-        Output fields: `future.image_uri`
+        Output fields: `future.text`, `future.segments` (optional), `future.chapters` (optional)
 
-        https://substrate.run/library#BigLaMa
+        https://substrate.run/library#TranscribeMedia
         """
         super().__init__(**args)
-        self.node = "BigLaMa"
+        self.node = "TranscribeMedia"
 
-    def output(self, response: SubstrateResponse) -> BigLaMaOut:
+    def output(self, response: SubstrateResponse) -> TranscribeMediaOut:
         """
         Retrieve this node's output from a response.
 
-        Output fields: `future.image_uri`
+        Output fields: `future.text`, `future.segments` (optional), `future.chapters` (optional)
 
-        https://substrate.run/library#BigLaMa
+        https://substrate.run/library#TranscribeMedia
         """
-        klass = BigLaMaOut
+        klass = TranscribeMediaOut
         json = response.api_response.json
         if json and json.get("data"):
             data = json["data"]
             node_id = self.id
             if data.get(self.id):
                 return klass(**data[self.id])
         raise ValueError(f"Node {self.id} not found in response")
 
     @property
-    def future(self) -> FutureBigLaMaOut:  # type: ignore
+    def future(self) -> FutureTranscribeMediaOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.image_uri`
+        Output fields: `future.text`, `future.segments` (optional), `future.chapters` (optional)
 
-        https://substrate.run/library#BigLaMa
+        https://substrate.run/library#TranscribeMedia
         """
         return super().future  # type: ignore
 
 
-class UpscaleImage(CoreNode):
+class GenerateSpeech(CoreNode):
     """
-    Upscale an image.
+    Generate speech from text.
 
-    https://substrate.run/library#UpscaleImage
+    https://substrate.run/library#GenerateSpeech
     """
 
-    def __init__(self, args: UpscaleImageIn):
+    def __init__(self, args: GenerateSpeechIn):
         """
-        Input arguments: `image_uri`, `store` (optional), `node` (optional)
+        Input arguments: `text`, `store` (optional), `node` (optional)
 
-        Output fields: `future.image_uri`
+        Output fields: `future.audio_uri`
 
-        https://substrate.run/library#UpscaleImage
+        https://substrate.run/library#GenerateSpeech
         """
         super().__init__(**args)
-        self.node = "UpscaleImage"
+        self.node = "GenerateSpeech"
 
-    def output(self, response: SubstrateResponse) -> UpscaleImageOut:
+    def output(self, response: SubstrateResponse) -> GenerateSpeechOut:
         """
         Retrieve this node's output from a response.
 
-        Output fields: `future.image_uri`
+        Output fields: `future.audio_uri`
 
-        https://substrate.run/library#UpscaleImage
+        https://substrate.run/library#GenerateSpeech
         """
-        klass = UpscaleImageOut
+        klass = GenerateSpeechOut
         json = response.api_response.json
         if json and json.get("data"):
             data = json["data"]
             node_id = self.id
             if data.get(self.id):
                 return klass(**data[self.id])
         raise ValueError(f"Node {self.id} not found in response")
 
     @property
-    def future(self) -> FutureUpscaleImageOut:  # type: ignore
+    def future(self) -> FutureGenerateSpeechOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.image_uri`
+        Output fields: `future.audio_uri`
 
-        https://substrate.run/library#UpscaleImage
+        https://substrate.run/library#GenerateSpeech
         """
         return super().future  # type: ignore
 
 
-class RealESRGAN(CoreNode):
+class XTTSV2(CoreNode):
     """
-    Upscale an image using [RealESRGAN](https://github.com/xinntao/Real-ESRGAN).
+    Generate speech from text using [XTTS v2](https://docs.coqui.ai/en/latest/models/xtts.html).
 
-    https://substrate.run/library#RealESRGAN
+    https://substrate.run/library#XTTSV2
     """
 
-    def __init__(self, args: RealESRGANIn):
+    def __init__(self, args: XTTSV2In):
         """
-        Input arguments: `image_uri`, `model` (optional), `store` (optional)
+        Input arguments: `text`, `audio_uri` (optional), `language` (optional), `store` (optional)
 
-        Output fields: `future.image_uri`
+        Output fields: `future.audio_uri`
 
-        https://substrate.run/library#RealESRGAN
+        https://substrate.run/library#XTTSV2
         """
         super().__init__(**args)
-        self.node = "RealESRGAN"
+        self.node = "XTTSV2"
 
-    def output(self, response: SubstrateResponse) -> RealESRGANOut:
+    def output(self, response: SubstrateResponse) -> XTTSV2Out:
         """
         Retrieve this node's output from a response.
 
-        Output fields: `future.image_uri`
+        Output fields: `future.audio_uri`
 
-        https://substrate.run/library#RealESRGAN
+        https://substrate.run/library#XTTSV2
         """
-        klass = RealESRGANOut
+        klass = XTTSV2Out
         json = response.api_response.json
         if json and json.get("data"):
             data = json["data"]
             node_id = self.id
             if data.get(self.id):
                 return klass(**data[self.id])
         raise ValueError(f"Node {self.id} not found in response")
 
     @property
-    def future(self) -> FutureRealESRGANOut:  # type: ignore
+    def future(self) -> FutureXTTSV2Out:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.image_uri`
+        Output fields: `future.audio_uri`
 
-        https://substrate.run/library#RealESRGAN
+        https://substrate.run/library#XTTSV2
         """
         return super().future  # type: ignore
 
 
 class RemoveBackground(CoreNode):
     """
     Remove the background from an image, with the option to return the foreground as a mask.
@@ -1067,57 +1070,104 @@
         Output fields: `future.image_uri`
 
         https://substrate.run/library#RemoveBackground
         """
         return super().future  # type: ignore
 
 
-class DISISNet(CoreNode):
+class FillMask(CoreNode):
     """
-    Segment an image using [DIS IS-Net](https://github.com/xuebinqin/DIS).
+    Fill (inpaint) part of an image, e.g. to 'remove' an object.
 
-    https://substrate.run/library#DISISNet
+    https://substrate.run/library#FillMask
     """
 
-    def __init__(self, args: DISISNetIn):
+    def __init__(self, args: FillMaskIn):
         """
-        Input arguments: `image_uri`, `return_mask` (optional), `background_color` (optional), `store` (optional)
+        Input arguments: `image_uri`, `mask_image_uri`, `store` (optional), `node` (optional)
 
         Output fields: `future.image_uri`
 
-        https://substrate.run/library#DISISNet
+        https://substrate.run/library#FillMask
         """
         super().__init__(**args)
-        self.node = "DISISNet"
+        self.node = "FillMask"
 
-    def output(self, response: SubstrateResponse) -> DISISNetOut:
+    def output(self, response: SubstrateResponse) -> FillMaskOut:
         """
         Retrieve this node's output from a response.
 
         Output fields: `future.image_uri`
 
-        https://substrate.run/library#DISISNet
+        https://substrate.run/library#FillMask
         """
-        klass = DISISNetOut
+        klass = FillMaskOut
         json = response.api_response.json
         if json and json.get("data"):
             data = json["data"]
             node_id = self.id
             if data.get(self.id):
                 return klass(**data[self.id])
         raise ValueError(f"Node {self.id} not found in response")
 
     @property
-    def future(self) -> FutureDISISNetOut:  # type: ignore
+    def future(self) -> FutureFillMaskOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.image_uri`
 
-        https://substrate.run/library#DISISNet
+        https://substrate.run/library#FillMask
+        """
+        return super().future  # type: ignore
+
+
+class UpscaleImage(CoreNode):
+    """
+    Upscale an image.
+
+    https://substrate.run/library#UpscaleImage
+    """
+
+    def __init__(self, args: UpscaleImageIn):
+        """
+        Input arguments: `image_uri`, `store` (optional), `node` (optional)
+
+        Output fields: `future.image_uri`
+
+        https://substrate.run/library#UpscaleImage
+        """
+        super().__init__(**args)
+        self.node = "UpscaleImage"
+
+    def output(self, response: SubstrateResponse) -> UpscaleImageOut:
+        """
+        Retrieve this node's output from a response.
+
+        Output fields: `future.image_uri`
+
+        https://substrate.run/library#UpscaleImage
+        """
+        klass = UpscaleImageOut
+        json = response.api_response.json
+        if json and json.get("data"):
+            data = json["data"]
+            node_id = self.id
+            if data.get(self.id):
+                return klass(**data[self.id])
+        raise ValueError(f"Node {self.id} not found in response")
+
+    @property
+    def future(self) -> FutureUpscaleImageOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.image_uri`
+
+        https://substrate.run/library#UpscaleImage
         """
         return super().future  # type: ignore
 
 
 class SegmentUnderPoint(CoreNode):
     """
     Segment an image under a point and return the segment.
@@ -1161,198 +1211,198 @@
         Output fields: `future.mask_image_uri`
 
         https://substrate.run/library#SegmentUnderPoint
         """
         return super().future  # type: ignore
 
 
-class SegmentAnything(CoreNode):
+class DISISNet(CoreNode):
     """
-    Segment an image using [SegmentAnything](https://github.com/facebookresearch/segment-anything).
+    Segment image foreground using [DIS IS-Net](https://github.com/xuebinqin/DIS).
 
-    https://substrate.run/library#SegmentAnything
+    https://substrate.run/library#DISISNet
     """
 
-    def __init__(self, args: SegmentAnythingIn):
+    def __init__(self, args: DISISNetIn):
         """
-        Input arguments: `image_uri`, `point_prompts` (optional), `box_prompts` (optional), `store` (optional)
+        Input arguments: `image_uri`, `store` (optional)
 
-        Output fields: `future.mask_image_uri`
+        Output fields: `future.image_uri`
 
-        https://substrate.run/library#SegmentAnything
+        https://substrate.run/library#DISISNet
         """
         super().__init__(**args)
-        self.node = "SegmentAnything"
+        self.node = "DISISNet"
 
-    def output(self, response: SubstrateResponse) -> SegmentAnythingOut:
+    def output(self, response: SubstrateResponse) -> DISISNetOut:
         """
         Retrieve this node's output from a response.
 
-        Output fields: `future.mask_image_uri`
+        Output fields: `future.image_uri`
 
-        https://substrate.run/library#SegmentAnything
+        https://substrate.run/library#DISISNet
         """
-        klass = SegmentAnythingOut
+        klass = DISISNetOut
         json = response.api_response.json
         if json and json.get("data"):
             data = json["data"]
             node_id = self.id
             if data.get(self.id):
                 return klass(**data[self.id])
         raise ValueError(f"Node {self.id} not found in response")
 
     @property
-    def future(self) -> FutureSegmentAnythingOut:  # type: ignore
+    def future(self) -> FutureDISISNetOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.mask_image_uri`
+        Output fields: `future.image_uri`
 
-        https://substrate.run/library#SegmentAnything
+        https://substrate.run/library#DISISNet
         """
         return super().future  # type: ignore
 
 
-class TranscribeMedia(CoreNode):
+class BigLaMa(CoreNode):
     """
-    Transcribe speech in an audio or video file.
+    Inpaint a mask using [LaMa](https://github.com/advimman/lama).
 
-    https://substrate.run/library#TranscribeMedia
+    https://substrate.run/library#BigLaMa
     """
 
-    def __init__(self, args: TranscribeMediaIn):
+    def __init__(self, args: BigLaMaIn):
         """
-        Input arguments: `audio_uri`, `prompt` (optional), `language` (optional), `segment` (optional), `align` (optional), `diarize` (optional), `suggest_chapters` (optional)
+        Input arguments: `image_uri`, `mask_image_uri`, `store` (optional)
 
-        Output fields: `future.text`, `future.segments` (optional), `future.chapters` (optional)
+        Output fields: `future.image_uri`
 
-        https://substrate.run/library#TranscribeMedia
+        https://substrate.run/library#BigLaMa
         """
         super().__init__(**args)
-        self.node = "TranscribeMedia"
+        self.node = "BigLaMa"
 
-    def output(self, response: SubstrateResponse) -> TranscribeMediaOut:
+    def output(self, response: SubstrateResponse) -> BigLaMaOut:
         """
         Retrieve this node's output from a response.
 
-        Output fields: `future.text`, `future.segments` (optional), `future.chapters` (optional)
+        Output fields: `future.image_uri`
 
-        https://substrate.run/library#TranscribeMedia
+        https://substrate.run/library#BigLaMa
         """
-        klass = TranscribeMediaOut
+        klass = BigLaMaOut
         json = response.api_response.json
         if json and json.get("data"):
             data = json["data"]
             node_id = self.id
             if data.get(self.id):
                 return klass(**data[self.id])
         raise ValueError(f"Node {self.id} not found in response")
 
     @property
-    def future(self) -> FutureTranscribeMediaOut:  # type: ignore
+    def future(self) -> FutureBigLaMaOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.text`, `future.segments` (optional), `future.chapters` (optional)
+        Output fields: `future.image_uri`
 
-        https://substrate.run/library#TranscribeMedia
+        https://substrate.run/library#BigLaMa
         """
         return super().future  # type: ignore
 
 
-class GenerateSpeech(CoreNode):
+class RealESRGAN(CoreNode):
     """
-    Generate speech from text.
+    Upscale an image using [RealESRGAN](https://github.com/xinntao/Real-ESRGAN).
 
-    https://substrate.run/library#GenerateSpeech
+    https://substrate.run/library#RealESRGAN
     """
 
-    def __init__(self, args: GenerateSpeechIn):
+    def __init__(self, args: RealESRGANIn):
         """
-        Input arguments: `text`, `store` (optional), `node` (optional)
+        Input arguments: `image_uri`, `store` (optional)
 
-        Output fields: `future.audio_uri`
+        Output fields: `future.image_uri`
 
-        https://substrate.run/library#GenerateSpeech
+        https://substrate.run/library#RealESRGAN
         """
         super().__init__(**args)
-        self.node = "GenerateSpeech"
+        self.node = "RealESRGAN"
 
-    def output(self, response: SubstrateResponse) -> GenerateSpeechOut:
+    def output(self, response: SubstrateResponse) -> RealESRGANOut:
         """
         Retrieve this node's output from a response.
 
-        Output fields: `future.audio_uri`
+        Output fields: `future.image_uri`
 
-        https://substrate.run/library#GenerateSpeech
+        https://substrate.run/library#RealESRGAN
         """
-        klass = GenerateSpeechOut
+        klass = RealESRGANOut
         json = response.api_response.json
         if json and json.get("data"):
             data = json["data"]
             node_id = self.id
             if data.get(self.id):
                 return klass(**data[self.id])
         raise ValueError(f"Node {self.id} not found in response")
 
     @property
-    def future(self) -> FutureGenerateSpeechOut:  # type: ignore
+    def future(self) -> FutureRealESRGANOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.audio_uri`
+        Output fields: `future.image_uri`
 
-        https://substrate.run/library#GenerateSpeech
+        https://substrate.run/library#RealESRGAN
         """
         return super().future  # type: ignore
 
 
-class XTTSV2(CoreNode):
+class SegmentAnything(CoreNode):
     """
-    Generate speech from text using [XTTS v2](https://docs.coqui.ai/en/latest/models/xtts.html).
+    Segment an image using [SegmentAnything](https://github.com/facebookresearch/segment-anything).
 
-    https://substrate.run/library#XTTSV2
+    https://substrate.run/library#SegmentAnything
     """
 
-    def __init__(self, args: XTTSV2In):
+    def __init__(self, args: SegmentAnythingIn):
         """
-        Input arguments: `text`, `audio_uri` (optional), `language` (optional), `store` (optional)
+        Input arguments: `image_uri`, `point_prompts` (optional), `box_prompts` (optional), `store` (optional)
 
-        Output fields: `future.audio_uri`
+        Output fields: `future.mask_image_uri`
 
-        https://substrate.run/library#XTTSV2
+        https://substrate.run/library#SegmentAnything
         """
         super().__init__(**args)
-        self.node = "XTTSV2"
+        self.node = "SegmentAnything"
 
-    def output(self, response: SubstrateResponse) -> XTTSV2Out:
+    def output(self, response: SubstrateResponse) -> SegmentAnythingOut:
         """
         Retrieve this node's output from a response.
 
-        Output fields: `future.audio_uri`
+        Output fields: `future.mask_image_uri`
 
-        https://substrate.run/library#XTTSV2
+        https://substrate.run/library#SegmentAnything
         """
-        klass = XTTSV2Out
+        klass = SegmentAnythingOut
         json = response.api_response.json
         if json and json.get("data"):
             data = json["data"]
             node_id = self.id
             if data.get(self.id):
                 return klass(**data[self.id])
         raise ValueError(f"Node {self.id} not found in response")
 
     @property
-    def future(self) -> FutureXTTSV2Out:  # type: ignore
+    def future(self) -> FutureSegmentAnythingOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.audio_uri`
+        Output fields: `future.mask_image_uri`
 
-        https://substrate.run/library#XTTSV2
+        https://substrate.run/library#SegmentAnything
         """
         return super().future  # type: ignore
 
 
 class EmbedText(CoreNode):
     """
     Generate embedding for a text document.
@@ -1781,15 +1831,15 @@
     Query a vector store for similar vectors.
 
     https://substrate.run/library#QueryVectorStore
     """
 
     def __init__(self, args: QueryVectorStoreIn):
         """
-        Input arguments: `name`, `model`, `query_ids` (optional), `query_image_uris` (optional), `query_vectors` (optional), `query_strings` (optional), `top_k` (optional), `ef_search` (optional), `include_values` (optional), `include_metadata` (optional), `filters` (optional)
+        Input arguments: `name`, `model`, `query_ids` (optional), `query_image_uris` (optional), `query_vectors` (optional), `query_strings` (optional), `top_k` (optional), `ef_search` (optional), `include_values` (optional), `include_metadata` (optional), `filters` (optional), `metric` (optional)
 
         Output fields: `future.results`, `future.name` (optional), `future.model` (optional), `future.metric` (optional)
 
         https://substrate.run/library#QueryVectorStore
         """
         super().__init__(**args)
         self.node = "QueryVectorStore"
```

### Comparing `substrate-120240405.0.3/substrate/substrate.py` & `substrate-120240411.0.4/substrate/substrate.py`

 * *Files identical despite different names*

### Comparing `substrate-120240405.0.3/substrate/typeddict_models.py` & `substrate-120240411.0.4/substrate/typeddict_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,22 +16,26 @@
     """
     The type of error returned.
     """
     message: NotRequired[str]
     """
     A message providing more details about the error.
     """
+    request_id: NotRequired[str]
+    """
+    (Optional) A unique identifier for the request.
+    """
 
 
 class GenerateTextIn(TypedDict):
     prompt: NotRequired[str]
     """
     Input prompt.
     """
-    temperature: NotRequired[int]
+    temperature: NotRequired[float]
     """
     (Optional) Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: NotRequired[int]
     """
     (Optional) Maximum number of tokens to generate.
     """
@@ -53,15 +57,15 @@
     """
     Input prompt.
     """
     json_schema: NotRequired[Dict[str, Any]]
     """
     JSON schema to guide `json_object` response.
     """
-    temperature: NotRequired[int]
+    temperature: NotRequired[float]
     """
     (Optional) Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: NotRequired[int]
     """
     (Optional) Maximum number of tokens to generate.
     """
@@ -83,15 +87,15 @@
     """
     Input prompt.
     """
     num_choices: NotRequired[int]
     """
     Number of choices to generate.
     """
-    temperature: NotRequired[int]
+    temperature: NotRequired[float]
     """
     (Optional) Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: NotRequired[int]
     """
     (Optional) Maximum number of tokens to generate.
     """
@@ -99,14 +103,17 @@
     """
     (Optional) Selected node.
     """
 
 
 class MultiGenerateTextOut(TypedDict):
     choices: NotRequired[List[GenerateTextOut]]
+    """
+    Response choices.
+    """
 
 
 class MultiGenerateJSONIn(TypedDict):
     prompt: NotRequired[str]
     """
     Input prompt.
     """
@@ -114,15 +121,15 @@
     """
     JSON schema to guide `json_object` response.
     """
     num_choices: NotRequired[int]
     """
     Number of choices to generate.
     """
-    temperature: NotRequired[int]
+    temperature: NotRequired[float]
     """
     (Optional) Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: NotRequired[int]
     """
     (Optional) Maximum number of tokens to generate.
     """
@@ -130,14 +137,17 @@
     """
     (Optional) Selected node.
     """
 
 
 class MultiGenerateJSONOut(TypedDict):
     choices: NotRequired[List[GenerateJSONOut]]
+    """
+    Response choices.
+    """
 
 
 class Mistral7BInstructIn(TypedDict):
     prompt: NotRequired[str]
     """
     Input prompt.
     """
@@ -168,29 +178,28 @@
     """
     (Optional) JSON response, if `json_schema` was provided.
     """
 
 
 class Mistral7BInstructOut(TypedDict):
     choices: NotRequired[List[Mistral7BInstructChoice]]
+    """
+    Response choices.
+    """
 
 
 class GenerateTextVisionIn(TypedDict):
     prompt: NotRequired[str]
     """
     Text prompt.
     """
     image_uris: NotRequired[List[str]]
     """
     Image prompts.
     """
-    temperature: NotRequired[int]
-    """
-    (Optional) Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
-    """
     max_tokens: NotRequired[int]
     """
     (Optional) Maximum number of tokens to generate.
     """
     node: NotRequired[Literal["Firellava13B"]]
     """
     (Optional) Selected node.
@@ -209,18 +218,14 @@
     """
     Text prompt.
     """
     image_uris: NotRequired[List[str]]
     """
     Image prompts.
     """
-    temperature: NotRequired[float]
-    """
-    (Optional) Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
-    """
     max_tokens: NotRequired[int]
     """
     (Optional) Maximum number of tokens to generate.
     """
 
 
 class Firellava13BOut(TypedDict):
@@ -269,14 +274,17 @@
     """
     (Optional) Selected node.
     """
 
 
 class MultiGenerateImageOut(TypedDict):
     outputs: NotRequired[List[GenerateImageOut]]
+    """
+    Generated images.
+    """
 
 
 class StableDiffusionXLIn(TypedDict):
     prompt: NotRequired[str]
     """
     Text prompt.
     """
@@ -286,29 +294,29 @@
     """
     steps: NotRequired[int]
     """
     (Optional) Number of diffusion steps.
     """
     num_images: NotRequired[int]
     """
-    (Optional) Number of images to generate.
+    Number of images to generate.
     """
     store: NotRequired[str]
     """
     (Optional) Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
     height: NotRequired[int]
     """
     (Optional) Height of output image, in pixels.
     """
     width: NotRequired[int]
     """
     (Optional) Width of output image, in pixels.
     """
-    seeds: NotRequired[int]
+    seeds: NotRequired[List[int]]
     """
     (Optional) Seeds for deterministic generation. Default is a random seed.
     """
     guidance_scale: NotRequired[float]
     """
     (Optional) Higher values adhere to the text prompt more strongly, typically at the expense of image quality.
     """
@@ -323,14 +331,55 @@
     """
     The random noise seed used for generation.
     """
 
 
 class StableDiffusionXLOut(TypedDict):
     outputs: NotRequired[List[StableDiffusionImage]]
+    """
+    Generated images.
+    """
+
+
+class StableDiffusionXLLightningIn(TypedDict):
+    prompt: NotRequired[str]
+    """
+    Text prompt.
+    """
+    negative_prompt: NotRequired[str]
+    """
+    (Optional) Negative input prompt.
+    """
+    num_images: NotRequired[int]
+    """
+    (Optional) Number of images to generate.
+    """
+    store: NotRequired[str]
+    """
+    (Optional) Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    """
+    height: NotRequired[int]
+    """
+    (Optional) Height of output image, in pixels.
+    """
+    width: NotRequired[int]
+    """
+    (Optional) Width of output image, in pixels.
+    """
+    seeds: NotRequired[List[int]]
+    """
+    (Optional) Seeds for deterministic generation. Default is a random seed.
+    """
+
+
+class StableDiffusionXLLightningOut(TypedDict):
+    outputs: NotRequired[List[StableDiffusionImage]]
+    """
+    Generated images.
+    """
 
 
 class StableDiffusionXLIPAdapterIn(TypedDict):
     prompt: NotRequired[str]
     """
     Text prompt.
     """
@@ -366,14 +415,17 @@
     """
     (Optional) Random noise seeds. Default is random seeds for each generation.
     """
 
 
 class StableDiffusionXLIPAdapterOut(TypedDict):
     outputs: NotRequired[List[StableDiffusionImage]]
+    """
+    Generated images.
+    """
 
 
 class StableDiffusionXLControlNetIn(TypedDict):
     image_uri: NotRequired[str]
     """
     Input image.
     """
@@ -409,14 +461,17 @@
     """
     (Optional) Random noise seeds. Default is random seeds for each generation.
     """
 
 
 class StableDiffusionXLControlNetOut(TypedDict):
     outputs: NotRequired[List[StableDiffusionImage]]
+    """
+    Generated images.
+    """
 
 
 class GenerativeEditImageIn(TypedDict):
     image_uri: NotRequired[str]
     """
     Original image.
     """
@@ -470,14 +525,17 @@
     """
     (Optional) Selected node.
     """
 
 
 class MultiGenerativeEditImageOut(TypedDict):
     outputs: NotRequired[List[GenerativeEditImageOut]]
+    """
+    Generated images.
+    """
 
 
 class StableDiffusionXLInpaintIn(TypedDict):
     image_uri: NotRequired[str]
     """
     Original image.
     """
@@ -513,14 +571,17 @@
     """
     (Optional) Random noise seeds. Default is random seeds for each generation.
     """
 
 
 class StableDiffusionXLInpaintOut(TypedDict):
     outputs: NotRequired[List[StableDiffusionImage]]
+    """
+    Generated images.
+    """
 
 
 class BoundingBox(TypedDict):
     x1: NotRequired[float]
     """
     Top left corner x.
     """
@@ -628,22 +689,14 @@
 
 
 class DISISNetIn(TypedDict):
     image_uri: NotRequired[str]
     """
     Input image.
     """
-    return_mask: NotRequired[bool]
-    """
-    (Optional) Return a mask image instead of the original content.
-    """
-    background_color: NotRequired[str]
-    """
-    (Optional) Hex value background color. Transparent if unset.
-    """
     store: NotRequired[str]
     """
     (Optional) Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 class DISISNetOut(TypedDict):
@@ -676,18 +729,14 @@
 
 
 class RealESRGANIn(TypedDict):
     image_uri: NotRequired[str]
     """
     Input image.
     """
-    model: NotRequired[Literal["real-esrgan-x4"]]
-    """
-    (Optional) Selected model.
-    """
     store: NotRequired[str]
     """
     (Optional) Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 class RealESRGANOut(TypedDict):
@@ -1328,14 +1377,18 @@
     """
     (Optional) Include the metadata of the vectors in the response.
     """
     filters: NotRequired[Dict[str, Any]]
     """
     (Optional) Filter metadata by key-value pairs.
     """
+    metric: NotRequired[Literal["cosine", "l2", "inner"]]
+    """
+    (Optional) The distance metric used for the query. Defaults to the distance metric the vector store was created with.
+    """
 
 
 class VectorStoreQueryResult(TypedDict):
     id: NotRequired[str]
     """
     Document ID.
     """
```

### Comparing `substrate-120240405.0.3/PKG-INFO` & `substrate-120240411.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrate
-Version: 120240405.0.3
+Version: 120240411.0.4
 Summary: Substrate Python SDK
 Author: vprtwn
 Author-email: ben@substrate.run
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


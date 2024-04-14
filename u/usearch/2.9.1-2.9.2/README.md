# Comparing `tmp/usearch-2.9.1-cp39-cp39-win_amd64.whl.zip` & `tmp/usearch-2.9.2-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 257604 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat      375 b- defN 24-Feb-27 01:38 usearch/__init__.py
--rw-rw-rw-  2.0 fat     4241 b- defN 24-Feb-27 01:38 usearch/client.py
--rw-rw-rw-  2.0 fat   544256 b- defN 24-Feb-27 01:39 usearch/compiled.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    15244 b- defN 24-Feb-27 01:38 usearch/eval.py
--rw-rw-rw-  2.0 fat    49575 b- defN 24-Feb-27 01:38 usearch/index.py
--rw-rw-rw-  2.0 fat     3274 b- defN 24-Feb-27 01:38 usearch/io.py
--rw-rw-rw-  2.0 fat     4100 b- defN 24-Feb-27 01:38 usearch/numba.py
--rw-rw-rw-  2.0 fat     3858 b- defN 24-Feb-27 01:38 usearch/server.py
--rw-rw-rw-  2.0 fat    11558 b- defN 24-Feb-27 01:39 usearch-2.9.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    27122 b- defN 24-Feb-27 01:39 usearch-2.9.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Feb-27 01:39 usearch-2.9.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-Feb-27 01:39 usearch-2.9.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      995 b- defN 24-Feb-27 01:39 usearch-2.9.1.dist-info/RECORD
-13 files, 664706 bytes uncompressed, 255980 bytes compressed:  61.5%
+Zip file size: 257883 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat      398 b- defN 24-Mar-05 00:41 usearch/__init__.py
+-rw-rw-rw-  2.0 fat     4241 b- defN 24-Mar-05 00:41 usearch/client.py
+-rw-rw-rw-  2.0 fat   545280 b- defN 24-Mar-05 00:43 usearch/compiled.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    15244 b- defN 24-Mar-05 00:41 usearch/eval.py
+-rw-rw-rw-  2.0 fat    49620 b- defN 24-Mar-05 00:41 usearch/index.py
+-rw-rw-rw-  2.0 fat     3274 b- defN 24-Mar-05 00:41 usearch/io.py
+-rw-rw-rw-  2.0 fat     4100 b- defN 24-Mar-05 00:41 usearch/numba.py
+-rw-rw-rw-  2.0 fat     3858 b- defN 24-Mar-05 00:41 usearch/server.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 24-Mar-05 00:43 usearch-2.9.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    26879 b- defN 24-Mar-05 00:43 usearch-2.9.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-Mar-05 00:43 usearch-2.9.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Mar-05 00:43 usearch-2.9.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      995 b- defN 24-Mar-05 00:43 usearch-2.9.2.dist-info/RECORD
+13 files, 665555 bytes uncompressed, 256259 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: usearch/numba.py
 Comment: 
 
 Filename: usearch/server.py
 Comment: 
 
-Filename: usearch-2.9.1.dist-info/LICENSE
+Filename: usearch-2.9.2.dist-info/LICENSE
 Comment: 
 
-Filename: usearch-2.9.1.dist-info/METADATA
+Filename: usearch-2.9.2.dist-info/METADATA
 Comment: 
 
-Filename: usearch-2.9.1.dist-info/WHEEL
+Filename: usearch-2.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: usearch-2.9.1.dist-info/top_level.txt
+Filename: usearch-2.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: usearch-2.9.1.dist-info/RECORD
+Filename: usearch-2.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## usearch/__init__.py

```diff
@@ -1,8 +1,9 @@
 import importlib
+import importlib.util
 
 from usearch.compiled import (
     VERSION_MAJOR,
     VERSION_MINOR,
     VERSION_PATCH,
 )
```

## usearch/index.py

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 from inspect import signature
+from collections.abc import Sequence
 
 # The purpose of this file is to provide Pythonic wrapper on top
 # the native precompiled CPython module. It improves compatibility
 # Python tooling, linters, and static analyzers. It also embeds JIT
 # into the primary `Index` class, connecting USearch with Numba.
 import os
 import math
@@ -309,15 +310,15 @@
         return [(int(l), float(d)) for l, d in zip(self.keys, self.distances)]
 
     def __repr__(self) -> str:
         return f"usearch.Matches({len(self)})"
 
 
 @dataclass
-class BatchMatches:
+class BatchMatches(Sequence):
     """This class contains information about multiple retrieved vectors for multiple queries,
     i.e it is a set of `Matches` instances."""
 
     keys: np.ndarray
     distances: np.ndarray
     counts: np.ndarray
 
@@ -418,15 +419,15 @@
             for j_key in keys[:i]:
                 d = self.index.pairwise_distance(i_key, j_key)
                 g.add_edge(i_key, j_key, distance=d)
 
         return g
 
 
-class IndexedKeys:
+class IndexedKeys(Sequence):
     """Smart-reference for the range of keys present in a specific `Index`"""
 
     def __init__(self, index: Index) -> None:
         self.index = index
 
     def __len__(self) -> int:
         return len(self.index)
@@ -1132,15 +1133,15 @@
 
     @property
     def keys(self) -> IndexedKeys:
         return IndexedKeys(self)
 
     @property
     def vectors(self) -> np.ndarray:
-        return self.get(self.keys, vstack=True)
+        return self.get(self.keys)
 
     @property
     def max_level(self) -> int:
         return self._compiled.max_level
 
     @property
     def nlevels(self) -> int:
```

## Comparing `usearch-2.9.1.dist-info/LICENSE` & `usearch-2.9.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `usearch-2.9.1.dist-info/METADATA` & `usearch-2.9.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usearch
-Version: 2.9.1
+Version: 2.9.2
 Summary: Smaller & Faster Single-File Vector Search Engine from Unum
 Author: Ash Vardanian
 Author-email: info@unum.cloud
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -57,46 +57,43 @@
 <a href="https://unum-cloud.github.io/usearch/java">Java</a> •
 <a href="https://unum-cloud.github.io/usearch/rust">Rust</a> •
 <a href="https://unum-cloud.github.io/usearch/c">C 99</a> •
 <a href="https://unum-cloud.github.io/usearch/objective-c">Objective-C</a> •
 <a href="https://unum-cloud.github.io/usearch/swift">Swift</a> •
 <a href="https://unum-cloud.github.io/usearch/csharp">C#</a> •
 <a href="https://unum-cloud.github.io/usearch/golang">GoLang</a> •
-<a href="https://unum-cloud.github.io/usearch/wolfram">Wolfram</a> •
-<a href="https://unum-cloud.github.io/usearch/sqlite">SQLite3</a>
+<a href="https://unum-cloud.github.io/usearch/wolfram">Wolfram</a>
 <br/>
-Linux • MacOS • Windows • iOS • WebAssembly
+Linux • MacOS • Windows • iOS • WebAssembly •
+<a href="https://unum-cloud.github.io/usearch/sqlite">SQLite3</a>
 </p>
 
 <div align="center">
-<a href="https://pepy.tech/project/usearch"> <img alt="PyPI" src="https://static.pepy.tech/personalized-badge/usearch?period=total&units=abbreviation&left_color=black&right_color=blue&left_text=USearch%20Python%20installs"> </a>
-<a href="https://www.npmjs.com/package/usearch"> <img alt="NPM" src="https://img.shields.io/npm/dy/usearch?label=NPM%20installs"> </a>
-<a href="https://crates.io/crates/usearch"> <img alt="Crate" src="https://img.shields.io/crates/d/usearch?label=Crate%20installs"> </a>
-<a href="https://www.nuget.org/packages/Cloud.Unum.USearch"> <img alt="NuGet" src="https://img.shields.io/nuget/dt/Cloud.Unum.USearch?label=NuGet%20installs"> </a>
-<a href="https://central.sonatype.com/artifact/cloud.unum/usearch/overview"> <img alt="Maven" src="https://img.shields.io/nexus/r/cloud.unum/usearch?server=https%3A%2F%2Fs01.oss.sonatype.org%2F&label=Maven%20version"> </a>
-<a href="https://hub.docker.com/r/unum/usearch"> <img alt="Docker" src="https://img.shields.io/docker/pulls/unum/usearch?label=Docker%20installs"> </a>
+<a href="https://pepy.tech/project/usearch"> <img alt="PyPI" src="https://static.pepy.tech/personalized-badge/usearch?period=total&units=abbreviation&left_color=black&right_color=blue&left_text=Python%20PyPi%20installs"> </a>
+<a href="https://www.npmjs.com/package/usearch"> <img alt="NPM" src="https://img.shields.io/npm/dy/usearch?label=JavaScript%20NPM%20installs"> </a>
+<a href="https://crates.io/crates/usearch"> <img alt="Crate" src="https://img.shields.io/crates/d/usearch?label=Rust%20Crate%20installs"> </a>
+<a href="https://www.nuget.org/packages/Cloud.Unum.USearch"> <img alt="NuGet" src="https://img.shields.io/nuget/dt/Cloud.Unum.USearch?label=CSharp%20NuGet%20installs"> </a>
+<a href="https://central.sonatype.com/artifact/cloud.unum/usearch/overview"> <img alt="Maven" src="https://img.shields.io/nexus/r/cloud.unum/usearch?server=https%3A%2F%2Fs01.oss.sonatype.org%2F&label=Java%20Maven%20version"> </a>
 <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/unum-cloud/usearch?label=Repo%20size">
 </div>
 
 ---
 
 - ✅ __[10x faster][faster-than-faiss]__ [HNSW][hnsw-algorithm] implementation than [FAISS][faiss].
 - ✅ Simple and extensible [single C++11 header][usearch-header] __library__.
-- ✅ Compatible with a dozen programming languages out of the box.
 - ✅ [Trusted](#integrations) by giants like Google and databases like [ClickHouse][clickhouse-docs].
 - ✅ [SIMD][simd]-optimized and [user-defined metrics](#user-defined-functions) with JIT compilation.
 - ✅ Hardware-agnostic `f16` & `i8` - [half-precision & quarter-precision support](#memory-efficiency-downcasting-and-quantization).
 - ✅ [View large indexes from disk](#serving-index-from-disk) without loading into RAM.
 - ✅ Heterogeneous lookups, renaming/relabeling, and on-the-fly deletions.
-- ✅ Variable dimensionality vectors for unique applications, including search over compressed data.
 - ✅ Binary Tanimoto and Sorensen coefficients for [Genomics and Chemistry applications](#usearch--rdkit--molecular-search).
 - ✅ Space-efficient point-clouds with `uint40_t`, accommodating 4B+ size.
-- ✅ Compatible with OpenMP and custom "executors" for fine-grained control over CPU utilization.
-- ✅ Near-real-time [clustering and sub-clustering](#clustering) for Tens or Millions of clusters.
+- ✅ Compatible with OpenMP and custom "executors" for fine-grained parallelism.
 - ✅ [Semantic Search](#usearch--ai--multi-modal-semantic-search) and [Joins](#joins-one-to-one-one-to-many-and-many-to-many-mappings).
+- 🔄 Near-real-time [clustering and sub-clustering](#clustering) for Tens or Millions of clusters.
 
 [faiss]: https://github.com/facebookresearch/faiss
 [usearch-header]: https://github.com/unum-cloud/usearch/blob/main/include/usearch/index.hpp
 [obscure-use-cases]: https://ashvardanian.com/posts/abusing-vector-search
 [hnsw-algorithm]: https://arxiv.org/abs/1603.09320
 [simd]: https://en.wikipedia.org/wiki/Single_instruction,_multiple_data
 [faster-than-faiss]: https://www.unum.cloud/blog/2023-11-07-scaling-vector-search-with-intel
@@ -160,15 +157,15 @@
 vector = np.array([0.2, 0.6, 0.4])
 index.add(42, vector)
 
 matches = index.search(vector, 10)
 
 assert matches[0].key == 42
 assert matches[0].distance <= 0.001
-assert np.allclose(index[42], vector)
+assert np.allclose(index[42], vector, atol=0.1) # Ensure high tolerance in mixed-precision comparisons
 ```
 
 More settings are always available, and the API is designed to be as flexible as possible.
 
 ```py
 index = Index(
     ndim=3, # Define the number of dimensions in input vectors
@@ -461,12 +458,12 @@
 
 ```txt
 @software{Vardanian_USearch_2023,
 doi = {10.5281/zenodo.7949416},
 author = {Vardanian, Ash},
 title = {{USearch by Unum Cloud}},
 url = {https://github.com/unum-cloud/usearch},
-version = {2.9.1},
+version = {2.9.2},
 year = {2023},
 month = oct,
 }
 ```
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: usearch Version: 2.9.1 Summary: Smaller & Faster
+Metadata-Version: 2.1 Name: usearch Version: 2.9.2 Summary: Smaller & Faster
 Single-File Vector Search Engine from Unum Author: Ash Vardanian Author-email:
 info@unum.cloud License: Apache-2.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Natural Language :: English Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: C++ Classifier: Programming Language :: Python :: 3 ::
 Only Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -18,39 +18,37 @@
                              ************ UUSSeeaarrcchh ************
                        ******** SSmmaalllleerr && _FF_aa_ss_tt_ee_rr SSiinnggllee--FFiillee
             SSiimmiillaarriittyy SSeeaarrcchh EEnnggiinnee ffoorr _VV_ee_cc_tt_oo_rr_ss && ?ð??? _TT_ee_xx_tt_ss ********
 
            _[_D_i_s_c_o_r_d_]    _[_L_i_n_k_e_d_I_n_]    _[_T_w_i_t_t_e_r_]    _[_B_l_o_g_]   _[_G_i_t_H_u_b_]
         Spatial â¢ Binary â¢ Probabilistic â¢ User-Defined Metrics
  _C_+_+_ _1_1 â¢ _P_y_t_h_o_n_ _3 â¢ _J_a_v_a_S_c_r_i_p_t â¢ _J_a_v_a â¢ _R_u_s_t â¢ _C_ _9_9 â¢ _O_b_j_e_c_t_i_v_e_-
-            _C â¢ _S_w_i_f_t â¢ _C_# â¢ _G_o_L_a_n_g â¢ _W_o_l_f_r_a_m â¢ _S_Q_L_i_t_e_3
-              Linux â¢ MacOS â¢ Windows â¢ iOS â¢ WebAssembly
-      _[_P_y_P_I_]_[_N_P_M_]_[_C_r_a_t_e_]_[_N_u_G_e_t_]_[_M_a_v_e_n_]_[_D_o_c_k_e_r_][GitHub code size in bytes]
+                  _C â¢ _S_w_i_f_t â¢ _C_# â¢ _G_o_L_a_n_g â¢ _W_o_l_f_r_a_m
+        Linux â¢ MacOS â¢ Windows â¢ iOS â¢ WebAssembly â¢ _S_Q_L_i_t_e_3
+          _[_P_y_P_I_]_[_N_P_M_]_[_C_r_a_t_e_]_[_N_u_G_e_t_]_[_M_a_v_e_n_][GitHub code size in bytes]
 --- - â __[10x faster][faster-than-faiss]__ [HNSW][hnsw-algorithm]
 implementation than [FAISS][faiss]. - â Simple and extensible [single C++11
-header][usearch-header] __library__. - â Compatible with a dozen programming
-languages out of the box. - â [Trusted](#integrations) by giants like Google
-and databases like [ClickHouse][clickhouse-docs]. - â [SIMD][simd]-optimized
-and [user-defined metrics](#user-defined-functions) with JIT compilation. - â
-Hardware-agnostic `f16` & `i8` - [half-precision & quarter-precision support]
-(#memory-efficiency-downcasting-and-quantization). - â [View large indexes
-from disk](#serving-index-from-disk) without loading into RAM. - â
-Heterogeneous lookups, renaming/relabeling, and on-the-fly deletions. - â
-Variable dimensionality vectors for unique applications, including search over
-compressed data. - â Binary Tanimoto and Sorensen coefficients for [Genomics
-and Chemistry applications](#usearch--rdkit--molecular-search). - â Space-
+header][usearch-header] __library__. - â [Trusted](#integrations) by giants
+like Google and databases like [ClickHouse][clickhouse-docs]. - â [SIMD]
+[simd]-optimized and [user-defined metrics](#user-defined-functions) with JIT
+compilation. - â Hardware-agnostic `f16` & `i8` - [half-precision & quarter-
+precision support](#memory-efficiency-downcasting-and-quantization). - â
+[View large indexes from disk](#serving-index-from-disk) without loading into
+RAM. - â Heterogeneous lookups, renaming/relabeling, and on-the-fly
+deletions. - â Binary Tanimoto and Sorensen coefficients for [Genomics and
+Chemistry applications](#usearch--rdkit--molecular-search). - â Space-
 efficient point-clouds with `uint40_t`, accommodating 4B+ size. - â
-Compatible with OpenMP and custom "executors" for fine-grained control over CPU
-utilization. - â Near-real-time [clustering and sub-clustering](#clustering)
-for Tens or Millions of clusters. - â [Semantic Search](#usearch--ai--multi-
-modal-semantic-search) and [Joins](#joins-one-to-one-one-to-many-and-many-to-
-many-mappings). [faiss]: https://github.com/facebookresearch/faiss [usearch-
-header]: https://github.com/unum-cloud/usearch/blob/main/include/usearch/
-index.hpp [obscure-use-cases]: https://ashvardanian.com/posts/abusing-vector-
-search [hnsw-algorithm]: https://arxiv.org/abs/1603.09320 [simd]: https://
+Compatible with OpenMP and custom "executors" for fine-grained parallelism. -
+â [Semantic Search](#usearch--ai--multi-modal-semantic-search) and [Joins]
+(#joins-one-to-one-one-to-many-and-many-to-many-mappings). - ð Near-real-
+time [clustering and sub-clustering](#clustering) for Tens or Millions of
+clusters. [faiss]: https://github.com/facebookresearch/faiss [usearch-header]:
+https://github.com/unum-cloud/usearch/blob/main/include/usearch/index.hpp
+[obscure-use-cases]: https://ashvardanian.com/posts/abusing-vector-search
+[hnsw-algorithm]: https://arxiv.org/abs/1603.09320 [simd]: https://
 en.wikipedia.org/wiki/Single_instruction,_multiple_data [faster-than-faiss]:
 https://www.unum.cloud/blog/2023-11-07-scaling-vector-search-with-intel
 [clickhouse-docs]: https://clickhouse.com/docs/en/engines/table-engines/
 mergetree-family/annindexes#usearch __Technical Insights__ and related
 articles: - [Uses Horner's method for polynomial approximations, beating GCC 12
 by 119x](https://ashvardanian.com/posts/gcc-12-vs-avx512fp16/). - [Uses Arm SVE
 and x86 AVX-512's masked loads to eliminate tail `for`-loops](https://
@@ -100,23 +98,24 @@
 deployments faster. [intel-benchmarks]: https://www.unum.cloud/blog/2023-11-07-
 scaling-vector-search-with-intel Base functionality is identical to FAISS, and
 the interface must be familiar if you have ever investigated Approximate
 Nearest Neighbors search: ```py $ pip install numpy usearch import numpy as np
 from usearch.index import Index index = Index(ndim=3) vector = np.array([0.2,
 0.6, 0.4]) index.add(42, vector) matches = index.search(vector, 10) assert
 matches[0].key == 42 assert matches[0].distance <= 0.001 assert np.allclose
-(index[42], vector) ``` More settings are always available, and the API is
-designed to be as flexible as possible. ```py index = Index( ndim=3, # Define
-the number of dimensions in input vectors metric='cos', # Choose 'l2sq',
-'haversine' or other metric, default = 'ip' dtype='f32', # Quantize to 'f16' or
-'i8' if needed, default = 'f32' connectivity=16, # Optional: Limit number of
-neighbors per graph node expansion_add=128, # Optional: Control the recall of
-indexing expansion_search=64, # Optional: Control the quality of the search
-multi=False, # Optional: Allow multiple vectors per key, default = False ) ```
-## Serialization & Serving `Index` from Disk USearch supports multiple forms of
+(index[42], vector, atol=0.1) # Ensure high tolerance in mixed-precision
+comparisons ``` More settings are always available, and the API is designed to
+be as flexible as possible. ```py index = Index( ndim=3, # Define the number of
+dimensions in input vectors metric='cos', # Choose 'l2sq', 'haversine' or other
+metric, default = 'ip' dtype='f32', # Quantize to 'f16' or 'i8' if needed,
+default = 'f32' connectivity=16, # Optional: Limit number of neighbors per
+graph node expansion_add=128, # Optional: Control the recall of indexing
+expansion_search=64, # Optional: Control the quality of the search multi=False,
+# Optional: Allow multiple vectors per key, default = False ) ``` ##
+Serialization & Serving `Index` from Disk USearch supports multiple forms of
 serialization: - Into a __file__ defined with a path. - Into a __stream__
 defined with a callback, serializing or reconstructing incrementally. - Into a
 __buffer__ of fixed length or a memory-mapped file that supports random access.
 The latter allows you to serve indexes from external memory, enabling you to
 optimize your server choices for indexing speed and serving costs. This can
 result in __20x cost reduction__ on AWS and other public clouds. ```py
 index.save("index.usearch") loaded_copy = index.load("index.usearch") view =
@@ -292,8 +291,8 @@
 langchainjs/releases/tag/0.0.125). - [x] ClickHouse: [C++](https://github.com/
 ClickHouse/ClickHouse/pull/53447). - [x] Microsoft Semantic Kernel: [Python]
 (https://github.com/microsoft/semantic-kernel/releases/tag/python-0.3.9.dev)
 and C#. - [x] LanternDB: [C++](https://github.com/lanterndata/lantern) and
 [Rust](https://github.com/lanterndata/lantern_extras). ## Citations ```txt
 @software{Vardanian_USearch_2023, doi = {10.5281/zenodo.7949416}, author =
 {Vardanian, Ash}, title = {{USearch by Unum Cloud}}, url = {https://github.com/
-unum-cloud/usearch}, version = {2.9.1}, year = {2023}, month = oct, } ```
+unum-cloud/usearch}, version = {2.9.2}, year = {2023}, month = oct, } ```
```


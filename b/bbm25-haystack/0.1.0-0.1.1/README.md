# Comparing `tmp/bbm25_haystack-0.1.0.tar.gz` & `tmp/bbm25_haystack-0.1.1.tar.gz`

## Comparing `bbm25_haystack-0.1.0.tar` & `bbm25_haystack-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.0/src/bbm25_haystack/__about__.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.0/src/bbm25_haystack/__init__.py
--rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.0/src/bbm25_haystack/bbm25_retriever.py
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.0/src/bbm25_haystack/bbm25_store.py
--rw-r--r--   0        0        0   253165 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.0/src/bbm25_haystack/default.model
--rw-r--r--   0        0        0     8498 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.0/src/bbm25_haystack/filters.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     5835 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.0/tests/test_document_store.py
--rw-r--r--   0        0        0     7333 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.0/tests/test_retriever.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.0/LICENSE
--rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.0/README.md
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.1/benchmarks/.gitkeep
+-rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.1/scripts/benchmark_beir.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.1/src/bbm25_haystack/__about__.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.1/src/bbm25_haystack/__init__.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.1/src/bbm25_haystack/bbm25_retriever.py
+-rw-r--r--   0        0        0    11314 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.1/src/bbm25_haystack/bbm25_store.py
+-rw-r--r--   0        0        0   499723 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.1/src/bbm25_haystack/default.model
+-rw-r--r--   0        0        0     8512 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.1/src/bbm25_haystack/filters.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.1/tests/test_document_store.py
+-rw-r--r--   0        0        0     7523 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.1/tests/test_retriever.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.1/README.md
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.1/PKG-INFO
```

### Comparing `bbm25_haystack-0.1.0/.github/workflows/test.yml` & `bbm25_haystack-0.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.1.0/src/bbm25_haystack/bbm25_retriever.py` & `bbm25_haystack-0.1.1/src/bbm25_haystack/bbm25_retriever.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,20 +52,22 @@
         *,
         filters: Optional[dict[str, Any]] = None,
         top_k: int = 10,
     ):
         """
         Create an BetterBM25Retriever component.
 
-        :param document_store: A Document Store object used to retrieve documents
+        :param document_store: A Document Store object used to
+            retrieve documents
         :type document_store: BetterBM25DocumentStore
-        :param filters: A dictionary with filters to narrow down the search space
-            (default is None).
+        :param filters: A dictionary with filters to narrow down the
+            search space (default is None).
         :type filters: Optional[dict[str, Any]]
-        :param top_k: The maximum number of documents to retrieve (default is 10).
+        :param top_k: The maximum number of documents to retrieve
+            (default is 10).
         :type top_k: int
 
         :raises ValueError: If the specified top_k is not > 0.
         """
         _validate_search_params(filters, top_k)
 
         self.filters = filters
@@ -84,28 +86,29 @@
         top_k: Optional[int] = None,
     ) -> dict[str, list[Document]]:
         """
         Run the Retriever on the given query.
 
         :param query: The query to run the Retriever on.
         :type query: str
-        :param filters: A dictionary with filters to narrow down the search space
-            (default is None).
+        :param filters: A dictionary with filters to narrow
+            down the search space (default is None).
         :type filters: Optional[dict[str, Any]]
-        :param top_k: The maximum number of documents to retrieve (default is None).
+        :param top_k: The maximum number of documents to
+            retrieve (default is None).
 
         :return: The retrieved documents.
         """
         filters = filters or self.filters
         top_k = top_k or self.top_k
 
         _validate_search_params(filters, top_k)
 
-        docs = self.document_store._retrieval(query, filters=filters, top_k=top_k)
-        return {"documents": docs}
+        sim = self.document_store._retrieval(query, filters=filters, top_k=top_k)
+        return {"documents": next(zip(*sim))}  # type: ignore
 
     def to_dict(self) -> dict[str, Any]:
         """
         Serializes the component to a dictionary.
 
         :return: dictionary with serialized data.
         """
@@ -129,11 +132,11 @@
             msg = "Missing 'document_store' in serialization data"
             raise DeserializationError(msg)
 
         if doc_store_params.get("type") is None:
             msg = "Missing 'type' in document store's serialization data"
             raise DeserializationError(msg)
 
-        data["init_parameters"]["document_store"] = BetterBM25DocumentStore.from_dict(
-            doc_store_params
+        data["init_parameters"]["document_store"] = (
+            BetterBM25DocumentStore.from_dict(doc_store_params)
         )
         return default_from_dict(cls, data)
```

### Comparing `bbm25_haystack-0.1.0/src/bbm25_haystack/bbm25_store.py` & `bbm25_haystack-0.1.1/src/bbm25_haystack/bbm25_store.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,86 +1,99 @@
 # SPDX-FileCopyrightText: 2024-present Yuxuan Wang <wangy49@seas.upenn.edu>
 #
 # SPDX-License-Identifier: Apache-2.0
 import heapq
-import logging
 import math
 import os
 from collections import Counter
 from typing import Any, Final, Optional, Union
 
-from haystack import Document, default_from_dict, default_to_dict
+from haystack import Document, default_from_dict, default_to_dict, logging
 from haystack.document_stores.errors import (
     DuplicateDocumentError,
     MissingDocumentError,
 )
 from haystack.document_stores.types import DuplicatePolicy
+from haystack.utils.filters import document_matches_filter
 from sentencepiece import SentencePieceProcessor  # type: ignore
 
 from bbm25_haystack.filters import apply_filters_to_document
 
 logger = logging.getLogger(__name__)
 
 
-DEFAULT_SP_MODEL: Final = os.path.join(
-    os.path.dirname(os.path.abspath(__file__)), "default.model"
-)
-
-
 class BetterBM25DocumentStore:
     """
     An in-memory document store intended to improve the default BM25 document
     store shipped with Haystack.
     """
 
+    default_sp_file: Final = os.path.join(
+        os.path.dirname(os.path.abspath(__file__)), "default.model"
+    )
+
     def __init__(
         self,
         *,
         k: float = 1.5,
         b: float = 0.75,
         delta: float = 1.0,
         sp_file: Optional[str] = None,
-    ):
+        haystack_filter_logic: bool = True,
+    ) -> None:
         """
         Creates a new BetterBM25DocumentStore instance.
 
-        An in-memory document store intended to improve the default BM25 document
-        store shipped with Haystack. The default store recompute the index for the
-        entire document store for every in-coming query, which is significantly
-        inefficient. This store aims to improve the efficiency by pre-computing
-        the index for all documents in the store and only do incremental updates
-        when new documents are added or removed. Further, it leverages a
-        SentencePiece model to tokenize the input text to allow more flexible
-        and dynamic tokenization adapted to domain-specific text.
+        An in-memory document store intended to improve the default
+        BM25 document store shipped with Haystack. The default store
+        recompute the index for the entire document store for every
+        in-coming query, which is significantly inefficient. This
+        store aims to improve the efficiency by pre-computing the
+        index for all documents in the store and only do incremental
+        updates when new documents are added or removed. Further, it
+        leverages a SentencePiece model to tokenize the input text
+        to allow more flexible and dynamic tokenization adapted to
+        domain-specific text.
 
         :param k: the k1 parameter in BM25+ formula.
         :type k: float, optional
         :param b: the b parameter in BM25+ formula.
         :type b: float, optional
         :param delta: the delta parameter in BM25+ formula.
         :type delta: float, optional
-        :param sp_file: the SentencePiece model file to use for tokenization.
+        :param sp_file: the SentencePiece model file to use for
+            tokenization.
         :type sp_file: Optional[str], optional
+        :param haystack_filter_logic: Whether to use the Haystack
+            filter logic or the one implemented in this store,
+            which is more conservative.
+        :type haystack_filter_logic: bool, optional
         """
         self.k = k
         self.b = b
 
         # Adjust the delta value so that we can bring the `(k1 + 1)`
         # term out of the 'term frequency' term in BM25+ formula and
         # delete it; this will not affect the ranking
         self.delta = delta / (self.k + 1.0)
 
         self._sp_file = sp_file
         self._sp_inst = SentencePieceProcessor(
-            model_file=(self._sp_file or DEFAULT_SP_MODEL)
+            model_file=(self._sp_file or self.default_sp_file)
+        )
+
+        self._haystack_filter_logic = haystack_filter_logic
+        self._filter_func = (
+            document_matches_filter
+            if self._haystack_filter_logic
+            else apply_filters_to_document
         )
 
         self._avg_doc_len: float = 0.0
         self._freq_doc: Counter = Counter()
-
         self._index: dict[str, tuple[Document, dict[str, int], int]] = {}
 
     def _tokenize(self, texts: Union[str, list[str]]) -> list[list[str]]:
         """
         Tokenize input text using SentencePiece model.
 
         The input text can either be a single string or a list of strings,
@@ -92,47 +105,32 @@
         :return: the tokenized text.
         :rtype: list[list[str]]
         """
         if isinstance(texts, str):
             texts = [texts]
         return self._sp_inst.encode(texts, out_type=str)
 
-    def _compute_damping(self, doc_len: int) -> float:
-        """The damping factor within the term-frequency component.
-
-        This damping factor controls how document length shrinks
-        the increment of term frequency. The longer the document,
-        the less the term frequency can increase final matching score.
-
-        :param doc_len: the number of tokens in a document.
-        :type doc_len: int
-
-        :return: the damping factor.
-        :rtype: float
-        """
-        return self.k * (1 - self.b + self.b * doc_len / self._avg_doc_len)
-
     def _compute_idf(self, tokens: list[str]) -> dict[str, float]:
         """
         Calculate the inverse document frequency for each token.
 
         :param tokens: the tokens to calculate the IDF for.
         :type tokens: list[str]
 
         :return: the IDF for each token.
         :rtype: dict[str, float]
         """
-        n = lambda t: self._freq_doc.get(t, 0)
+        cnt = lambda token: self._freq_doc.get(token, 0)
         idf = {
-            t: math.log(1 + (len(self._index) - n(t) + 0.5) / (n(t) + 0.5))
+            t: math.log(1 + (len(self._index) - cnt(t) + 0.5) / (cnt(t) + 0.5))
             for t in tokens
         }
         return idf
 
-    def _compute_all_bm25plus(
+    def _compute_bm25plus(
         self,
         idf: dict[str, float],
         documents: list[Document],
     ) -> list[tuple[Document, float]]:
         """
         Calculate the BM25+ score for all documents in this index.
 
@@ -140,68 +138,61 @@
         :type idf: dict[str, float]
         :param documents: the pool of documents to calculate the BM25+ score for.
         :type documents: list[Document]
 
         :return: the BM25+ scores for all documents.
         :rtype: list[tuple[Document, float]]
         """
+        sim = []
+        for doc in documents:
+            _, freq, doc_len = self._index[doc.id]
+            doc_len_scaled = doc_len / self._avg_doc_len
 
-        def bm25(token: str, freq: dict[str, int], doc_len: int) -> float:
-            """
-            Complete BM25+ formula for a single token.
-            """
-            damp = self._compute_damping(doc_len)  # Repeated compute here
-            freq_term = freq.get(token, 0.0)
-            freq_norm = freq_term / (freq_term + damp) + self.delta
-            return idf[token] * freq_norm
-
-        store = {doc.id: self._index[doc.id] for doc in documents}
-        scores = [
-            (
-                doc,
-                sum(bm25(token, freq, doc_len) for token in idf.keys()),
-            )
-            for doc, freq, doc_len in store.values()
-        ]
-        return scores
+            scr = 0.0
+            for token, idf_val in idf.items():
+                freq_term = freq.get(token, 0.0)
+                freq_damp = self.k * (1 + self.b * (doc_len_scaled - 1))
+
+                tf_val = freq_term / (freq_term + freq_damp) + self.delta
+                scr += idf_val * tf_val
+
+            sim.append((doc, scr))
+
+        return sim
 
     def _retrieval(
         self,
         query: str,
         *,
         filters: Optional[dict[str, Any]] = None,
         top_k: Optional[int] = None,
-    ) -> list[Document]:
+    ) -> list[tuple[Document, float]]:
         """
         Retrieve documents from the store using the given query.
 
         :param query: the query to search for.
         :type query: str
         :param filters: the filters to apply to the document list.
         :type filters: Optional[dict[str, Any]]
         :param top_k: the number of documents to return.
         :type top_k: int
 
-        :return: the top-k documents that match the query.
-        :rtype: list[Document]
+        :return: the top-k documents and corresponding sim score.
+        :rtype: list[tuple[Document, float]]
         """
         documents = self.filter_documents(filters)
         if not documents:
             return []
 
         idf = self._compute_idf(self._tokenize(query)[0])
-        sim = self._compute_all_bm25plus(idf, documents)
+        sim = self._compute_bm25plus(idf, documents)
 
-        key = lambda x: x[1]
         if top_k is None:
-            top = sorted(sim, key=key, reverse=True)
-        else:
-            top = heapq.nlargest(top_k, sim, key=key)
-
-        return next(zip(*top))  # type: ignore
+            return sorted(sim, key=lambda x: x[1], reverse=True)
+        return heapq.nlargest(top_k, sim, key=lambda x: x[1])
 
     def count_documents(self) -> int:
         """
         Returns how many documents are present in the document store.
 
         :return: the number of documents in the store.
         :rtype: int
@@ -216,39 +207,41 @@
 
         :param filters: the filters to apply to the document list.
         :type filters: Optional[dict[str, Any]]
 
         :return: the list of documents that match the given filters.
         :rtype: list[Document]
         """
+        if filters is None or not filters:
+            return [doc for doc, _, _ in self._index.values()]
         return [
             doc
             for doc, _, _ in self._index.values()
-            if apply_filters_to_document(filters, doc)
+            if self._filter_func(filters, doc)
         ]
 
     def write_documents(
         self,
         documents: list[Document],
         policy: DuplicatePolicy = DuplicatePolicy.FAIL,
     ) -> int:
         """
         Writes (or overwrites) documents into the store.
 
         :param documents: a list of documents.
         :type documents: list[Document]
-        :param policy: documents with the same ID count as duplicates. When
-            duplicates are met, the store can:
+        :param policy: documents with the same ID count as duplicates.
+            When duplicates are met, the store can:
              - skip: keep the existing document and ignore the new one.
              - overwrite: remove the old document and write the new one.
              - fail: an error is raised
         :type policy: DuplicatePolicy, optional
 
-        :raises DuplicateDocumentError: Exception trigger on duplicate document if
-            `policy=DuplicatePolicy.FAIL`
+        :raises DuplicateDocumentError: Exception trigger on duplicate
+            document if `policy=DuplicatePolicy.FAIL`
 
         :return: Number of documents written.
         :rtype: int
         """
         n_written = 0
         for doc in documents:
             if not isinstance(doc, Document):
@@ -268,34 +261,34 @@
                 )
                 self.delete_documents([doc.id])
 
             tokens = self._tokenize(doc.content or "")[0]
 
             self._index[doc.id] = (doc, Counter(tokens), len(tokens))
             self._freq_doc.update(set(tokens))
-            self._avg_doc_len = (len(tokens) + self._avg_doc_len * len(self._index)) / (
-                len(self._index) + 1
-            )
+            self._avg_doc_len = (
+                len(tokens) + self._avg_doc_len * len(self._index)
+            ) / (len(self._index) + 1)
 
             logger.debug(f"Document '{doc.id}' written to store.")
             n_written += 1
 
         return n_written
 
     def delete_documents(self, document_ids: list[str]) -> int:
         """
-        Deletes all documents with a matching document_ids from the document store.
+        Deletes all documents with a matching document_ids.
 
-        Fails with `MissingDocumentError` if no document with this id is present in
-        the store.
+        Fails with `MissingDocumentError` if no document with
+        this id is present in the store.
 
         :param object_ids: the object_ids to delete
         :type object_ids: list[str]
 
-        :raises MissingDocumentError: Exception trigger on missing document.
+        :raises MissingDocumentError: trigger on missing document.
 
         :return: Number of documents deleted.
         :rtype: int
         """
         n_removal = 0
         for doc_id in document_ids:
             try:
@@ -320,13 +313,14 @@
         """Serializes this store to a dictionary."""
         return default_to_dict(
             self,
             k=self.k,
             b=self.b,
             delta=self.delta,
             sp_file=self._sp_file,
+            haystack_filter_logic=self._haystack_filter_logic,
         )
 
     @classmethod
     def from_dict(cls, data: dict[str, Any]) -> "BetterBM25DocumentStore":
         """Deserializes the store from a dictionary."""
         return default_from_dict(cls, data)
```

### Comparing `bbm25_haystack-0.1.0/src/bbm25_haystack/filters.py` & `bbm25_haystack-0.1.1/src/bbm25_haystack/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,17 @@
     :type document: Document
     :param conditions: The conditions to check against the document.
     :type conditions: list[dict[str, Any]]
 
     :return: True if not all conditions are met.
     :rtype: bool
     """
-    return all(_run_comparison_condition(condition, document) for condition in conditions)
+    return all(
+        _run_comparison_condition(condition, document) for condition in conditions
+    )
 
 
 def _or(document: Document, conditions: list[dict[str, Any]]) -> bool:
     """
     Return True if any condition is met.
 
     :param document: The document to check the conditions against.
```

### Comparing `bbm25_haystack-0.1.0/tests/test_document_store.py` & `bbm25_haystack-0.1.1/tests/test_document_store.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 class TestDocumentStore(DocumentStoreBaseTests):
     """Common test cases will be provided by `DocumentStoreBaseTests`."""
 
     @pytest.fixture
     def document_store(self) -> BetterBM25DocumentStore:
         return BetterBM25DocumentStore()
 
+    @pytest.fixture
+    def document_store_bbm25_filter(self) -> BetterBM25DocumentStore:
+        return BetterBM25DocumentStore(haystack_filter_logic=False)
+
     def test_write_documents(self, document_store: DocumentStore):
         docs = [Document(id="1")]
         assert document_store.write_documents(docs) == 1
         with pytest.raises(DuplicateDocumentError):
             document_store.write_documents(docs, DuplicatePolicy.FAIL)
 
         document_store.write_documents(
@@ -68,89 +72,91 @@
             Document(content="Haystack supports multiple languages"),
         ]
         document_store.write_documents(docs)
 
         results = document_store._retrieval(query="What languages?", top_k=1)
 
         assert len(results) == 1
-        assert results[0].content == "Haystack supports multiple languages"
+        assert results[0][0].content == "Haystack supports multiple languages"
 
     # Override a few filter test cases to account for new comparison logic
     # Specifically, we alter the expected behavior when comparison involves
     # None, DataFrame, and Iterables.
-    def test_comparison_equal_with_none(self, document_store, filterable_docs):
-        document_store.write_documents(filterable_docs)
-        result = document_store.filter_documents(
+    def test_comparison_equal_with_none_bbm25_filter(
+        self, document_store_bbm25_filter, filterable_docs
+    ):
+        document_store_bbm25_filter.write_documents(filterable_docs)
+        result = document_store_bbm25_filter.filter_documents(
             filters={"field": "meta.number", "operator": "==", "value": None}
         )
         self.assert_documents_are_equal(result, [])
 
-    def test_comparison_not_equal_with_none(self, document_store, filterable_docs):
-        document_store.write_documents(filterable_docs)
-        result = document_store.filter_documents(
+    def test_comparison_not_equal_with_none_bbm25_filter(
+        self, document_store_bbm25_filter, filterable_docs
+    ):
+        document_store_bbm25_filter.write_documents(filterable_docs)
+        result = document_store_bbm25_filter.filter_documents(
             filters={"field": "meta.number", "operator": "!=", "value": None}
         )
         self.assert_documents_are_equal(result, [])
 
-    def test_comparison_not_equal(self, document_store, filterable_docs):
-        """Comparison with missing values will always return False. So the ground
-        truth is that we should only return documents with a non-missing value."""
-        document_store.write_documents(filterable_docs)
-        result = document_store.filter_documents(
+    def test_comparison_not_equal_bbm25_filter(
+        self, document_store_bbm25_filter, filterable_docs
+    ):
+        """Comparison with missing values will always return False.
+        So the ground truth is that we should only return documents
+        with a non-missing value."""
+        document_store_bbm25_filter.write_documents(filterable_docs)
+        result = document_store_bbm25_filter.filter_documents(
             {"field": "meta.number", "operator": "!=", "value": 100}
         )
         self.assert_documents_are_equal(
             result,
             [
                 d
                 for d in filterable_docs
                 if d.meta.get("number") != 100 and "number" in d.meta
             ],
         )
 
-    def test_comparison_not_in(self, document_store, filterable_docs):
+    def test_comparison_not_in_bbm25_filter(
+        self, document_store_bbm25_filter, filterable_docs
+    ):
         """Similar to the test above."""
-        document_store.write_documents(filterable_docs)
-        result = document_store.filter_documents(
+        document_store_bbm25_filter.write_documents(filterable_docs)
+        result = document_store_bbm25_filter.filter_documents(
             {"field": "meta.number", "operator": "not in", "value": [9, 10]}
         )
         self.assert_documents_are_equal(
             result,
             [
                 d
                 for d in filterable_docs
                 if d.meta.get("number") not in [9, 10] and "number" in d.meta
             ],
         )
 
-    def test_comparison_equal_with_dataframe(self, document_store, filterable_docs):
-        document_store.write_documents(filterable_docs)
+    def test_comparison_equal_with_dataframe_bbm25_filter(
+        self, document_store_bbm25_filter, filterable_docs
+    ):
+        document_store_bbm25_filter.write_documents(filterable_docs)
         with pytest.raises(FilterError):
-            _ = document_store.filter_documents(
+            _ = document_store_bbm25_filter.filter_documents(
                 filters={
                     "field": "dataframe",
                     "operator": "==",
                     "value": pd.DataFrame([1]),
                 }
             )
 
-    def test_comparison_not_equal_with_dataframe(self, document_store, filterable_docs):
-        document_store.write_documents(filterable_docs)
+    def test_comparison_not_equal_with_dataframe_bbm25_filter(
+        self, document_store_bbm25_filter, filterable_docs
+    ):
+        document_store_bbm25_filter.write_documents(filterable_docs)
         with pytest.raises(FilterError):
-            _ = document_store.filter_documents(
+            _ = document_store_bbm25_filter.filter_documents(
                 filters={
                     "field": "dataframe",
                     "operator": "==",
                     "value": pd.DataFrame([1]),
                 }
             )
-
-    # Pass these two tests as we now support iterables other than lists
-    def test_comparison_in_with_with_non_list_iterable(
-        self, document_store, filterable_docs
-    ):
-        pass
-
-    def test_comparison_not_in_with_with_non_list_iterable(
-        self, document_store, filterable_docs
-    ):
-        pass
```

### Comparing `bbm25_haystack-0.1.0/tests/test_retriever.py` & `bbm25_haystack-0.1.1/tests/test_retriever.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,22 +48,28 @@
             BetterBM25Retriever(BetterBM25DocumentStore(), filters="invalid")
 
     def test_to_dict(self):
         store_class = document_store_class(
             "MyFakeStore", bases=(BetterBM25DocumentStore,)
         )
         document_store = store_class()
-        document_store.to_dict = lambda: {"type": "MyFakeStore", "init_parameters": {}}
+        document_store.to_dict = lambda: {
+            "type": "MyFakeStore",
+            "init_parameters": {},
+        }
         component = BetterBM25Retriever(document_store=document_store)
 
         data = component.to_dict()
         assert data == {
             "type": "bbm25_haystack.bbm25_retriever.BetterBM25Retriever",
             "init_parameters": {
-                "document_store": {"type": "MyFakeStore", "init_parameters": {}},
+                "document_store": {
+                    "type": "MyFakeStore",
+                    "init_parameters": {},
+                },
                 "filters": None,
                 "top_k": 10,
             },
         }
 
     def test_to_dict_with_custom_init_parameters(self):
         ds = BetterBM25DocumentStore()
@@ -100,15 +106,16 @@
         assert isinstance(component.document_store, BetterBM25DocumentStore)
         assert component.filters == {"name": "test.txt"}
         assert component.top_k == 5
 
     def test_from_dict_without_docstore(self):
         data = {"type": "BetterBM25Retriever", "init_parameters": {}}
         with pytest.raises(
-            DeserializationError, match="Missing 'document_store' in serialization data"
+            DeserializationError,
+            match="Missing 'document_store' in serialization data",
         ):
             BetterBM25Retriever.from_dict(data)
 
     def test_from_dict_without_docstore_type(self):
         data = {
             "type": "BetterBM25Retriever",
             "init_parameters": {"document_store": {"init_parameters": {}}},
@@ -119,30 +126,35 @@
         ):
             BetterBM25Retriever.from_dict(data)
 
     def test_from_dict_nonexisting_docstore(self):
         data = {
             "type": "bbm25_haystack.BetterBM25Retriever",
             "init_parameters": {
-                "document_store": {"type": "Nonexisting.Docstore", "init_parameters": {}}
+                "document_store": {
+                    "type": "Nonexisting.Docstore",
+                    "init_parameters": {},
+                }
             },
         }
         with pytest.raises(DeserializationError):
             BetterBM25Retriever.from_dict(data)
 
     def test_retriever_valid_run(self, mock_docs):
         ds = BetterBM25DocumentStore()
         ds.write_documents(mock_docs)
 
         retriever = BetterBM25Retriever(ds, top_k=5)
         result = retriever.run(query="PHP")
 
         assert "documents" in result
         assert len(result["documents"]) == 5
-        assert result["documents"][0].content == "PHP is a popular programming language"
+        assert (
+            result["documents"][0].content == "PHP is a popular programming language"
+        )
 
     def test_invalid_run_wrong_store_type(self):
         store_class = document_store_class("SomeOtherDocumentStore")
         with pytest.raises(
             TypeError,
             match="document_store must be an instance of BetterBM25DocumentStore",
         ):
```

### Comparing `bbm25_haystack-0.1.0/.gitignore` & `bbm25_haystack-0.1.1/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -157,7 +157,10 @@
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 # VS Code
 .vscode
+
+# Benchmarking datasets
+benchmarks/beir/*
```

### Comparing `bbm25_haystack-0.1.0/LICENSE` & `bbm25_haystack-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.1.0/README.md` & `bbm25_haystack-0.1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -2,27 +2,33 @@
 [![codecov](https://codecov.io/gh/Guest400123064/bbm25-haystack/graph/badge.svg?token=IGRIRBHZ3U)](https://codecov.io/gh/Guest400123064/bbm25-haystack)
 [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy)
 [![Python 3.9](https://img.shields.io/badge/python-3.9%20|%203.10%20|%203.11-blue.svg)](https://www.python.org/downloads/release/python-390/)
 
 # Better BM25 In-Memory Document Store
 
-An in-memory document store is a great starting point for prototyping and debugging before migrating to production-grade stores like Elasticsearch. However, [the original implementation](https://github.com/deepset-ai/haystack/blob/0dbb98c0a017b499560521aa93186d0640aab659/haystack/document_stores/in_memory/document_store.py#L148) of BM25 retrieval recreates an inverse index for the entire document store on every new search. Furthermore, the tokenization method is primitive, only permitting splitters based on regular expressions, making localization and domain adaptation challenging. Therefore, this implementation is a slight upgrade to the default BM25 in-memory document store by implementing incremental index update and incorporation of [SentencePiece](https://github.com/google/sentencepiece) statistical sub-word tokenization.
+An in-memory document store is a great starting point for prototyping and debugging before migrating to production-grade stores like Elasticsearch. However, [the original implementation](https://github.com/deepset-ai/haystack/blob/0dbb98c0a017b499560521aa93186d0640aab659/haystack/document_stores/in_memory/document_store.py#L148) of BM25 retrieval recreates an inverse index for the entire document store __on every new search__. Furthermore, the tokenization method is primitive, only permitting splitters based on regular expressions, making localization and domain adaptation challenging. Therefore, this implementation is a slight upgrade to the default BM25 in-memory document store by implementing incremental index update and incorporation of [SentencePiece](https://github.com/google/sentencepiece) statistical sub-word tokenization.
 
 ## Installation
 
-This package has not yet been published to PyPI. Please install the package directly from the `main` branch using:
+```bash
+$ pip install bbm25-haystack
+```
+
+Alternatively, you can clone the repository and build from source to be able to reflect changes to the source code:
 
 ```bash
-pip install git+https://github.com/Guest400123064/bbm25-haystack.git@main
+$ git clone https://github.com/Guest400123064/bbm25-haystack.git
+$ cd bbm25-haystack
+$ pip install -e .
 ```
 
 ## Usage
 
-The initializer takes [three BM25+ hyperparameters](https://en.wikipedia.org/wiki/Okapi_BM25), namely `k1`, `b`, and `delta`, and one path to a trained SentencePiece tokenizer `.model` file. All parameters are optional. The default tokenizer is directly copied from [this SentencePiece test tokenizer](https://github.com/google/sentencepiece/blob/master/python/test/test_model.model) with a vocab size of 1000.
+The initializer takes [three BM25+ hyperparameters](https://en.wikipedia.org/wiki/Okapi_BM25), namely `k1`, `b`, and `delta`, one path to a trained SentencePiece tokenizer `.model` file, and a filtering logic flag ([see below](#filtering-logic)). All parameters are optional. The default tokenizer is directly copied from [LLaMA-2-7B-32K tokenizer](https://huggingface.co/togethercomputer/LLaMA-2-7B-32K/blob/main/tokenizer.model) with a vocab size of 32,000.
 
 ```python
 from haystack import Document
 from bbm25_haystack import BetterBM25DocumentStore, BetterBM25Retriever
 
 
 document_store = BetterBM25DocumentStore()
@@ -32,20 +38,44 @@
    Document(content="In certain parts of the world, like the Maldives, Puerto Rico, and San Diego, you can witness the phenomenon of bioluminescent waves.")
 ])
 
 retriever = BetterBM25Retriever(document_store)
 retriever.run(query="How many languages are spoken around the world today?")
 ```
 
-## Filtering Logic and Caveats
+## Filtering Logic
 
-The filtering logic is slightly different from the default implementation shipped with Haystack, but this logic may be subject to changes, and I am open to different suggestions. Please find comments and implementation details in [`filters.py`](./src/bbm25_haystack/filters.py). TL;DR:
+The current document store uses `document_matches_filter` shipped with Haystack to perform filtering by default, which is the same as `InMemoryDocumentStore` except that it is DOES NOT support legacy operator names.
+
+However, there is also an alternative filtering logic shipped with this implementation that is more conservative (and unstable at this point). To use this alternative logic, initialize the document store with `haystack_filter_logic=False` Please find comments and implementation details in [`filters.py`](./src/bbm25_haystack/filters.py). TL;DR:
 
 - Comparison with `None`, i.e., missing values, involved will always return `False`, no matter the document attribute value or filter value.
 - Comparison with `DataFrame` is always prohibited to reduce surprises.
 - No implicit `datetime` conversion from string values.
 
 These differences lead to a few caveats. Firstly, some test cases are overridden to take into account the different expectations. However, this means that passed, non-overridden tests may not be faithful, i.e., the filters behave in the same way as the old implementation while different behaviors are expected. Further, the negation logic needs to be considered again because `False` can now issue from both input check and the actual comparisons. But I think having input processing and comparisons separated makes the filtering behavior more transparent.
 
+## Search Quality Evaluation
+
+This repo has [a simple script](./scripts/benchmark_beir.py) to help evaluate the search quality over [BEIR](https://github.com/beir-cellar/beir/tree/main) benchmark. You need to clone the repository (you can also manually download the script and place it under a folder named `scripts`) and you have to install additional dependencies to run the script.
+
+```bash
+$ pip install beir
+```
+
+To run the script, you may want to specify the dataset name and BM25 hyperparameters. For example:
+
+```bash
+$ python scripts/benchmark_beir.py --datasets scifact arguana --bm25-k1 1.2 --output eval.csv
+```
+
+It automatically downloads the benchmarking dataset to `benchmarks/beir`, where `benchmarks` is at the same level as `scripts`. You may also check the help page for more information.
+
+```bash
+$ python scripts/benchmark_beir.py --help
+```
+
+New benchmarking scripts are expected to be added in the future.
+
 ## License
 
 `bbm25-haystack` is distributed under the terms of the [Apache-2.0](https://spdx.org/licenses/Apache-2.0.html) license.
```

### Comparing `bbm25_haystack-0.1.0/pyproject.toml` & `bbm25_haystack-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
   "pytest-cov",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
-  "coverage report",
+  "coverage xml",
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
@@ -81,20 +81,20 @@
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.black]
 target-version = ["py39"]
-line-length = 90
+line-length = 85
 skip-string-normalization = true
 
 [tool.ruff]
 target-version = "py39"
-line-length = 90
+line-length = 85
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
   "E",
```

### Comparing `bbm25_haystack-0.1.0/PKG-INFO` & `bbm25_haystack-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bbm25-haystack
-Version: 0.1.0
+Version: 0.1.1
 Summary: Haystack 2.x In-memory Document Store with Enhanced Efficiency
 Project-URL: Documentation, https://github.com/Guest400123064/bbm25-haystack#readme
 Project-URL: Issues, https://github.com/Guest400123064/bbm25-haystack/issues
 Project-URL: Source, https://github.com/Guest400123064/bbm25-haystack
 Author-email: Yuxuan Wang <wangy49@seas.upenn.edu>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -26,27 +26,33 @@
 [![codecov](https://codecov.io/gh/Guest400123064/bbm25-haystack/graph/badge.svg?token=IGRIRBHZ3U)](https://codecov.io/gh/Guest400123064/bbm25-haystack)
 [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy)
 [![Python 3.9](https://img.shields.io/badge/python-3.9%20|%203.10%20|%203.11-blue.svg)](https://www.python.org/downloads/release/python-390/)
 
 # Better BM25 In-Memory Document Store
 
-An in-memory document store is a great starting point for prototyping and debugging before migrating to production-grade stores like Elasticsearch. However, [the original implementation](https://github.com/deepset-ai/haystack/blob/0dbb98c0a017b499560521aa93186d0640aab659/haystack/document_stores/in_memory/document_store.py#L148) of BM25 retrieval recreates an inverse index for the entire document store on every new search. Furthermore, the tokenization method is primitive, only permitting splitters based on regular expressions, making localization and domain adaptation challenging. Therefore, this implementation is a slight upgrade to the default BM25 in-memory document store by implementing incremental index update and incorporation of [SentencePiece](https://github.com/google/sentencepiece) statistical sub-word tokenization.
+An in-memory document store is a great starting point for prototyping and debugging before migrating to production-grade stores like Elasticsearch. However, [the original implementation](https://github.com/deepset-ai/haystack/blob/0dbb98c0a017b499560521aa93186d0640aab659/haystack/document_stores/in_memory/document_store.py#L148) of BM25 retrieval recreates an inverse index for the entire document store __on every new search__. Furthermore, the tokenization method is primitive, only permitting splitters based on regular expressions, making localization and domain adaptation challenging. Therefore, this implementation is a slight upgrade to the default BM25 in-memory document store by implementing incremental index update and incorporation of [SentencePiece](https://github.com/google/sentencepiece) statistical sub-word tokenization.
 
 ## Installation
 
-This package has not yet been published to PyPI. Please install the package directly from the `main` branch using:
+```bash
+$ pip install bbm25-haystack
+```
+
+Alternatively, you can clone the repository and build from source to be able to reflect changes to the source code:
 
 ```bash
-pip install git+https://github.com/Guest400123064/bbm25-haystack.git@main
+$ git clone https://github.com/Guest400123064/bbm25-haystack.git
+$ cd bbm25-haystack
+$ pip install -e .
 ```
 
 ## Usage
 
-The initializer takes [three BM25+ hyperparameters](https://en.wikipedia.org/wiki/Okapi_BM25), namely `k1`, `b`, and `delta`, and one path to a trained SentencePiece tokenizer `.model` file. All parameters are optional. The default tokenizer is directly copied from [this SentencePiece test tokenizer](https://github.com/google/sentencepiece/blob/master/python/test/test_model.model) with a vocab size of 1000.
+The initializer takes [three BM25+ hyperparameters](https://en.wikipedia.org/wiki/Okapi_BM25), namely `k1`, `b`, and `delta`, one path to a trained SentencePiece tokenizer `.model` file, and a filtering logic flag ([see below](#filtering-logic)). All parameters are optional. The default tokenizer is directly copied from [LLaMA-2-7B-32K tokenizer](https://huggingface.co/togethercomputer/LLaMA-2-7B-32K/blob/main/tokenizer.model) with a vocab size of 32,000.
 
 ```python
 from haystack import Document
 from bbm25_haystack import BetterBM25DocumentStore, BetterBM25Retriever
 
 
 document_store = BetterBM25DocumentStore()
@@ -56,20 +62,44 @@
    Document(content="In certain parts of the world, like the Maldives, Puerto Rico, and San Diego, you can witness the phenomenon of bioluminescent waves.")
 ])
 
 retriever = BetterBM25Retriever(document_store)
 retriever.run(query="How many languages are spoken around the world today?")
 ```
 
-## Filtering Logic and Caveats
+## Filtering Logic
 
-The filtering logic is slightly different from the default implementation shipped with Haystack, but this logic may be subject to changes, and I am open to different suggestions. Please find comments and implementation details in [`filters.py`](./src/bbm25_haystack/filters.py). TL;DR:
+The current document store uses `document_matches_filter` shipped with Haystack to perform filtering by default, which is the same as `InMemoryDocumentStore` except that it is DOES NOT support legacy operator names.
+
+However, there is also an alternative filtering logic shipped with this implementation that is more conservative (and unstable at this point). To use this alternative logic, initialize the document store with `haystack_filter_logic=False` Please find comments and implementation details in [`filters.py`](./src/bbm25_haystack/filters.py). TL;DR:
 
 - Comparison with `None`, i.e., missing values, involved will always return `False`, no matter the document attribute value or filter value.
 - Comparison with `DataFrame` is always prohibited to reduce surprises.
 - No implicit `datetime` conversion from string values.
 
 These differences lead to a few caveats. Firstly, some test cases are overridden to take into account the different expectations. However, this means that passed, non-overridden tests may not be faithful, i.e., the filters behave in the same way as the old implementation while different behaviors are expected. Further, the negation logic needs to be considered again because `False` can now issue from both input check and the actual comparisons. But I think having input processing and comparisons separated makes the filtering behavior more transparent.
 
+## Search Quality Evaluation
+
+This repo has [a simple script](./scripts/benchmark_beir.py) to help evaluate the search quality over [BEIR](https://github.com/beir-cellar/beir/tree/main) benchmark. You need to clone the repository (you can also manually download the script and place it under a folder named `scripts`) and you have to install additional dependencies to run the script.
+
+```bash
+$ pip install beir
+```
+
+To run the script, you may want to specify the dataset name and BM25 hyperparameters. For example:
+
+```bash
+$ python scripts/benchmark_beir.py --datasets scifact arguana --bm25-k1 1.2 --output eval.csv
+```
+
+It automatically downloads the benchmarking dataset to `benchmarks/beir`, where `benchmarks` is at the same level as `scripts`. You may also check the help page for more information.
+
+```bash
+$ python scripts/benchmark_beir.py --help
+```
+
+New benchmarking scripts are expected to be added in the future.
+
 ## License
 
 `bbm25-haystack` is distributed under the terms of the [Apache-2.0](https://spdx.org/licenses/Apache-2.0.html) license.
```


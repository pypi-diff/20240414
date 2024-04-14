# Comparing `tmp/wttch-train-helper-0.0.8.tar.gz` & `tmp/wttch-train-helper-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wttch-train-helper-0.0.8.tar", last modified: Sun Jan 21 09:25:32 2024, max compression
+gzip compressed data, was "wttch-train-helper-0.0.9.tar", last modified: Sun Jan 21 10:04:07 2024, max compression
```

## Comparing `wttch-train-helper-0.0.8.tar` & `wttch-train-helper-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 wttch      (501) staff       (20)        0 2024-01-21 09:25:32.433026 wttch-train-helper-0.0.8/
--rw-r--r--   0 wttch      (501) staff       (20)     1073 2024-01-18 08:00:11.000000 wttch-train-helper-0.0.8/LICENSE
--rw-r--r--   0 wttch      (501) staff       (20)     2709 2024-01-21 09:25:32.432721 wttch-train-helper-0.0.8/PKG-INFO
--rw-r--r--   0 wttch      (501) staff       (20)     2147 2024-01-20 12:33:31.000000 wttch-train-helper-0.0.8/README.md
--rw-r--r--   0 wttch      (501) staff       (20)      562 2024-01-21 09:23:29.000000 wttch-train-helper-0.0.8/pyproject.toml
--rw-r--r--   0 wttch      (501) staff       (20)       38 2024-01-21 09:25:32.433094 wttch-train-helper-0.0.8/setup.cfg
--rw-r--r--   0 wttch      (501) staff       (20)      448 2024-01-21 09:24:54.000000 wttch-train-helper-0.0.8/setup.py
-drwxr-xr-x   0 wttch      (501) staff       (20)        0 2024-01-21 09:25:32.425186 wttch-train-helper-0.0.8/src/
-drwxr-xr-x   0 wttch      (501) staff       (20)        0 2024-01-21 09:25:32.425849 wttch-train-helper-0.0.8/src/wttch-train-helper/
-drwxr-xr-x   0 wttch      (501) staff       (20)        0 2024-01-21 09:25:32.425344 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/
-drwxr-xr-x   0 wttch      (501) staff       (20)        0 2024-01-21 09:25:32.427291 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/
--rw-r--r--   0 wttch      (501) staff       (20)       15 2024-01-20 12:33:32.000000 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/__init__.py
-drwxr-xr-x   0 wttch      (501) staff       (20)        0 2024-01-21 09:25:32.427973 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/data/
--rw-r--r--   0 wttch      (501) staff       (20)       73 2024-01-21 09:23:29.000000 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/data/__init__.py
--rw-r--r--   0 wttch      (501) staff       (20)     2637 2024-01-21 09:23:29.000000 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/data/seq_data_loader.py
-drwxr-xr-x   0 wttch      (501) staff       (20)        0 2024-01-21 09:25:32.429166 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/notification/
--rw-r--r--   0 wttch      (501) staff       (20)      167 2024-01-17 09:16:56.000000 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/notification/__init__.py
--rw-r--r--   0 wttch      (501) staff       (20)      216 2024-01-20 18:00:22.000000 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/notification/base.py
--rw-r--r--   0 wttch      (501) staff       (20)     2346 2024-01-21 09:23:29.000000 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/notification/dingtalk.py
--rw-r--r--   0 wttch      (501) staff       (20)     1284 2024-01-17 09:16:56.000000 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/notification/wechat.py
-drwxr-xr-x   0 wttch      (501) staff       (20)        0 2024-01-21 09:25:32.429613 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/torch/
--rw-r--r--   0 wttch      (501) staff       (20)        0 2024-01-17 09:03:21.000000 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/torch/__init__.py
--rw-r--r--   0 wttch      (501) staff       (20)     1198 2024-01-20 12:33:32.000000 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/torch/utils.py
-drwxr-xr-x   0 wttch      (501) staff       (20)        0 2024-01-21 09:25:32.430511 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/utils/
--rw-r--r--   0 wttch      (501) staff       (20)      119 2024-01-20 12:33:32.000000 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/utils/__init__.py
--rw-r--r--   0 wttch      (501) staff       (20)     2971 2024-01-20 12:33:32.000000 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/utils/cache.py
--rw-r--r--   0 wttch      (501) staff       (20)     1118 2024-01-20 12:33:32.000000 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/utils/stopwatch.py
-drwxr-xr-x   0 wttch      (501) staff       (20)        0 2024-01-21 09:25:32.432360 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch_train_helper.egg-info/
--rw-r--r--   0 wttch      (501) staff       (20)     2709 2024-01-21 09:25:32.000000 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch_train_helper.egg-info/PKG-INFO
--rw-r--r--   0 wttch      (501) staff       (20)     1005 2024-01-21 09:25:32.000000 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch_train_helper.egg-info/SOURCES.txt
--rw-r--r--   0 wttch      (501) staff       (20)        1 2024-01-21 09:25:32.000000 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch_train_helper.egg-info/dependency_links.txt
--rw-r--r--   0 wttch      (501) staff       (20)        6 2024-01-21 09:25:32.000000 wttch-train-helper-0.0.8/src/wttch-train-helper/wttch_train_helper.egg-info/top_level.txt
-drwxr-xr-x   0 wttch      (501) staff       (20)        0 2024-01-21 09:25:32.431979 wttch-train-helper-0.0.8/tests/
--rw-r--r--   0 wttch      (501) staff       (20)      423 2024-01-20 12:33:32.000000 wttch-train-helper-0.0.8/tests/test_torch_utils.py
--rw-r--r--   0 wttch      (501) staff       (20)      416 2024-01-20 12:33:32.000000 wttch-train-helper-0.0.8/tests/test_utils_cache.py
+drwxr-xr-x   0 wttch      (501) staff       (20)        0 2024-01-21 10:04:07.284345 wttch-train-helper-0.0.9/
+-rw-r--r--   0 wttch      (501) staff       (20)     1073 2024-01-18 08:00:11.000000 wttch-train-helper-0.0.9/LICENSE
+-rw-r--r--   0 wttch      (501) staff       (20)     2709 2024-01-21 10:04:07.284013 wttch-train-helper-0.0.9/PKG-INFO
+-rw-r--r--   0 wttch      (501) staff       (20)     2147 2024-01-20 12:33:31.000000 wttch-train-helper-0.0.9/README.md
+-rw-r--r--   0 wttch      (501) staff       (20)      562 2024-01-21 10:03:45.000000 wttch-train-helper-0.0.9/pyproject.toml
+-rw-r--r--   0 wttch      (501) staff       (20)       38 2024-01-21 10:04:07.284412 wttch-train-helper-0.0.9/setup.cfg
+-rw-r--r--   0 wttch      (501) staff       (20)      448 2024-01-21 10:03:45.000000 wttch-train-helper-0.0.9/setup.py
+drwxr-xr-x   0 wttch      (501) staff       (20)        0 2024-01-21 10:04:07.275712 wttch-train-helper-0.0.9/src/
+drwxr-xr-x   0 wttch      (501) staff       (20)        0 2024-01-21 10:04:07.276403 wttch-train-helper-0.0.9/src/wttch-train-helper/
+drwxr-xr-x   0 wttch      (501) staff       (20)        0 2024-01-21 10:04:07.275881 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/
+drwxr-xr-x   0 wttch      (501) staff       (20)        0 2024-01-21 10:04:07.277912 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/
+-rw-r--r--   0 wttch      (501) staff       (20)       15 2024-01-20 12:33:32.000000 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/__init__.py
+drwxr-xr-x   0 wttch      (501) staff       (20)        0 2024-01-21 10:04:07.278544 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/data/
+-rw-r--r--   0 wttch      (501) staff       (20)       73 2024-01-21 09:23:29.000000 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/data/__init__.py
+-rw-r--r--   0 wttch      (501) staff       (20)     3021 2024-01-21 10:03:33.000000 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/data/seq_data_loader.py
+drwxr-xr-x   0 wttch      (501) staff       (20)        0 2024-01-21 10:04:07.280109 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/notification/
+-rw-r--r--   0 wttch      (501) staff       (20)      167 2024-01-17 09:16:56.000000 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/notification/__init__.py
+-rw-r--r--   0 wttch      (501) staff       (20)      216 2024-01-20 18:00:22.000000 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/notification/base.py
+-rw-r--r--   0 wttch      (501) staff       (20)     2346 2024-01-21 09:23:29.000000 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/notification/dingtalk.py
+-rw-r--r--   0 wttch      (501) staff       (20)     1284 2024-01-17 09:16:56.000000 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/notification/wechat.py
+drwxr-xr-x   0 wttch      (501) staff       (20)        0 2024-01-21 10:04:07.280790 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/torch/
+-rw-r--r--   0 wttch      (501) staff       (20)        0 2024-01-17 09:03:21.000000 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/torch/__init__.py
+-rw-r--r--   0 wttch      (501) staff       (20)     1198 2024-01-20 12:33:32.000000 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/torch/utils.py
+drwxr-xr-x   0 wttch      (501) staff       (20)        0 2024-01-21 10:04:07.281889 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/utils/
+-rw-r--r--   0 wttch      (501) staff       (20)      119 2024-01-20 12:33:32.000000 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/utils/__init__.py
+-rw-r--r--   0 wttch      (501) staff       (20)     2971 2024-01-20 12:33:32.000000 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/utils/cache.py
+-rw-r--r--   0 wttch      (501) staff       (20)     1118 2024-01-20 12:33:32.000000 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/utils/stopwatch.py
+drwxr-xr-x   0 wttch      (501) staff       (20)        0 2024-01-21 10:04:07.283589 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch_train_helper.egg-info/
+-rw-r--r--   0 wttch      (501) staff       (20)     2709 2024-01-21 10:04:07.000000 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch_train_helper.egg-info/PKG-INFO
+-rw-r--r--   0 wttch      (501) staff       (20)     1005 2024-01-21 10:04:07.000000 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch_train_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 wttch      (501) staff       (20)        1 2024-01-21 10:04:07.000000 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch_train_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 wttch      (501) staff       (20)        6 2024-01-21 10:04:07.000000 wttch-train-helper-0.0.9/src/wttch-train-helper/wttch_train_helper.egg-info/top_level.txt
+drwxr-xr-x   0 wttch      (501) staff       (20)        0 2024-01-21 10:04:07.283203 wttch-train-helper-0.0.9/tests/
+-rw-r--r--   0 wttch      (501) staff       (20)      423 2024-01-20 12:33:32.000000 wttch-train-helper-0.0.9/tests/test_torch_utils.py
+-rw-r--r--   0 wttch      (501) staff       (20)      416 2024-01-20 12:33:32.000000 wttch-train-helper-0.0.9/tests/test_utils_cache.py
```

### Comparing `wttch-train-helper-0.0.8/LICENSE` & `wttch-train-helper-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wttch-train-helper-0.0.8/PKG-INFO` & `wttch-train-helper-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wttch-train-helper
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wttch's train helper
 Author: wttch
 Author-email: Wttch <wttch@wttch.com>
 Project-URL: Homepage, https://github.com/wttch96/train-helper
 Project-URL: Issues, https://github.com/wttch96/train-helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wttch-train-helper-0.0.8/README.md` & `wttch-train-helper-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `wttch-train-helper-0.0.8/pyproject.toml` & `wttch-train-helper-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wttch-train-helper"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Wttch", email="wttch@wttch.com" },
 ]
 description = "Wttch's train helper"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/data/seq_data_loader.py` & `wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/data/seq_data_loader.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,80 +1,94 @@
 import random
+from typing import Union
 
 import numpy as np
 
 
-def seq_data_iter_random(corpus: np.ndarray, batch_size: int, seq_len: int) -> tuple[np.ndarray, np.ndarray]:
+def seq_data_iter_random(corpus: np.ndarray, batch_size: int, seq_len: int, label=False) \
+        -> Union[tuple[np.ndarray, np.ndarray], np.ndarray]:
     """
     随机生成序列数据，只保证序列内的顺序和原始顺序一致，不能保证小批量数据之间连续。
     Args:
         corpus: 原始语料库
         batch_size: 批处理大小
         seq_len: 序列长度
 
     Returns:
 
     """
     # 偏移
-    corpus = corpus[random.randint(0, seq_len - 1):]
+    corpus = corpus[random.randint(0, seq_len):]
     # -1, 因为标签 +1, 序列的下一个数据就是标签
-    num_seqs = (len(corpus) - 1) // seq_len
+    num_seqs = (len(corpus) - (1 if label else 0)) // seq_len
     # 抽样开始的位置
     init_indices = list(range(0, num_seqs * seq_len, seq_len))
     # 打乱, batch 内序列不一定连续
     random.shuffle(init_indices)
 
-    def get_data(pos): return corpus[pos: pos + seq_len]
+    def get_data(pos):
+        return corpus[pos: pos + seq_len]
 
     # 可以生成多少批数据
     num_batches = num_seqs // batch_size
     for i in range(0, batch_size * num_batches, batch_size):
         init_indices_per_batch = init_indices[i:i + batch_size]
-        data_array = np.array([[get_data(j), get_data(j + 1)] for j in init_indices_per_batch])
-        yield data_array[:, 0], data_array[:, 1]
+        X = [get_data(j) for j in init_indices_per_batch]
+        if label:
+            Y = [get_data(j + 1) for j in init_indices_per_batch]
+            yield np.array(X), np.array(Y)
+        else:
+            yield np.array(X)
 
 
-def seq_data_iter_sequential(corpus: np.ndarray, batch_size: int, seq_len: int) -> tuple[np.ndarray, np.ndarray]:
+def seq_data_iter_sequential(corpus: np.ndarray, batch_size: int, seq_len: int, label: bool = False) \
+        -> Union[tuple[np.ndarray, np.ndarray], np.ndarray]:
     """
     顺序生成序列数据，能保证小批量数据之间连续。
     Args:
         corpus: 原始语料库
         batch_size: 批处理大小
         seq_len: 序列长度
 
     Returns:
 
     """
     corpus = corpus[random.randint(0, seq_len):]
-    num_tokens = ((len(corpus) - 1) // batch_size) * batch_size
+    num_tokens = ((len(corpus) - (1 if label else 0)) // batch_size) * batch_size
 
     Xs = corpus[0: num_tokens]
-    Ys = corpus[1: num_tokens + 1]
-    Xs, Ys = Xs.reshape(batch_size, -1), Ys.reshape(batch_size, -1)
+    Xs = Xs.reshape(batch_size, -1)
+    if label:
+        Ys = corpus[1: num_tokens + 1]
+        Ys = Ys.reshape(batch_size, -1)
 
     num_batches = Xs.shape[1] // seq_len
     for i in range(0, seq_len * num_batches, seq_len):
         X = Xs[:, i: i + seq_len]
-        Y = Ys[:, i: i + seq_len]
-        yield X, Y
+        if label:
+            Y = Ys[:, i: i + seq_len]
+            yield X, Y
+        else:
+            yield X
 
 
 class SeqDataLoader:
 
-    def __init__(self, data: numpy.ndarray, batch_size: int, seq_len: int, shuffle: bool = True):
+    def __init__(self, data: np.ndarray, batch_size: int, seq_len: int, shuffle: bool = True, label: bool = False):
         """
         序列数据加载器。
         Args:
             data: 原始数据
             batch_size: 批处理长度
             seq_len: 序列长度
             shuffle: 批之间收否随机
         """
         # 分开处理是因为使用 yield, 也可以同一个函数处理，之后随机一下
         self.data_iter_fn = seq_data_iter_random if shuffle else seq_data_iter_sequential
 
         self.data = data
         self.batch_size = batch_size
         self.seq_len = seq_len
+        self.label = label
 
     def __iter__(self):
-        return self.data_iter_fn(self.data, self.batch_size, self.seq_len)
+        return self.data_iter_fn(self.data, self.batch_size, self.seq_len, self.label)
```

### Comparing `wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/notification/dingtalk.py` & `wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/notification/dingtalk.py`

 * *Files identical despite different names*

### Comparing `wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/notification/wechat.py` & `wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/notification/wechat.py`

 * *Files identical despite different names*

### Comparing `wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/torch/utils.py` & `wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/torch/utils.py`

 * *Files identical despite different names*

### Comparing `wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/utils/cache.py` & `wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/utils/cache.py`

 * *Files identical despite different names*

### Comparing `wttch-train-helper-0.0.8/src/wttch-train-helper/wttch/train/utils/stopwatch.py` & `wttch-train-helper-0.0.9/src/wttch-train-helper/wttch/train/utils/stopwatch.py`

 * *Files identical despite different names*

### Comparing `wttch-train-helper-0.0.8/src/wttch-train-helper/wttch_train_helper.egg-info/PKG-INFO` & `wttch-train-helper-0.0.9/src/wttch-train-helper/wttch_train_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wttch-train-helper
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wttch's train helper
 Author: wttch
 Author-email: Wttch <wttch@wttch.com>
 Project-URL: Homepage, https://github.com/wttch96/train-helper
 Project-URL: Issues, https://github.com/wttch96/train-helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wttch-train-helper-0.0.8/src/wttch-train-helper/wttch_train_helper.egg-info/SOURCES.txt` & `wttch-train-helper-0.0.9/src/wttch-train-helper/wttch_train_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*


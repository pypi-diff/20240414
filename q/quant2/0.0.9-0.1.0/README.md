# Comparing `tmp/quant2-0.0.9.tar.gz` & `tmp/quant2-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant2-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "quant2-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `quant2-0.0.9.tar` & `quant2-0.1.0.tar`

### file list

```diff
@@ -1,30 +1,51 @@
--rw-r--r--   0        0        0      556 2024-03-29 02:51:50.428398 quant2-0.0.9/.gitignore
--rw-r--r--   0        0        0    11357 2024-03-20 11:12:02.832412 quant2-0.0.9/LICENSE
--rw-r--r--   0        0        0        7 2024-03-20 11:12:02.832412 quant2-0.0.9/README.md
--rw-r--r--   0        0        0      658 2024-03-28 02:47:13.721511 quant2-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     1841 2024-03-23 05:01:23.359992 quant2-0.0.9/quant/README.md
--rw-r--r--   0        0        0      559 2024-03-29 09:36:39.917189 quant2-0.0.9/quant/__init__.py
--rw-r--r--   0        0        0       67 2024-03-23 04:17:48.269987 quant2-0.0.9/quant/__main__.py
--rw-r--r--   0        0        0      422 2024-03-23 04:21:50.819993 quant2-0.0.9/quant/football/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 14:09:03.305285 quant2-0.0.9/quant/football/data/__init__.py
--rw-r--r--   0        0        0     1617 2024-03-27 14:21:31.002567 quant2-0.0.9/quant/football/data/dataset.py
--rw-r--r--   0        0        0     1227 2024-03-27 14:21:31.002567 quant2-0.0.9/quant/football/data/functional.py
--rw-r--r--   0        0        0     1881 2024-03-28 05:23:26.661515 quant2-0.0.9/quant/football/data/stats.py
--rw-r--r--   0        0        0     4057 2024-03-28 04:00:36.851517 quant2-0.0.9/quant/football/data/utils.py
--rw-r--r--   0        0        0    11529 2024-03-26 04:17:29.502157 quant2-0.0.9/quant/football/etk_titan.py
--rw-r--r--   0        0        0        0 2024-03-25 14:09:03.335285 quant2-0.0.9/quant/football/models/__init__.py
--rw-r--r--   0        0        0     3742 2024-03-27 13:28:52.012568 quant2-0.0.9/quant/football/models/base.py
--rw-r--r--   0        0        0        0 2024-03-25 14:13:16.096778 quant2-0.0.9/quant/football/models/mtnet.py
--rw-r--r--   0        0        0     3230 2024-03-30 04:08:13.910978 quant2-0.0.9/quant/football/models/stnet.py
--rw-r--r--   0        0        0        0 2024-03-27 06:43:54.622569 quant2-0.0.9/quant/football/transforms/__init__.py
--rw-r--r--   0        0        0     4858 2024-03-29 09:27:22.184980 quant2-0.0.9/quant/football/transforms/table20240326.py
--rw-r--r--   0        0        0        0 2024-03-25 00:38:54.232911 quant2-0.0.9/quant/io/__init__.py
--rw-r--r--   0        0        0      496 2024-03-27 14:22:43.112566 quant2-0.0.9/quant/io/utils.py
--rw-r--r--   0        0        0      483 2024-03-28 09:12:19.609652 quant2-0.0.9/quant/layers/layer_scale.py
--rw-r--r--   0        0        0     1070 2024-03-28 09:13:06.741829 quant2-0.0.9/quant/layers/mlp.py
--rw-r--r--   0        0        0     1314 2024-03-28 09:40:33.643889 quant2-0.0.9/quant/layers/normalization.py
--rw-r--r--   0        0        0      852 2024-03-28 09:16:09.540017 quant2-0.0.9/quant/layers/swiglu_ffn.py
--rw-r--r--   0        0        0      182 2024-03-28 01:09:02.081511 quant2-0.0.9/tests/football/data/test_utils.py
--rw-r--r--   0        0        0     4837 2024-03-30 03:57:24.923775 quant2-0.0.9/tools/experimental/train_table20240326_v1.py
--rw-r--r--   0        0        0     5038 2024-03-30 01:29:54.595817 quant2-0.0.9/tools/experimental/train_table20240326_v2.py
--rw-r--r--   0        0        0     2173 1970-01-01 00:00:00.000000 quant2-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      574 2024-04-06 14:41:03.615629 quant2-0.1.0/.gitignore
+-rw-r--r--   0        0        0    11357 2024-03-20 11:12:02.832412 quant2-0.1.0/LICENSE
+-rw-r--r--   0        0        0        7 2024-03-20 11:12:02.832412 quant2-0.1.0/README.md
+-rw-r--r--   0        0        0      969 2024-04-12 09:00:06.695344 quant2-0.1.0/configs/stnetv3/stnetv3_table20240326_2201to2312.cfg
+-rw-r--r--   0        0        0     1049 2024-04-12 08:57:23.226862 quant2-0.1.0/configs/stnetv4/stnetv4_table20240410_2201to2312.cfg
+-rw-r--r--   0        0        0      664 2024-04-10 00:12:18.347578 quant2-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1841 2024-03-23 05:01:23.359992 quant2-0.1.0/quant/README.md
+-rw-r--r--   0        0        0      559 2024-04-14 03:09:20.608493 quant2-0.1.0/quant/__init__.py
+-rw-r--r--   0        0        0       67 2024-03-23 04:17:48.269987 quant2-0.1.0/quant/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-08 01:35:10.284089 quant2-0.1.0/quant/evaluate/__init__.py
+-rw-r--r--   0        0        0     2646 2024-04-12 06:45:48.719809 quant2-0.1.0/quant/evaluate/table20240326.py
+-rw-r--r--   0        0        0     2006 2024-04-12 04:48:31.980573 quant2-0.1.0/quant/evaluate/utils.py
+-rw-r--r--   0        0        0      422 2024-03-23 04:21:50.819993 quant2-0.1.0/quant/football/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 14:09:03.305285 quant2-0.1.0/quant/football/data/__init__.py
+-rw-r--r--   0        0        0     4342 2024-04-12 06:01:55.322140 quant2-0.1.0/quant/football/data/dataset.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:24:35.916611 quant2-0.1.0/quant/football/data/functional.py
+-rw-r--r--   0        0        0     1329 2024-04-08 11:39:25.763545 quant2-0.1.0/quant/football/data/preprocessing.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:08:36.928001 quant2-0.1.0/quant/football/data/stats.py
+-rw-r--r--   0        0        0     4560 2024-04-13 08:19:58.059662 quant2-0.1.0/quant/football/data/utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 16:55:37.649284 quant2-0.1.0/quant/football/infer/__init__.py
+-rw-r--r--   0        0        0     1537 2024-04-11 17:24:14.938089 quant2-0.1.0/quant/football/infer/fastapi_app.py
+-rw-r--r--   0        0        0      468 2024-04-11 16:55:50.160241 quant2-0.1.0/quant/football/infer/fastapi_app_test.py
+-rw-r--r--   0        0        0     7795 2024-04-12 06:41:29.194262 quant2-0.1.0/quant/football/infer/football_infer_overunder_v1.py
+-rw-r--r--   0        0        0      473 2024-04-11 16:56:07.430215 quant2-0.1.0/quant/football/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 04:22:28.629548 quant2-0.1.0/quant/football/models/mtnet.py
+-rw-r--r--   0        0        0     6110 2024-04-11 17:12:37.365849 quant2-0.1.0/quant/football/models/stnet.py
+-rw-r--r--   0        0        0      295 2024-04-11 16:56:18.371576 quant2-0.1.0/quant/football/transforms/__init__.py
+-rw-r--r--   0        0        0     6526 2024-04-13 09:05:20.929454 quant2-0.1.0/quant/football/transforms/table20240326.py
+-rw-r--r--   0        0        0     8445 2024-04-13 08:16:37.019602 quant2-0.1.0/quant/football/transforms/table20240410.py
+-rw-r--r--   0        0        0        0 2024-03-31 10:26:04.538951 quant2-0.1.0/quant/layers/__init__.py
+-rw-r--r--   0        0        0      483 2024-03-28 09:12:19.609652 quant2-0.1.0/quant/layers/layer_scale.py
+-rw-r--r--   0        0        0     1070 2024-03-28 09:13:06.741829 quant2-0.1.0/quant/layers/mlp.py
+-rw-r--r--   0        0        0     1314 2024-03-28 09:40:33.643889 quant2-0.1.0/quant/layers/normalization.py
+-rw-r--r--   0        0        0      852 2024-03-28 09:16:09.540017 quant2-0.1.0/quant/layers/swiglu_ffn.py
+-rw-r--r--   0        0        0        0 2024-04-03 13:03:10.745509 quant2-0.1.0/quant/utils/__init__.py
+-rw-r--r--   0        0        0     1695 2024-04-11 16:56:25.721657 quant2-0.1.0/quant/utils/archive.py
+-rw-r--r--   0        0        0     1882 2024-04-13 12:43:31.456303 quant2-0.1.0/quant/utils/config.py
+-rw-r--r--   0        0        0     1047 2024-04-09 01:40:57.919653 quant2-0.1.0/quant/utils/io.py
+-rw-r--r--   0        0        0     1006 2024-04-03 13:19:59.255567 quant2-0.1.0/quant/utils/logging.py
+-rw-r--r--   0        0        0      182 2024-03-28 01:09:02.081511 quant2-0.1.0/tests/football/data/test_utils.py
+-rw-r--r--   0        0        0     1632 2024-04-12 06:45:57.389803 quant2-0.1.0/tools/analysis_tools/analyze_cls_results.py
+-rw-r--r--   0        0        0     2411 2024-04-13 14:52:53.164541 quant2-0.1.0/tools/experimental/make_dataset.py
+-rw-r--r--   0        0        0     1580 2024-04-13 14:41:36.176420 quant2-0.1.0/tools/experimental/make_split.py
+-rw-r--r--   0        0        0     6456 2024-04-14 03:08:49.930582 quant2-0.1.0/tools/experimental/nni_football.py
+-rw-r--r--   0        0        0      429 2024-04-14 03:05:10.735273 quant2-0.1.0/tools/experimental/nni_football_config.yaml
+-rw-r--r--   0        0        0     1578 2024-04-13 16:51:58.165877 quant2-0.1.0/tools/experimental/nni_football_config_search_space.json
+-rw-r--r--   0        0        0      523 2024-04-14 02:37:47.884925 quant2-0.1.0/tools/experimental/nni_model.py
+-rw-r--r--   0        0        0      420 2024-04-14 02:35:53.649253 quant2-0.1.0/tools/experimental/nni_model_config.yaml
+-rw-r--r--   0        0        0     2854 2024-04-12 06:25:44.029850 quant2-0.1.0/tools/fb_cls_test.py
+-rw-r--r--   0        0        0     5945 2024-04-13 12:40:38.861046 quant2-0.1.0/tools/fb_cls_train.py
+-rw-r--r--   0        0        0     2187 1970-01-01 00:00:00.000000 quant2-0.1.0/PKG-INFO
```

### Comparing `quant2-0.0.9/.gitignore` & `quant2-0.1.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -56,8 +56,11 @@
 docs/build/
 
 # Outputs
 results/
 runs/
 
 # Sync
-.sync
+.sync
+
+# Test
+ab*.ipynb
```

### Comparing `quant2-0.0.9/LICENSE` & `quant2-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quant2-0.0.9/quant/README.md` & `quant2-0.1.0/quant/README.md`

 * *Files identical despite different names*

### Comparing `quant2-0.0.9/quant/__init__.py` & `quant2-0.1.0/quant/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A collection of useful tools!"""
 import sys
 
-__version__ = "0.0.9"
+__version__ = "0.1.0"
 
 help_doc_str = """\
 usage: quant [--version] [--help]
 
 shell command:
     quant -h
```

### Comparing `quant2-0.0.9/quant/football/data/utils.py` & `quant2-0.1.0/quant/football/data/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,63 @@
 import copy
 import numpy as np
 from datetime import datetime
 from prettytable import PrettyTable
-from typing import Union
+from typing import Optional, Union
 
 
 def time_secs2str(secs: Union[int, float]):
     return datetime.fromtimestamp(secs).strftime("%Y-%m-%d %H:%M:%S")
 
 
-def time_str2secs(text: str, year: str = None):
-    str_date, str_time = text.split(" ")
+def time_str2secs(text: str, year: Optional[str] = None):
+    if " " in text:
+        str_date, str_time = text.split(" ")
+    else:
+        str_date, str_time = text, "00:00:00"
 
     arr_date = [f"0{s}" if len(s) == 1 else s for s in str_date.split("-")]
     arr_time = [f"0{s}" if len(s) == 1 else s for s in str_time.split(":")]
 
     if year is not None and len(arr_date) == 2:
         arr_date = [year] + arr_date
 
     text = "-".join(arr_date) + " " + ":".join(arr_time)
     return datetime.fromisoformat(text).timestamp()
 
 
-def get_start_time(data: list[dict]):
+def extract_start_time(data: list[dict]):
+    # data = [dict(match_id=, match_time=, match_state=, real_start_time=, ...)]
     first_start_time, second_start_time = 0, 0
     for row in data:
         if row["match_state"] == "1":  # 上半场
             first_start_time = max(first_start_time, row["real_start_time"])
         elif row["match_state"] == "3":  # 下半场
             second_start_time = max(second_start_time, row["real_start_time"])
     return int(first_start_time), int(second_start_time)
 
 
-def trans_odds_data(data: list[list]):
+def convert_odds_data(data: list[list]):
+    # data = [['77', '1-2', '1.60', '3.5', '0.47', '10-02 00:39', '滚']]
     def _trans(val):
         if isinstance(val, str):
             if "/" in val:  # 2.5/3
                 nums = [float(s) for s in val.split("/")]
                 return f"{sum(nums)/len(nums):.2f}"
             return val
         return ""
 
+    data = [["", ""] + v if len(v) == 5 else v for v in data]
+
+    assert all([len(v) == 7 for v in data]), "Odds data must be a list of length 7."
     return [[_trans(vi) for vi in v] for v in data if "封" not in v]
 
 
-def x_avg_max_min(data: list, weights: list = None):
-    if len(data) < 1:
-        return [-1.0, -1.0, -1.0]
+def sequence_avg_max_min(data: list, weights: Optional[list] = None):
+    assert len(data) > 1
 
     if isinstance(data[0], str):
         data = [float(x) for x in data]
 
     if weights is not None:
         x_avg = sum([x * w for x, w in zip(data, weights)]) / sum(weights)
     else:
@@ -58,76 +65,72 @@
 
     x_max = max(data)
     x_min = min(data)
 
     return [x_avg, x_max, x_min]
 
 
-def odds_avg_max_min(data: list[list]):
-    data = trans_odds_data(data)
-    x1 = x_avg_max_min([row[2] for row in data])
-    x2 = x_avg_max_min([row[3] for row in data])
-    x3 = x_avg_max_min([row[4] for row in data])
+def odds_data_avg_max_min(data: list[list]):
+    # data = [['77', '1-2', '1.60', '3.5', '0.47', '10-02 00:39', '滚']]
+    data = convert_odds_data(data)
+    x1 = sequence_avg_max_min([row[2] for row in data])
+    x2 = sequence_avg_max_min([row[3] for row in data])
+    x3 = sequence_avg_max_min([row[4] for row in data])
     return x1 + x2 + x3
 
 
-def cycle_difference(seq: list, cycle: int, keeps: list[int]):
-    mat = np.asarray(seq).reshape((-1, cycle))
+def cycle_difference(seq: list, cycle_size: int, keep_columns: list[int]):
+    # seq = [x1, x2, x3, x1, x2, x3, x1, x2, x3, ...]
+    mat = np.asarray(seq).reshape((-1, cycle_size))
 
     ref = np.zeros_like(mat)
     ref[1:, :] = mat[:-1, :]
 
-    for idx in keeps:
+    for idx in keep_columns:
         ref[:, idx] = 0
 
     ref[mat < 0] = 0
 
     return (mat - ref).reshape(-1).tolist()
 
 
-def filter_samples(data: list[list], start_idxs: list, end_idxs: list):
-    assert (
-        isinstance(start_idxs, list)
-        and isinstance(end_idxs, list)
-        and len(start_idxs) == len(end_idxs)
-    )
-
-    check_list = []
-    for start_idx, end_idx in zip(start_idxs, end_idxs):
-        for idx in range(start_idx, end_idx):
-            check_list.append(idx)
-
-    data = copy.deepcopy(data)
+def train_test(data: list[list], date_sep: str, date_min: str = "2020-01-01", date_max: str = "2099-01-01"):
+    _data = copy.deepcopy(data)
 
-    _data = []
-    for row in data:
-        if any([row[idx] < 0 for idx in check_list]):
+    date_sep = time_str2secs(date_sep)
+    date_min = time_str2secs(date_min)
+    date_max = time_str2secs(date_max)
+
+    train_data, test_data = [], []
+    for row in _data:
+        ts = row[1]  # match_time
+        if ts < date_min:
             continue
-        _data.append(row)
-    return _data
-
-
-def train_val(data: list[list], point: str = "2023-12-01 00:00:01"):
-    data = copy.deepcopy(data)
-    point = time_str2secs(point)
-
-    train_data, val_data = [], []
-    for row in data:
-        if row[1] < point:  # match_time
+        elif ts < date_sep:
             train_data.append(row)
-        else:
-            val_data.append(row)
+        elif ts < date_max:
+            test_data.append(row)
 
-    return train_data, val_data
+    return train_data, test_data
 
 
 def one_hot_encoder(names: list[str]):
     names = sorted(set(names))
     eye = np.eye(len(names), k=0, dtype=int)
     encoder = {n: v for n, v in zip(names, eye.tolist())}
+    encoder["__len__"] = len(names)
+    encoder["__dim__"] = len(names)
+    return encoder
+
+
+def label_encoder(names: list[str]):
+    names = sorted(set(names))
+    encoder = {n: [i] for i, n in enumerate(names)}
+    encoder["__len__"] = len(names)
+    encoder["__dim__"] = 1
     return encoder
 
 
 def count_values(data: list, sort_by: str = "label"):
     counts = {}
     for x in data:
         if x in counts:
```

### Comparing `quant2-0.0.9/quant/layers/mlp.py` & `quant2-0.1.0/quant/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `quant2-0.0.9/quant/layers/normalization.py` & `quant2-0.1.0/quant/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `quant2-0.0.9/quant/layers/swiglu_ffn.py` & `quant2-0.1.0/quant/layers/swiglu_ffn.py`

 * *Files identical despite different names*

### Comparing `quant2-0.0.9/tools/experimental/train_table20240326_v1.py` & `quant2-0.1.0/tools/fb_cls_train.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,136 +1,165 @@
-# 1) PYTHONPATH=$(pwd) python tools/experimental/train_table20240326_v1.py
-# 2) python tools/experimental/train_table20240326_v1.py
+# PYTHONPATH=$(pwd) python tools/fb_cls_train.py
 import numpy as np
 import random
+import sys
 import time
 import torch
-import torch.nn as nn
-import torch.nn.functional as F
+from copy import deepcopy
 from pathlib import Path
-from quant.football.data.dataset import ClassificationDataset
-from quant.layers.normalization import RMSNorm
-from quant.layers.swiglu_ffn import SwiGLUFFN
-from torch.optim.lr_scheduler import StepLR
+from quant.football.data.dataset import get_dataset
+from quant.football.models import get_model
+from quant.utils.config import get_config, merge_from_dict
+from quant.utils.io import copy_file, save_json
+from quant.utils.logging import get_logger, print_log
 
 
-def init_weights(m):
-    if isinstance(m, nn.Linear):
-        nn.init.normal_(m.weight, 0, 0.02)
-        if hasattr(m, "bias") and m.bias is not None:
-            nn.init.constant_(m.bias, 0.0)
-
-
-class Net(nn.Module):
-
-    def __init__(self, in_features, hidden_features, out_features, bias=True):
-        super(Net, self).__init__()
-        self.emb = nn.Linear(in_features, hidden_features, bias=bias)
-        self.ffn_norm = RMSNorm(hidden_features)
-        self.ffn = SwiGLUFFN(hidden_features, bias=bias)
-        self.out_norm = RMSNorm(hidden_features)
-        self.out = nn.Linear(hidden_features, out_features, bias=bias)
-
-    def forward(self, x):
-        x = F.silu(self.emb(x))
-        x = F.silu(self.ffn(self.ffn_norm(x)))
-        x = self.out(self.out_norm(x))
-        return x
-
-
-def train(model, device, train_loader, criterion, optimizer, epoch, log_interval=10, dry_run=False):
+def train(model, device, train_loader, loss_fn, optimizer, epoch, log_interval, verbose, logger):
     model.train()
-    for batch_idx, (data, target) in enumerate(train_loader):
-        data, target = data.to(device), target.to(device)
+    dataloader_size = len(train_loader)
+    for batch_idx, (data, target) in enumerate(train_loader, 1):
+        data = [e.to(device) for e in data] if isinstance(
+            data, (list, tuple)) else data.to(device)
+        target = [e.to(device) for e in target] if isinstance(
+            target, (list, tuple)) else target.to(device)
         optimizer.zero_grad()
         output = model(data)
-        loss = criterion(output, target)
+        loss = loss_fn(output, target)
         loss.backward()
         optimizer.step()
         if batch_idx % log_interval == 0:
-            print("Train Epoch: {} [{}/{} ({:.0f}%)]\tLoss: {:.6f}".format(
-                epoch, batch_idx * len(data), len(train_loader.dataset),
-                100. * batch_idx / len(train_loader), loss.item()))
-            if dry_run:
-                break
+            print_log(
+                f"Train Epoch: {epoch} [{batch_idx}/{dataloader_size}] Loss: {loss.item():.6f}", verbose, logger)
 
 
-def test(model, device, test_loader, criterion):
+def test(model, device, test_loader, loss_fn, verbose, logger):
     model.eval()
-    test_loss = 0
-    correct = 0
+    test_loss, correct = 0, 0
     with torch.no_grad():
         for data, target in test_loader:
-            data, target = data.to(device), target.to(device)
+            data = [e.to(device) for e in data] if isinstance(
+                data, (list, tuple)) else data.to(device)
+            target = [e.to(device) for e in target] if isinstance(
+                target, (list, tuple)) else target.to(device)
             output = model(data)
-            test_loss += criterion(output, target).item()
+            test_loss += loss_fn(output, target).item()
             pred = output.argmax(dim=1, keepdim=True)
             correct += pred.eq(target.view_as(pred)).sum().item()
 
     test_loss /= len(test_loader)
+    dataset_size = len(test_loader.dataset)
+    test_acc = correct / dataset_size
 
-    print("\nTest set: Average loss: {:.4f}, Accuracy: {}/{} ({:.0f}%)\n".format(
-        test_loss, correct, len(test_loader.dataset),
-        100. * correct / len(test_loader.dataset)))
-    return correct / len(test_loader.dataset)
-
+    print_log(
+        f"\nTest set: Avg loss: {test_loss:.6f}, Acc: {correct}/{dataset_size} ({test_acc:.4f})\n", verbose, logger)
+    return test_acc
+
+
+def main(cfg, verbose=True):
+    _cfg = deepcopy(cfg)
+    data, model, loss, optimizer, scheduler, runtime = \
+        cfg["data"], cfg["model"], cfg["loss"], cfg["optimizer"], cfg["scheduler"], cfg["runtime"]
+
+    seed = runtime.get("seed", 1)
+    epochs = runtime.get("epochs", 90)
+    device = runtime.get("device", "cuda")
+    log_interval = runtime.get("log_interval", 10)
 
-def main(train_file, test_file, seed=1, device="cuda", batch_size=128, lr=0.1, epochs=90, log_interval=10):
     random.seed(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
     torch.backends.cudnn.deterministic = True
     torch.backends.cudnn.benchmark = False
 
     if device == "cuda" and torch.cuda.is_available():
         device = torch.device("cuda")
     else:
         device = torch.device("cpu")
 
-    train_dataset = ClassificationDataset(train_file)
-    test_dataset = ClassificationDataset(test_file)
+    dataset_type = data.pop("type")
+    data_root = Path(data["data_root"])
+    train_dataset = get_dataset(dataset_type, data_root / data["train_file"])
+    test_dataset = get_dataset(dataset_type, data_root / data["test_file"])
 
     train_loader = torch.utils.data.DataLoader(
-        train_dataset, batch_size=batch_size, shuffle=True
+        train_dataset, batch_size=data["batch_size"], shuffle=True
     )
     test_loader = torch.utils.data.DataLoader(
-        test_dataset, batch_size=1
+        test_dataset, batch_size=128
     )
 
-    model = Net(806, 384, 10, bias=True).to(device)
-    # model.apply(init_weights)
-    criterion = nn.CrossEntropyLoss().to(device)
-    optimizer = torch.optim.SGD(model.parameters(), lr, 0.9, weight_decay=1e-4)
-    scheduler = StepLR(optimizer, step_size=30, gamma=0.1)
-    out_dir = Path("runs") / time.strftime("%m%d%H%M%S")
+    model_type = model.pop("type")
+    model = get_model(model_type, **model).to(device)
+
+    loss_type = loss.pop("type")
+    if loss_type == "CrossEntropyLoss":
+        from torch.nn import CrossEntropyLoss
+        loss_fn = CrossEntropyLoss(**loss).to(device)
+    else:
+        raise NotImplementedError(f"Not supported <{loss_type}>.")
+
+    optimizer_type = optimizer.pop("type")
+    if optimizer_type == "SGD":
+        from torch.optim import SGD
+        optimizer = SGD(model.parameters(), **optimizer)
+    elif optimizer_type == "AdamW":
+        from torch.optim import AdamW
+        optimizer = AdamW(model.parameters(), **optimizer)
+    else:
+        raise NotImplementedError(f"Not supported <{optimizer_type}>.")
+
+    scheduler_type = scheduler.pop("type")
+    if scheduler_type == "StepLR":
+        from torch.optim.lr_scheduler import StepLR
+        scheduler = StepLR(optimizer, **scheduler)
+    else:
+        raise NotImplementedError(f"Not supported <{scheduler_type}>.")
+
+    out_dir = Path("runs") / data_root.name / time.strftime("%Y%m%d%H%M%S")
     out_dir.mkdir(parents=True, exist_ok=True)
-    best_acc = 0.0
-    best_epoch = -1
+    copy_file(data_root, out_dir, "*.cfg")
+
+    logger = get_logger(__name__, False, out_dir / "log.txt")
+
+    best_acc, best_epoch = 0.0, -1
     for epoch in range(1, epochs + 1):
-        train(model, device, train_loader, criterion,
-              optimizer, epoch, log_interval)
-        curr_acc = test(model, device, test_loader, criterion)
+        train(model, device, train_loader, loss_fn, optimizer,
+              epoch, log_interval, verbose, logger)
+        curr_acc = test(model, device, test_loader, loss_fn,
+                        verbose, logger)
         if curr_acc > best_acc:
             best_acc, best_epoch = curr_acc, epoch
+            torch.save(model.state_dict(), out_dir / "best.pt")
         scheduler.step()
-        torch.save(model.state_dict(), out_dir / f"model{epoch:03d}.pt")
+    torch.save(model.state_dict(), out_dir / "last.pt")
 
-    print("[best model]")
-    print(f"\n{best_acc=:.5f}, {best_epoch=}, path={out_dir}\n")
+    print_log("[best model]", verbose, logger)
+    print_log(f"\noutput dir: {out_dir}", verbose, logger)
+    print_log(f"{best_acc=:.4f}, {best_epoch=:03d}\n", verbose, logger)
+
+    print_log("[check train dataset]", verbose, logger)
+    check_loader = torch.utils.data.DataLoader(train_dataset, batch_size=128)
+    acc_train = test(model, device, check_loader, loss_fn,
+                     verbose, logger)
+
+    _cfg["log"] = {
+        "out_dir": str(out_dir),
+        "date": time.strftime("%Y-%m-%d %H:%M:%S"),
+        "best_acc": best_acc,
+        "best_epoch": best_epoch,
+        "acc_train": acc_train,
+    }
+    save_json(out_dir / "model.cfg", _cfg, indent=4)
 
-    print("[check train dataset]")
-    check_loader = torch.utils.data.DataLoader(train_dataset, batch_size=1)
-    test(model, device, check_loader, criterion)
+    return best_acc, _cfg
 
 
 if __name__ == "__main__":
-    data_root = Path("/workspace/xlab/datasets")
-    main(
-        train_file=data_root / "table20240326_03281154_torch_norm/20240329_101534.dat",
-        test_file=data_root / "table20240326_03281154_torch_norm/20240329_101539.dat",
-        seed=1,
-        device="cuda",
-        batch_size=128,
-        lr=0.1,
-        epochs=90,
-        log_interval=10,
-    )
+    options = {}
+    for arg in sys.argv[1:]:
+        key, val = arg.split("=", maxsplit=1)
+        options[key] = eval(val)
+
+    cfg = get_config(options.get("config", None))
+    cfg = merge_from_dict(cfg, options)
+
+    main(cfg)
```

### Comparing `quant2-0.0.9/PKG-INFO` & `quant2-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: quant2
-Version: 0.0.9
+Version: 0.1.0
 Summary: A collection of useful tools!
 Author-email: Hejian <flystarhe@qq.com>
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: simplejson
-Requires-Dist: requests >=2.6
+Requires-Dist: numpy
+Requires-Dist: prettytable
 Requires-Dist: scikit-learn
+Requires-Dist: torch
 Project-URL: Home, https://github.com/flystarhe/quant
 
 A collection of useful tools!
 
 ## Publish
 [quant2 · PyPI](https://pypi.org/project/quant2/)
 ```sh
```


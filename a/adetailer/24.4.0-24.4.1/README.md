# Comparing `tmp/adetailer-24.4.0.tar.gz` & `tmp/adetailer-24.4.1.tar.gz`

## Comparing `adetailer-24.4.0.tar` & `adetailer-24.4.1.tar`

### file list

```diff
@@ -1,39 +1,44 @@
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 adetailer-24.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    15469 2020-02-02 00:00:00.000000 adetailer-24.4.0/CHANGELOG.md
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 adetailer-24.4.0/Taskfile.yml
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 adetailer-24.4.0/install.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 adetailer-24.4.0/preload.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 adetailer-24.4.0/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 adetailer-24.4.0/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 adetailer-24.4.0/.github/ISSUE_TEMPLATE/question.yaml
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 adetailer-24.4.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 adetailer-24.4.0/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 adetailer-24.4.0/.github/workflows/stale.yml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 adetailer-24.4.0/.vscode/extensions.json
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 adetailer-24.4.0/.vscode/settings.json
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 adetailer-24.4.0/adetailer/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 adetailer-24.4.0/adetailer/__version__.py
--rw-r--r--   0        0        0     8701 2020-02-02 00:00:00.000000 adetailer-24.4.0/adetailer/args.py
--rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 adetailer-24.4.0/adetailer/common.py
--rw-r--r--   0        0        0     6995 2020-02-02 00:00:00.000000 adetailer-24.4.0/adetailer/mask.py
--rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 adetailer-24.4.0/adetailer/mediapipe.py
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 adetailer-24.4.0/adetailer/traceback.py
--rw-r--r--   0        0        0    23157 2020-02-02 00:00:00.000000 adetailer-24.4.0/adetailer/ui.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 adetailer-24.4.0/adetailer/ultralytics.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 adetailer-24.4.0/controlnet_ext/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 adetailer-24.4.0/controlnet_ext/common.py
--rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 adetailer-24.4.0/controlnet_ext/controlnet_ext.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 adetailer-24.4.0/controlnet_ext/controlnet_ext_forge.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 adetailer-24.4.0/controlnet_ext/restore.py
--rw-r--r--   0        0        0    35424 2020-02-02 00:00:00.000000 adetailer-24.4.0/scripts/!adetailer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adetailer-24.4.0/tests/__init__.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 adetailer-24.4.0/tests/conftest.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 adetailer-24.4.0/tests/test_common.py
--rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 adetailer-24.4.0/tests/test_mask.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 adetailer-24.4.0/tests/test_mediapipe.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 adetailer-24.4.0/tests/test_ultralytics.py
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 adetailer-24.4.0/.gitignore
--rw-r--r--   0        0        0    34931 2020-02-02 00:00:00.000000 adetailer-24.4.0/LICENSE.md
--rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 adetailer-24.4.0/README.md
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 adetailer-24.4.0/pyproject.toml
--rw-r--r--   0        0        0     9009 2020-02-02 00:00:00.000000 adetailer-24.4.0/PKG-INFO
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 adetailer-24.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    15889 2020-02-02 00:00:00.000000 adetailer-24.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 adetailer-24.4.1/Taskfile.yml
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 adetailer-24.4.1/install.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 adetailer-24.4.1/preload.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 adetailer-24.4.1/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 adetailer-24.4.1/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 adetailer-24.4.1/.github/ISSUE_TEMPLATE/question.yaml
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 adetailer-24.4.1/.github/workflows/notlint.yml
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 adetailer-24.4.1/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 adetailer-24.4.1/.github/workflows/stale.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 adetailer-24.4.1/.vscode/extensions.json
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 adetailer-24.4.1/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adetailer-24.4.1/aaaaaa/__init__.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 adetailer-24.4.1/aaaaaa/conditional.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 adetailer-24.4.1/aaaaaa/helper.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 adetailer-24.4.1/aaaaaa/p_method.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 adetailer-24.4.1/adetailer/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 adetailer-24.4.1/adetailer/__version__.py
+-rw-r--r--   0        0        0     9190 2020-02-02 00:00:00.000000 adetailer-24.4.1/adetailer/args.py
+-rw-r--r--   0        0        0     4346 2020-02-02 00:00:00.000000 adetailer-24.4.1/adetailer/common.py
+-rw-r--r--   0        0        0     6995 2020-02-02 00:00:00.000000 adetailer-24.4.1/adetailer/mask.py
+-rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 adetailer-24.4.1/adetailer/mediapipe.py
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 adetailer-24.4.1/adetailer/traceback.py
+-rw-r--r--   0        0        0    23810 2020-02-02 00:00:00.000000 adetailer-24.4.1/adetailer/ui.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 adetailer-24.4.1/adetailer/ultralytics.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 adetailer-24.4.1/controlnet_ext/__init__.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 adetailer-24.4.1/controlnet_ext/common.py
+-rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 adetailer-24.4.1/controlnet_ext/controlnet_ext.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 adetailer-24.4.1/controlnet_ext/controlnet_ext_forge.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 adetailer-24.4.1/controlnet_ext/restore.py
+-rw-r--r--   0        0        0    34616 2020-02-02 00:00:00.000000 adetailer-24.4.1/scripts/!adetailer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adetailer-24.4.1/tests/__init__.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 adetailer-24.4.1/tests/conftest.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 adetailer-24.4.1/tests/test_args.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 adetailer-24.4.1/tests/test_common.py
+-rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 adetailer-24.4.1/tests/test_mask.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 adetailer-24.4.1/tests/test_mediapipe.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 adetailer-24.4.1/tests/test_ultralytics.py
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 adetailer-24.4.1/.gitignore
+-rw-r--r--   0        0        0    34270 2020-02-02 00:00:00.000000 adetailer-24.4.1/LICENSE.md
+-rw-r--r--   0        0        0     8597 2020-02-02 00:00:00.000000 adetailer-24.4.1/README.md
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 adetailer-24.4.1/pyproject.toml
+-rw-r--r--   0        0        0     9185 2020-02-02 00:00:00.000000 adetailer-24.4.1/PKG-INFO
```

### Comparing `adetailer-24.4.0/.pre-commit-config.yaml` & `adetailer-24.4.1/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -11,22 +11,18 @@
       - id: check-case-conflict
       - id: check-ast
       - id: trailing-whitespace
         args: [--markdown-linebreak-ext=md]
       - id: end-of-file-fixer
       - id: mixed-line-ending
 
-  - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.5
-    hooks:
-      - id: ruff
-        args: [--fix, --exit-non-zero-on-fix]
-
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v4.0.0-alpha.8"
     hooks:
       - id: prettier
 
-  - repo: https://github.com/psf/black-pre-commit-mirror
-    rev: 24.3.0
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.3.7
     hooks:
-      - id: black
+      - id: ruff
+        args: [--fix, --exit-non-zero-on-fix]
+      - id: ruff-format
```

### Comparing `adetailer-24.4.0/CHANGELOG.md` & `adetailer-24.4.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+## 2024-04-14
+
+- v24.4.1
+- webui 1.9.0에서 발생한 에러 수정
+  - extra generation params에 callable이 들어와서 생긴 문제
+  - assign_current_image에 None이 들어갈 수 있던 문제
+- webui 1.9.0에서 변경된 scheduler 지원
+- 컨트롤넷 모델을 찾을 때, 대소문자 구분을 하지 않음 (PR #577)
+- 몇몇 기능을 스크립트에서 분리하여 별도 파일로 빼냄
+
 ## 2024-04-10
 
 - v24.4.0
 - txt2img에서 hires를 설정했을 때, 이미지의 exif에서 Denoising Strength가 adetailer의 denoisiog stregnth로 덮어 쓰이는 문제 수정
 - ad prompt, ad negative prompt에 프롬프트를 변경하는 기능을 적용했을 때(와일드카드 등), 적용된 프롬프트가 이미지의 exif에 제대로 표시됨
 
 ## 2024-03-29
```

### Comparing `adetailer-24.4.0/Taskfile.yml` & `adetailer-24.4.1/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `adetailer-24.4.0/install.py` & `adetailer-24.4.1/install.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.4.0/.github/ISSUE_TEMPLATE/bug_report.yaml` & `adetailer-24.4.1/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `adetailer-24.4.0/.github/ISSUE_TEMPLATE/feature_request.yaml` & `adetailer-24.4.1/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `adetailer-24.4.0/adetailer/args.py` & `adetailer-24.4.1/adetailer/args.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,14 +78,15 @@
     ad_cfg_scale: NonNegativeFloat = 7.0
     ad_use_checkpoint: bool = False
     ad_checkpoint: Optional[str] = None
     ad_use_vae: bool = False
     ad_vae: Optional[str] = None
     ad_use_sampler: bool = False
     ad_sampler: str = "DPM++ 2M Karras"
+    ad_scheduler: str = "Use same scheduler"
     ad_use_noise_multiplier: bool = False
     ad_noise_multiplier: confloat(ge=0.5, le=1.5) = 1.0
     ad_use_clip_skip: bool = False
     ad_clip_skip: conint(ge=1, le=12) = 1
     ad_restore_face: bool = False
     ad_controlnet_model: str = "None"
     ad_controlnet_module: str = "None"
@@ -156,16 +157,21 @@
         )
         ppop(
             "ADetailer use separate VAE",
             ["ADetailer use separate VAE", "ADetailer VAE"],
         )
         ppop(
             "ADetailer use separate sampler",
-            ["ADetailer use separate sampler", "ADetailer sampler"],
+            [
+                "ADetailer use separate sampler",
+                "ADetailer sampler",
+                "ADetailer scheduler",
+            ],
         )
+        ppop("ADetailer scheduler", cond="Use same scheduler")
         ppop(
             "ADetailer use separate noise multiplier",
             ["ADetailer use separate noise multiplier", "ADetailer noise multiplier"],
         )
 
         ppop(
             "ADetailer use separate CLIP skip",
@@ -221,14 +227,15 @@
     ("ad_cfg_scale", "ADetailer CFG scale"),
     ("ad_use_checkpoint", "ADetailer use separate checkpoint"),
     ("ad_checkpoint", "ADetailer checkpoint"),
     ("ad_use_vae", "ADetailer use separate VAE"),
     ("ad_vae", "ADetailer VAE"),
     ("ad_use_sampler", "ADetailer use separate sampler"),
     ("ad_sampler", "ADetailer sampler"),
+    ("ad_scheduler", "ADetailer scheduler"),
     ("ad_use_noise_multiplier", "ADetailer use separate noise multiplier"),
     ("ad_noise_multiplier", "ADetailer noise multiplier"),
     ("ad_use_clip_skip", "ADetailer use separate CLIP skip"),
     ("ad_clip_skip", "ADetailer CLIP skip"),
     ("ad_restore_face", "ADetailer restore face"),
     ("ad_controlnet_model", "ADetailer ControlNet model"),
     ("ad_controlnet_module", "ADetailer ControlNet module"),
@@ -243,7 +250,18 @@
 BBOX_SORTBY = [
     "None",
     "Position (left to right)",
     "Position (center to edge)",
     "Area (large to small)",
 ]
 MASK_MERGE_INVERT = ["None", "Merge", "Merge and Invert"]
+
+_script_default = (
+    "dynamic_prompting",
+    "dynamic_thresholding",
+    "wildcard_recursive",
+    "wildcards",
+    "lora_block_weight",
+    "negpip",
+    "soft_inpainting",
+)
+SCRIPT_DEFAULT = ",".join(sorted(_script_default))
```

### Comparing `adetailer-24.4.0/adetailer/common.py` & `adetailer-24.4.1/adetailer/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import os
 from collections import OrderedDict
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Any, Optional
 
 from huggingface_hub import hf_hub_download
 from PIL import Image, ImageDraw
@@ -33,24 +34,35 @@
         msg = f"[-] ADetailer: Failed to load model {file!r} from huggingface"
         print(msg)
         path = "INVALID"
         _download_failed = True
     return path
 
 
-def scan_model_dir(path_: str | Path) -> list[Path]:
-    if not path_ or not (path := Path(path_)).is_dir():
+def safe_mkdir(path: str | os.PathLike[str]) -> None:
+    path = Path(path)
+    if not path.exists() and path.parent.exists() and os.access(path.parent, os.W_OK):
+        path.mkdir()
+
+
+def scan_model_dir(path: Path) -> list[Path]:
+    if not path.is_dir():
         return []
-    return [p for p in path.rglob("*") if p.is_file() and p.suffix in (".pt", ".pth")]
+    return [p for p in path.rglob("*") if p.is_file() and p.suffix == ".pt"]
 
 
 def get_models(
-    model_dir: str | Path, extra_dir: str | Path = "", huggingface: bool = True
+    *dirs: str | os.PathLike[str], huggingface: bool = True
 ) -> OrderedDict[str, str]:
-    model_paths = [*scan_model_dir(model_dir), *scan_model_dir(extra_dir)]
+    model_paths = []
+
+    for dir_ in dirs:
+        if not dir_:
+            continue
+        model_paths.extend(scan_model_dir(Path(dir_)))
 
     models = OrderedDict()
     if huggingface:
         models.update(
             {
                 "face_yolov8n.pt": hf_download("face_yolov8n.pt"),
                 "face_yolov8s.pt": hf_download("face_yolov8s.pt"),
```

### Comparing `adetailer-24.4.0/adetailer/mask.py` & `adetailer-24.4.1/adetailer/mask.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.4.0/adetailer/mediapipe.py` & `adetailer-24.4.1/adetailer/mediapipe.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.4.0/adetailer/traceback.py` & `adetailer-24.4.1/adetailer/traceback.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.4.0/adetailer/ui.py` & `adetailer-24.4.1/adetailer/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         return [getattr(self, attr) for attr in ALL_ARGS.attrs]
 
 
 @dataclass
 class WebuiInfo:
     ad_model_list: list[str]
     sampler_names: list[str]
+    scheduler_names: list[str]
     t2i_button: gr.Button
     i2i_button: gr.Button
     checkpoints_list: list[str]
     vae_list: list[str]
 
 
 def gr_interactive(value: bool = True):
@@ -533,28 +534,41 @@
             w.ad_use_sampler = gr.Checkbox(
                 label="Use separate sampler" + suffix(n),
                 value=False,
                 visible=True,
                 elem_id=eid("ad_use_sampler"),
             )
 
-            w.ad_sampler = gr.Dropdown(
-                label="ADetailer sampler" + suffix(n),
-                choices=webui_info.sampler_names,
-                value=webui_info.sampler_names[0],
-                visible=True,
-                elem_id=eid("ad_sampler"),
-            )
+            with gr.Row():
+                w.ad_sampler = gr.Dropdown(
+                    label="ADetailer sampler" + suffix(n),
+                    choices=webui_info.sampler_names,
+                    value=webui_info.sampler_names[0],
+                    visible=True,
+                    elem_id=eid("ad_sampler"),
+                )
+
+                scheduler_names = [
+                    "Use same scheduler",
+                    *webui_info.scheduler_names,
+                ]
+                w.ad_scheduler = gr.Dropdown(
+                    label="ADetailer scheduler" + suffix(n),
+                    choices=scheduler_names,
+                    value=scheduler_names[0],
+                    visible=len(scheduler_names) > 1,
+                    elem_id=eid("ad_scheduler"),
+                )
 
-            w.ad_use_sampler.change(
-                gr_interactive,
-                inputs=w.ad_use_sampler,
-                outputs=w.ad_sampler,
-                queue=False,
-            )
+                w.ad_use_sampler.change(
+                    lambda value: (gr_interactive(value), gr_interactive(value)),
+                    inputs=w.ad_use_sampler,
+                    outputs=[w.ad_sampler, w.ad_scheduler],
+                    queue=False,
+                )
 
         with gr.Row():
             with gr.Column(variant="compact"):
                 w.ad_use_noise_multiplier = gr.Checkbox(
                     label="Use separate noise multiplier" + suffix(n),
                     value=False,
                     visible=True,
```

### Comparing `adetailer-24.4.0/adetailer/ultralytics.py` & `adetailer-24.4.1/adetailer/ultralytics.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.4.0/controlnet_ext/__init__.py` & `adetailer-24.4.1/controlnet_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.4.0/controlnet_ext/controlnet_ext.py` & `adetailer-24.4.1/controlnet_ext/controlnet_ext.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.4.0/controlnet_ext/controlnet_ext_forge.py` & `adetailer-24.4.1/controlnet_ext/controlnet_ext_forge.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.4.0/controlnet_ext/restore.py` & `adetailer-24.4.1/controlnet_ext/restore.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.4.0/scripts/!adetailer.py` & `adetailer-24.4.1/scripts/!adetailer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,48 @@
 from __future__ import annotations
 
-import os
 import platform
 import re
 import sys
 import traceback
-from contextlib import contextmanager, suppress
+from contextlib import suppress
 from copy import copy
 from functools import partial
 from pathlib import Path
 from textwrap import dedent
-from typing import TYPE_CHECKING, Any, NamedTuple
+from typing import TYPE_CHECKING, Any, NamedTuple, cast
 
 import gradio as gr
-import torch
 from PIL import Image, ImageChops
 from rich import print
 
 import modules
+from aaaaaa.conditional import create_binary_mask, schedulers
+from aaaaaa.helper import (
+    change_torch_load,
+    copy_extra_params,
+    pause_total_tqdm,
+    preseve_prompts,
+)
+from aaaaaa.p_method import (
+    get_i,
+    is_img2img_inpaint,
+    is_inpaint_only_masked,
+    need_call_postprocess,
+    need_call_process,
+)
 from adetailer import (
     AFTER_DETAILER,
     __version__,
     get_models,
     mediapipe_predict,
     ultralytics_predict,
 )
-from adetailer.args import BBOX_SORTBY, ADetailerArgs, SkipImg2ImgOrig
-from adetailer.common import PredictOutput, ensure_pil_image
+from adetailer.args import BBOX_SORTBY, SCRIPT_DEFAULT, ADetailerArgs, SkipImg2ImgOrig
+from adetailer.common import PredictOutput, ensure_pil_image, safe_mkdir
 from adetailer.mask import (
     filter_by_ratio,
     filter_k_largest,
     has_intersection,
     is_all_black,
     mask_preprocess,
     sort_bboxes,
@@ -41,88 +53,48 @@
     CNHijackRestore,
     ControlNetExt,
     cn_allow_script_control,
     controlnet_exists,
     controlnet_type,
     get_cn_models,
 )
-from modules import images, paths, safe, script_callbacks, scripts, shared
+from modules import images, paths, script_callbacks, scripts, shared
 from modules.devices import NansException
 from modules.processing import (
     Processed,
     StableDiffusionProcessingImg2Img,
     create_infotext,
     process_images,
 )
 from modules.sd_samplers import all_samplers
 from modules.shared import cmd_opts, opts, state
 
-try:
-    from modules.processing import create_binary_mask
-except ImportError:
-
-    def create_binary_mask(image: Image.Image):
-        return image.convert("L")
-
-
 if TYPE_CHECKING:
     from fastapi import FastAPI
 
 no_huggingface = getattr(cmd_opts, "ad_no_huggingface", False)
 adetailer_dir = Path(paths.models_path, "adetailer")
+safe_mkdir(adetailer_dir)
+
 extra_models_dir = shared.opts.data.get("ad_extra_models_dir", "")
 model_mapping = get_models(
-    adetailer_dir, extra_dir=extra_models_dir, huggingface=not no_huggingface
+    adetailer_dir,
+    extra_models_dir,
+    huggingface=not no_huggingface,
 )
-txt2img_submit_button = img2img_submit_button = None
-SCRIPT_DEFAULT = "dynamic_prompting,dynamic_thresholding,wildcard_recursive,wildcards,lora_block_weight,negpip,soft_inpainting"
 
-if (
-    not adetailer_dir.exists()
-    and adetailer_dir.parent.exists()
-    and os.access(adetailer_dir.parent, os.W_OK)
-):
-    adetailer_dir.mkdir()
+txt2img_submit_button = img2img_submit_button = None
+txt2img_submit_button = cast(gr.Button, txt2img_submit_button)
+img2img_submit_button = cast(gr.Button, img2img_submit_button)
 
 print(
     f"[-] ADetailer initialized. version: {__version__}, num models: {len(model_mapping)}"
 )
 
 
-@contextmanager
-def change_torch_load():
-    orig = torch.load
-    try:
-        torch.load = safe.unsafe_torch_load
-        yield
-    finally:
-        torch.load = orig
-
-
-@contextmanager
-def pause_total_tqdm():
-    orig = opts.data.get("multiple_tqdm", True)
-    try:
-        opts.data["multiple_tqdm"] = False
-        yield
-    finally:
-        opts.data["multiple_tqdm"] = orig
-
-
-@contextmanager
-def preseve_prompts(p):
-    all_pt = copy(p.all_prompts)
-    all_ng = copy(p.all_negative_prompts)
-    try:
-        yield
-    finally:
-        p.all_prompts = all_pt
-        p.all_negative_prompts = all_ng
-
-
 class AfterDetailerScript(scripts.Script):
     def __init__(self):
         super().__init__()
         self.ultralytics_device = self.get_ultralytics_device()
 
         self.controlnet_ext = None
 
@@ -135,24 +107,26 @@
     def show(self, is_img2img):
         return scripts.AlwaysVisible
 
     def ui(self, is_img2img):
         num_models = opts.data.get("ad_max_models", 2)
         ad_model_list = list(model_mapping.keys())
         sampler_names = [sampler.name for sampler in all_samplers]
+        scheduler_names = [x.label for x in schedulers]
 
         try:
             checkpoint_list = modules.sd_models.checkpoint_tiles(use_shorts=True)
         except TypeError:
             checkpoint_list = modules.sd_models.checkpoint_tiles()
         vae_list = modules.shared_items.sd_vae_items()
 
         webui_info = WebuiInfo(
             ad_model_list=ad_model_list,
             sampler_names=sampler_names,
+            scheduler_names=scheduler_names,
             t2i_button=txt2img_submit_button,
             i2i_button=img2img_submit_button,
             checkpoints_list=checkpoint_list,
             vae_list=vae_list,
         )
 
         components, infotext_fields = adui(num_models, is_img2img, webui_info)
@@ -220,15 +194,15 @@
             p._ad_skip_img2img = args_[1]
         else:
             p._ad_skip_img2img = False
 
         if not p._ad_skip_img2img:
             return
 
-        if self.is_img2img_inpaint(p):
+        if is_img2img_inpaint(p):
             p._ad_disabled = True
             msg = "[-] ADetailer: img2img inpainting with skip img2img is not supported. (because it's buggy)"
             print(msg)
             return
 
         p._ad_orig = SkipImg2ImgOrig(
             steps=p.steps,
@@ -237,21 +211,14 @@
             height=p.height,
         )
         p.steps = 1
         p.sampler_name = "Euler"
         p.width = 128
         p.height = 128
 
-    @staticmethod
-    def get_i(p) -> int:
-        it = p.iteration
-        bs = p.batch_size
-        i = p.batch_index
-        return it * bs + i
-
     def get_args(self, p, *args_) -> list[ADetailerArgs]:
         """
         `args_` is at least 1 in length by `is_ad_enabled` immediately above
         """
         args = [arg for arg in args_ if isinstance(arg, dict)]
 
         if not args:
@@ -319,22 +286,22 @@
     ) -> list[str]:
         prompts = re.split(r"\s*\[SEP\]\s*", ad_prompt)
         blank_replacement = self.prompt_blank_replacement(all_prompts, i, default)
         for n in range(len(prompts)):
             if not prompts[n]:
                 prompts[n] = blank_replacement
             elif "[PROMPT]" in prompts[n]:
-                prompts[n] = prompts[n].replace("[PROMPT]", f" {blank_replacement} ")
+                prompts[n] = prompts[n].replace("[PROMPT]", blank_replacement)
 
             for pair in replacements:
                 prompts[n] = prompts[n].replace(pair.s, pair.r)
         return prompts
 
     def get_prompt(self, p, args: ADetailerArgs) -> tuple[list[str], list[str]]:
-        i = self.get_i(p)
+        i = get_i(p)
         prompt_sr = p._ad_xyz_prompt_sr if hasattr(p, "_ad_xyz_prompt_sr") else []
 
         prompt = self._get_prompt(
             ad_prompt=args.ad_prompt,
             all_prompts=p.all_prompts,
             i=i,
             default=p.prompt,
@@ -347,15 +314,15 @@
             default=p.negative_prompt,
             replacements=prompt_sr,
         )
 
         return prompt, negative_prompt
 
     def get_seed(self, p) -> tuple[int, int]:
-        i = self.get_i(p)
+        i = get_i(p)
 
         if not p.all_seeds:
             seed = p.seed
         elif i < len(p.all_seeds):
             seed = p.all_seeds[i]
         else:
             j = i % len(p.all_seeds)
@@ -397,14 +364,25 @@
     def get_sampler(self, p, args: ADetailerArgs) -> str:
         if args.ad_use_sampler:
             return args.ad_sampler
         if hasattr(p, "_ad_orig"):
             return p._ad_orig.sampler_name
         return p.sampler_name
 
+    def get_scheduler(self, p, args: ADetailerArgs) -> dict[str, str]:
+        "webui >= 1.9.0"
+        if not args.ad_use_sampler:
+            return {}
+
+        if args.ad_scheduler == "Use same scheduler":
+            value = getattr(p, "scheduler", "Automatic")
+        else:
+            value = args.ad_scheduler
+        return {"scheduler": value}
+
     def get_override_settings(self, p, args: ADetailerArgs) -> dict[str, Any]:
         d = {}
 
         if args.ad_use_clip_skip:
             d["CLIP_stop_at_last_layers"] = args.ad_clip_skip
 
         if (
@@ -494,14 +472,18 @@
         width, height = self.get_width_height(p, args)
         steps = self.get_steps(p, args)
         cfg_scale = self.get_cfg_scale(p, args)
         initial_noise_multiplier = self.get_initial_noise_multiplier(p, args)
         sampler_name = self.get_sampler(p, args)
         override_settings = self.get_override_settings(p, args)
 
+        version_args = {}
+        if schedulers:
+            version_args.update(self.get_scheduler(p, args))
+
         i2i = StableDiffusionProcessingImg2Img(
             init_images=[image],
             resize_mode=0,
             denoising_strength=args.ad_denoising_strength,
             mask=None,
             mask_blur=args.ad_mask_blur,
             inpainting_fill=1,
@@ -525,18 +507,19 @@
             n_iter=1,
             steps=steps,
             cfg_scale=cfg_scale,
             width=width,
             height=height,
             restore_faces=args.ad_restore_face,
             tiling=p.tiling,
-            extra_generation_params=p.extra_generation_params.copy(),
+            extra_generation_params=copy_extra_params(p.extra_generation_params),
             do_not_save_samples=True,
             do_not_save_grid=True,
             override_settings=override_settings,
+            **version_args,
         )
 
         i2i.cached_c = [None, None]
         i2i.cached_uc = [None, None]
         i2i.scripts, i2i.script_args = self.script_filter(p, args)
         i2i._ad_disabled = True
         i2i._ad_inner = True
@@ -548,15 +531,15 @@
             self.update_controlnet_args(i2i, args)
         elif args.ad_controlnet_model == "None":
             i2i.control_net_enabled = False
 
         return i2i
 
     def save_image(self, p, image, *, condition: str, suffix: str) -> None:
-        i = self.get_i(p)
+        i = get_i(p)
         if p.all_prompts:
             i %= len(p.all_prompts)
             save_prompt = p.all_prompts[i]
         else:
             save_prompt = p.prompt
         seed, _ = self.get_seed(p)
 
@@ -594,15 +577,15 @@
             pred.masks,
             kernel=args.ad_dilate_erode,
             x_offset=args.ad_x_offset,
             y_offset=args.ad_y_offset,
             merge_invert=args.ad_mask_merge_invert,
         )
 
-        if self.is_img2img_inpaint(p) and not self.is_inpaint_only_masked(p):
+        if is_img2img_inpaint(p) and not is_inpaint_only_masked(p):
             image_mask = self.get_image_mask(p)
             masks = self.inpaint_mask_filter(image_mask, masks)
         return masks
 
     @staticmethod
     def i2i_prompts_replace(
         i2i, prompts: list[str], negative_prompts: list[str], j: int
@@ -630,47 +613,25 @@
         if ng in extra_params and extra_params[ng] != processed.all_negative_prompts[0]:
             print(
                 f"[-] ADetailer: applied {ordinal(n + 1)} ad_negative_prompt: {processed.all_negative_prompts[0]!r}"
             )
             p._ad_extra_params_result[ng] = processed.all_negative_prompts[0]
 
     @staticmethod
-    def need_call_process(p) -> bool:
-        if p.scripts is None:
-            return False
-        i = p.batch_index
-        bs = p.batch_size
-        return i == bs - 1
-
-    @staticmethod
-    def need_call_postprocess(p) -> bool:
-        if p.scripts is None:
-            return False
-        return p.batch_index == 0
-
-    @staticmethod
     def get_i2i_init_image(p, pp):
         if getattr(p, "_ad_skip_img2img", False):
             return p.init_images[0]
         return pp.image
 
     @staticmethod
     def get_each_tap_seed(seed: int, i: int):
         use_same_seed = shared.opts.data.get("ad_same_seed_for_each_tap", False)
         return seed if use_same_seed else seed + i
 
     @staticmethod
-    def is_img2img_inpaint(p) -> bool:
-        return hasattr(p, "image_mask") and p.image_mask is not None
-
-    @staticmethod
-    def is_inpaint_only_masked(p) -> bool:
-        return hasattr(p, "inpaint_full_res") and p.inpaint_full_res
-
-    @staticmethod
     def inpaint_mask_filter(
         img2img_mask: Image.Image, ad_mask: list[Image.Image]
     ) -> list[Image.Image]:
         if ad_mask and img2img_mask.size != ad_mask[0].size:
             img2img_mask = img2img_mask.resize(ad_mask[0].size, resample=images.LANCZOS)
         return [mask for mask in ad_mask if has_intersection(img2img_mask, mask)]
 
@@ -692,15 +653,15 @@
         return images.resize_image(p.resize_mode, mask, width, height)
 
     @rich_traceback
     def process(self, p, *args_):
         if getattr(p, "_ad_disabled", False):
             return
 
-        if self.is_img2img_inpaint(p) and is_all_black(self.get_image_mask(p)):
+        if is_img2img_inpaint(p) and is_all_black(self.get_image_mask(p)):
             p._ad_disabled = True
             msg = (
                 "[-] ADetailer: img2img inpainting with no mask -- adetailer disabled."
             )
             print(msg)
             return
 
@@ -734,15 +695,15 @@
             bool
 
             `True` if image was processed, `False` otherwise.
         """
         if state.interrupted or state.skipped:
             return False
 
-        i = self.get_i(p)
+        i = get_i(p)
 
         i2i = self.get_i2i_p(p, args, pp.image)
         seed, subseed = self.get_seed(p)
         ad_prompts, ad_negatives = self.get_prompt(p, args)
 
         is_mediapipe = args.ad_model.lower().startswith("mediapipe")
 
@@ -755,23 +716,23 @@
             ad_model = self.get_ad_model(args.ad_model)
             kwargs["device"] = self.ultralytics_device
             kwargs["classes"] = args.ad_model_classes
 
         with change_torch_load():
             pred = predictor(ad_model, pp.image, args.ad_confidence, **kwargs)
 
-        masks = self.pred_preprocessing(p, pred, args)
-        shared.state.assign_current_image(pred.preview)
-
-        if not masks:
+        if pred.preview is None:
             print(
                 f"[-] ADetailer: nothing detected on image {i + 1} with {ordinal(n + 1)} settings."
             )
             return False
 
+        masks = self.pred_preprocessing(p, pred, args)
+        shared.state.assign_current_image(pred.preview)
+
         self.save_image(
             p,
             pred.preview,
             condition="ad_save_previews",
             suffix="-ad-preview" + suffix(n, "-"),
         )
 
@@ -820,15 +781,15 @@
 
         pp.image = self.get_i2i_init_image(p, pp)
         pp.image = ensure_pil_image(pp.image, "RGB")
         init_image = copy(pp.image)
         arg_list = self.get_args(p, *args_)
         params_txt_content = Path(paths.data_path, "params.txt").read_text("utf-8")
 
-        if self.need_call_postprocess(p):
+        if need_call_postprocess(p):
             dummy = Processed(p, [], p.seed, "")
             with preseve_prompts(p):
                 p.scripts.postprocess(copy(p), dummy)
 
         is_processed = False
         with CNHijackRestore(), pause_total_tqdm(), cn_allow_script_control():
             for n, args in enumerate(arg_list):
@@ -837,15 +798,15 @@
                 is_processed |= self._postprocess_image_inner(p, pp, args, n=n)
 
         if is_processed and not getattr(p, "_ad_skip_img2img", False):
             self.save_image(
                 p, init_image, condition="ad_save_images_before", suffix="-ad-before"
             )
 
-        if self.need_call_process(p):
+        if need_call_process(p):
             with preseve_prompts(p):
                 copy_p = copy(p)
                 if hasattr(p.scripts, "before_process"):
                     p.scripts.before_process(copy_p)
                 p.scripts.process(copy_p)
 
         self.write_params_txt(params_txt_content)
```

### Comparing `adetailer-24.4.0/tests/test_common.py` & `adetailer-24.4.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.4.0/tests/test_mask.py` & `adetailer-24.4.1/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.4.0/tests/test_ultralytics.py` & `adetailer-24.4.1/tests/test_ultralytics.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.4.0/.gitignore` & `adetailer-24.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adetailer-24.4.0/LICENSE.md` & `adetailer-24.4.1/LICENSE.md`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,661 +1,661 @@
-                    GNU AFFERO GENERAL PUBLIC LICENSE
-                       Version 3, 19 November 2007
-
-Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
-Everyone is permitted to copy and distribute verbatim copies
-of this license document, but changing it is not allowed.
-
-                            Preamble
-
-The GNU Affero General Public License is a free, copyleft license for
-software and other kinds of works, specifically designed to ensure
-cooperation with the community in the case of network server software.
-
-The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works. By contrast,
-our General Public Licenses are intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.
-
-When we speak of free software, we are referring to freedom, not
-price. Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-Developers that use our General Public Licenses protect your rights
-with two steps: (1) assert copyright on the software, and (2) offer
-you this License which gives you legal permission to copy, distribute
-and/or modify the software.
-
-A secondary benefit of defending all users' freedom is that
-improvements made in alternate versions of the program, if they
-receive widespread use, become available for other developers to
-incorporate. Many developers of free software are heartened and
-encouraged by the resulting cooperation. However, in the case of
-software used on network servers, this result may fail to come about.
-The GNU General Public License permits making a modified version and
-letting the public access it on a server without ever releasing its
-source code to the public.
-
-The GNU Affero General Public License is designed specifically to
-ensure that, in such cases, the modified source code becomes available
-to the community. It requires the operator of a network server to
-provide the source code of the modified version running there to the
-users of that server. Therefore, public use of a modified version, on
-a publicly accessible server, gives the public access to the source
-code of the modified version.
-
-An older license, called the Affero General Public License and
-published by Affero, was designed to accomplish similar goals. This is
-a different license, not a version of the Affero GPL, but Affero has
-released a new version of the Affero GPL which permits relicensing under
-this license.
-
-The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-0. Definitions.
-
-"This License" refers to version 3 of the GNU Affero General Public License.
-
-"Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-"The Program" refers to any copyrightable work licensed under this
-License. Each licensee is addressed as "you". "Licensees" and
-"recipients" may be individuals or organizations.
-
-To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy. The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy. Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies. Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License. If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-1. Source Code.
-
-The "source code" for a work means the preferred form of the work
-for making modifications to it. "Object code" means any non-source
-form of a work.
-
-A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form. A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities. However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work. For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-The Corresponding Source for a work in source code form is that
-same work.
-
-2. Basic Permissions.
-
-All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met. This License explicitly affirms your unlimited
-permission to run the unmodified Program. The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work. This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force. You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright. Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-Conveying under any other circumstances is permitted solely under
-the conditions stated below. Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-4. Conveying Verbatim Copies.
-
-You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-5. Conveying Modified Source Versions.
-
-You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit. Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-6. Conveying Non-Source Forms.
-
-You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling. In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage. For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product. A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-"Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source. The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information. But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed. Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-7. Additional Terms.
-
-"Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law. If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it. (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.) You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10. If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term. If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-8. Termination.
-
-You may not propagate or modify a covered work except as expressly
-provided under this License. Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License. If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-9. Acceptance Not Required for Having Copies.
-
-You are not required to accept this License in order to receive or
-run a copy of the Program. Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance. However,
-nothing other than this License grants you permission to propagate or
-modify any covered work. These actions infringe copyright if you do
-not accept this License. Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-10. Automatic Licensing of Downstream Recipients.
-
-Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License. You are not responsible
-for enforcing compliance by third parties with this License.
-
-An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations. If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License. For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-11. Patents.
-
-A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based. The
-work thus licensed is called the contributor's "contributor version".
-
-A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version. For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement). To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients. "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License. You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-12. No Surrender of Others' Freedom.
-
-If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License. If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all. For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-13. Remote Network Interaction; Use with the GNU General Public License.
-
-Notwithstanding any other provision of this License, if you modify the
-Program, your modified version must prominently offer all users
-interacting with it remotely through a computer network (if your version
-supports such interaction) an opportunity to receive the Corresponding
-Source of your version by providing access to the Corresponding Source
-from a network server at no charge, through some standard or customary
-means of facilitating copying of software. This Corresponding Source
-shall include the Corresponding Source for any work covered by version 3
-of the GNU General Public License that is incorporated pursuant to the
-following paragraph.
-
-Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU General Public License into a single
-combined work, and to convey the resulting work. The terms of this
-License will continue to apply to the part which is the covered work,
-but the work with which it is combined will remain governed by version
-3 of the GNU General Public License.
-
-14. Revised Versions of this License.
-
-The Free Software Foundation may publish revised and/or new versions of
-the GNU Affero General Public License from time to time. Such new versions
-will be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-Each version is given a distinguishing version number. If the
-Program specifies that a certain numbered version of the GNU Affero General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation. If the Program does not specify a version number of the
-GNU Affero General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-If the Program specifies that a proxy can decide which future
-versions of the GNU Affero General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-Later license versions may give you additional or different
-permissions. However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-15. Disclaimer of Warranty.
-
-THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-16. Limitation of Liability.
-
-IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-17. Interpretation of Sections 15 and 16.
-
-If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-To do so, attach the following notices to the program. It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU Affero General Public License as published
-    by the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU Affero General Public License for more details.
-
-    You should have received a copy of the GNU Affero General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-If your software can interact with users remotely through a computer
-network, you should also make sure that it provides a way for users to
-get its source. For example, if your program is a web application, its
-interface could display a "Source" link that leads users to an archive
-of the code. There are many ways you could offer source, and different
-solutions will be better for different programs; see section 13 for the
-specific requirements.
-
-You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU AGPL, see
-<http://www.gnu.org/licenses/>.
+                    GNU AFFERO GENERAL PUBLIC LICENSE
+                       Version 3, 19 November 2007
+
+Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+Everyone is permitted to copy and distribute verbatim copies
+of this license document, but changing it is not allowed.
+
+                            Preamble
+
+The GNU Affero General Public License is a free, copyleft license for
+software and other kinds of works, specifically designed to ensure
+cooperation with the community in the case of network server software.
+
+The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works. By contrast,
+our General Public Licenses are intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.
+
+When we speak of free software, we are referring to freedom, not
+price. Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+Developers that use our General Public Licenses protect your rights
+with two steps: (1) assert copyright on the software, and (2) offer
+you this License which gives you legal permission to copy, distribute
+and/or modify the software.
+
+A secondary benefit of defending all users' freedom is that
+improvements made in alternate versions of the program, if they
+receive widespread use, become available for other developers to
+incorporate. Many developers of free software are heartened and
+encouraged by the resulting cooperation. However, in the case of
+software used on network servers, this result may fail to come about.
+The GNU General Public License permits making a modified version and
+letting the public access it on a server without ever releasing its
+source code to the public.
+
+The GNU Affero General Public License is designed specifically to
+ensure that, in such cases, the modified source code becomes available
+to the community. It requires the operator of a network server to
+provide the source code of the modified version running there to the
+users of that server. Therefore, public use of a modified version, on
+a publicly accessible server, gives the public access to the source
+code of the modified version.
+
+An older license, called the Affero General Public License and
+published by Affero, was designed to accomplish similar goals. This is
+a different license, not a version of the Affero GPL, but Affero has
+released a new version of the Affero GPL which permits relicensing under
+this license.
+
+The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+0. Definitions.
+
+"This License" refers to version 3 of the GNU Affero General Public License.
+
+"Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+"The Program" refers to any copyrightable work licensed under this
+License. Each licensee is addressed as "you". "Licensees" and
+"recipients" may be individuals or organizations.
+
+To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy. The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy. Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies. Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License. If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+1. Source Code.
+
+The "source code" for a work means the preferred form of the work
+for making modifications to it. "Object code" means any non-source
+form of a work.
+
+A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form. A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities. However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work. For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+The Corresponding Source for a work in source code form is that
+same work.
+
+2. Basic Permissions.
+
+All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met. This License explicitly affirms your unlimited
+permission to run the unmodified Program. The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work. This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force. You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright. Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+Conveying under any other circumstances is permitted solely under
+the conditions stated below. Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+4. Conveying Verbatim Copies.
+
+You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+5. Conveying Modified Source Versions.
+
+You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit. Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+6. Conveying Non-Source Forms.
+
+You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling. In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage. For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product. A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+"Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source. The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information. But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed. Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+7. Additional Terms.
+
+"Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law. If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it. (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.) You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10. If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term. If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+8. Termination.
+
+You may not propagate or modify a covered work except as expressly
+provided under this License. Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License. If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+9. Acceptance Not Required for Having Copies.
+
+You are not required to accept this License in order to receive or
+run a copy of the Program. Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance. However,
+nothing other than this License grants you permission to propagate or
+modify any covered work. These actions infringe copyright if you do
+not accept this License. Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+10. Automatic Licensing of Downstream Recipients.
+
+Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License. You are not responsible
+for enforcing compliance by third parties with this License.
+
+An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations. If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License. For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+11. Patents.
+
+A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based. The
+work thus licensed is called the contributor's "contributor version".
+
+A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version. For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement). To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients. "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License. You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+12. No Surrender of Others' Freedom.
+
+If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License. If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all. For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+13. Remote Network Interaction; Use with the GNU General Public License.
+
+Notwithstanding any other provision of this License, if you modify the
+Program, your modified version must prominently offer all users
+interacting with it remotely through a computer network (if your version
+supports such interaction) an opportunity to receive the Corresponding
+Source of your version by providing access to the Corresponding Source
+from a network server at no charge, through some standard or customary
+means of facilitating copying of software. This Corresponding Source
+shall include the Corresponding Source for any work covered by version 3
+of the GNU General Public License that is incorporated pursuant to the
+following paragraph.
+
+Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU General Public License into a single
+combined work, and to convey the resulting work. The terms of this
+License will continue to apply to the part which is the covered work,
+but the work with which it is combined will remain governed by version
+3 of the GNU General Public License.
+
+14. Revised Versions of this License.
+
+The Free Software Foundation may publish revised and/or new versions of
+the GNU Affero General Public License from time to time. Such new versions
+will be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+Each version is given a distinguishing version number. If the
+Program specifies that a certain numbered version of the GNU Affero General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation. If the Program does not specify a version number of the
+GNU Affero General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+If the Program specifies that a proxy can decide which future
+versions of the GNU Affero General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+Later license versions may give you additional or different
+permissions. However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+15. Disclaimer of Warranty.
+
+THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+16. Limitation of Liability.
+
+IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+17. Interpretation of Sections 15 and 16.
+
+If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+To do so, attach the following notices to the program. It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU Affero General Public License as published
+    by the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Affero General Public License for more details.
+
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+If your software can interact with users remotely through a computer
+network, you should also make sure that it provides a way for users to
+get its source. For example, if your program is a web application, its
+interface could display a "Source" link that leads users to an archive
+of the code. There are many ways you could offer source, and different
+solutions will be better for different programs; see section 13 for the
+specific requirements.
+
+You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU AGPL, see
+<http://www.gnu.org/licenses/>.
```

### Comparing `adetailer-24.4.0/README.md` & `adetailer-24.4.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,110 +1,118 @@
-# ADetailer
-
-ADetailer is an extension for the stable diffusion webui that does automatic masking and inpainting. It is similar to the Detection Detailer.
-
-## Install
-
-(from Mikubill/sd-webui-controlnet)
-
-1. Open "Extensions" tab.
-2. Open "Install from URL" tab in the tab.
-3. Enter `https://github.com/Bing-su/adetailer.git` to "URL for extension's git repository".
-4. Press "Install" button.
-5. Wait 5 seconds, and you will see the message "Installed into stable-diffusion-webui\extensions\adetailer. Use Installed tab to restart".
-6. Go to "Installed" tab, click "Check for updates", and then click "Apply and restart UI". (The next time you can also use this method to update extensions.)
-7. Completely restart A1111 webui including your terminal. (If you do not know what is a "terminal", you can reboot your computer: turn your computer off and turn it on again.)
-
-You can now install it directly from the Extensions tab.
-
-![image](https://i.imgur.com/g6GdRBT.png)
-
-## Options
-
-| Model, Prompts                    |                                                                                    |                                                                                                                                                        |
-| --------------------------------- | ---------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
-| ADetailer model                   | Determine what to detect.                                                          | `None` = disable                                                                                                                                       |
-| ADetailer model classes           | Comma separated class names to detect. only available when using YOLO World models | If blank, use default values.<br/>default = [COCO 80 classes](https://github.com/ultralytics/ultralytics/blob/main/ultralytics/cfg/datasets/coco.yaml) |
-| ADetailer prompt, negative prompt | Prompts and negative prompts to apply                                              | If left blank, it will use the same as the input.                                                                                                      |
-| Skip img2img                      | Skip img2img. In practice, this works by changing the step count of img2img to 1.  | img2img only                                                                                                                                           |
-
-| Detection                            |                                                                                              |              |
-| ------------------------------------ | -------------------------------------------------------------------------------------------- | ------------ |
-| Detection model confidence threshold | Only objects with a detection model confidence above this threshold are used for inpainting. |              |
-| Mask min/max ratio                   | Only use masks whose area is between those ratios for the area of the entire image.          |              |
-| Mask only the top k largest          | Only use the k objects with the largest area of the bbox.                                    | 0 to disable |
-
-If you want to exclude objects in the background, try setting the min ratio to around `0.01`.
-
-| Mask Preprocessing              |                                                                                                                                     |                                                                                         |
-| ------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
-| Mask x, y offset                | Moves the mask horizontally and vertically by                                                                                       |                                                                                         |
-| Mask erosion (-) / dilation (+) | Enlarge or reduce the detected mask.                                                                                                | [opencv example](https://docs.opencv.org/4.7.0/db/df6/tutorial_erosion_dilatation.html) |
-| Mask merge mode                 | `None`: Inpaint each mask<br/>`Merge`: Merge all masks and inpaint<br/>`Merge and Invert`: Merge all masks and Invert, then inpaint |                                                                                         |
-
-Applied in this order: x, y offset → erosion/dilation → merge/invert.
-
-#### Inpainting
-
-Each option corresponds to a corresponding option on the inpaint tab. Therefore, please refer to the inpaint tab for usage details on how to use each option.
-
-## ControlNet Inpainting
-
-You can use the ControlNet extension if you have ControlNet installed and ControlNet models.
-
-Support `inpaint, scribble, lineart, openpose, tile, depth` controlnet models. Once you choose a model, the preprocessor is set automatically. It works separately from the model set by the Controlnet extension.
-
-If you select `Passthrough`, the controlnet settings you set outside of ADetailer will be used.
-
-## Advanced Options
-
-API request example: [wiki/REST-API](https://github.com/Bing-su/adetailer/wiki/REST-API)
-
-`[SEP], [SKIP], [PROMPT]` tokens: [wiki/Advanced](https://github.com/Bing-su/adetailer/wiki/Advanced)
-
-## Media
-
-- 🎥 [どこよりも詳しいAfter Detailer (adetailer)の使い方① 【Stable Diffusion】](https://youtu.be/sF3POwPUWCE)
-- 🎥 [どこよりも詳しいAfter Detailer (adetailer)の使い方② 【Stable Diffusion】](https://youtu.be/urNISRdbIEg)
-
-- 📜 [ADetailer Installation and 5 Usage Methods](https://kindanai.com/en/manual-adetailer/)
-
-## Model
-
-| Model                 | Target                | mAP 50                        | mAP 50-95                     |
-| --------------------- | --------------------- | ----------------------------- | ----------------------------- |
-| face_yolov8n.pt       | 2D / realistic face   | 0.660                         | 0.366                         |
-| face_yolov8s.pt       | 2D / realistic face   | 0.713                         | 0.404                         |
-| hand_yolov8n.pt       | 2D / realistic hand   | 0.767                         | 0.505                         |
-| person_yolov8n-seg.pt | 2D / realistic person | 0.782 (bbox)<br/>0.761 (mask) | 0.555 (bbox)<br/>0.460 (mask) |
-| person_yolov8s-seg.pt | 2D / realistic person | 0.824 (bbox)<br/>0.809 (mask) | 0.605 (bbox)<br/>0.508 (mask) |
-| mediapipe_face_full   | realistic face        | -                             | -                             |
-| mediapipe_face_short  | realistic face        | -                             | -                             |
-| mediapipe_face_mesh   | realistic face        | -                             | -                             |
-
-The YOLO models can be found on huggingface [Bingsu/adetailer](https://huggingface.co/Bingsu/adetailer).
-
-For a detailed description of the YOLO8 model, see: https://docs.ultralytics.com/models/yolov8/#overview
-
-YOLO World model: https://docs.ultralytics.com/models/yolo-world/
-
-### Additional Model
-
-Put your [ultralytics](https://github.com/ultralytics/ultralytics) yolo model in `models/adetailer`. The model name should end with `.pt`.
-
-It must be a bbox detection or segment model and use all label.
-
-## How it works
-
-ADetailer works in three simple steps.
-
-1. Create an image.
-2. Detect object with a detection model and create a mask image.
-3. Inpaint using the image from 1 and the mask from 2.
-
-## Development
-
-ADetailer is developed and tested using the stable-diffusion 1.5 model, for the latest version of [AUTOMATIC1111/stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) repository only.
-
-## License
-
-ADetailer is a derivative work that uses two AGPL-licensed works (stable-diffusion-webui, ultralytics) and is therefore distributed under the AGPL license.
+# ADetailer
+
+ADetailer is an extension for the stable diffusion webui that does automatic masking and inpainting. It is similar to the Detection Detailer.
+
+## Install
+
+You can install it directly from the Extensions tab.
+
+![image](https://i.imgur.com/qaXtoI6.png)
+
+Or
+
+(from Mikubill/sd-webui-controlnet)
+
+1. Open "Extensions" tab.
+2. Open "Install from URL" tab in the tab.
+3. Enter `https://github.com/Bing-su/adetailer.git` to "URL for extension's git repository".
+4. Press "Install" button.
+5. Wait 5 seconds, and you will see the message "Installed into stable-diffusion-webui\extensions\adetailer. Use Installed tab to restart".
+6. Go to "Installed" tab, click "Check for updates", and then click "Apply and restart UI". (The next time you can also use this method to update extensions.)
+7. Completely restart A1111 webui including your terminal. (If you do not know what is a "terminal", you can reboot your computer: turn your computer off and turn it on again.)
+
+## Options
+
+| Model, Prompts                    |                                                                                    |                                                                                                                                                        |
+| --------------------------------- | ---------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
+| ADetailer model                   | Determine what to detect.                                                          | `None` = disable                                                                                                                                       |
+| ADetailer model classes           | Comma separated class names to detect. only available when using YOLO World models | If blank, use default values.<br/>default = [COCO 80 classes](https://github.com/ultralytics/ultralytics/blob/main/ultralytics/cfg/datasets/coco.yaml) |
+| ADetailer prompt, negative prompt | Prompts and negative prompts to apply                                              | If left blank, it will use the same as the input.                                                                                                      |
+| Skip img2img                      | Skip img2img. In practice, this works by changing the step count of img2img to 1.  | img2img only                                                                                                                                           |
+
+| Detection                            |                                                                                              |              |
+| ------------------------------------ | -------------------------------------------------------------------------------------------- | ------------ |
+| Detection model confidence threshold | Only objects with a detection model confidence above this threshold are used for inpainting. |              |
+| Mask min/max ratio                   | Only use masks whose area is between those ratios for the area of the entire image.          |              |
+| Mask only the top k largest          | Only use the k objects with the largest area of the bbox.                                    | 0 to disable |
+
+If you want to exclude objects in the background, try setting the min ratio to around `0.01`.
+
+| Mask Preprocessing              |                                                                                                                                     |                                                                                         |
+| ------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
+| Mask x, y offset                | Moves the mask horizontally and vertically by                                                                                       |                                                                                         |
+| Mask erosion (-) / dilation (+) | Enlarge or reduce the detected mask.                                                                                                | [opencv example](https://docs.opencv.org/4.7.0/db/df6/tutorial_erosion_dilatation.html) |
+| Mask merge mode                 | `None`: Inpaint each mask<br/>`Merge`: Merge all masks and inpaint<br/>`Merge and Invert`: Merge all masks and Invert, then inpaint |                                                                                         |
+
+Applied in this order: x, y offset → erosion/dilation → merge/invert.
+
+#### Inpainting
+
+Each option corresponds to a corresponding option on the inpaint tab. Therefore, please refer to the inpaint tab for usage details on how to use each option.
+
+## ControlNet Inpainting
+
+You can use the ControlNet extension if you have ControlNet installed and ControlNet models.
+
+Support `inpaint, scribble, lineart, openpose, tile, depth` controlnet models. Once you choose a model, the preprocessor is set automatically. It works separately from the model set by the Controlnet extension.
+
+If you select `Passthrough`, the controlnet settings you set outside of ADetailer will be used.
+
+## Advanced Options
+
+API request example: [wiki/REST-API](https://github.com/Bing-su/adetailer/wiki/REST-API)
+
+`[SEP], [SKIP], [PROMPT]` tokens: [wiki/Advanced](https://github.com/Bing-su/adetailer/wiki/Advanced)
+
+## Media
+
+- 🎥 [どこよりも詳しい After Detailer (adetailer)の使い方 ① 【Stable Diffusion】](https://youtu.be/sF3POwPUWCE)
+- 🎥 [どこよりも詳しい After Detailer (adetailer)の使い方 ② 【Stable Diffusion】](https://youtu.be/urNISRdbIEg)
+
+- 📜 [ADetailer Installation and 5 Usage Methods](https://kindanai.com/en/manual-adetailer/)
+
+## Model
+
+| Model                 | Target                | mAP 50                        | mAP 50-95                     |
+| --------------------- | --------------------- | ----------------------------- | ----------------------------- |
+| face_yolov8n.pt       | 2D / realistic face   | 0.660                         | 0.366                         |
+| face_yolov8s.pt       | 2D / realistic face   | 0.713                         | 0.404                         |
+| hand_yolov8n.pt       | 2D / realistic hand   | 0.767                         | 0.505                         |
+| person_yolov8n-seg.pt | 2D / realistic person | 0.782 (bbox)<br/>0.761 (mask) | 0.555 (bbox)<br/>0.460 (mask) |
+| person_yolov8s-seg.pt | 2D / realistic person | 0.824 (bbox)<br/>0.809 (mask) | 0.605 (bbox)<br/>0.508 (mask) |
+| mediapipe_face_full   | realistic face        | -                             | -                             |
+| mediapipe_face_short  | realistic face        | -                             | -                             |
+| mediapipe_face_mesh   | realistic face        | -                             | -                             |
+
+The YOLO models can be found on huggingface [Bingsu/adetailer](https://huggingface.co/Bingsu/adetailer).
+
+For a detailed description of the YOLO8 model, see: https://docs.ultralytics.com/models/yolov8/#overview
+
+YOLO World model: https://docs.ultralytics.com/models/yolo-world/
+
+### Additional Model
+
+Put your [ultralytics](https://github.com/ultralytics/ultralytics) yolo model in `models/adetailer`. The model name should end with `.pt`.
+
+It must be a bbox detection or segment model and use all label.
+
+## How it works
+
+ADetailer works in three simple steps.
+
+1. Create an image.
+2. Detect object with a detection model and create a mask image.
+3. Inpaint using the image from 1 and the mask from 2.
+
+## Development
+
+ADetailer is developed and tested using the stable-diffusion 1.5 model, for the latest version of [AUTOMATIC1111/stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) repository only.
+
+## License
+
+ADetailer is a derivative work that uses two AGPL-licensed works (stable-diffusion-webui, ultralytics) and is therefore distributed under the AGPL license.
+
+## See Also
+
+- https://github.com/ototadana/sd-face-editor
+- https://github.com/continue-revolution/sd-webui-segment-anything
+- https://github.com/portu-sim/sd-webui-bmab
```

### Comparing `adetailer-24.4.0/pyproject.toml` & `adetailer-24.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `adetailer-24.4.0/PKG-INFO` & `adetailer-24.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: adetailer
-Version: 24.4.0
+Version: 24.4.1
 Summary: An object detection and auto-mask extension for stable diffusion webui.
 Project-URL: repository, https://github.com/Bing-su/adetailer
 Author-email: dowon <ks2515@naver.com>
 License: AGPL-3.0
 License-File: LICENSE.md
 Keywords: adetailer,stable-diffusion,stable-diffusion-webui,ultralytics
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -19,28 +19,30 @@
 
 # ADetailer
 
 ADetailer is an extension for the stable diffusion webui that does automatic masking and inpainting. It is similar to the Detection Detailer.
 
 ## Install
 
+You can install it directly from the Extensions tab.
+
+![image](https://i.imgur.com/qaXtoI6.png)
+
+Or
+
 (from Mikubill/sd-webui-controlnet)
 
 1. Open "Extensions" tab.
 2. Open "Install from URL" tab in the tab.
 3. Enter `https://github.com/Bing-su/adetailer.git` to "URL for extension's git repository".
 4. Press "Install" button.
 5. Wait 5 seconds, and you will see the message "Installed into stable-diffusion-webui\extensions\adetailer. Use Installed tab to restart".
 6. Go to "Installed" tab, click "Check for updates", and then click "Apply and restart UI". (The next time you can also use this method to update extensions.)
 7. Completely restart A1111 webui including your terminal. (If you do not know what is a "terminal", you can reboot your computer: turn your computer off and turn it on again.)
 
-You can now install it directly from the Extensions tab.
-
-![image](https://i.imgur.com/g6GdRBT.png)
-
 ## Options
 
 | Model, Prompts                    |                                                                                    |                                                                                                                                                        |
 | --------------------------------- | ---------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
 | ADetailer model                   | Determine what to detect.                                                          | `None` = disable                                                                                                                                       |
 | ADetailer model classes           | Comma separated class names to detect. only available when using YOLO World models | If blank, use default values.<br/>default = [COCO 80 classes](https://github.com/ultralytics/ultralytics/blob/main/ultralytics/cfg/datasets/coco.yaml) |
 | ADetailer prompt, negative prompt | Prompts and negative prompts to apply                                              | If left blank, it will use the same as the input.                                                                                                      |
@@ -78,16 +80,16 @@
 
 API request example: [wiki/REST-API](https://github.com/Bing-su/adetailer/wiki/REST-API)
 
 `[SEP], [SKIP], [PROMPT]` tokens: [wiki/Advanced](https://github.com/Bing-su/adetailer/wiki/Advanced)
 
 ## Media
 
-- 🎥 [どこよりも詳しいAfter Detailer (adetailer)の使い方① 【Stable Diffusion】](https://youtu.be/sF3POwPUWCE)
-- 🎥 [どこよりも詳しいAfter Detailer (adetailer)の使い方② 【Stable Diffusion】](https://youtu.be/urNISRdbIEg)
+- 🎥 [どこよりも詳しい After Detailer (adetailer)の使い方 ① 【Stable Diffusion】](https://youtu.be/sF3POwPUWCE)
+- 🎥 [どこよりも詳しい After Detailer (adetailer)の使い方 ② 【Stable Diffusion】](https://youtu.be/urNISRdbIEg)
 
 - 📜 [ADetailer Installation and 5 Usage Methods](https://kindanai.com/en/manual-adetailer/)
 
 ## Model
 
 | Model                 | Target                | mAP 50                        | mAP 50-95                     |
 | --------------------- | --------------------- | ----------------------------- | ----------------------------- |
@@ -123,7 +125,13 @@
 ## Development
 
 ADetailer is developed and tested using the stable-diffusion 1.5 model, for the latest version of [AUTOMATIC1111/stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) repository only.
 
 ## License
 
 ADetailer is a derivative work that uses two AGPL-licensed works (stable-diffusion-webui, ultralytics) and is therefore distributed under the AGPL license.
+
+## See Also
+
+- https://github.com/ototadana/sd-face-editor
+- https://github.com/continue-revolution/sd-webui-segment-anything
+- https://github.com/portu-sim/sd-webui-bmab
```


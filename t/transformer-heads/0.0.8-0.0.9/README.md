# Comparing `tmp/transformer_heads-0.0.8.tar.gz` & `tmp/transformer_heads-0.0.9.tar.gz`

## Comparing `transformer_heads-0.0.8.tar` & `transformer_heads-0.0.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/.readthedocs.yaml
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0    66320 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/_images/example_architecture.svg
--rw-r--r--   0        0        0    64089 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/_images/multi_linear_probe.svg
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/docs/make.bat
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/docs/requirements.txt
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/docs/source/conf.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/docs/source/getting_started.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/docs/source/images.rst
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/docs/source/index.rst
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/docs/source/modules.rst
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/docs/source/readme.rst
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/docs/source/transformer_heads.model.rst
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/docs/source/transformer_heads.rst
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/docs/source/transformer_heads.tests.rst
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/docs/source/transformer_heads.util.rst
--rw-r--r--   0        0        0    85722 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/notebooks/gpt2/joint_multitask_learning.ipynb
--rw-r--r--   0        0        0    48378 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/notebooks/gpt2/linear_probe.ipynb
--rw-r--r--   0        0        0    70663 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/notebooks/gpt2/multi_linear_probe.ipynb
--rw-r--r--   0        0        0    15095 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/notebooks/gpt2/saving_and_loading.ipynb
--rw-r--r--   0        0        0    74344 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/notebooks/gpt2/text_classification_full_finetune.ipynb
--rw-r--r--   0        0        0   722448 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/notebooks/gpt2/text_classification_linear_probe.ipynb
--rw-r--r--   0        0        0    79822 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/notebooks/gpt2/text_classification_qlora.ipynb
--rw-r--r--   0        0        0    59619 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/notebooks/llama/linear_probe.ipynb
--rw-r--r--   0        0        0    81976 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/notebooks/llama/multi_linear_probe.ipynb
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/other/pip_freeze.txt
--rwxr-xr-x   0        0        0     4755 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/scripts/paper_shredder.bash
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/scripts/remove_eval_spam.py
--rwxr-xr-x   0        0        0      487 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/scripts/run_slurm.sh
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/scripts/shredder_papers.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/transformer_heads/__init__.py
--rw-r--r--   0        0        0     6744 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/transformer_heads/config.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/transformer_heads/constants.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/transformer_heads/output.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/transformer_heads/model/__init__.py
--rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/transformer_heads/model/head.py
--rw-r--r--   0        0        0    13817 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/transformer_heads/model/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/transformer_heads/tests/__init__.py
--rw-r--r--   0        0        0     6931 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/transformer_heads/tests/test_load_model.py
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/transformer_heads/tests/test_loss_compute.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/transformer_heads/util/__init__.py
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/transformer_heads/util/evaluate.py
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/transformer_heads/util/helpers.py
--rw-r--r--   0        0        0    10837 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/transformer_heads/util/load_model.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/transformer_heads/util/load_tokenizer.py
--rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/transformer_heads/util/model.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/LICENSE
--rw-r--r--   0        0        0     6167 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/README.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 transformer_heads-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/.readthedocs.yaml
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0    66320 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/_images/example_architecture.svg
+-rw-r--r--   0        0        0    64089 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/_images/multi_linear_probe.svg
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/make.bat
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/requirements.txt
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/source/conf.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/source/getting_started.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/source/images.rst
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/source/index.rst
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/source/modules.rst
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/source/readme.rst
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/source/transformer_heads.model.rst
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/source/transformer_heads.rst
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/source/transformer_heads.tests.rst
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/source/transformer_heads.util.rst
+-rw-r--r--   0        0        0    85722 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/notebooks/gpt2/joint_multitask_learning.ipynb
+-rw-r--r--   0        0        0    48378 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/notebooks/gpt2/linear_probe.ipynb
+-rw-r--r--   0        0        0    70663 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/notebooks/gpt2/multi_linear_probe.ipynb
+-rw-r--r--   0        0        0    15095 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/notebooks/gpt2/saving_and_loading.ipynb
+-rw-r--r--   0        0        0    74344 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/notebooks/gpt2/text_classification_full_finetune.ipynb
+-rw-r--r--   0        0        0   722448 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/notebooks/gpt2/text_classification_linear_probe.ipynb
+-rw-r--r--   0        0        0    79822 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/notebooks/gpt2/text_classification_qlora.ipynb
+-rw-r--r--   0        0        0    59619 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/notebooks/llama/linear_probe.ipynb
+-rw-r--r--   0        0        0    81976 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/notebooks/llama/multi_linear_probe.ipynb
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/other/pip_freeze.txt
+-rwxr-xr-x   0        0        0     4755 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/scripts/paper_shredder.bash
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/scripts/remove_eval_spam.py
+-rwxr-xr-x   0        0        0      487 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/scripts/run_slurm.sh
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/scripts/shredder_papers.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/__init__.py
+-rw-r--r--   0        0        0     6744 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/config.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/constants.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/output.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/model/__init__.py
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/model/head.py
+-rw-r--r--   0        0        0    13817 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/model/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/tests/__init__.py
+-rw-r--r--   0        0        0     6931 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/tests/test_load_model.py
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/tests/test_loss_compute.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/util/__init__.py
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/util/evaluate.py
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/util/helpers.py
+-rw-r--r--   0        0        0    10882 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/util/load_model.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/util/load_tokenizer.py
+-rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/util/model.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/LICENSE
+-rw-r--r--   0        0        0     6167 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/README.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/PKG-INFO
```

### Comparing `transformer_heads-0.0.8/.readthedocs.yaml` & `transformer_heads-0.0.9/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/.github/workflows/publish_to_pypi.yml` & `transformer_heads-0.0.9/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/_images/example_architecture.svg` & `transformer_heads-0.0.9/_images/example_architecture.svg`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/_images/multi_linear_probe.svg` & `transformer_heads-0.0.9/_images/multi_linear_probe.svg`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/docs/Makefile` & `transformer_heads-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/docs/make.bat` & `transformer_heads-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/docs/source/conf.py` & `transformer_heads-0.0.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/docs/source/getting_started.md` & `transformer_heads-0.0.9/docs/source/getting_started.md`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/docs/source/index.rst` & `transformer_heads-0.0.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/docs/source/transformer_heads.model.rst` & `transformer_heads-0.0.9/docs/source/transformer_heads.model.rst`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/docs/source/transformer_heads.rst` & `transformer_heads-0.0.9/docs/source/transformer_heads.rst`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/docs/source/transformer_heads.util.rst` & `transformer_heads-0.0.9/docs/source/transformer_heads.util.rst`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/notebooks/gpt2/joint_multitask_learning.ipynb` & `transformer_heads-0.0.9/notebooks/gpt2/joint_multitask_learning.ipynb`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/notebooks/gpt2/linear_probe.ipynb` & `transformer_heads-0.0.9/notebooks/gpt2/linear_probe.ipynb`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/notebooks/gpt2/multi_linear_probe.ipynb` & `transformer_heads-0.0.9/notebooks/gpt2/multi_linear_probe.ipynb`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/notebooks/gpt2/saving_and_loading.ipynb` & `transformer_heads-0.0.9/notebooks/gpt2/saving_and_loading.ipynb`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/notebooks/gpt2/text_classification_full_finetune.ipynb` & `transformer_heads-0.0.9/notebooks/gpt2/text_classification_full_finetune.ipynb`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/notebooks/gpt2/text_classification_linear_probe.ipynb` & `transformer_heads-0.0.9/notebooks/gpt2/text_classification_linear_probe.ipynb`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/notebooks/gpt2/text_classification_qlora.ipynb` & `transformer_heads-0.0.9/notebooks/gpt2/text_classification_qlora.ipynb`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/notebooks/llama/linear_probe.ipynb` & `transformer_heads-0.0.9/notebooks/llama/linear_probe.ipynb`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/notebooks/llama/multi_linear_probe.ipynb` & `transformer_heads-0.0.9/notebooks/llama/multi_linear_probe.ipynb`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/scripts/paper_shredder.bash` & `transformer_heads-0.0.9/scripts/paper_shredder.bash`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/scripts/remove_eval_spam.py` & `transformer_heads-0.0.9/scripts/remove_eval_spam.py`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/scripts/shredder_papers.py` & `transformer_heads-0.0.9/scripts/shredder_papers.py`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/transformer_heads/config.py` & `transformer_heads-0.0.9/transformer_heads/config.py`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/transformer_heads/constants.py` & `transformer_heads-0.0.9/transformer_heads/constants.py`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/transformer_heads/output.py` & `transformer_heads-0.0.9/transformer_heads/output.py`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/transformer_heads/model/head.py` & `transformer_heads-0.0.9/transformer_heads/model/head.py`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/transformer_heads/model/model.py` & `transformer_heads-0.0.9/transformer_heads/model/model.py`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/transformer_heads/tests/test_load_model.py` & `transformer_heads-0.0.9/transformer_heads/tests/test_load_model.py`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/transformer_heads/tests/test_loss_compute.py` & `transformer_heads-0.0.9/transformer_heads/tests/test_loss_compute.py`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/transformer_heads/util/evaluate.py` & `transformer_heads-0.0.9/transformer_heads/util/evaluate.py`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/transformer_heads/util/helpers.py` & `transformer_heads-0.0.9/transformer_heads/util/helpers.py`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/transformer_heads/util/load_model.py` & `transformer_heads-0.0.9/transformer_heads/util/load_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     head_configs=None,
     head_folder_path=None,
     only_inference: bool = False,
     device_map="auto",
     quantization_config: BitsAndBytesConfig = None,
     freeze_base_model: bool = True,
     **kwargs,
-):
+) -> HeadedModel:
     """
     Loads a transformer model with additional heads.
 
     Args:
         base_model_class (Type[PreTrainedModel]): The class of the base transformer model.
         model_name (str): The huggingface name of the model to load.
         head_configs (list, optional): A list of head configurations.
@@ -122,15 +122,15 @@
     quantization_config: BitsAndBytesConfig = None,
     only_inference: bool = False,
     fully_trained_heads: bool = True,
     device_map="auto",
     torch_dtype=torch.float32,
     gradient_checkpointing: bool = False,
     **kwargs,
-):
+) -> HeadedModel:
     """
     Loads a LoRA (Low Rank Adaptation) transformer model with additional heads.
 
     Args:
         base_model_class (Type[PreTrainedModel]): The class of the base transformer model.
         path (str): The path (saved or huggingface) to the headed model to load.
         quantization_config (BitsAndBytesConfig, optional): The quantization configuration to use when loading the model.
@@ -203,15 +203,15 @@
     quantization_config: BitsAndBytesConfig,
     lora_config: LoraConfig,
     head_configs: list[HeadConfig],
     fully_trained_heads: bool = True,
     device_map="auto",
     gradient_checkpointing: bool = False,
     **kwargs,
-):
+) -> HeadedModel:
     """
     Creates a quantized LoRA (Low Rank Adaptation) transformer model with additional heads.
 
     Args:
         base_model_class (Type[PreTrainedModel]): The class of the base transformer model.
         model_name (str): The name of the pretrained base model (e.g. it's huggingface name).
         quantization_config (BitsAndBytesConfig): The quantization configuration to use when creating the model.
```

### Comparing `transformer_heads-0.0.8/transformer_heads/util/load_tokenizer.py` & `transformer_heads-0.0.9/transformer_heads/util/load_tokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,8 +31,11 @@
     if os.path.exists(adapt_config_path):
         with open(adapt_config_path, "r") as f:
             base_model_path = json.load(f)["base_model_name_or_path"]
     else:
         raise FileNotFoundError(
             f"Adapter config file not found in {model_path}. If you are not trying to load from an adapter_model, just load the tokenizer with AutoTokenizer.from_pretrained"
         )
-    return AutoTokenizer.from_pretrained(base_model_path)
+    tk = AutoTokenizer.from_pretrained(base_model_path)
+    if tk.pad_token is None:
+        tk.pad_token = tk.eos_token
+    return tk
```

### Comparing `transformer_heads-0.0.8/transformer_heads/util/model.py` & `transformer_heads-0.0.9/transformer_heads/util/model.py`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/LICENSE` & `transformer_heads-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/README.md` & `transformer_heads-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/pyproject.toml` & `transformer_heads-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.8/PKG-INFO` & `transformer_heads-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: transformer_heads
-Version: 0.0.8
+Version: 0.0.9
 Summary: Attach custom heads to transformer models.
 Author-email: Yannik Keller <yannik@kelnet.de>
 License: MIT License
 License-File: LICENSE
 Keywords: Linear Probe,Qlora,Transformer
 Requires-Python: >=3.10
 Requires-Dist: bitsandbytes
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: transformer_heads Version: 0.0.8 Summary: Attach
+Metadata-Version: 2.3 Name: transformer_heads Version: 0.0.9 Summary: Attach
 custom heads to transformer models. Author-email: Yannik Keller
 kelnet.de> License: MIT License License-File: LICENSE Keywords: Linear
 Probe,Qlora,Transformer Requires-Python: >=3.10 Requires-Dist: bitsandbytes
 Requires-Dist: datasets Requires-Dist: fire Requires-Dist: pandas Requires-
 Dist: peft Requires-Dist: torch Requires-Dist: tqdm Requires-Dist: transformers
 Description-Content-Type: text/markdown
      ****** _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn || _GG_ee_tt_tt_ii_nn_gg_ _SS_tt_aa_rr_tt_ee_dd || _RR_ee_dd_dd_ii_tt_ _PP_oo_ss_tt_ _ww_ii_tt_hh_ _mm_oo_rr_ee_ _ii_nn_ff_oo ******
```


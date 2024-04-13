# Comparing `tmp/nn_wrapper-1.0.1.tar.gz` & `tmp/nn_wrapper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nn_wrapper-1.0.1.tar", max compression
+gzip compressed data, was "nn_wrapper-1.0.2.tar", max compression
```

## Comparing `nn_wrapper-1.0.1.tar` & `nn_wrapper-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1089 2024-04-12 21:11:26.168898 nn_wrapper-1.0.1/LICENSE
--rw-r--r--   0        0        0       43 2024-04-13 19:55:50.828702 nn_wrapper-1.0.1/NetworkWrapper/__init__.py
--rw-r--r--   0        0        0    33351 2024-04-13 19:57:25.924521 nn_wrapper-1.0.1/NetworkWrapper/NetworkWrapper.py
--rw-r--r--   0        0        0      837 2024-04-13 21:37:53.914985 nn_wrapper-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    10252 2024-04-13 21:37:21.523136 nn_wrapper-1.0.1/README.md
--rw-r--r--   0        0        0    10769 1970-01-01 00:00:00.000000 nn_wrapper-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-12 21:11:26.168898 nn_wrapper-1.0.2/LICENSE
+-rw-r--r--   0        0        0       43 2024-04-13 19:55:50.828702 nn_wrapper-1.0.2/NetworkWrapper/__init__.py
+-rw-r--r--   0        0        0    33351 2024-04-13 19:57:25.924521 nn_wrapper-1.0.2/NetworkWrapper/NetworkWrapper.py
+-rw-r--r--   0        0        0      838 2024-04-13 21:55:08.674549 nn_wrapper-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    10256 2024-04-13 21:55:08.678546 nn_wrapper-1.0.2/README.md
+-rw-r--r--   0        0        0    10905 1970-01-01 00:00:00.000000 nn_wrapper-1.0.2/PKG-INFO
```

### Comparing `nn_wrapper-1.0.1/LICENSE` & `nn_wrapper-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nn_wrapper-1.0.1/NetworkWrapper/NetworkWrapper.py` & `nn_wrapper-1.0.2/NetworkWrapper/NetworkWrapper.py`

 * *Files identical despite different names*

### Comparing `nn_wrapper-1.0.1/pyproject.toml` & `nn_wrapper-1.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "nn-wrapper"
-version = "1.0.1"
+version = "1.0.2"
 description = "A wrapper class for neural networks that makes working with them easier."
 authors = ["JohnConnor123 <ivan.eudokimoff2014@gmail.com>"]
 readme = "README.md"
 packages = [{include = "NetworkWrapper"}]
+repository = "https://github.com/JohnConnor123/NetworkWrapper"
 
 # poetry config pypi-token.testpypi <API-token>
 #[[tool.poetry.source]]
 #name = "torch-cuda"
 #url = "https://download.pytorch.org/whl/cu118/"
 #priority = "supplemental"
 
@@ -21,14 +22,10 @@
 tqdm = "4.66.1"
 matplotlib = "3.8.0"
 scikit-learn = "1.3.0"
 torch = ">= 2.1.0"
 torchvision= ">= 0.16.0"
 torchaudio = ">= 2.1.0"
 
-[[tool.poetry.source]]
-name = "PyPI"
-priority = "primary"
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nn_wrapper-1.0.1/README.md` & `nn_wrapper-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 The class contains 650 lines of code, and it took almost a month to write. Everything - from paths, separators, depending on the type of OS, type of device for training, and right down to the display formats of progress bars, figsizes (without processing in PyCharm, the pbar of Jupiter/colab moves out, but in Jupiter/colab the pbar PyCharm is moving out) are done AUTOMATICALLY :)
 
 And this class can do a lot more - incl. and further train the model from some epoch :) I started training for 20,50 or even 100 epochs and went for a walk/mind my own business - and then came and looked at all the statistics and loaded into the desired epoch (if you want). Or, using 1 line of code, I trimmed the saved model and optimizer weights for all epochs, starting with the desired one. Or even threw out all the era weights except the best one. And there is no need to restart training many times, fearing that the model will be overtrained or undertrained for the entered number of epochs. Just a fairy tale)
 
 The best way to support my creation is to star the project on Github :)
 
-GitHub: https://github.com/JohnConnor123/nn-wrapper
+GitHub: https://github.com/JohnConnor123/NetworkWrapper
 
 Contact email: ivan.eudokimoff2014@gmail.com
 
 P.s. There may be minor bugs (and I tried very hard to avoid them and spent more than a week debugging the code). If you have a bug, open an issue on the project's Github or just write to me by email.
 
 ## Quick usage guide
 P.s. Contains only the basic possibilities of the class
```

### Comparing `nn_wrapper-1.0.1/PKG-INFO` & `nn_wrapper-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: nn-wrapper
-Version: 1.0.1
+Version: 1.0.2
 Summary: A wrapper class for neural networks that makes working with them easier.
+Home-page: https://github.com/JohnConnor123/NetworkWrapper
 Author: JohnConnor123
 Author-email: ivan.eudokimoff2014@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: matplotlib (==3.8.0)
@@ -13,14 +14,15 @@
 Requires-Dist: pandas (==2.0.0)
 Requires-Dist: scikit-learn (==1.3.0)
 Requires-Dist: seaborn (==0.12.2)
 Requires-Dist: torch (>=2.1.0)
 Requires-Dist: torchaudio (>=2.1.0)
 Requires-Dist: torchvision (>=0.16.0)
 Requires-Dist: tqdm (==4.66.1)
+Project-URL: Repository, https://github.com/JohnConnor123/NetworkWrapper
 Description-Content-Type: text/markdown
 
 ## Description:
 
 NetworkWrapper is a convenience class for working with neural networks using PyTorch. 
 With it you can:
 * Train and retrain models
@@ -33,15 +35,15 @@
 
 The class contains 650 lines of code, and it took almost a month to write. Everything - from paths, separators, depending on the type of OS, type of device for training, and right down to the display formats of progress bars, figsizes (without processing in PyCharm, the pbar of Jupiter/colab moves out, but in Jupiter/colab the pbar PyCharm is moving out) are done AUTOMATICALLY :)
 
 And this class can do a lot more - incl. and further train the model from some epoch :) I started training for 20,50 or even 100 epochs and went for a walk/mind my own business - and then came and looked at all the statistics and loaded into the desired epoch (if you want). Or, using 1 line of code, I trimmed the saved model and optimizer weights for all epochs, starting with the desired one. Or even threw out all the era weights except the best one. And there is no need to restart training many times, fearing that the model will be overtrained or undertrained for the entered number of epochs. Just a fairy tale)
 
 The best way to support my creation is to star the project on Github :)
 
-GitHub: https://github.com/JohnConnor123/nn-wrapper
+GitHub: https://github.com/JohnConnor123/NetworkWrapper
 
 Contact email: ivan.eudokimoff2014@gmail.com
 
 P.s. There may be minor bugs (and I tried very hard to avoid them and spent more than a week debugging the code). If you have a bug, open an issue on the project's Github or just write to me by email.
 
 ## Quick usage guide
 P.s. Contains only the basic possibilities of the class
```


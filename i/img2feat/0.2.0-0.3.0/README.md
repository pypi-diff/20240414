# Comparing `tmp/img2feat-0.2.0.tar.gz` & `tmp/img2feat-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/img2feat-0.2.0.tar", last modified: Wed Apr 14 05:49:15 2021, max compression
+gzip compressed data, was "dist/img2feat-0.3.0.tar", last modified: Fri Apr 12 07:33:36 2024, max compression
```

## Comparing `img2feat-0.2.0.tar` & `img2feat-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 mtanaka   (1000) mtanaka   (1000)        0 2021-04-14 05:49:15.671953 img2feat-0.2.0/
--rw-rw-r--   0 mtanaka   (1000) mtanaka   (1000)     8465 2021-04-14 05:49:15.671953 img2feat-0.2.0/PKG-INFO
--rw-rw-r--   0 mtanaka   (1000) mtanaka   (1000)     5915 2021-04-14 05:49:04.000000 img2feat-0.2.0/README.rst
-drwxrwxr-x   0 mtanaka   (1000) mtanaka   (1000)        0 2021-04-14 05:49:15.667952 img2feat-0.2.0/img2feat/
--rw-rw-r--   0 mtanaka   (1000) mtanaka   (1000)      229 2021-04-14 05:48:01.000000 img2feat-0.2.0/img2feat/__init__.py
--rw-rw-r--   0 mtanaka   (1000) mtanaka   (1000)     4967 2021-04-14 05:48:01.000000 img2feat-0.2.0/img2feat/antbee.py
--rw-rw-r--   0 mtanaka   (1000) mtanaka   (1000)     3029 2021-04-14 05:48:01.000000 img2feat-0.2.0/img2feat/aug.py
--rw-rw-r--   0 mtanaka   (1000) mtanaka   (1000)     5322 2021-04-14 05:48:30.000000 img2feat-0.2.0/img2feat/buildnet.py
--rw-rw-r--   0 mtanaka   (1000) mtanaka   (1000)     5111 2021-04-14 05:48:01.000000 img2feat-0.2.0/img2feat/cnn.py
-drwxrwxr-x   0 mtanaka   (1000) mtanaka   (1000)        0 2021-04-14 05:49:15.671953 img2feat-0.2.0/img2feat.egg-info/
--rw-rw-r--   0 mtanaka   (1000) mtanaka   (1000)     8465 2021-04-14 05:49:15.000000 img2feat-0.2.0/img2feat.egg-info/PKG-INFO
--rw-rw-r--   0 mtanaka   (1000) mtanaka   (1000)      312 2021-04-14 05:49:15.000000 img2feat-0.2.0/img2feat.egg-info/SOURCES.txt
--rw-rw-r--   0 mtanaka   (1000) mtanaka   (1000)        1 2021-04-14 05:49:15.000000 img2feat-0.2.0/img2feat.egg-info/dependency_links.txt
--rw-rw-r--   0 mtanaka   (1000) mtanaka   (1000)       76 2021-04-14 05:49:15.000000 img2feat-0.2.0/img2feat.egg-info/requires.txt
--rw-rw-r--   0 mtanaka   (1000) mtanaka   (1000)       15 2021-04-14 05:49:15.000000 img2feat-0.2.0/img2feat.egg-info/top_level.txt
--rw-rw-r--   0 mtanaka   (1000) mtanaka   (1000)       38 2021-04-14 05:49:15.671953 img2feat-0.2.0/setup.cfg
--rw-rw-r--   0 mtanaka   (1000) mtanaka   (1000)     1435 2021-04-14 05:48:11.000000 img2feat-0.2.0/setup.py
-drwxrwxr-x   0 mtanaka   (1000) mtanaka   (1000)        0 2021-04-14 05:49:15.671953 img2feat-0.2.0/tests/
--rw-rw-r--   0 mtanaka   (1000) mtanaka   (1000)        0 2021-04-14 05:48:01.000000 img2feat-0.2.0/tests/__init__.py
--rw-rw-r--   0 mtanaka   (1000) mtanaka   (1000)     3769 2021-04-14 05:48:01.000000 img2feat-0.2.0/tests/test_img2feat.py
+drwxrwxr-x   0 mtanaka   (1004) mtanaka   (1004)        0 2024-04-12 07:33:36.864314 img2feat-0.3.0/
+-rw-rw-r--   0 mtanaka   (1004) mtanaka   (1004)     6311 2024-04-12 07:33:36.864314 img2feat-0.3.0/PKG-INFO
+-rw-rw-r--   0 mtanaka   (1004) mtanaka   (1004)     5937 2024-04-12 07:31:28.000000 img2feat-0.3.0/README.rst
+drwxrwxr-x   0 mtanaka   (1004) mtanaka   (1004)        0 2024-04-12 07:33:36.860314 img2feat-0.3.0/img2feat/
+-rw-rw-r--   0 mtanaka   (1004) mtanaka   (1004)      229 2023-07-07 04:11:32.000000 img2feat-0.3.0/img2feat/__init__.py
+-rw-rw-r--   0 mtanaka   (1004) mtanaka   (1004)     4967 2023-07-07 04:11:32.000000 img2feat-0.3.0/img2feat/antbee.py
+-rw-rw-r--   0 mtanaka   (1004) mtanaka   (1004)     3029 2023-07-07 04:11:32.000000 img2feat-0.3.0/img2feat/aug.py
+-rw-rw-r--   0 mtanaka   (1004) mtanaka   (1004)     7471 2024-04-12 07:29:19.000000 img2feat-0.3.0/img2feat/buildnet.py
+-rw-rw-r--   0 mtanaka   (1004) mtanaka   (1004)     5111 2023-07-07 04:11:32.000000 img2feat-0.3.0/img2feat/cnn.py
+drwxrwxr-x   0 mtanaka   (1004) mtanaka   (1004)        0 2024-04-12 07:33:36.864314 img2feat-0.3.0/img2feat.egg-info/
+-rw-rw-r--   0 mtanaka   (1004) mtanaka   (1004)     6311 2024-04-12 07:33:36.000000 img2feat-0.3.0/img2feat.egg-info/PKG-INFO
+-rw-rw-r--   0 mtanaka   (1004) mtanaka   (1004)      312 2024-04-12 07:33:36.000000 img2feat-0.3.0/img2feat.egg-info/SOURCES.txt
+-rw-rw-r--   0 mtanaka   (1004) mtanaka   (1004)        1 2024-04-12 07:33:36.000000 img2feat-0.3.0/img2feat.egg-info/dependency_links.txt
+-rw-rw-r--   0 mtanaka   (1004) mtanaka   (1004)       76 2024-04-12 07:33:36.000000 img2feat-0.3.0/img2feat.egg-info/requires.txt
+-rw-rw-r--   0 mtanaka   (1004) mtanaka   (1004)       15 2024-04-12 07:33:36.000000 img2feat-0.3.0/img2feat.egg-info/top_level.txt
+-rw-rw-r--   0 mtanaka   (1004) mtanaka   (1004)       38 2024-04-12 07:33:36.864314 img2feat-0.3.0/setup.cfg
+-rw-rw-r--   0 mtanaka   (1004) mtanaka   (1004)     1435 2024-04-12 07:28:49.000000 img2feat-0.3.0/setup.py
+drwxrwxr-x   0 mtanaka   (1004) mtanaka   (1004)        0 2024-04-12 07:33:36.864314 img2feat-0.3.0/tests/
+-rw-rw-r--   0 mtanaka   (1004) mtanaka   (1004)        0 2023-07-07 04:11:32.000000 img2feat-0.3.0/tests/__init__.py
+-rw-rw-r--   0 mtanaka   (1004) mtanaka   (1004)     3781 2024-04-12 07:29:31.000000 img2feat-0.3.0/tests/test_img2feat.py
```

### Comparing `img2feat-0.2.0/README.rst` & `img2feat-0.3.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,36 +6,34 @@
 
 `Github <https://github.com/mastnk/img2feat/>`__
 `PyPI <https://pypi.org/project/img2feat/>`__
 
 Installation
 ------------
 
-::
-
-   % pip install img2feat
+``% pip install img2feat``
 
 Required libraries: numpy, torch, torchvision, opencv-python
 
 *class* CNN
 -----------
 
 The CNN converts a list of numpy images to features, where numpy image
 is assumed opencv format, or [Height, Width, BGR]. The shape of the
 output features is [ length of the list of the input images,
 *dim_feature* of the CNN].
 
 Available networks: alexnet, vgg11, vgg13, vgg16, vgg19, resnet18,
 resnet34, resnet101, resnet152, densenet121, densenet161, densenet169,
-densenet201 googlenet, mobilenet
+densenet201 googlenet, mobilenet vit_b_16
 
 .. code:: python
 
-   from img2feat import CNN
-   net = CNN('vgg11')
+   from img2feat import BuildNet
+   net = BuildNet.build('vgg11')
    x = net( [img] )
 
 Methods
 ~~~~~~~
 
 -  **available_networks**\ () -> list of string
```

### Comparing `img2feat-0.2.0/img2feat/antbee.py` & `img2feat-0.3.0/img2feat/antbee.py`

 * *Files identical despite different names*

### Comparing `img2feat-0.2.0/img2feat/aug.py` & `img2feat-0.3.0/img2feat/aug.py`

 * *Files identical despite different names*

### Comparing `img2feat-0.2.0/img2feat/cnn.py` & `img2feat-0.3.0/img2feat/cnn.py`

 * *Files identical despite different names*

### Comparing `img2feat-0.2.0/setup.py` & `img2feat-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from setuptools import setup, find_packages
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name= 'img2feat', # Application name:
-    version= '0.2.0', # Version number
+    version= '0.3.0', # Version number
 
     author= 'Masayuki Tanaka', # Author name
     author_email= 'mastnk@gmail.com', # Author mail
 
     url='https://github.com/mastnk/img2feat', # Details
     description='Convert image to feature based on convolutional neural network (CNN).', # short description
     long_description=read('README.rst'), # long description
```

### Comparing `img2feat-0.2.0/tests/test_img2feat.py` & `img2feat-0.3.0/tests/test_img2feat.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 ###################################################################
     def test_buildnet(self):
         img = torch.rand( (1,3,224,224), dtype=torch.float32 )
 
 #        names = BuildNet.available_names()
-        names = ['vgg11', 'resnet18']
+        names = ['vgg11', 'resnet18', 'vit_b_16']
         for name in names:
             net, dim_feature = BuildNet.build( name )
             feat = net( img )
             self.assertEqual( feat.shape[0], 1 )
             self.assertEqual( feat.shape[1], dim_feature )
             self.assertEqual( feat.shape[2], 1 )
             self.assertEqual( feat.shape[3], 1 )
```


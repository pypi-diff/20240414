# Comparing `tmp/xaivision-0.1.0.tar.gz` & `tmp/xaivision-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xaivision-0.1.0.tar", max compression
+gzip compressed data, was "xaivision-0.2.0.tar", max compression
```

## Comparing `xaivision-0.1.0.tar` & `xaivision-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1114 2024-04-11 11:21:56.989947 xaivision-0.1.0/README.md
--rw-r--r--   0        0        0      265 2024-04-13 18:45:31.122738 xaivision-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       61 2024-04-13 15:44:32.244089 xaivision-0.1.0/xaivision/__init__.py
--rw-r--r--   0        0        0     2494 2024-02-07 15:13:44.910944 xaivision-0.1.0/xaivision/nmf_func.py
--rw-r--r--   0        0        0    12421 2024-04-13 13:35:46.683250 xaivision-0.1.0/xaivision/utils.py
--rw-r--r--   0        0        0     6619 2024-04-13 14:37:46.935839 xaivision-0.1.0/xaivision/xai_tools.py
--rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 xaivision-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1114 2024-04-11 11:21:56.989947 xaivision-0.2.0/README.md
+-rw-r--r--   0        0        0      265 2024-04-13 22:16:20.110120 xaivision-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-04-13 15:44:32.244089 xaivision-0.2.0/xaivision/__init__.py
+-rw-r--r--   0        0        0     2847 2024-04-13 21:30:38.041957 xaivision-0.2.0/xaivision/nmf_func.py
+-rw-r--r--   0        0        0    12632 2024-04-13 22:06:09.038199 xaivision-0.2.0/xaivision/utils.py
+-rw-r--r--   0        0        0     6856 2024-04-13 22:02:31.965352 xaivision-0.2.0/xaivision/xai_tools.py
+-rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 xaivision-0.2.0/PKG-INFO
```

### Comparing `xaivision-0.1.0/README.md` & `xaivision-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `xaivision-0.1.0/xaivision/nmf_func.py` & `xaivision-0.2.0/xaivision/nmf_func.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,24 @@
-import torch, math, time
+import torch
+import math
+import time
 
 EPSILON = 1e-7
 
+
 # NMF by multiplictive updates
-def NMF(V, k, W=None, H=None, random_seed=None, max_iter=200, tol=1e-4, cuda=True, verbose=False):
+def NMF(V,
+        k,
+        W=None,
+        H=None,
+        random_seed=None,
+        max_iter=200,
+        tol=1e-4,
+        cuda=True,
+        verbose=False):
 
     if verbose:
         start_time = time.time()
 
     scale = math.sqrt(abs(V.mean()) / k)
 
     if random_seed is not None:
@@ -46,23 +57,30 @@
 
     error_at_init = approximation_error(V, W, H, square_root=True)
     previous_error = error_at_init
 
     VH = None
     HH = None
     for n_iter in range(max_iter):
-        W, H, VH, HH = multiplicative_update_step(V, W, H, update_H=update_H, VH = VH, HH = HH)
+        W, H, VH, HH = multiplicative_update_step(V,
+                                                  W,
+                                                  H,
+                                                  update_H=update_H,
+                                                  VH=VH,
+                                                  HH=HH)
         if tol > 0 and n_iter % 10 == 0:
             error = approximation_error(V, W, H, square_root=True)
 
             if (previous_error - error) / error_at_init < tol:
                 break
             previous_error = error
     if verbose:
-        print('Exited after {} iterations. Total time: {} seconds'.format(n_iter+1, time.time()-start_time))
+        print('Exited after {} iterations. Total time: {} seconds'.format(
+            n_iter + 1,
+            time.time() - start_time))
     return W, H
 
 
 def multiplicative_update_step(V, W, H, update_H=True, VH=None, HH=None):
     # update operation for W
     if VH is None:
         assert HH is None
@@ -85,8 +103,8 @@
 
     return W, H, VH, HH
 
 
 # NMF objective
 def approximation_error(V, W, H, square_root=True):
     # Frobenius norm
-    return torch.norm(V - torch.mm(W, H))
+    return torch.norm(V - torch.mm(W, H))
```

### Comparing `xaivision-0.1.0/xaivision/utils.py` & `xaivision-0.2.0/xaivision/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,55 +5,58 @@
 from torchinfo import summary
 from torchviz import make_dot
 
 import h5py
 import torch.nn as nn
 
 import onnx
-import os
 
 import sys
 from pathlib import Path
 
 sys.path.append(str(Path(__file__).resolve().parent))
-from nmf_func import NMF
+try:
+    from nmf_func import NMF
+except (Exception, ):
+    raise
+
 
-    
 class MedPCacheDataset_normalised():
     """
-    Dataset interface of RAISE-LPBF-Laser benchmark cache single frame power prediction.
+    Dataset interface of RAISE-LPBF-Laser benchmark cache single frame power
+    prediction.
     """
 
     def __init__(self, cache_fp, nominal_laser_params=[900, 215], **_):
         self.cache_fp = cache_fp
-        self.nominal_laser_params = np.array(nominal_laser_params).astype(np.float32)
+        self.nominal_laser_params = np.array(nominal_laser_params).astype(
+            np.float32)
 
-        with h5py.File(self.cache_fp,"r") as h5f:
+        with h5py.File(self.cache_fp, "r") as h5f:
             self._len = len(h5f["x"])
 
     def __len__(self):
         return self._len
 
     def __getitem__(self, index):
-        with h5py.File(self.cache_fp,"r") as h5f:
-            x = (
-                np.expand_dims(np.array(h5f["x"][index]).astype(np.float32), axis=0)
-            )
-            y = (
-                np.array(h5f["y"][index], dtype=np.float32)
-                / self.nominal_laser_params
-            )
+        with h5py.File(self.cache_fp, "r") as h5f:
+            x = (np.expand_dims(np.array(h5f["x"][index]).astype(np.float32),
+                                axis=0))
+            y = (np.array(h5f["y"][index], dtype=np.float32) /
+                 self.nominal_laser_params)
         return x, y
-    
+
 
 class YourModelWithoutLastLayers(nn.Module):
+
     def __init__(self, original_model, remove_layers):
         super(YourModelWithoutLastLayers, self).__init__()
-        
-        self.features = nn.Sequential(*list(original_model.children())[:-1*remove_layers])
+
+        self.features = nn.Sequential(
+            *list(original_model.children())[:-1 * remove_layers])
 
     def forward(self, x):
         # Forward pass through the modified layers
         x = self.features(x)
         return x
 
 
@@ -65,15 +68,14 @@
         - model (str): Path to the model or the actual model loaded
 
     Returns:
         Model in Python format.
 
     .. todo::
         -
-        
     """
     model_py = convert(model)
     return model_py
 
 
 def load_sample(data, sample):
     """
@@ -95,254 +97,274 @@
 def check_onnx_torch_out(onnx_model_path, torch_model, model_input):
     """
     Compare outputs of an ONNX model and a PyTorch model given a data point.
 
     Parameters:
         - onnx_model_path (str): Path to the ONNX model file.
         - torch_model (torch.nn.Module): PyTorch model.
-        - datapoint (tuple): A tuple containing input data and its corresponding labels.
+        - datapoint (tuple): A tuple containing input data and its
+        corresponding labels.
 
     Returns:
         None
     """
-    
-        
+
     data_inp = np.expand_dims(model_input, axis=0)
-    
+
     # for layers in dict(torch_model.named_modules()): print (layers)
 
     data_torch = torch.from_numpy(data_inp)
     torch_model.eval()
     out_torch = torch_model(data_torch)
 
-    
-
-    
     # output =[node.name for node in model.graph.output]
     onnx_model = onnx.load(onnx_model_path)
     input_all = [node.name for node in onnx_model.graph.input]
-    input_initializer =  [node.name for node in onnx_model.graph.initializer]
-    net_feed_input = list(set(input_all)  - set(input_initializer))
+    input_initializer = [node.name for node in onnx_model.graph.initializer]
+    net_feed_input = list(set(input_all) - set(input_initializer))
 
     # print('Inputs: ', net_feed_input[0])
     # print('Outputs: ', output[0])
     ort_sess = ort.InferenceSession(onnx_model_path)
     outputs_ort = ort_sess.run(None, {net_feed_input[0]: data_inp})
 
     diagnosis = "Torch output : " + str(out_torch) + "\n"
     diagnosis = diagnosis + "ONNX output : " + str(outputs_ort) + "\n"
     diagnosis = diagnosis + "-------------------------------\n"
     diagnosis = diagnosis + "Difference between onnx and pytorch model: "
-    diagnosis = diagnosis + str(torch.max(torch.abs(torch.from_numpy(outputs_ort[0]) - out_torch)))
-        # print(np.allclose(outputs_ort, out_torch.detach().numpy(), atol=1.e-7))
+    diagnosis = diagnosis + str(
+        torch.max(torch.abs(torch.from_numpy(outputs_ort[0]) - out_torch)))
+    # print(np.allclose(outputs_ort, out_torch.detach().numpy(), atol=1.e-7))
     return diagnosis
 
-def check_model_data_compatibility(model,data_size, output_size):
+
+def check_model_data_compatibility(model, data_size, output_size):
     # create some sample input data
     x = np.expand_dims(torch.randn(data_size), axis=0)
     x = torch.from_numpy(x)
     # generate predictions for the sample data
     y = model(x).squeeze(0).detach().numpy()
     return y.shape == output_size
 
-def model_details(model,data_size):
+
+def model_details(model, data_size):
     """
-    Retrieve details about the model including architecture visualization and summary.
+    Retrieve details about the model including architecture visualization and
+    summary.
 
     Parameters:
         - model (torch.nn.Module): The PyTorch model to inspect.
-        - data_size (tuple): The size of the input data (e.g., (channels, height, width)).
+        - data_size (tuple): The size of the input data (e.g., (channels,
+        height, width)).
 
     Returns:
         tuple: A tuple containing two elements:
-            - dot (graphviz.Digraph): Graph visualization of the model architecture.
-            - sum (str): Summary of the model including the number of parameters and layers.
+            - dot (graphviz.Digraph): Graph visualization of the model
+            architecture.
+            - sum (str): Summary of the model including the number of
+            parameters and layers.
     """
 
     # create some sample input data
     x = np.expand_dims(torch.randn(data_size), axis=0)
     x = torch.from_numpy(x)
     # generate predictions for the sample data
     y = model(x)
 
     # generate a model architecture visualization
     dot = make_dot(y.mean(),
-            params=dict(model.named_parameters()),
-            show_attrs=True,
-            show_saved=True)
-    
+                   params=dict(model.named_parameters()),
+                   show_attrs=True,
+                   show_saved=True)
 
     sum = summary(model, input_size=x.shape, verbose=0)
-    
+
     model_output = y.squeeze(0).detach().numpy()
     model_input_txt = "Model input shape: " + str(data_size)
     model_output_txt = "Model output shape: " + str(model_output.shape)
-    summary_with_text = str(sum) + "\n" + model_input_txt + "\n" + model_output_txt
-    summary_with_text = summary_with_text + "\n" + "=========================================================================================="
-
+    summary_with_text = str(
+        sum) + "\n" + model_input_txt + "\n" + model_output_txt
+    summary_with_text = summary_with_text + "\n" + "=\
+=======================================================================\
+=================="
 
     return dot, summary_with_text
 
-def sample_details(model,datapoint):
+
+def sample_details(model, datapoint):
     """
     Get details about a sample by passing it through the model.
 
     Parameters:
         - model (torch.nn.Module): The PyTorch model to use.
         - datapoint (numpy.ndarray): The input data point.
 
     Returns:
         tuple: A tuple containing two elements:
             - input_data (numpy.ndarray): The input data after squeezing.
-            - output_data (numpy.ndarray): The output data from the model after squeezing, converting to numpy array,
+            - output_data (numpy.ndarray): The output data from the model
+            after squeezing, converting to numpy array,
               and detaching from the computation graph.
     """
 
     data_inp = np.expand_dims(datapoint, axis=0)
     data_torch = torch.from_numpy(data_inp)
     model.eval()
-    out_torch = model(data_torch).squeeze(0).detach().numpy().astype(np.float64)
-    
+    out_torch = model(data_torch).squeeze(0).detach().numpy().astype(
+        np.float64)
+
     return out_torch
-   
 
-def conv2d_feature_vis_no_extra_layers(model,datasample):
+
+def conv2d_feature_vis_no_extra_layers(model, datasample):
     """
-    Extracts and visualizes feature maps from Conv2d layers in a given model without additional layers.
+    Extracts and visualizes feature maps from Conv2d layers in a given model
+    without additional layers.
 
     Parameters:
-        - model (torch.nn.Module): The PyTorch model from which to extract feature maps.
-        - datasample (tuple): A tuple containing input data and its corresponding labels.
+        - model (torch.nn.Module): The PyTorch model from which to extract
+        feature maps.
+        - datasample (tuple): A tuple containing input data and its
+        corresponding labels.
 
     Returns:
         tuple: A tuple containing two elements:
             - processed (list): A list of processed feature maps.
-            - names (list): A list of names of the Conv2d layers whose feature maps were extracted.
+            - names (list): A list of names of the Conv2d layers whose feature
+            maps were extracted.
     """
 
-    model_weights =[]
+    model_weights = []
     conv_layers = []
 
     model_children = list(model.children())
     counter = 0
 
     for child in range(len(model_children)):
-        if type(model_children[child]) == nn.Conv2d:
-            counter+=1
+        if type(model_children[child]) is nn.Conv2d:
+            counter += 1
             model_weights.append(model_children[child].weight)
             conv_layers.append(model_children[child])
-        elif type(model_children[child]) == nn.Sequential:
+        elif type(model_children[child]) is nn.Sequential:
             for i in range(len(model_children[child])):
                 for c in model_children[child][i].children():
-                    if type(c) == nn.Conv2d:
-                        counter+=1
+                    if type(c) is nn.Conv2d:
+                        counter += 1
                         model_weights.append(c.weight)
                         conv_layers.append(c)
 
     outputs = []
     names = []
     data_inp = np.expand_dims(datasample, axis=0)
     image = torch.from_numpy(data_inp)
-    
+
     for layer in conv_layers:
         image = layer(image)
         outputs.append(image)
         names.append(str(layer))
-    
-    #print feature_maps
+
+    # print feature_maps
     # for feature_map in outputs:
     #     print(feature_map.shape)
 
     processed = []
     for feature_map in outputs:
         feature_map = feature_map.squeeze(0)
-        gray_scale = torch.sum(feature_map,0)
+        gray_scale = torch.sum(feature_map, 0)
         gray_scale = gray_scale / feature_map.shape[0]
         processed.append(gray_scale.data.cpu().numpy())
     # for fm in processed:
     #     print(fm.shape)
 
     return processed, names
 
 
 def find_convolutions(model):
     """
     Finds convolutional layers within a PyTorch model.
 
     Args:
-        - model (torch.nn.Module): The PyTorch model to search for convolutional layers.
+        - model (torch.nn.Module): The PyTorch model to search for
+        convolutional layers.
 
     Returns:
         tuple: A tuple containing two lists:
             - The indices of convolutional layers found in the model.
             - The layers containing convolutional layers found in the model.
     """
 
     model_children = list(model.children())
     layers = []
     spot_convs = []
 
     for layer_cnt, child in enumerate(range(len(model_children))):
-        if type(model_children[child]) == nn.Sequential:
+        if type(model_children[child]) is nn.Sequential:
             for i in range(len(model_children[child])):
                 for cnt, c in enumerate(model_children[child][i].children()):
                     layers.append(model_children[child])
-                    if type(c) == nn.Conv2d:
+                    if type(c) is nn.Conv2d:
                         spot_convs.append(cnt)
         else:
             layers.append(model_children[child])
-            if type(model_children[child]) == nn.Conv2d:
+            if type(model_children[child]) is nn.Conv2d:
                 spot_convs.append(layer_cnt)
-    
-    return spot_convs,layers
+
+    return spot_convs, layers
 
 
-def conv2d_feature_vis_extra_layers(model,datasample):
+def conv2d_feature_vis_extra_layers(model, datasample):
     """
-    Extracts and visualizes feature maps from Conv2d layers in a given model with additional layers.
+    Extracts and visualizes feature maps from Conv2d layers in a given model
+    with additional layers.
 
     Parameters:
-        - model (torch.nn.Module): The PyTorch model from which to extract feature maps.
-        - datasample (tuple): A tuple containing input data and its corresponding labels.
+        - model (torch.nn.Module): The PyTorch model from which to extract
+        feature maps.
+        - datasample (tuple): A tuple containing input data and its
+        corresponding labels.
 
     Returns:
         tuple: A tuple containing two elements:
             - processed (list): A list of processed feature maps.
-            - names (list): A list of names of the Conv2d layers whose feature maps were extracted.
+            - names (list): A list of names of the Conv2d layers whose feature
+            maps were extracted.
     """
 
-    spot_convs,layers = find_convolutions(model)
+    spot_convs, layers = find_convolutions(model)
 
     conv_outputs = []
     conv_names = []
     data_inp = np.expand_dims(datasample, axis=0)
     image = torch.from_numpy(data_inp)
-    
-    for i,layer in enumerate(layers[:spot_convs[-1]+1]):
+
+    for i, layer in enumerate(layers[:spot_convs[-1] + 1]):
         image = layer(image)
         if i in spot_convs:
             conv_outputs.append(image)
             conv_names.append(str(layer))
 
     processed = []
     for feature_map in conv_outputs:
         feature_map = feature_map.squeeze(0)
-        gray_scale = torch.sum(feature_map,0)
+        gray_scale = torch.sum(feature_map, 0)
         gray_scale = gray_scale / feature_map.shape[0]
         processed.append(gray_scale.data.cpu().numpy())
 
     return processed, conv_names
 
+
 def find_components(model, datasample, components):
     """
-    Find components using Non-Negative Matrix Factorization (NMF) based on model activations.
+    Find components using Non-Negative Matrix Factorization (NMF) based on
+    model activations.
 
     Args:
         - model (torch.nn.Module): The neural network model.
-        - datasample (tuple): A tuple containing input data and its corresponding label, Expected format: (input_data, label).
+        - datasample (tuple): A tuple containing input data and its
+        corresponding label, Expected format: (input_data, label).
         - components (int): The number of components to extract.
 
     Returns:
         numpy.ndarray: Heatmaps of the components for the given input data.
 
     Raises:
         ValueError: If the components argument is not a positive integer.
@@ -351,32 +373,28 @@
     image = torch.from_numpy(data_inp)
 
     spot_convs, layers = find_convolutions(model)
     remove_until_conv = len(layers) - (spot_convs[-1] + 1)
 
     new_model = YourModelWithoutLastLayers(model, remove_until_conv)
     features = new_model(image)
-    
-    flat_features = features.permute(0, 2, 3, 1).contiguous().view((-1, features.size(1))) # NxCxHxW -> (N*H*W)xC
+
+    flat_features = features.permute(0, 2, 3, 1).contiguous().view(
+        (-1, features.size(1)))  # NxCxHxW -> (N*H*W)xC
 
     K = components
     with torch.no_grad():
         W, _ = NMF(flat_features, K, random_seed=0, cuda=False, max_iter=50)
 
-    heatmaps = W.cpu().view(features.size(0), features.size(2), features.size(3), K).permute(0, 3, 1, 2) # (N*H*W)xK -> NxKxHxW
-    heatmaps = torch.nn.functional.interpolate(heatmaps, size=np.squeeze(datasample).shape, mode='bilinear', align_corners=False) ## 14x14 ->
-    heatmaps /= heatmaps.max(dim=3, keepdim=True)[0].max(dim=2, keepdim=True)[0] # normalize by factor (i.e., 1 of K)
+    heatmaps = W.cpu().view(features.size(0), features.size(2),
+                            features.size(3),
+                            K).permute(0, 3, 1, 2)  # (N*H*W)xK -> NxKxHxW
+    heatmaps = torch.nn.functional.interpolate(
+        heatmaps,
+        size=np.squeeze(datasample).shape,
+        mode='bilinear',
+        align_corners=False)
+    heatmaps /= heatmaps.max(dim=3, keepdim=True)[0].max(
+        dim=2, keepdim=True)[0]  # normalize by factor (i.e., 1 of K)
     heatmaps = heatmaps.cpu().numpy()
 
     return heatmaps
-        
-        
-    
-
-            
-
-
-
-
-
-
-
```

### Comparing `xaivision-0.1.0/xaivision/xai_tools.py` & `xaivision-0.2.0/xaivision/xai_tools.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import numpy as np
 
 import torch
 from torch.utils.data import DataLoader
 
 import matplotlib.pyplot as plt
 
@@ -11,199 +10,206 @@
 import h5py
 
 import pandas as pd
 
 from captum.attr import IntegratedGradients, DeepLift
 
 from itertools import chain
-        
+
+
 class ImageDataset_normalised(torch.utils.data.Dataset):
-    def __init__(self,path,nominal_laser_params=[900, 215]):
+
+    def __init__(self, path, nominal_laser_params=[900, 215]):
         self.path = path
-        self.nominal_laser_params = np.array(nominal_laser_params).astype(np.float32)
+        self.nominal_laser_params = np.array(nominal_laser_params).astype(
+            np.float32)
 
     def __getitem__(self, idx):
         """Get image and target y values"""
         with h5py.File(self.path) as h5f:
-            x = (
-                np.expand_dims(np.array(h5f["x"][idx]).astype(np.float32), axis=0)
-            )
-            y = (
-                np.array(h5f["y"][idx], dtype=np.float32)
-                / self.nominal_laser_params
-            )
-        
+            x = (np.expand_dims(np.array(h5f["x"][idx]).astype(np.float32),
+                                axis=0))
+            y = (np.array(h5f["y"][idx], dtype=np.float32) /
+                 self.nominal_laser_params)
+
         image = np.array(x)
 
         # Get target
         target = torch.tensor(y)
         return image, target
-    
+
     def __len__(self):
         with h5py.File(self.path) as h5f:
             return len(h5f['x'])
 
-def vision_shap(data,batch_size,model_py,model_input):
 
+def vision_shap(data, batch_size, model_py, model_input):
     """Compute SHAP (SHapley Additive exPlanations) values for a given image.
 
     Args:
         - data: The dataset to be used.
         - batch_size (int): Batch size for DataLoader.
         - model_py: The PyTorch model.
-        - sample_index (int): Index of the sample image for which SHAP values are computed.
+        - sample_index (int): Index of the sample image for which SHAP values
+        are computed.
 
     Returns:
         list: A list of matplotlib figures containing SHAP value plots.
 
     """
 
     ds = ImageDataset_normalised(data)
-    
+
     device = torch.device('cpu')
-    shap_loader = DataLoader(ds,batch_size=batch_size,shuffle=True)
-    background,_ = next(iter(shap_loader))
-    background=background.to(device)
+    shap_loader = DataLoader(ds, batch_size=batch_size, shuffle=True)
+    background, _ = next(iter(shap_loader))
+    background = background.to(device)
 
     model = model_py.to(device)
 
     explainer = shap.DeepExplainer(model, background)
 
-    test_image = np.expand_dims(model_input,axis=0)
+    test_image = np.expand_dims(model_input, axis=0)
     test_image = torch.tensor(test_image).to(device)
     shap_values = explainer.shap_values(test_image)
 
     if len(np.array(shap_values).shape) == 5:
-        shap_numpy = np.array(shap_values).transpose(0,1,3,4,2)  
+        shap_numpy = np.array(shap_values).transpose(4, 0, 2, 3, 1)
     else:
-        shap_numpy = np.array(shap_values).transpose(0,2,3,1)
-        shap_numpy = np.expand_dims(shap_numpy,axis=0)
-        
-    test_numpy = np.array([np.array(img) for img in test_image]).transpose(0,2,3,1)
-    
+        shap_numpy = np.array(shap_values).transpose(0, 2, 3, 1)
+        shap_numpy = np.expand_dims(shap_numpy, axis=0)
+
+    test_numpy = np.array([np.array(img)
+                           for img in test_image]).transpose(0, 2, 3, 1)
+
     plots = []
     for value in shap_numpy:
-        shap.image_plot(value,test_numpy,show=False)
+        shap.image_plot(value, test_numpy, show=False)
         plots.append(plt.gcf())
         plt.close()
     return plots
 
-def shap_overview(data,batch_background,batch_test,model_py):
 
-    """Compute SHAP (SHapley Additive exPlanations) overview for a given dataset.
+def shap_overview(data, batch_background, batch_test, model_py):
+    """Compute SHAP (SHapley Additive exPlanations) overview for a given
+    dataset.
 
     Args:
         - data: The dataset to be used.
-        - batch_background (int): Batch size for background data for SHAP computation.
+        - batch_background (int): Batch size for background data for SHAP
+        computation.
         - batch_test (int): Batch size for test data for SHAP computation.
         - model_py: The PyTorch model.
 
     Returns:
         list: A list of matplotlib figures containing SHAP summary plots.
     """
 
     ds = ImageDataset_normalised(data)
-    
 
     device = torch.device('cpu')
 
-    shap_loader = DataLoader(ds,batch_size=batch_background,shuffle=True)
-    background,_ = next(iter(shap_loader))
-    background=background.to(device)
-
-    shap_tester = DataLoader(ds,batch_size=batch_test,shuffle=True)
-    test_batch,_ = next(iter(shap_tester))
-    test_batch=test_batch.to(device)
+    shap_loader = DataLoader(ds, batch_size=batch_background, shuffle=True)
+    background, _ = next(iter(shap_loader))
+    background = background.to(device)
+
+    shap_tester = DataLoader(ds, batch_size=batch_test, shuffle=True)
+    test_batch, _ = next(iter(shap_tester))
+    test_batch = test_batch.to(device)
 
     model = model_py.to(device)
 
     explainer = shap.DeepExplainer(model, background)
 
     shap_values = explainer.shap_values(test_batch)
-    
+
     if len(np.array(shap_values).shape) == 5:
-        shap_numpy = np.array(shap_values).transpose(0,1,3,4,2)
+        shap_numpy = np.array(shap_values).transpose(4, 0, 2, 3, 1)
     else:
-        shap_numpy = np.array(shap_values).transpose(0,2,3,1)
-        shap_numpy = np.expand_dims(shap_numpy,axis=0)
+        shap_numpy = np.array(shap_values).transpose(0, 2, 3, 1)
+        shap_numpy = np.expand_dims(shap_numpy, axis=0)
     plots = []
-    for i,value in enumerate(shap_numpy):
+    for i, value in enumerate(shap_numpy):
         shap_lists = []
         value_lists = []
         for j, sample in enumerate(value):
-            x,y = np.squeeze(sample).shape[0], np.squeeze(sample).shape[1]
+            x, y = np.squeeze(sample).shape[0], np.squeeze(sample).shape[1]
             flatten_list_shap = list(chain.from_iterable(np.squeeze(sample)))
-            flatten_list_value = list(chain.from_iterable(np.squeeze(test_batch[j])))
+            flatten_list_value = list(
+                chain.from_iterable(np.squeeze(test_batch[j])))
             shap_lists.append(flatten_list_shap)
             value_lists.append(flatten_list_value)
-        
+
         df = pd.DataFrame({
-    "mean_abs_shap": np.mean(np.abs(np.array(shap_lists)), axis=0), 
-    "stdev_abs_shap": np.std(np.abs(np.array(shap_lists)), axis=0)
-})
+            "mean_abs_shap":
+            np.mean(np.abs(np.array(shap_lists)), axis=0),
+            "stdev_abs_shap":
+            np.std(np.abs(np.array(shap_lists)), axis=0)
+        })
         df_sorted = df.sort_values("stdev_abs_shap", ascending=False)[:10]
         shap_values = []
         pixel_values = []
         feature_names = []
         num_values = 10
         for k in range(num_values):
-             pixel_num = df_sorted.index[k]
-             x_unflattened, y_unflattened = int(pixel_num/x), int(pixel_num%y)
-             name = "Pixel ("+str(x_unflattened)+","+str(y_unflattened)+")"
-             shap_values.append(np.array(shap_lists)[:,pixel_num])
-             pixel_values.append(np.array(value_lists)[:,pixel_num])
-             feature_names.append(name)
-        shap_values = np.array(shap_values).transpose(1,0)
-        pixel_values = np.array(pixel_values).transpose(1,0)
-        
-        shap.summary_plot(shap_values,pixel_values,feature_names=feature_names,show=False)
-        
+            pixel_num = df_sorted.index[k]
+            x_unflattened, y_unflattened = int(pixel_num / x), int(pixel_num %
+                                                                   y)
+            name = "Pixel (" + str(x_unflattened) + "," + str(
+                y_unflattened) + ")"
+            shap_values.append(np.array(shap_lists)[:, pixel_num])
+            pixel_values.append(np.array(value_lists)[:, pixel_num])
+            feature_names.append(name)
+        shap_values = np.array(shap_values).transpose(1, 0)
+        pixel_values = np.array(pixel_values).transpose(1, 0)
+
+        shap.summary_plot(shap_values,
+                          pixel_values,
+                          feature_names=feature_names,
+                          show=False)
+
         plots.append(plt.gcf())
         plt.close()
     return plots
-    
 
-def integrated_grad(model, datasample):
 
+def integrated_grad(model, datasample):
     """Compute Integrated Gradients for a given data sample and model.
 
     Args:
         - model: The PyTorch model.
         - datasample: The input data sample.
 
     Returns:
         list: A list of integrated gradients for each feature.
     """
 
-    input_py = torch.from_numpy(np.expand_dims(datasample,axis=0))
+    input_py = torch.from_numpy(np.expand_dims(datasample, axis=0))
     ig = IntegratedGradients(model)
     len_targets = len(model(input_py).detach().numpy()[0])
     grads = []
     for i in range(len_targets):
-         attributions = ig.attribute(input_py, target=i)
-         grads.append(attributions[0][0])
+        attributions = ig.attribute(input_py, target=i)
+        grads.append(attributions[0][0])
     return grads
 
-def deeplift(model, datasample):
 
+def deeplift(model, datasample):
     """Compute DeepLift attributions for a given data sample and model.
 
     Args:
         - model: The PyTorch model.
         - datasample: The input data sample.
 
     Returns:
         list: A list of DeepLift attributions for each feature.
     """
 
-    input_py = torch.from_numpy(np.expand_dims(datasample,axis=0))
+    input_py = torch.from_numpy(np.expand_dims(datasample, axis=0))
     input_py.requires_grad = True
     ig = DeepLift(model.eval())
     len_targets = len(model(input_py).detach().numpy()[0])
     dl_arrays = []
     for i in range(len_targets):
         attributions = ig.attribute(input_py, target=i).detach().numpy()
         dl_arrays.append(attributions[0][0])
     return dl_arrays
-
-    
-
```

### Comparing `xaivision-0.1.0/PKG-INFO` & `xaivision-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xaivision
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: philorfa
 Author-email: phil.orfa@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```


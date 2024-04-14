# Comparing `tmp/connectome_interpreter-1.1.0.tar.gz` & `tmp/connectome_interpreter-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectome_interpreter-1.1.0.tar", last modified: Sun Apr  7 22:16:08 2024, max compression
+gzip compressed data, was "connectome_interpreter-1.2.0.tar", last modified: Sun Apr 14 17:32:47 2024, max compression
```

## Comparing `connectome_interpreter-1.1.0.tar` & `connectome_interpreter-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 22:16:08.026905 connectome_interpreter-1.1.0/
--rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      913 2024-04-07 22:16:08.026905 connectome_interpreter-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      467 2024-03-04 09:40:07.000000 connectome_interpreter-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 22:16:07.991096 connectome_interpreter-1.1.0/connectome_interpreter/
--rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.1.0/connectome_interpreter/__init__.py
--rw-rw-rw-   0        0        0    15178 2024-04-02 10:49:52.000000 connectome_interpreter-1.1.0/connectome_interpreter/activation_maximisation.py
--rw-rw-rw-   0        0        0    18051 2024-03-20 19:23:39.000000 connectome_interpreter-1.1.0/connectome_interpreter/compress_paths.py
--rw-rw-rw-   0        0        0    13084 2024-04-07 22:13:37.000000 connectome_interpreter-1.1.0/connectome_interpreter/path_finding.py
--rw-rw-rw-   0        0        0    17919 2024-03-31 16:43:03.000000 connectome_interpreter-1.1.0/connectome_interpreter/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-07 22:16:08.023742 connectome_interpreter-1.1.0/connectome_interpreter.egg-info/
--rw-rw-rw-   0        0        0      913 2024-04-07 22:16:07.000000 connectome_interpreter-1.1.0/connectome_interpreter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2024-04-07 22:16:07.000000 connectome_interpreter-1.1.0/connectome_interpreter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 22:16:07.000000 connectome_interpreter-1.1.0/connectome_interpreter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2024-04-07 22:16:07.000000 connectome_interpreter-1.1.0/connectome_interpreter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-04-07 22:16:07.000000 connectome_interpreter-1.1.0/connectome_interpreter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 22:16:08.026905 connectome_interpreter-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1511 2024-04-07 22:12:25.000000 connectome_interpreter-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 22:16:08.024736 connectome_interpreter-1.1.0/tests/
--rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.1.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 17:32:47.105167 connectome_interpreter-1.2.0/
+-rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      938 2024-04-14 17:32:47.103873 connectome_interpreter-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 17:32:47.070086 connectome_interpreter-1.2.0/connectome_interpreter/
+-rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.2.0/connectome_interpreter/__init__.py
+-rw-rw-rw-   0        0        0    19210 2024-04-14 17:00:07.000000 connectome_interpreter-1.2.0/connectome_interpreter/activation_maximisation.py
+-rw-rw-rw-   0        0        0    18200 2024-04-10 13:11:37.000000 connectome_interpreter-1.2.0/connectome_interpreter/compress_paths.py
+-rw-rw-rw-   0        0        0    16261 2024-04-14 17:16:24.000000 connectome_interpreter-1.2.0/connectome_interpreter/path_finding.py
+-rw-rw-rw-   0        0        0    26846 2024-04-14 17:30:48.000000 connectome_interpreter-1.2.0/connectome_interpreter/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-14 17:32:47.101905 connectome_interpreter-1.2.0/connectome_interpreter.egg-info/
+-rw-rw-rw-   0        0        0      938 2024-04-14 17:32:46.000000 connectome_interpreter-1.2.0/connectome_interpreter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2024-04-14 17:32:47.000000 connectome_interpreter-1.2.0/connectome_interpreter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 17:32:46.000000 connectome_interpreter-1.2.0/connectome_interpreter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2024-04-14 17:32:46.000000 connectome_interpreter-1.2.0/connectome_interpreter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-04-14 17:32:46.000000 connectome_interpreter-1.2.0/connectome_interpreter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 17:32:47.105167 connectome_interpreter-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1532 2024-04-10 15:37:20.000000 connectome_interpreter-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 17:32:47.102951 connectome_interpreter-1.2.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.2.0/tests/__init__.py
```

### Comparing `connectome_interpreter-1.1.0/LICENSE` & `connectome_interpreter-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.1.0/PKG-INFO` & `connectome_interpreter-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectome_interpreter
-Version: 1.1.0
+Version: 1.2.0
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
 Keywords: connectomics,neural network,mechanistic interpretability
@@ -12,11 +12,12 @@
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: torch
 Requires-Dist: tqdm
 Requires-Dist: plotly
 Requires-Dist: matplotlib
+Requires-Dist: networkx
 Provides-Extra: get-ngl-link
 Requires-Dist: nglscenes; extra == "get-ngl-link"
 Provides-Extra: wandb
 Requires-Dist: wandb; extra == "wandb"
```

### Comparing `connectome_interpreter-1.1.0/connectome_interpreter/activation_maximisation.py` & `connectome_interpreter-1.2.0/connectome_interpreter/activation_maximisation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from typing import Callable, Dict, List, Tuple
 
 import torch
 import torch.nn as nn
 import numpy as np
+import pandas as pd
+from scipy.sparse import issparse
 
 from tqdm import tqdm
 
+from .compress_paths import result_summary
+from .utils import adjacency_df_to_el, get_activations
+
 
 class MultilayeredNetwork(nn.Module):
     """
     A PyTorch module representing a multilayered neural network model. 
     This network architecture is designed to process temporal sequences of sensory data 
     through multiple layers, with the initial layer handling sensory inputs and subsequent 
     layers processing sensory + non-sensory input.
@@ -246,15 +251,15 @@
             model.activations)
         # Apply custom regularisation
         in_regularisation_loss = in_regularisation_lambda * custom_in_regularisation(
             input_tensor)
         loss = activation_loss + in_regularisation_loss + out_regularisation_loss
         losses.append(loss.item())
 
-        if early_stopping and iteration > n_runs:
+        if early_stopping and (iteration > n_runs):
             # when the difference between the max and the min < stopping_threshold
             if np.max(losses[-n_runs:]) - np.min(losses[-n_runs:]) < stopping_threshold:
                 break
 
         if wandb:
             dct = {"activation_loss": activation_loss.item(
             ), "in_regularisation_loss": in_regularisation_loss.item(),
@@ -279,7 +284,78 @@
     input_tensor = torch.where(input_tensor >= model.threshold,
                                input_tensor, 0)  # Thresholded ReLU
     # Limit the range between 0 and 1
     input_tensor = torch.tanh(input_tensor)
     return (input_tensor.cpu().detach().numpy(),
             output_after.cpu().detach().numpy(),
             act_loss, out_reg_loss, in_reg_loss, input_snapshots)
+
+
+def activations_to_df(inprop, opt_in, out, sensory_indices, inidx_mapping=None, outidx_mapping=None, activation_threshold=0, connectivity_threshold=0):
+    """
+    Generates a dataframe representing the paths in a layered plot, filtering by activation and connectivity thresholds.
+
+    This function takes the direct connectivity matrix (inprop), optimal input, output data, indices for sensory neurons, and mapping between input and output indices to groups. It generates a dataframe that represents the paths through the network layers.
+
+    Args:
+        inprop (scipy.sparse matrix or numpy.ndarray): Matrix representing the synaptic strengths 
+            between neurons, can be dense or sparse. Presynaptic is in the rows, postsynaptic in the columns.
+        opt_in (numpy.ndarray): A 2D array representing optimal input to the network.
+        out (numpy.ndarray): A 2D array representing the output from the network. The second dimension represents timepoints.
+        sensory_indices (list of int): A list of indices corresponding to sensory neurons in `inprop`.
+        inidx_mapping (dict, optional): A dictionary mapping indices in `inprop` to new indices. If None, indices are not remapped.
+                                       Defaults to None.
+        outidx_mapping (dict, optional): A dictionary mapping indices in `out` to new indices. If None, `inidx_mapping` is used for
+                                         mapping. Defaults to None.
+        activation_threshold (float, optional): A threshold value for activation. Neurons with activations below this threshold are
+                                                not considered. Defaults to 0.
+        connectivity_threshold (float, optional): A threshold for filtering connections. Connections with weights below this threshold
+                                                  are ignored. Defaults to 0.
+
+    Returns:
+        pandas.DataFrame: A dataframe representing the paths in the network. Each row is a connection, with columns for 'pre' and
+                          'post' neuron indices, 'layer', and their respective activations ('pre_activation', 'post_activation').
+    """
+    non_sensory_indices = [i for i in range(
+        inprop.shape[0]) if i not in sensory_indices]
+
+    if outidx_mapping is None:
+        outidx_mapping = inidx_mapping
+
+    if issparse(inprop):
+        inprop = inprop.toarray()
+
+    sensory_act = get_activations(
+        opt_in, sensory_indices, inidx_mapping, threshold=activation_threshold)
+
+    non_sensory_act = get_activations(
+        out, non_sensory_indices, outidx_mapping, threshold=activation_threshold)
+
+    conn = result_summary(inprop, inidx=sensory_indices + non_sensory_indices,
+                          outidx=non_sensory_indices, inidx_map=inidx_mapping, outidx_map=outidx_mapping, display_output=False)
+
+    conn_el = adjacency_df_to_el(
+        conn, threshold=connectivity_threshold)
+
+    # make paths df
+    paths = []
+    for layer in range(out.shape[1]):
+        if layer == 0:
+            pre = sensory_act[layer]
+            post = non_sensory_act[layer]
+        else:
+            pre = sensory_act[layer]
+            pre.update(non_sensory_act[layer-1])
+            post = non_sensory_act[layer]
+
+        connections = conn_el[conn_el.pre.isin(
+            pre.keys()) & conn_el.post.isin(post.keys())]
+        # so that direct connectivity is layer 1
+        connections.loc[:, ['layer']] = layer+1
+        connections.loc[:, ['pre_activation']] = connections.pre.map(pre)
+        connections.loc[:, ['post_activation']] = connections.post.map(post)
+        if connections.shape[0] > 0:
+            paths.append(connections)
+        else:
+            print(f"No connections found in layer {layer+1}.")
+    paths = pd.concat(paths)
+    return paths
```

### Comparing `connectome_interpreter-1.1.0/connectome_interpreter/compress_paths.py` & `connectome_interpreter-1.2.0/connectome_interpreter/compress_paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,40 +205,42 @@
     sum_matrix = matrices[0].copy()
     for i in range(1, n):
         sum_matrix += matrices[i]
 
     return sum_matrix
 
 
-def result_summary(stepsn, inidx, outidx, inidx_map, outidx_map=None, display_output=True, sort_by_column=None):
+def result_summary(stepsn, inidx, outidx, inidx_map=None, outidx_map=None, display_output=True, sort_by_column=None):
     """
     Generates a summary of connections between different types of neurons, 
     represented by their input and output indexes. The function calculates 
     the total synaptic input from presynaptic neuron groups to an average neuron in each 
     postsynaptic neuron group.
 
     Args:
         stepsn (scipy.sparse matrix or numpy.ndarray): Matrix representing the synaptic strengths 
             between neurons, can be dense or sparse.
         inidx (numpy.ndarray): Array of indices representing the input (presynaptic) neurons, used to subset stepsn. nan values are removed.
         outidx (numpy.ndarray): Array of indices representing the output (postsynaptic) neurons.
-        inidx_map (dict): Mapping from indices to neuron groups for the input neurons.
+        inidx_map (dict, optional): Mapping from indices to neuron groups for the input neurons. Defaults to None, in which case neurons are not grouped. 
         outidx_map (dict, optional): Mapping from indices to neuron groups for the output neurons.
             Defaults to None, in which case it is set to be the same as inidx_map.
         display_output (bool, optional): Whether to display the output in a coloured dataframe. Defaults to True.
         sort_by_column (str or list, optional): the column name(s) to sort the result by. If none is provided, then sort by the first column. 
 
     Returns:
         pd.DataFrame: A dataframe representing the summed synaptic input from presynaptic neuron groups 
             to an average neuron in each postsynaptic neuron group. This dataframe is always returned, regardless of the
             value of display_output.
 
     Displays:
         If display_output is True, the function will display a styled version of the resulting dataframe.
     """
+    if inidx_map is None:
+        inidx_map = {idx: idx for idx in inidx}
     if outidx_map is None:
         outidx_map = inidx_map
 
     # remove nan values in inidx and outidx
     inidx = to_nparray(inidx)
     outidx = to_nparray(outidx)
```

### Comparing `connectome_interpreter-1.1.0/connectome_interpreter/path_finding.py` & `connectome_interpreter-1.2.0/connectome_interpreter/path_finding.py`

 * *Files 22% similar despite different names*

```diff
@@ -137,96 +137,144 @@
 
         # Update the outidx for the next iteration to move backwards through layers
         current_outidx = set(df['pre'])
 
     return pd.concat(dfs)
 
 
-def create_layered_positions(df):
+def create_layered_positions(df, priority_indices=None, sort_dict=None):
     """
     Creates a dictionary of positions for each neuron in the paths, so that the paths can be visualized in a layered manner. It assumes that `df` contains the columns 'layer', 'pre_layer', 'post_layer' (or 'layer', 'pre', 'post'). If a neuron exists in multiple layers, it is plotted multiple times.
     Args:
         df (pd.DataFrame): The DataFrame containing the path data, including the layer number, pre-synaptic index, and post-synaptic index.
+        priority_indices (list, set, pd.Series, numpy.ndarray optional): A list of neuron indices that should be plotted on top of each layer. Defaults to None.
+        sort_dict (dict, optional): A dictionary of neuron indices as keys and their sorting order as values. Defaults to None.
     Returns:
         dict: A dictionary of positions for each neuron in the paths, with the keys as the neuron indices and the values as the (x, y) coordinates.
     """
 
     # if post_layer and pre_layer are not present, create them
     if 'post_layer' not in df.columns:
         df['post_layer'] = df['post'].astype(
             str) + '_' + df['layer'].astype(str)
     if 'pre_layer' not in df.columns:
         df['pre_layer'] = df['pre'].astype(
             str) + '_' + (df.layer-1).astype(str)
 
+    if priority_indices is not None:
+        priority_indices = set(priority_indices)
+
     number_of_layers = df.layer.nunique()
     layer_width = 1.0 / (number_of_layers + 1)
     positions = {}
 
-    pre_neurons = df[df['layer'] == 1]['pre_layer'].unique()
-    vertical_spacing = 1.0 / (len(pre_neurons) + 1)
-    for index, neuron in enumerate(pre_neurons, start=1):
-        positions[neuron] = (0, index * vertical_spacing)
-
-    for layer in range(1, number_of_layers + 1):
-        posts_in_layer = df[df['layer'] == layer]['post_layer'].unique()
-        vertical_spacing = 1.0 / (len(posts_in_layer) + 1)
-        for index, post in enumerate(posts_in_layer, start=1):
-            positions[post] = (layer * layer_width, index * vertical_spacing)
+    all_names = set(df['pre_layer']) | set(df['post_layer'])
+    name_to_idx = dict(zip(df.pre_layer, df.pre))
+    name_to_idx.update(dict(zip(df.post_layer, df.post)))
+
+    for layer in range(0, number_of_layers + 1):
+        layer_name = [item for item in all_names if '_'+str(layer) in item]
+        if sort_dict is not None:
+            layer_name = sorted(layer_name, key=lambda x: sort_dict[x])
+
+        if priority_indices is not None:
+            layer_name_priority = [
+                item for item in layer_name if name_to_idx[item] in priority_indices]
+            layer_name_not = [
+                item for item in layer_name if name_to_idx[item] not in priority_indices]
+
+            layer_name = layer_name_not + layer_name_priority
+        for index, neuron in enumerate(layer_name, start=1):
+            positions[neuron] = (layer * layer_width,
+                                 index * 1.0 / (len(layer_name) + 1))
+
     return positions
 
 
-def remove_excess_neurons(df):
+def remove_excess_neurons(df, keep=None, target_indices=None, keep_targets_in_middle=False):
     """After filtering, some neurons are no longer on the paths between the input and output neurons. This function removes those neurons from the paths.
 
     Args:
         df (pd.Dataframe): a filtered dataframe with similar structure as the dataframe returned by `find_path_iteratively()`.
+        keep (list, set, pd.Series, numpy.ndarray, optional): A list of neuron indices that should be kept in the paths, even if they don't connect between input and target in the last layer. Defaults to None.
+        target_indices (list, set, pd.Series, numpy.ndarray, optional): A list of target neuron indices that should be kept in the last layer. Defaults to None, in which case all neurons in the last layer in `df` would be kept.
+        keep_targets_in_middle (bool, optional): If True, the target_indices are kept in the middle layers as well, even if they don't connect between input and target in the last layer. Defaults to False.
 
     Returns:
         pd.Dataframe: a dataframe with similar structure as the result of `find_path_iteratively()`, with the excess neurons removed.
     """
     if df.layer.max() == 1:
         return df
 
+    # if target_indices are provided, first use this to filter the last layer
+    if target_indices is not None:
+        target_indices = set(target_indices)
+        if not target_indices.issubset(df[df.layer == df.layer.max()].post):
+            raise ValueError('The target indices are not in the post-synaptic neurons of the last layer. Here are the indices of the last layer: ',
+                             df[df.layer == df.layer.max()].post, '. Your target_indices should be a subset.')
+
+        df = df[(df.layer != df.layer.max()) | df.post.isin(target_indices)]
+
     while any([set(df[df.layer == i].post) != set(df[df.layer == (i+1)].pre) for i in range(1, df.layer.max())]):
-        df_layers_update = []
+        if keep is not None:
+            keep = set(keep)
 
+            if all([set(df[df.layer == i].post).union(keep) == set(df[df.layer == (i+1)].pre).union(keep) for i in range(1, df.layer.max())]):
+                break
+        else:
+            keep = set()
+
+        if keep_targets_in_middle:
+            if target_indices is not None:
+                keep = keep.union(target_indices)
+
+        # start adding each layer to df_layers_update
+        df_layers_update = []
         if df.layer.max() == 2:
             df_layer = df[df.layer == 2]
             df_prev_layer = df[df.layer == 1]
 
             df_layers_update.append(
-                df_layer[df_layer.pre.isin(df_prev_layer.post)])
+                df_layer[df_layer.pre.isin(set(df_prev_layer.post).union(keep))])
             df_layers_update.append(
-                df_prev_layer[df_prev_layer.post.isin(df_layer.pre)])
+                df_prev_layer[df_prev_layer.post.isin(set(df_layer.pre).union(keep))])
             df = pd.concat(df_layers_update)
 
         else:
             for i in range(2, df.layer.max()):
                 df_layer = df[df.layer == i]
                 df_next_layer = df[df.layer == i+1]
                 df_prev_layer = df[df.layer == i-1]
 
                 df_pre = set.intersection(
                     set(df_prev_layer.post) & set(df_layer.pre))
                 df_post = set.intersection(
                     set(df_layer.post), set(df_next_layer.pre))
 
                 if i == 2:
+                    # add edges in the first layer
                     df_prev_layer = df_prev_layer[df_prev_layer.post.isin(
-                        df_pre)]
+                        df_pre.union(keep))]
                     df_layers_update.append(df_prev_layer)
 
                 df_layer = df_layer[df_layer.pre.isin(
-                    df_pre) & df_layer.post.isin(df_post)]
+                    df_pre.union(keep)) & df_layer.post.isin(df_post.union(keep))]
+                if df_layer.shape[0] == 0:
+                    raise ValueError(
+                        'No path found. Try lowering the threshold for the edges to be included in the path.')
                 df_layers_update.append(df_layer)
 
                 if i == (df.layer.max()-1):
-                    df_next_layer = df_next_layer[df_next_layer.pre.isin(
-                        df_post)]
+                    # add edges in the last layer
+                    if target_indices is None:
+                        df_next_layer = df_next_layer[df_next_layer.pre.isin(
+                            df_post.union(keep))]
+                    else:
+                        df_next_layer = df_next_layer[df_next_layer.pre.isin(
+                            df_post.union(keep).union(target_indices))]
                     df_layers_update.append(df_next_layer)
 
             df = pd.concat(df_layers_update)
     return df
 
 
 def filter_paths(df, threshold=0, necessary_intermediate=None):
```

### Comparing `connectome_interpreter-1.1.0/connectome_interpreter/utils.py` & `connectome_interpreter-1.2.0/connectome_interpreter/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import torch
 import pandas as pd
 import numpy as np
 from scipy.sparse import coo_matrix, csr_matrix, issparse
 import matplotlib.colors as mcl
 import matplotlib.pyplot as plt
 from tqdm import tqdm
+import networkx as nx
 
 
 def dynamic_representation(tensor, density_threshold=0.2):
     """Convert tensor to sparse if density is below threshold, otherwise to dense."""
     nonzero_elements = torch.nonzero(tensor).size(0)
     total_elements = tensor.numel()
     density = nonzero_elements / total_elements
@@ -78,62 +79,100 @@
 
 
 def coo_tensor_to_el(coo_tensor):
     """
     Convert a PyTorch sparse COO tensor to a DataFrame representing an edge list.
 
     This function checks if the input tensor is sparse. If not, it converts it to a sparse COO tensor.
-    It then extracts the indices and values, and creates a DataFrame with columns 'row_idx', 'col_idx', and 'value'.
-    Each row in the DataFrame represents an edge in the graph, where 'row_idx' and 'col_idx' are the nodes connected by the edge,
-    and 'value' is the weight of the edge.
+    It then extracts the indices and values, and creates a DataFrame with columns 'pre', 'post', and 'weight'.
+    Each row in the DataFrame represents an edge in the graph, where 'pre' and 'post' are the nodes connected by the edge,
+    and 'weight' is the weight of the edge.
 
     Args:
       coo_tensor (torch.Tensor): A PyTorch tensor, either already in sparse COO format or dense.
 
     Returns:
-      pd.DataFrame: A DataFrame with columns 'row_idx', 'col_idx', and 'value', representing the edge list of the graph.
+      pd.DataFrame: A DataFrame with columns 'pre', 'post', and 'weight', representing the edge list of the graph.
     """
 
     if not coo_tensor.is_sparse:
         coo_tensor = coo_tensor.to_sparse_coo()
 
     # Transpose and convert to numpy array
     indices = coo_tensor.indices().t().cpu().numpy()
     values = coo_tensor.values().cpu().numpy()
 
     # Split the indices to row and column
-    row_idx, col_idx = indices[:, 0], indices[:, 1]
+    pre, post = indices[:, 0], indices[:, 1]
 
     edge_list_df = pd.DataFrame(
-        {'row_idx': row_idx, 'col_idx': col_idx, 'value': values})
+        {'pre': pre, 'post': post, 'weight': values})
     return edge_list_df
 
 
-def coo_to_el(coo):
+def coo_to_el(coo, row_indices=None, col_indices=None):
     """
-    Convert a SciPy sparse COO matrix to a DataFrame representing an edge list.
-
-    Extracts the row indices, column indices, and data from a COO matrix to create a DataFrame.
-    Each row in the DataFrame represents an edge in the graph, where 'row_idx' and 'col_idx' are the nodes connected by the edge,
+    Extracts an edgelist from a COO matrix, optionally using pre-specified row and/or column indices.
+    If row_indices or col_indices are None, all rows or columns are considered, respectively.
+    Each row in the resulting DataFrame represents an edge in the graph, where 'pre' and 'post' are the nodes connected by the edge,
     and 'value' is the weight of the edge.
 
     Args:
-      coo (scipy.sparse.coo_matrix): A COO matrix from SciPy representing a sparse matrix.
+      coo: A scipy.sparse.coo_matrix instance.
+      row_indices: Optional; A list or array of row indices of interest.
+      col_indices: Optional; A list or array of column indices of interest.
 
     Returns:
-      pd.DataFrame: A DataFrame with columns 'row_idx', 'col_idx', and 'value', representing the edge list of the graph.
+      pd.DataFrame: A DataFrame with columns 'pre', 'post', and 'value', representing the edge list of the graph.
     """
-    row = coo.row
-    col = coo.col
-    data = coo.data
-    all_el = pd.DataFrame({'row_idx': row, 'col_idx': col, 'value': data})
+    # Determine whether to filter on rows/columns based on provided indices
+    row_mask = np.full(coo.shape[0], True) if row_indices is None else np.isin(
+        coo.row, row_indices)
+    col_mask = np.full(coo.shape[1], True) if col_indices is None else np.isin(
+        coo.col, col_indices)
+
+    # Combine row and column masks
+    mask = row_mask & col_mask
+
+    # Filter rows, cols, and data based on the combined mask
+    rows = coo.row[mask]
+    cols = coo.col[mask]
+    data = coo.data[mask]
+
+    all_el = pd.DataFrame({'pre': rows, 'post': cols, 'value': data})
 
     return all_el
 
 
+def adjacency_df_to_el(adjacency, threshold=None):
+    """
+    Convert a DataFrame representing an adjacency matrix to an edge list.
+
+    This function takes a DataFrame where the index and columns represent nodes in the graph,
+    and the values represent the weights of the edges between them. It converts this DataFrame to an edge list,
+    where each row represents an edge in the graph, with columns 'pre', 'post', and 'weight'.
+
+    Args:
+      adjacency (pd.DataFrame): A DataFrame representing an adjacency matrix.
+      threshold (float, optional): If provided, edges with values below this threshold are removed. Default to None.
+
+    Returns:
+      pd.DataFrame: A DataFrame with columns 'pre', 'post', and 'weight', representing the edge list of the graph.
+    """
+    if threshold is not None:
+        adjacency = adjacency.where(adjacency >= threshold, 0)
+
+    # Stack the DataFrame to create a long format
+    adjacency = adjacency.stack().reset_index()
+    adjacency.columns = ['pre', 'post', 'weight']
+    adjacency = adjacency[adjacency['weight'] != 0]
+
+    return adjacency
+
+
 def modify_coo_matrix(sparse_matrix, input_idx=None, output_idx=None, value=None, updates_df=None, re_normalize=True):
     """
     Modify the values of a sparse matrix (either COO or CSR format) at specified indices.
 
     There are two modes of operation:
     1. Single update mode: where `input_idx`, `output_idx`, and `value` are provided as individual arguments. In this case all combinations of input_idx and output_idx are updated.
     2. Batch update mode: where `updates_df` is provided, a DataFrame with columns ['input_idx', 'output_idx', 'value'].
@@ -327,28 +366,27 @@
             layer['segmentColors'][str(df_group.columns[0])] = '#43A7FF'
 
         scene.add_layers(layer)
 
     return scene.url
 
 
-def top_n_activated(array, global_indices, idx_map, n=None, threshold=None):
+def get_activations(array, global_indices, idx_map=None, top_n=None, threshold=None):
     """
     Identifies the top activated neurons for each column in the array,
     either by number (top n) or by a minimum activation threshold, or both.
 
     Args:
         array (np.ndarray): 2D array of neuron activations, where rows represent neurons
             and columns represent different time steps.
         global_indices (int, list, set, np.ndarray, pd.Series): Array of global neuron indices corresponding to the rows of the array.
-        idx_map (dict): Mapping from neuron index (`global_indices`) to neuron identifier.
-        n (int, optional): Number of top activations to return for each column. If None,
+        idx_map (dict, optional): Mapping from neuron index (`global_indices`) to neuron identifier. If not None, and if multiple neurons map to the same identifier, the activations are averaged. Defaults to None.
+        top_n (int, optional): Number of top activations to return for each column. If None,
             all activations above the threshold are returned. Defaults to None.
-        threshold (float, optional): Minimum activation level to consider. If None,
-            the top n activations are returned regardless of their magnitude. Defaults to None.
+        threshold (float, dict, optional): Minimum activation level to consider. If a dictionary is provided, the threshold for each column is specified by the column index. Defaults to None.
 
     Returns:
         dict: A dictionary where each key is a column index and each value is a nested dictionary
             of neuron identifiers and their activations, for those activations that are either
             in the top n, above the threshold, or both.
 
     Note:
@@ -369,28 +407,158 @@
         # Determine which indices to use based on the 'sensory' flag
         # these are global indices in the all-to-all connectivity
 
         column_values = array[:, col]
 
         # Filter activations by threshold if provided
         if threshold is not None:
-            # these are local indices
-            filtered_indices = np.where(column_values >= threshold)[0]
-            # these are global indices
-            threshold_indices = indices[filtered_indices]
+            if isinstance(threshold, dict):
+                if col not in threshold:
+                    thresh = 0
+                else:
+                    thresh = threshold[col]
+            else:
+                thresh = threshold
+
+            if thresh > 0:
+                # these are local indices
+                filtered_indices = np.where(column_values >= thresh)[0]
+                # these are global indices
+                threshold_indices = indices[filtered_indices]
+            else:
+                threshold_indices = indices
         else:
             threshold_indices = indices
 
         # Sort the filtered activations
         # these are the local indices corresponding to only sensory/non-sensory neurons, but not both
         sorted_indices = np.argsort(
-            column_values)[-n:] if n is not None else np.argsort(column_values)
+            column_values)[-top_n:] if top_n is not None else np.argsort(column_values)
         # these are global indices
         topn_indices = indices[sorted_indices]
 
         selected = np.intersect1d(threshold_indices, topn_indices)
 
         # Build the result dictionary
-        result[col] = {idx_map[idx]: column_values[global_to_local_map[idx]]
-                       for idx in selected}
+        if idx_map is None:
+            result[col] = {idx: column_values[global_to_local_map[idx]]
+                           for idx in selected}
+        else:
+            # initialise a zero dict
+            result[col] = {idx_map[idx]: [] for idx in selected}
+            # calculate the average
+            for idx in selected:
+                result[col][idx_map[idx]].append(
+                    column_values[global_to_local_map[idx]])
+            new_indices = result[col].keys()
+            result[col] = {idx: np.mean(result[col][idx])
+                           for idx in new_indices}
 
     return result
+
+
+def plot_layered_paths(path_df, figsize=(10, 8), priority_indices=None, sort_by_activation=False, fraction=0.03, pad=0.02):
+    """
+    Plots a directed graph of layered paths with optional node coloring based on activation values.
+
+    This function creates a visualization of a directed graph with nodes placed in layers. Nodes can be optionally
+    colored based on 'pre_activation' and 'post_activation' columns present in the dataframe. If these columns are
+    missing, a default color is used for all nodes. The edges are weighted, and their labels represent the weight values.
+
+    Args:
+        path_df (pandas.DataFrame): A dataframe containing the columns 'pre', 'post', 'layer', 'weight', and optionally 
+                                    'pre_activation', 'post_activation', 'pre_layer', 'post_layer'. Each row represents an
+                                    edge in the graph. The 'pre' and 'post' columns refer to the source and target nodes, respectively.
+                                    The 'layer' column is used to place nodes in layers, and 'weight' indicates the edge weight.
+                                    If present, 'pre_activation' and 'post_activation' are used to color the nodes based on
+                                    their activation values.
+        figsize (tuple, optional): A tuple indicating the size of the matplotlib figure. Defaults to (10, 8).
+        priority_indices (list, optional): A list of indices to prioritize when creating the layered positions. Nodes with these
+                                    indices will be placed at the top of their respective layers. Defaults to None. 
+        sort_by_activation (bool, optional): A flag to sort the nodes based on their activation values (after grouping by priority). Defaults to False.
+        fraction (float, optional): The fraction of the figure width to use for the colorbar. Defaults to 0.03.
+        pad (float, optional): The padding between the colorbar and the plot. Defaults to 0.02.
+
+    Returns:
+        None: This function does not return a value. It generates a plot using matplotlib.
+
+    Note:
+        If 'pre_layer' and 'post_layer' columns are not in the dataframe, they will be created within the function
+        to uniquely identify the nodes based on their 'pre'/'post' values and 'layer'.
+        The function automatically checks for the presence of 'pre_activation' and 'post_activation' columns to
+        determine whether to color the nodes based on activation values.
+        The positions of the nodes are determined by a custom positioning function (`connectome_interpreter.path_finding.create_layered_positions`).
+        This function requires the networkx library for graph operations and matplotlib for plotting.
+    """
+    if path_df.shape[0] == 0:
+        raise ValueError("The provided DataFrame is empty.")
+
+    # Create a 'post_layer' column to use as unique identifiers
+    if 'post_layer' not in path_df.columns:
+        path_df['post_layer'] = path_df['post'].astype(
+            str) + '_' + path_df['layer'].astype(str)
+    if 'pre_layer' not in path_df.columns:
+        path_df['pre_layer'] = path_df['pre'].astype(
+            str) + '_' + (path_df.layer-1).astype(str)
+
+    # Create the graph using the new 'post_layer' identifiers
+    G = nx.from_pandas_edgelist(path_df, 'pre_layer', 'post_layer', [
+                                'weight'], create_using=nx.DiGraph())
+
+    # Labels for nodes
+    labels = dict(zip(path_df.post_layer, path_df.post))
+    labels.update(dict(zip(path_df.pre_layer, path_df.pre)))
+
+    # Determine the width of the edges
+    weights = [G[u][v]['weight'] for u, v in G.edges()]
+    widths = [max(0.1, w * 5) for w in weights]  # Scale weights for visibility
+
+    # Generate positions
+    if sort_by_activation:
+        node_activation_dict = dict(
+            zip(path_df.post_layer, path_df.post_activation))
+        node_activation_dict.update(
+            dict(zip(path_df.pre_layer, path_df.pre_activation)))
+        positions = create_layered_positions(
+            path_df, priority_indices, sort_dict=node_activation_dict)
+    else:
+        positions = create_layered_positions(path_df, priority_indices)
+
+    # Node colors based on activation values
+    if ('pre_activation' in path_df.columns) & ('post_activation' in path_df.columns):
+        activations = np.concatenate(
+            [path_df['pre_activation'].values, path_df['post_activation'].values])
+        norm = plt.Normalize(vmin=activations.min(), vmax=activations.max())
+        color_map = plt.get_cmap('viridis')
+        # Update graph with activation data
+        nx.set_node_attributes(
+            G, dict(zip(path_df.pre_layer, path_df.pre_activation)), 'activation')
+        nx.set_node_attributes(
+            G, dict(zip(path_df.post_layer, path_df.post_activation)), 'activation')
+
+        node_colors = [color_map(norm(G.nodes[node]['activation']))
+                       for node in G.nodes()]
+
+    # Plot the graph
+    fig, ax = plt.subplots(figsize=figsize)
+    if ('pre_activation' in path_df.columns) & ('post_activation' in path_df.columns):
+        nx.draw(G, pos=positions,
+                labels=labels,
+                with_labels=True, node_size=100,
+                node_color=node_colors,
+                arrows=True, arrowstyle='-|>', arrowsize=10,
+                font_size=8, width=widths, edge_color='lightgrey', ax=ax)
+        plt.colorbar(plt.cm.ScalarMappable(
+            norm=norm, cmap=color_map), ax=ax, label='Activation', fraction=fraction, pad=pad)
+    else:
+        nx.draw(G, pos=positions,
+                labels=labels,
+                with_labels=True, node_size=100,
+                node_color='lightblue', arrows=True, arrowstyle='-|>', arrowsize=10, font_size=8, width=widths, ax=ax)
+
+    edge_labels = {(u, v): f'{data["weight"]:.2f}' for u,
+                   v, data in G.edges(data=True)}
+    nx.draw_networkx_edge_labels(G, pos=positions, edge_labels=edge_labels,
+                                 #  font_color='red'
+                                 ax=ax)
+    ax.set_ylim(0, 1)
+    plt.show()
```

### Comparing `connectome_interpreter-1.1.0/connectome_interpreter.egg-info/PKG-INFO` & `connectome_interpreter-1.2.0/connectome_interpreter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectome-interpreter
-Version: 1.1.0
+Version: 1.2.0
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
 Keywords: connectomics,neural network,mechanistic interpretability
@@ -12,11 +12,12 @@
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: torch
 Requires-Dist: tqdm
 Requires-Dist: plotly
 Requires-Dist: matplotlib
+Requires-Dist: networkx
 Provides-Extra: get-ngl-link
 Requires-Dist: nglscenes; extra == "get-ngl-link"
 Provides-Extra: wandb
 Requires-Dist: wandb; extra == "wandb"
```

### Comparing `connectome_interpreter-1.1.0/setup.py` & `connectome_interpreter-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='connectome_interpreter',
     # If you're making a patch or a minor bug fix, increment the patch version, e.g., from 0.1.0 to 0.1.1.
     # If you're adding functionality in a backwards-compatible manner, increment the minor version, e.g., from 0.1.0 to 0.2.0.
     # If you're making incompatible API changes, increment the major version, e.g., from 0.1.0 to 1.0.0.
-    version='1.1.0',
+    version='1.2.0',
     packages=find_packages(),
     install_requires=[
         # List your package dependencies here
         'numpy',
         'pandas',
         'scipy',
         'torch',
         'tqdm',
         'plotly',
         'matplotlib',
+        'networkx',
     ],
     extras_require={
         'get_ngl_link': ['nglscenes'],
         'wandb': ['wandb'],
     },
     # Optional metadata
     author='Yijie Yin',
```


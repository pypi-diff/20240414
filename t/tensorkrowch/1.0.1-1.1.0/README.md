# Comparing `tmp/tensorkrowch-1.0.1.tar.gz` & `tmp/tensorkrowch-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorkrowch-1.0.1.tar", last modified: Wed Mar  6 17:55:17 2024, max compression
+gzip compressed data, was "tensorkrowch-1.1.0.tar", last modified: Sun Apr 14 00:29:11 2024, max compression
```

## Comparing `tensorkrowch-1.0.1.tar` & `tensorkrowch-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-03-06 17:55:17.254500 tensorkrowch-1.0.1/
--rw-rw-r--   0 jose      (1000) jose      (1000)     1086 2023-05-25 11:43:07.000000 tensorkrowch-1.0.1/LICENSE.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)       11 2024-03-06 14:43:09.000000 tensorkrowch-1.0.1/MANIFEST.in
--rw-r--r--   0 jose      (1000) jose      (1000)     8862 2024-03-06 17:55:17.254500 tensorkrowch-1.0.1/PKG-INFO
--rw-rw-r--   0 jose      (1000) jose      (1000)     6454 2024-03-06 11:04:32.000000 tensorkrowch-1.0.1/README.md
--rw-rw-r--   0 jose      (1000) jose      (1000)     1293 2024-03-06 16:39:40.000000 tensorkrowch-1.0.1/pyproject.toml
--rw-rw-r--   0 jose      (1000) jose      (1000)       38 2024-03-06 17:55:17.254500 tensorkrowch-1.0.1/setup.cfg
--rw-rw-r--   0 jose      (1000) jose      (1000)       38 2024-03-06 14:57:42.000000 tensorkrowch-1.0.1/setup.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-03-06 17:55:17.254500 tensorkrowch-1.0.1/tensorkrowch/
--rw-rw-r--   0 jose      (1000) jose      (1000)     1232 2024-03-06 16:19:38.000000 tensorkrowch-1.0.1/tensorkrowch/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)   190692 2024-03-06 17:04:03.000000 tensorkrowch-1.0.1/tensorkrowch/components.py
--rw-rw-r--   0 jose      (1000) jose      (1000)     5867 2024-01-02 17:16:03.000000 tensorkrowch-1.0.1/tensorkrowch/embeddings.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    11806 2024-01-02 17:16:03.000000 tensorkrowch-1.0.1/tensorkrowch/initializers.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-03-06 17:55:17.254500 tensorkrowch-1.0.1/tensorkrowch/models/
--rw-rw-r--   0 jose      (1000) jose      (1000)      341 2024-01-02 17:16:03.000000 tensorkrowch-1.0.1/tensorkrowch/models/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    50646 2024-03-05 17:32:24.000000 tensorkrowch-1.0.1/tensorkrowch/models/mps.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    72376 2024-03-05 17:48:47.000000 tensorkrowch-1.0.1/tensorkrowch/models/mps_layer.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    58350 2024-03-05 17:34:01.000000 tensorkrowch-1.0.1/tensorkrowch/models/peps.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    37360 2024-01-02 17:16:03.000000 tensorkrowch-1.0.1/tensorkrowch/models/tree.py
--rw-rw-r--   0 jose      (1000) jose      (1000)   131842 2024-03-06 17:54:16.000000 tensorkrowch-1.0.1/tensorkrowch/operations.py
--rw-rw-r--   0 jose      (1000) jose      (1000)     7240 2024-02-29 16:09:10.000000 tensorkrowch-1.0.1/tensorkrowch/utils.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-03-06 17:55:17.254500 tensorkrowch-1.0.1/tensorkrowch.egg-info/
--rw-r--r--   0 jose      (1000) jose      (1000)     8862 2024-03-06 17:55:17.000000 tensorkrowch-1.0.1/tensorkrowch.egg-info/PKG-INFO
--rw-rw-r--   0 jose      (1000) jose      (1000)      541 2024-03-06 17:55:17.000000 tensorkrowch-1.0.1/tensorkrowch.egg-info/SOURCES.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)        1 2024-03-06 17:55:17.000000 tensorkrowch-1.0.1/tensorkrowch.egg-info/dependency_links.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)      270 2024-03-06 17:55:17.000000 tensorkrowch-1.0.1/tensorkrowch.egg-info/requires.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)       13 2024-03-06 17:55:17.000000 tensorkrowch-1.0.1/tensorkrowch.egg-info/top_level.txt
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-04-14 00:29:11.506365 tensorkrowch-1.1.0/
+-rw-rw-r--   0 jose      (1000) jose      (1000)     1086 2023-05-25 11:43:07.000000 tensorkrowch-1.1.0/LICENSE.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)       11 2024-03-06 17:59:45.000000 tensorkrowch-1.1.0/MANIFEST.in
+-rw-r--r--   0 jose      (1000) jose      (1000)     8770 2024-04-14 00:29:11.506365 tensorkrowch-1.1.0/PKG-INFO
+-rw-rw-r--   0 jose      (1000) jose      (1000)     6358 2024-04-14 00:27:40.000000 tensorkrowch-1.1.0/README.md
+-rw-rw-r--   0 jose      (1000) jose      (1000)     1349 2024-04-14 00:06:08.000000 tensorkrowch-1.1.0/pyproject.toml
+-rw-rw-r--   0 jose      (1000) jose      (1000)       38 2024-04-14 00:29:11.506365 tensorkrowch-1.1.0/setup.cfg
+-rw-rw-r--   0 jose      (1000) jose      (1000)       38 2024-03-06 17:59:45.000000 tensorkrowch-1.1.0/setup.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-04-14 00:29:11.502365 tensorkrowch-1.1.0/tensorkrowch/
+-rw-rw-r--   0 jose      (1000) jose      (1000)     1325 2024-04-14 00:27:40.000000 tensorkrowch-1.1.0/tensorkrowch/__init__.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)   197961 2024-04-14 00:06:08.000000 tensorkrowch-1.1.0/tensorkrowch/components.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-04-14 00:29:11.502365 tensorkrowch-1.1.0/tensorkrowch/decompositions/
+-rw-rw-r--   0 jose      (1000) jose      (1000)       81 2024-04-14 00:28:38.000000 tensorkrowch-1.1.0/tensorkrowch/decompositions/__init__.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)     8830 2024-04-14 00:06:08.000000 tensorkrowch-1.1.0/tensorkrowch/decompositions/svd_decompositions.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    12476 2024-04-14 00:06:08.000000 tensorkrowch-1.1.0/tensorkrowch/embeddings.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    11806 2024-03-06 17:59:45.000000 tensorkrowch-1.1.0/tensorkrowch/initializers.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-04-14 00:29:11.502365 tensorkrowch-1.1.0/tensorkrowch/models/
+-rw-rw-r--   0 jose      (1000) jose      (1000)      384 2024-04-14 00:06:08.000000 tensorkrowch-1.1.0/tensorkrowch/models/__init__.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    40695 2024-04-14 00:06:08.000000 tensorkrowch-1.1.0/tensorkrowch/models/mpo.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)   154694 2024-04-14 00:06:08.000000 tensorkrowch-1.1.0/tensorkrowch/models/mps.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    21219 2024-04-14 00:06:08.000000 tensorkrowch-1.1.0/tensorkrowch/models/mps_data.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    58350 2024-03-06 17:59:45.000000 tensorkrowch-1.1.0/tensorkrowch/models/peps.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    37360 2024-03-06 17:59:45.000000 tensorkrowch-1.1.0/tensorkrowch/models/tree.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)   160118 2024-04-14 00:06:08.000000 tensorkrowch-1.1.0/tensorkrowch/operations.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)     9156 2024-04-14 00:06:08.000000 tensorkrowch-1.1.0/tensorkrowch/utils.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-04-14 00:29:11.506365 tensorkrowch-1.1.0/tensorkrowch.egg-info/
+-rw-r--r--   0 jose      (1000) jose      (1000)     8770 2024-04-14 00:29:11.000000 tensorkrowch-1.1.0/tensorkrowch.egg-info/PKG-INFO
+-rw-rw-r--   0 jose      (1000) jose      (1000)      657 2024-04-14 00:29:11.000000 tensorkrowch-1.1.0/tensorkrowch.egg-info/SOURCES.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)        1 2024-04-14 00:29:11.000000 tensorkrowch-1.1.0/tensorkrowch.egg-info/dependency_links.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)      270 2024-04-14 00:29:11.000000 tensorkrowch-1.1.0/tensorkrowch.egg-info/requires.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)       13 2024-04-14 00:29:11.000000 tensorkrowch-1.1.0/tensorkrowch.egg-info/top_level.txt
```

### Comparing `tensorkrowch-1.0.1/LICENSE.txt` & `tensorkrowch-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.0.1/PKG-INFO` & `tensorkrowch-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorkrowch
-Version: 1.0.1
+Version: 1.1.0
 Summary: Tensor Networks with PyTorch
 Author-email: José Ramón Pareja Monturiol <joserapa98@gmail.com>
 Maintainer-email: José Ramón Pareja Monturiol <joserapa98@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 José Ramón Pareja Monturiol
         
@@ -24,15 +24,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: GitHub, https://github.com/joserapa98/tensorkrowch
 Project-URL: Documentation, https://joserapa98.github.io/tensorkrowch
-Keywords: tensor,network,tensor network,tensor networks,mps,peps,quantum
+Keywords: tensor,network,tensor network,tensor networks,mps,mpo,peps,quantum
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: torch>=1.9
 Requires-Dist: opt_einsum>=3.0
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
@@ -47,16 +47,14 @@
 Requires-Dist: sphinxcontrib-serializinghtml==1.1.5; extra == "docs"
 
 ![logo](https://github.com/joserapa98/tensorkrowch/blob/master/docs/figures/svg/tensorkrowch_logo_dark.svg#gh-dark-mode-only)
 ![logo](https://github.com/joserapa98/tensorkrowch/blob/master/docs/figures/svg/tensorkrowch_logo_light.svg#gh-light-mode-only)
 
 [![DOI](https://zenodo.org/badge/453954432.svg)](https://zenodo.org/badge/latestdoi/453954432)
 
-[![DOI](https://zenodo.org/badge/453954432.svg)](https://zenodo.org/badge/latestdoi/453954432)
-
 # Tensor Networks with PyTorch
 
 **TensorKrowch** is a Python library built on top of **PyTorch** that simplifies
 the training of Tensor Networks as machine learning models and their integration
 into deep learning pipelines.
 
 The primary goal of **TensorKrowch** is to offer an efficient and user-friendly
@@ -168,15 +166,15 @@
 In **TensorKrowch** ``TensorNetworks`` work like **PyTorch** layers. Thus
 creating hybrid neural-tensor network models is straightforward:
 
 ```python
 import torch.nn as nn
 
 my_model = nn.Sequential(
-    tk.models.MPSLayer(n_features=100,
+    tk.models.MPSLayer(n_features=101,
                        in_dim=3,
                        out_dim=10,
                        bond_dim=5),
     nn.ReLU(),
     nn.Linear(10, 10))
 
 data = torch.randn(500, 100, 3)  # batch x n_features x in_dim
```

### Comparing `tensorkrowch-1.0.1/README.md` & `tensorkrowch-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 ![logo](https://github.com/joserapa98/tensorkrowch/blob/master/docs/figures/svg/tensorkrowch_logo_dark.svg#gh-dark-mode-only)
 ![logo](https://github.com/joserapa98/tensorkrowch/blob/master/docs/figures/svg/tensorkrowch_logo_light.svg#gh-light-mode-only)
 
 [![DOI](https://zenodo.org/badge/453954432.svg)](https://zenodo.org/badge/latestdoi/453954432)
 
-[![DOI](https://zenodo.org/badge/453954432.svg)](https://zenodo.org/badge/latestdoi/453954432)
-
 # Tensor Networks with PyTorch
 
 **TensorKrowch** is a Python library built on top of **PyTorch** that simplifies
 the training of Tensor Networks as machine learning models and their integration
 into deep learning pipelines.
 
 The primary goal of **TensorKrowch** is to offer an efficient and user-friendly
@@ -120,15 +118,15 @@
 In **TensorKrowch** ``TensorNetworks`` work like **PyTorch** layers. Thus
 creating hybrid neural-tensor network models is straightforward:
 
 ```python
 import torch.nn as nn
 
 my_model = nn.Sequential(
-    tk.models.MPSLayer(n_features=100,
+    tk.models.MPSLayer(n_features=101,
                        in_dim=3,
                        out_dim=10,
                        bond_dim=5),
     nn.ReLU(),
     nn.Linear(10, 10))
 
 data = torch.randn(500, 100, 3)  # batch x n_features x in_dim
```

### Comparing `tensorkrowch-1.0.1/pyproject.toml` & `tensorkrowch-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 license = {file = "LICENSE.txt"}
 keywords = [
     "tensor",
     "network",
     "tensor network",
     "tensor networks",
     "mps",
+    "mpo",
     "peps",
     "quantum"
 ]
 requires-python = ">=3.8"
 dependencies = [
   "torch>=1.9",
   "opt_einsum>=3.0",
@@ -45,13 +46,17 @@
 
 [tool.setuptools.dynamic]
 version = {attr = "tensorkrowch.__version__"}
 readme = {file = "README.md", content-type = "text/markdown"}
 
 
 [tool.setuptools]
-packages = ["tensorkrowch", "tensorkrowch.models"]
+packages = [
+    "tensorkrowch",
+    "tensorkrowch.models",
+    "tensorkrowch.decompositions"
+]
 
 
 [project.urls]
 GitHub = "https://github.com/joserapa98/tensorkrowch"
 Documentation = "https://joserapa98.github.io/tensorkrowch"
```

### Comparing `tensorkrowch-1.0.1/tensorkrowch/__init__.py` & `tensorkrowch-1.1.0/tensorkrowch/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,38 +2,41 @@
 TensorKrowch
 ============
 
 Tensor Networks with PyTorch
 """
 
 # Version
-__version__ = '1.0.1'
+__version__ = '1.1.0'
 
 # Network components
 from tensorkrowch.components import Axis
 from tensorkrowch.components import AbstractNode, Node, ParamNode
 from tensorkrowch.components import StackNode, ParamStackNode
 from tensorkrowch.components import Edge, StackEdge
 from tensorkrowch.components import Successor, TensorNetwork
 
 # Initializers
 from tensorkrowch.initializers import empty, zeros, ones, copy, rand, randn
 
 # Embeddings
 import tensorkrowch.embeddings as embeddings
 
+# Decompositions
+import tensorkrowch.decompositions as decompositions
+
 # Edge operations
 from tensorkrowch.components import connect, connect_stack, disconnect
-from tensorkrowch.operations import svd_, svdr_, qr_, rq_
-from tensorkrowch.operations import contract_
+from tensorkrowch.operations import (svd, svd_, svdr, svdr_, qr, qr_, rq, rq_,
+                                     contract, contract_)
 
 # Node operations
 from tensorkrowch.operations import Operation
 from tensorkrowch.operations import get_shared_edges  # Not in docs
 
 from tensorkrowch.operations import permute, permute_, tprod, mul, add, sub
-from tensorkrowch.operations import (split, split_, contract_edges, contract_,
+from tensorkrowch.operations import (split, split_, contract_edges,
                                      contract_between, contract_between_,
                                      stack, unbind, einsum, stacked_einsum)
 
 # Models
 import tensorkrowch.models as models
```

### Comparing `tensorkrowch-1.0.1/tensorkrowch/components.py` & `tensorkrowch-1.1.0/tensorkrowch/components.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from tensorkrowch.utils import (check_name_style, enum_repeated_names, erase_enum,
                                 print_list, stack_unequal_tensors, tab_string)
 
 
 ###############################################################################
 #                                     AXIS                                    #
 ###############################################################################
-class Axis:
+class Axis:  # MARK: Axis
     """
     Axes are the objects that stick edges to nodes. Each instance of the
     :class:`AbstractNode` class has a list of :math:`N` axes, each corresponding
     to one edge. Each axis stores information that facilitates accessing that
     edge, such as its :attr:`name` and :attr:`num` (index). Additionally, an axis
     keeps track of its :meth:`batch <is_batch>` and :meth:`node1 <is_node1>`
     attributes.
@@ -282,15 +282,15 @@
 ###############################################################################
 #                                    NODES                                    #
 ###############################################################################
 Ax = Union[int, Text, Axis]
 Shape = Union[Sequence[int], Size]
 
 
-class AbstractNode(ABC):
+class AbstractNode(ABC):  # MARK: AbstractNode
     """
     Abstract class for all types of nodes. Defines what a node is and most of its
     properties and methods. Since it is an abstract class, cannot be instantiated.
       
     Nodes are the elements that make up a :class:`TensorNetwork`. At its most
     basic level, a node is a container for a ``torch.Tensor`` that stores other
     relevant information which enables to build any network and operate nodes
@@ -380,26 +380,30 @@
     * **"stack_data_memory"**: Name of the ``virtual`` :class:`StackNode` that
       is created in :meth:`~TensorNetwork.set_data_nodes` to store the whole
       data tensor from which each ``data`` node might take just one `slice`.
       There should be at most one ``"stack_data_memory"`` in the network.
       To learn more about this, see :meth:`~TensorNetwork.set_data_nodes` and
       :meth:`~TensorNetwork.add_data`.
     
-    * **"virtual_stack"**: Name of the ``virtual`` :class:`ParamStackNode` that
+    * **"virtual_result"**: Name of ``virtual`` nodes that are not explicitly
+      part of the network, but are required for some situations during
+      contraction. For instance, the :class:`ParamStackNode` that
       results from stacking :class:`ParamNodes <ParamNode>` as the first
       operation in the network contraction, if ``auto_stack`` mode is set to
-      ``True``. There might be as much ``"virtual_stack"`` nodes as stacks are
-      created from ``ParamNodes``. To learn more about this, see
-      :class:`ParamStackNode`.
+      ``True``. To learn more about this, see :class:`ParamStackNode`.
     
     * **"virtual_uniform"**: Name of the ``virtual`` :class:`Node` or
       :class:`ParamNode` that is used in uniform (translationally invariant)
       tensor networks to store the tensor that will be shared by all ``leaf``
       nodes. There might be as much ``"virtual_uniform"`` nodes as shared
       memories are used for the ``leaf`` nodes in the network (usually just one).
+    
+    For ``"virtual_result"`` and ``"virtual_uniform"``, these special
+    behaviours are not restricted to nodes having those names, but also nodes
+    whose names contain those strings.
       
     Although these names can in principle be used for other nodes, this can lead
     to undesired behaviour.
       
     See :meth:`~TensorNetwork.reset` to learn more about the importance of these
     reserved nodes' names.
     
@@ -461,33 +465,32 @@
                                  '`tensor`\'s shape should be equal to `shape`')
 
         # Check shape type
         if shape is not None:
             if not isinstance(shape, (tuple, list, Size)):
                 raise TypeError(
                     '`shape` should be tuple[int], list[int] or torch.Size type')
-            if isinstance(shape, (tuple, list)):
-                for i in shape:
-                    if not isinstance(i, int):
-                        raise TypeError('`shape` elements should be int type')
+            if isinstance(shape, Sequence):
+                if any([not isinstance(i, int) for i in shape]):
+                    raise TypeError('`shape` elements should be int type')
             aux_shape = Size(shape)
         else:
             aux_shape = tensor.shape
 
         # Check tensor type
         if tensor is not None:
             if not isinstance(tensor, Tensor):
                 raise TypeError('`tensor` should be torch.Tensor type')
 
         # Check axes_names
         if axes_names is None:
             axes = [Axis(num=i, name=f'axis_{i}', node=self)
                     for i, _ in enumerate(aux_shape)]
         else:
-            if not isinstance(axes_names, (tuple, list)):
+            if not isinstance(axes_names, Sequence):
                 raise TypeError(
                     '`axes_names` should be tuple[str] or list[str] type')
             if len(axes_names) != len(aux_shape):
                 raise ValueError(
                     '`axes_names` length should match `shape` length')
             else:
                 axes_names = enum_repeated_names(axes_names)
@@ -709,14 +712,21 @@
     @abstractmethod
     def parameterize(self, set_param: bool) -> 'AbstractNode':
         pass
 
     @abstractmethod
     def copy(self, share_tensor: bool = False) -> 'AbstractNode':
         pass
+    
+    @abstractmethod
+    def change_type(self,
+                    leaf: bool = False,
+                    data: bool = False,
+                    virtual: bool = False,) -> None:
+        pass
 
     # -------
     # Methods
     # -------
     def is_leaf(self) -> bool:
         """
         Returns a boolean indicating if the node is a ``leaf`` node. These are
@@ -841,14 +851,25 @@
 
         neighbours = set()
         for i, edge in enumerate(self._edges):
             if not edge.is_dangling():
                 node2 = edge._nodes[node1_list[i]]
                 neighbours.add(node2)
         return list(neighbours)
+    
+    def is_connected_to(self, other: 'AbstractNode') -> List[Tuple[Axis]]:
+        """Returns list of tuples of axes where the node is connected to ``other``"""
+        connected_axes = []
+        for i1, edge1 in enumerate(self._edges):
+            for i2, edge2 in enumerate(other._edges):
+                if (edge1 == edge2) and not edge1.is_dangling():
+                    if self.is_node1(i1) != other.is_node1(i2):
+                        connected_axes.append((self._axes[i1],
+                                               other._axes[i2]))
+        return connected_axes
 
     def _change_axis_name(self, axis: Axis, name: Text) -> None:
         """
         Changes the name of an axis. If an axis belongs to a node, we have to
         take care of repeated names. If the name that is going to be assigned
         to the axis is already set for another axis, we change  those names by
         an enumerated version of them.
@@ -947,25 +968,25 @@
         """Returns axis' ``num`` given the :class:`Axis` or its ``name``."""
         if isinstance(axis, int):
             if axis < 0:
                 axis = axis % self.rank  # When indexing with -1, -2, ...
             for ax in self._axes:
                 if axis == ax._num:
                     return ax._num
-            raise IndexError(f'Node {self!s} has no axis with index {axis}')
+            raise IndexError(f'Node "{self!s}" has no axis with index {axis}')
         elif isinstance(axis, str):
             for ax in self._axes:
                 if axis == ax._name:
                     return ax._num
-            raise IndexError(f'Node {self!s} has no axis with name {axis}')
+            raise IndexError(f'Node "{self!s}" has no axis with name "{axis}"')
         elif isinstance(axis, Axis):
             for ax in self._axes:
                 if axis == ax:
                     return ax._num
-            raise IndexError(f'Node {self!s} has no axis {axis!r}')
+            raise IndexError(f'Node "{self!s}" has no axis "{axis!r}"')
         else:
             raise TypeError('`axis` should be int, str or Axis type')
 
     def _add_edge(self,
                   edge: 'Edge',
                   axis: Ax,
                   node1: bool = True) -> None:
@@ -990,15 +1011,15 @@
         """
         Returns :class:`Edge` given the :class:`Axis` (or its ``name``
         or ``num``) where it is attached to the node.
         """
         axis_num = self.get_axis_num(axis)
         return self._edges[axis_num]
 
-    def in_which_axis(self, edge: 'Edge') -> Union[Axis, List[Axis]]:
+    def in_which_axis(self, edge: 'Edge') -> Union[Axis, Tuple[Axis]]:
         """
         Returns :class:`Axis` given the :class:`Edge` that is attached
         to the node through it.
         """
         lst = []
         for ax, ed in zip(self._axes, self._edges):
             if ed == edge:
@@ -1006,31 +1027,36 @@
 
         if len(lst) == 0:
             raise ValueError(f'Edge {edge} not in node {self}')
         elif len(lst) == 1:
             return lst[0]
         else:
             # Case of trace edges (attached to the node in two axes)
-            return lst
+            return tuple(lst)
 
-    def reattach_edges(self, override: bool = False) -> None:
+    def reattach_edges(self,
+                       axes: Optional[Sequence[Ax]] = None,
+                       override: bool = False) -> None:
         """
         Substitutes current edges by copies of them that are attached to the node.
         It can happen that an edge is not attached to the node if it is the result
         of an :class:`Operation` and, hence, it inherits edges from the operands.
         In that case, the new copied edges will be attached to the resultant node,
         replacing each previous ``node1`` or ``node2`` with it (according to the
         ``node1`` attribute of each axis).
 
         Used for in-place operations like :func:`permute_` or :func:`split_` and
         to (de)parameterize nodes.
 
         Parameters
         ----------
-        override: bool
+        axis : list[int, str or Axis] or tuple[int, str or Axis], optional
+            The edge attached to these axes will be reattached. If ``None``,
+            all edges will be reattached.
+        override : bool
             Boolean indicating if the new, reattached edges should also replace
             the corresponding edges in the node's neighbours (``True``). Otherwise,
             the neighbours' edges will be pointing to the original nodes from which
             the current node inherits its edges (``False``).
             
         Examples
         --------
@@ -1058,38 +1084,54 @@
         >>> result.reattach_edges()
         >>> result in result['right'].nodes
         True
         
         If ``override`` is ``True``, ``nodeB['right']`` would be replaced by the
         new ``result['right']``.
         """
-        for i, (edge, node1) in enumerate(zip(self._edges, self.is_node1())):
+        if axes is None:
+            edges = list(enumerate(self._edges))
+        else:
+            edges = []
+            for axis in axes:
+                axis_num = self.get_axis_num(axis)
+                edges.append((axis_num, self._edges[axis_num]))
+        
+        skip_edges = []
+        for i, edge in edges:
+            if i in skip_edges:
+                continue
+            
+            node1 = self._axes[i]._node1
             node = edge._nodes[1 - node1]
             if node != self:
                 # New edges are always a copy, so that the original
                 # nodes have different edges from the current node
                 new_edge = edge.copy()
                 self._edges[i] = new_edge
 
                 new_edge._nodes[1 - node1] = self
                 new_edge._axes[1 - node1] = self._axes[i]
 
                 # Case of trace edges (attached to the node in two axes)
                 neighbour = new_edge._nodes[node1]
-                if neighbour == node:
-                    for j, other_edge in enumerate(self._edges):
-                        if (other_edge == edge) and (i != j):
-                            self._edges[j] = new_edge
-                            new_edge._nodes[node1] = self
-                            new_edge._axes[node1] = self._axes[j]
+                if not new_edge.is_dangling():
+                    if neighbour != self:
+                        for j, other_edge in edges[(i + 1):]:
+                            if other_edge == edge:
+                                new_edge._nodes[node1] = self
+                                new_edge._axes[node1] = self._axes[j]
+                                self._edges[j] = new_edge
+                                skip_edges.append(j)
 
                 if override:
-                    if not new_edge.is_dangling() and (neighbour != node):
-                        neighbour._add_edge(
-                            new_edge, new_edge._axes[node1], not node1)
+                    if not new_edge.is_dangling():
+                        if new_edge._nodes[0] != new_edge._nodes[1]:
+                            new_edge._nodes[node1]._add_edge(
+                                new_edge, new_edge._axes[node1], not node1)
 
     def disconnect(self, axis: Optional[Ax] = None) -> None:
         """
         Disconnects all edges of the node if they were connected to other nodes.
         If ``axis`` is sepcified, only the corresponding edge is disconnected.
 
         Parameters
@@ -1123,15 +1165,18 @@
 
     @staticmethod
     def _make_copy_tensor(shape: Shape,
                           device: torch.device = torch.device('cpu')) -> Tensor:
         """Returns copy tensor (ones in the "diagonal", zeros elsewhere)."""
         copy_tensor = torch.zeros(shape, device=device)
         rank = len(shape)
-        i = torch.arange(min(shape), device=device)
+        if rank <= 1:
+            i = 0
+        else:
+            i = torch.arange(min(shape), device=device)
         copy_tensor[(i,) * rank] = 1.
         return copy_tensor
 
     @staticmethod
     def _make_rand_tensor(shape: Shape,
                           low: float = 0.,
                           high: float = 1.,
@@ -1393,14 +1438,17 @@
         >>> tensor = torch.randn(2, 3)
         >>> node.set_tensor(tensor)
         >>> torch.equal(node.tensor, tensor)
         True
         """
         # If node stores its own tensor
         if not self.is_resultant() and (self._tensor_info['address'] is not None):
+            if (tensor is not None) and not self._compatible_shape(tensor):
+                warnings.warn(f'`tensor` is being cropped to fit the shape of '
+                              f'node "{self!s}" at non-batch edges')
             self._unrestricted_set_tensor(tensor=tensor,
                                           init_method=init_method,
                                           device=device,
                                           **kwargs)
         else:
             raise ValueError('Node\'s tensor can only be changed if it is not'
                              ' resultant and stores its own tensor')
@@ -1845,26 +1893,44 @@
             if isinstance(axis, (list, tuple)):
                 for ax in axis:
                     axis_num.append(self.get_axis_num(ax))
             else:
                 axis_num.append(self.get_axis_num(axis))
         return self.tensor.norm(p=p, dim=axis_num)
 
+    def numel(self) -> Tensor:
+        """
+        Returns the total number of elements in the node's tensor.
+
+        See also `torch.numel() <https://pytorch.org/docs/stable/generated/torch.numel.html>`_.
+
+        Returns
+        -------
+        int
+        
+        Examples
+        --------
+        >>> node = tk.randn(shape=(2, 3), axes_names=('left', 'right'))
+        >>> node.numel()
+        6
+        """
+        return self.tensor.numel()
+
     def __str__(self) -> Text:
         return self._name
 
     def __repr__(self) -> Text:
         return f'{self.__class__.__name__}(\n ' \
                f'\tname: {self._name}\n' \
                f'\ttensor:\n{tab_string(repr(self.tensor), 2)}\n' \
                f'\taxes:\n{tab_string(print_list(self.axes_names), 2)}\n' \
                f'\tedges:\n{tab_string(print_list(self._edges), 2)})'
 
 
-class Node(AbstractNode):
+class Node(AbstractNode):  # MARK: Node
     """
     Base class for non-trainable nodes. Should be subclassed by any class of nodes
     that are not intended to be trained (e.g. :class:`StackNode`).
 
     Can be used for fixed nodes of the :class:`TensorNetwork`, or intermediate
     nodes that are resultant from an :class:`Operation` between nodes.
     
@@ -2124,17 +2190,65 @@
                             axes_names=self.axes_names,
                             name=self._name + '_copy',
                             network=self._network,
                             tensor=self.tensor,
                             edges=self._edges,
                             node1_list=self.is_node1())
         return new_node
+    
+    def change_type(self,
+                    leaf: bool = False,
+                    data: bool = False,
+                    virtual: bool = False,) -> None:
+        """
+        Changes node type, only if node is not a resultant node.
+        
+        Parameters
+        ----------
+        leaf : bool
+            Boolean indicating if the new node type is ``leaf``.
+        data : bool
+            Boolean indicating if the new node type is ``data``.
+        virtual : bool
+            Boolean indicating if the new node type is ``virtual``.
+        """
+        if self.is_resultant():
+            raise ValueError('Only non-resultant nodes\' types can be changed')
+        
+        if (leaf + data + virtual) != 1:
+            raise ValueError('One, and only one, of `leaf`, `data` and `virtual`'
+                             ' can be set to True')
+        
+        # Unset current type
+        if self._leaf and not leaf:
+            node_dict = self._network._leaf_nodes
+            self._leaf = False
+            del node_dict[self._name]
+        elif self._data and not data:
+            node_dict = self._network._data_nodes
+            self._data = False
+            del node_dict[self._name]
+        elif self._virtual and not virtual:
+            node_dict = self._network._virtual_nodes
+            self._virtual = False
+            del node_dict[self._name]
+        
+        # Set new type
+        if leaf:
+            self._leaf = True
+            self._network._leaf_nodes[self._name] = self
+        elif data:
+            self._data = True
+            self._network._data_nodes[self._name] = self
+        elif virtual:
+            self._virtual = True
+            self._network._virtual_nodes[self._name] = self
 
 
-class ParamNode(AbstractNode):
+class ParamNode(AbstractNode):  # MARK: ParamNode
     """
     Class for trainable nodes. Should be subclassed by any class of nodes that
     are intended to be trained (e.g. :class:`ParamStackNode`).
 
     Should be used as the initial nodes conforming the :class:`TensorNetwork`,
     if it is going to be trained. When operating these initial nodes, the resultant
     nodes will be non-parameterized (e.g. :class:`Node`, :class:`StackNode`).
@@ -2488,20 +2602,55 @@
                                  axes_names=self.axes_names,
                                  name=self._name + '_copy',
                                  network=self._network,
                                  tensor=self.tensor,
                                  edges=self._edges,
                                  node1_list=self.is_node1())
         return new_node
+    
+    def change_type(self,
+                    leaf: bool = False,
+                    virtual: bool = False,) -> None:
+        """
+        Changes node type, only if node is not a resultant node.
+        
+        Parameters
+        ----------
+        leaf : bool
+            Boolean indicating if the new node type is ``leaf``.
+        virtual : bool
+            Boolean indicating if the new node type is ``virtual``.
+        """
+        if (leaf + virtual) != 1:
+            raise ValueError('One, and only one, of `leaf`, and `virtual`'
+                             ' can be set to True')
+        
+        # Unset current type
+        if self._leaf and not leaf:
+            node_dict = self._network._leaf_nodes
+            self._leaf = False
+            del node_dict[self._name]
+        elif self._virtual and not virtual:
+            node_dict = self._network._virtual_nodes
+            self._virtual = False
+            del node_dict[self._name]
+        
+        # Set new type
+        if leaf:
+            self._leaf = True
+            self._network._leaf_nodes[self._name] = self
+        elif virtual:
+            self._virtual = True
+            self._network._virtual_nodes[self._name] = self
 
 
 ###############################################################################
 #                                 STACK NODES                                 #
 ###############################################################################
-class StackNode(Node):
+class StackNode(Node):  # MARK: StackNode
     """
     Class for stacked nodes. ``StackNodes`` are nodes that store the information
     of a list of nodes that are stacked via :func:`stack`, although they can also
     be instantiated directly. To do so, there are two options:
 
     * Provide a sequence of nodes: if ``nodes`` are provided, their tensors will
       be stacked and stored in the ``StackNode``. It is necessary that all nodes
@@ -2603,20 +2752,18 @@
                  network: Optional['TensorNetwork'] = None,
                  override_node: bool = False,
                  tensor: Optional[Tensor] = None,
                  edges: Optional[List['Edge']] = None,
                  node1_list: Optional[List[bool]] = None) -> None:
 
         if nodes is not None:
-            if not isinstance(nodes, (list, tuple)):
+            if not isinstance(nodes, Sequence):
                 raise TypeError('`nodes` should be a list or tuple of nodes')
-            for node in nodes:
-                if isinstance(node, (StackNode, ParamStackNode)):
-                    raise TypeError(
-                        'Cannot create a stack using (Param)StackNode\'s')
+            if any([isinstance(node, (StackNode, ParamStackNode)) for node in nodes]):
+                raise TypeError('Cannot create a stack using (Param)StackNode\'s')
             if tensor is not None:
                 raise ValueError(
                     'If `nodes` are provided, `tensor` must not be given')
 
             # Check all nodes share properties
             for i in range(len(nodes[:-1])):
                 if not isinstance(nodes[i], type(nodes[i + 1])):
@@ -2723,31 +2870,45 @@
         if axis._num == 0:
             # Stack axis
             return Edge(node1=self, axis1=axis)
         else:
             return StackEdge(edges=self._edges_dict[axis._name],
                              node1_list=self._node1_lists_dict[axis._name],
                              node1=self, axis1=axis)
+    
+    def reconnect(self, other: Union['StackNode', 'ParamStackNode']) -> None:
+        """
+        Re-connects the ``StackNode`` to another ``(Param)StackNode``, in the
+        axes where the original stacked nodes were already connected.
+        """
+        for axis1 in self._edges_dict:
+            for axis2 in other._edges_dict:
+                if self._edges_dict[axis1][0] == other._edges_dict[axis2][0]:
+                    connect_stack(self.get_edge(axis1), other.get_edge(axis2))
+    
+    def __xor__(self, other: Union['StackNode', 'ParamStackNode']) -> None:
+        self.reconnect(other)
 
 
-class ParamStackNode(ParamNode):
+class ParamStackNode(ParamNode):  # MARK: ParamStackNode
     """
     Class for parametric stacked nodes. They are essentially the same as
     :class:`StackNodes <StackNode>` but they are :class:`ParamNodes <ParamNode>`.
     
     They are used to optimize memory usage and save some time when the first
     operation that occurs to param-nodes in a contraction (that might be
     computed several times during training) is :func:`stack`. If this is the case,
     the param-nodes no longer store their own tensors, but rather they make
     reference to a slide of a greater ``ParamStackNode`` (if ``auto_stack``
     attribute of the :class:`TensorNetwork` is set to ``True``). Hence, that
     first :func:`stack` is never actually computed.
     
-    The ``ParamStackNode`` that results from this process uses the reserved name
-    ``"virtual_stack"``, as explained :class:`here <AbstractNode>`. This node
+    The ``ParamStackNode`` that results from this process has the name
+    ``"virtual_result_stack"``, which contains the reserved name
+    ``"virtual_result"``, as explained :class:`here <AbstractNode>`. This node
     stores the tensor from which all the stacked :class:`ParamNodes <ParamNode>`
     just take one `slice`.
     
     This behaviour occurs when stacking param-nodes via :func:`stack`, not when
     instantiating ``ParamStackNode`` manually.
     
     |
@@ -2819,21 +2980,18 @@
 
     def __init__(self,
                  nodes: Sequence[AbstractNode],
                  name: Optional[Text] = None,
                  virtual: bool = False,
                  override_node: bool = False) -> None:
 
-        if not isinstance(nodes, (list, tuple)):
+        if not isinstance(nodes, Sequence):
             raise TypeError('`nodes` should be a list or tuple of nodes')
-
-        for node in nodes:
-            if isinstance(node, (StackNode, ParamStackNode)):
-                raise TypeError(
-                    'Cannot create a stack using (Param)StackNode\'s')
+        if any([isinstance(node, (StackNode, ParamStackNode)) for node in nodes]):
+                raise TypeError('Cannot create a stack using (Param)StackNode\'s')
 
         for i in range(len(nodes[:-1])):
             if not isinstance(nodes[i], type(nodes[i + 1])):
                 raise TypeError('Cannot stack nodes of different types. Nodes '
                                 'must be either all Node or all ParamNode type')
             if nodes[i].rank != nodes[i + 1].rank:
                 raise ValueError(
@@ -2902,37 +3060,51 @@
         if axis.num == 0:
             # Stack axis
             return Edge(node1=self, axis1=axis)
         else:
             return StackEdge(edges=self._edges_dict[axis._name],
                              node1_list=self._node1_lists_dict[axis._name],
                              node1=self, axis1=axis)
+    
+    def reconnect(self, other: Union['StackNode', 'ParamStackNode']) -> None:
+        """
+        Re-connects the ``StackNode`` to another ``(Param)StackNode``, in the
+        axes where the original stacked nodes were already connected.
+        """
+        for axis1 in self._edges_dict:
+            for axis2 in other._edges_dict:
+                if self._edges_dict[axis1][0] == other._edges_dict[axis2][0]:
+                    connect_stack(self.get_edge(axis1), other.get_edge(axis2))
+    
+    def __xor__(self, other: Union['StackNode', 'ParamStackNode']) -> None:
+        self.reconnect(other)
 
 
 ###############################################################################
 #                                    EDGES                                    #
 ###############################################################################
-class Edge:
+class Edge:  # MARK: Edge
     """
     Base class for edges. Should be subclassed by any new class of edges.
 
     An edge is nothing more than an object that wraps references to the nodes it
     connects. Thus, it stores information like the nodes it connects, the
     corresponding nodes' axes it is attached to, whether it is dangling or
     batch, its size, etc.
 
     Above all, its importance lies in that edges enable to connect nodes, forming
     any possible graph, and to perform easily :class:`Operations <Operation>` like
     contracting and splitting nodes.
     
     |
 
-    Furthermore, edges have specific operations like :meth:`contract_` or
-    :meth:`svd_` (and its variations) that allow in-place modification of the
-    :class:`TensorNetwork`.
+    Furthermore, edges have specific operations like :meth:`contract` or
+    :meth:`svd` (and its variations), as well as in-place versions of them 
+    (:meth:`contract_`, :meth:`svd_`, etc.) that allow in-place modification
+    of the :class:`TensorNetwork`.
     
     |
 
     Parameters
     ----------
     node1 : AbstractNode
         First node to which the edge is connected.
@@ -3166,15 +3338,15 @@
         Connects dangling edge to another dangling edge. It is necessary that
         both edges have the same size so that contractions along that edge can
         be computed.
         
         Note that this connectes edges from ``leaf`` (or ``data``, ``virtual``)
         nodes, but never from ``resultant`` nodes. If one tries to connect
         one of the inherited edges of a ``resultant`` node, the new connected
-        edge will be attached to the original ``leaf` nodes from which the
+        edge will be attached to the original ``leaf`` nodes from which the
         ``resultant`` node inherited its edges. Hence, the ``resultant`` node
         will not "see" the connection until the :class:`TensorNetwork` is
         :meth:`~TensorNetwork.reset`.
         
         If the nodes that are being connected come from different networks, the
         ``node2`` (and its connected component) will be moved to ``node1``'s
         network. See also :meth:`~AbstractNode.move_to_network`.
@@ -3257,15 +3429,15 @@
 
 ###############################################################################
 #                                 STACK EDGES                                 #
 ###############################################################################
 AbstractStackNode = Union[StackNode, ParamStackNode]
 
 
-class StackEdge(Edge):
+class StackEdge(Edge):  # MARK: StackEdge
     """
     Class for stacked edges. They are just like :class:`Edges <Edge>` but used
     when stacking a collection of nodes into a :class:`StackNode`. When doing
     this, all edges of the stacked nodes must be kept, since they have the
     information regarding the nodes' neighbours, which will be used when :func:
     `unbinding <unbind>` the stack.
     
@@ -3370,15 +3542,15 @@
     """
     Connects two dangling edges. It is necessary that both edges have the same
     size so that contractions along that edge can be computed.
     
     Note that this connectes edges from ``leaf`` (or ``data``, ``virtual``)
     nodes, but never from ``resultant`` nodes. If one tries to connect one of
     the inherited edges of a ``resultant`` node, the new connected edge will be
-    attached to the original ``leaf` nodes from which the ``resultant`` node
+    attached to the original ``leaf`` nodes from which the ``resultant`` node
     inherited its edges. Hence, the ``resultant`` node will not "see" the
     connection until the :class:`TensorNetwork` is :meth:`~TensorNetwork.reset`.
     
     If the nodes that are being connected come from different networks, the
     ``node2`` (and its connected component) will be movec to ``node1``'s network.
     See also :meth:`~AbstractNode.move_to_network`.
 
@@ -3417,25 +3589,25 @@
 
     # Case edge is already connected
     if edge1 == edge2:
         return edge1
 
     for edge in [edge1, edge2]:
         if not edge.is_dangling():
-            raise ValueError(f'Edge {edge!s} is not a dangling edge. '
-                             f'This edge points to nodes: {edge.node1!s} and '
-                             f'{edge.node2!s}')
+            raise ValueError(f'Edge "{edge!s}" is not a dangling edge. '
+                             f'This edge points to nodes: "{edge.node1!s}" and '
+                             f'"{edge.node2!s}"')
         if edge.is_batch():
-            raise ValueError(f'Edge {edge!s} is a batch edge. Batch edges '
+            raise ValueError(f'Edge "{edge!s}" is a batch edge. Batch edges '
                              'cannot be connected')
 
     if edge1.size() != edge2.size():
         raise ValueError(f'Cannot connect edges of unequal size. '
-                         f'Size of edge {edge1!s}: {edge1.size()}. '
-                         f'Size of edge {edge2!s}: {edge2.size()}')
+                         f'Size of edge "{edge1!s}": {edge1.size()}. '
+                         f'Size of edge "{edge2!s}": {edge2.size()}')
 
     node1, axis1 = edge1.node1, edge1.axis1
     node2, axis2 = edge2.node1, edge2.axis1
     net1, net2 = node1._network, node2._network
 
     if net1 != net2:
         node2.move_to_network(net1)
@@ -3480,17 +3652,17 @@
                          'stack nodes.')
     # Case edge is already connected
     if edge1 == edge2:
         return edge1
 
     for edge in [edge1, edge2]:
         if not edge.is_dangling():
-            raise ValueError(f'Edge {edge!s} is not a dangling edge. '
-                             f'This edge points to nodes: {edge.node1!s} and '
-                             f'{edge.node2!s}')
+            raise ValueError(f'Edge "{edge!s}" is not a dangling edge. '
+                             f'This edge points to nodes: "{edge.node1!s}" and '
+                             f'"{edge.node2!s}"')
 
     node1, axis1 = edge1.node1, edge1.axis1
     node2, axis2 = edge2.node1, edge2.axis1
     net1, net2 = node1._network, node2._network
 
     net1._remove_edge(edge1)
     net1._remove_edge(edge2)
@@ -3557,15 +3729,15 @@
 
     return tuple(new_edges)
 
 
 ###############################################################################
 #                                   SUCCESSOR                                 #
 ###############################################################################
-class Successor:
+class Successor:  # MARK: Successor
     """
     Class for successors. This is a sort of cache memory for :class:`Operations
     <Operation>` that have been already computed.
 
     For instance, when contracting two nodes, the result gives a new node that
     stores the tensor resultant from contracting both nodes' tensors. However,
     when training a :class:`TensorNetwork`, the tensors inside the nodes will
@@ -3636,15 +3808,15 @@
         self.child = child
         self.hints = hints
 
 
 ###############################################################################
 #                                TENSOR NETWORK                               #
 ###############################################################################
-class TensorNetwork(nn.Module):
+class TensorNetwork(nn.Module):  # MARK: TensorNetwork
     """
     Class for arbitrary Tensor Networks. Subclass of **PyTorch**
     ``torch.nn.Module``.
 
     Tensor Networks are the central objects of **TensorKrowch**. Basically,
     a tensor network is a graph with vertices (:class:`Nodes <AbstractNode>`)
     connected by :class:`Edges <Edge>`. In these models, nodes' tensors will be
@@ -3808,15 +3980,15 @@
 
         # Memories
         self._memory_nodes = dict()    # address -> memory
         self._inverse_memory = dict()  # address -> nodes using that memory
 
         # TN modes
         # Auto-management of memory mode
-        self._auto_stack = False   # train -> True / eval -> True
+        self._auto_stack = True   # train -> True / eval -> True
         self._auto_unbind = False  # train -> False / eval -> True
         self._tracing = False      # Tracing mode (True while calling .trace())
         self._traced = False       # True if .trace() is called, False if reset()
 
         # Lis of operations used to contract the TN
         self._seq_ops = []
 
@@ -3877,15 +4049,15 @@
         """
         return self._edges
 
     @property
     def auto_stack(self) -> bool:
         """
         Returns boolean indicating whether ``auto_stack`` mode is active. By
-        default, it is ``False``.
+        default, it is ``True``.
         
         This mode indicates whether the operation :func:`stack` can take control
         of the memory management of the network to skip some steps in future
         computations. If ``auto_stack`` is set to ``True`` and a collection of
         :class:`ParamNodes <ParamNode>` are :func:`stacked <stack>` (as the
         first operation in which these nodes are involved), then those nodes
         will no longer store their own tensors, but rather a ``virtual``
@@ -4089,15 +4261,19 @@
         >>> _ = nodeA[1] ^ nodeB[0]
         >>> nodeB.network.delete_node(nodeB, False)
         >>> print(nodeA.name)
         node_0
         """
         node.disconnect()
         self._remove_node(node, move_names)
-        del node
+        node._temp_tensor = None
+    
+    def delete(self) -> None:
+        for node in self.nodes.values():
+            self.delete_node(node)
 
     def _update_node_info(self, node: AbstractNode, new_name: Text) -> None:
         """
         Updates a single node's ``tensor_info`` "address" and its corresponding
         address in ``memory_nodes`` and ``inverse_memory``.
         """
         prev_name = node._name
@@ -4130,32 +4306,33 @@
             node._temp_tensor = None
             node._tensor_info['address'] = new_name
 
     def _update_node_name(self, node: AbstractNode, new_name: Text) -> None:
         """Updates a single node's name, without taking care of the other names."""
         # Node is ParamNode and tensor is not None
         if isinstance(node.tensor, Parameter):
-            delattr(self, '_'.join(['param', node._name]))
+            if hasattr(self, 'param_' + node._name):
+                delattr(self, 'param_' + node._name)
         for edge in node._edges:
             if edge.is_attached_to(node):
                 self._remove_edge(edge)
 
         self._update_node_info(node, new_name)
         node._name = new_name
 
         if isinstance(node.tensor, Parameter):
-            if not hasattr(self, '_'.join(['param', node._name])):
-                self.register_parameter(
-                    '_'.join(['param', node._name]),
-                    self._memory_nodes[node._name])
-            else:
-                # Nodes names are never repeated, so it is likely that
-                # this case will never occur
-                raise ValueError(
-                    f'Network already has attribute named {node._name}')
+            if node._tensor_info['address'] is not None:
+                if not hasattr(self, 'param_' + node._name):
+                    self.register_parameter('param_' + node._name,
+                                            self._memory_nodes[node._name])
+                else:
+                    # Nodes names are never repeated, so it is likely that
+                    # this case will never occur
+                    raise ValueError(
+                        f'Network already has attribute named {node._name}')
 
         for edge in node._edges:
             self._add_edge(edge)
 
     def _assign_node_name(self, node: AbstractNode,
                           name: Text,
                           first_time: bool = False) -> None:
@@ -4241,18 +4418,17 @@
             node._name = new_name
         else:
             self._update_node_info(node, new_name)
             node._name = new_name
 
         # Node is ParamNode and tensor is not None
         if isinstance(node.tensor, Parameter):
-            if not hasattr(self, '_'.join(['param', node._name])):
-                self.register_parameter(
-                    '_'.join(['param', node._name]),
-                    self._memory_nodes[node._name])
+            if not hasattr(self, 'param_' + node._name,):
+                self.register_parameter( 'param_' + node._name,
+                                        self._memory_nodes[node._name])
             else:
                 # Nodes names are never repeated, so it is likely that
                 # this case will never occur
                 raise ValueError(
                     f'Network already has attribute named {node._name}')
 
         for edge in node._edges:
@@ -4284,15 +4460,16 @@
             when removing a node (``True``) or kept as they are (``False``).
             This is useful when several nodes are being modified at once, and
             each resultant node has the same enumeration as the corresponding
             original node.
         """
         # Node is ParamNode and tensor is not None
         if isinstance(node.tensor, Parameter):
-            delattr(self, '_'.join(['param', node._name]))
+            if hasattr(self, 'param_' + node._name):
+                delattr(self, 'param_' + node._name)
         for edge in node._edges:
             if edge.is_attached_to(node):
                 self._remove_edge(edge)
 
         non_enum_prev_name = erase_enum(node.name)
         count = self._repeated_nodes_names[non_enum_prev_name]
         if move_names:
@@ -4347,16 +4524,16 @@
             Boolean indicating whether the tensor network has to be parameterized
             (``True``) or de-parameterized (``False``).
         override : bool
             Boolean indicating whether the tensor network should be parameterized
             in-place (``True``) or copied and then parameterized (``False``).
         """
         if self._resultant_nodes:
-            warnings.warn('Resultant nodes will be removed before parameterizing'
-                          ' the TN')
+            warnings.warn(
+                'Resultant nodes will be removed before parameterizing the TN')
             self.reset()
 
         if override:
             net = self
         else:
             net = self.copy()
 
@@ -4496,15 +4673,15 @@
         data_nodes = []
         for i, edge in enumerate(input_edges):
             if isinstance(edge, int):
                 edge = self[edge]
             elif isinstance(edge, Edge):
                 if edge not in self._edges:
                     raise ValueError(
-                        f'Edge {edge!r} should be a dangling edge of the '
+                        f'Edge "{edge!r}" should be a dangling edge of the '
                         'Tensor Network')
             else:
                 raise TypeError(
                     '`input_edges` should be list[int] or list[Edge] type')
 
             node = Node(shape=(*([1] * num_batch_edges), edge.size()),
                         axes_names=(*(['batch'] * num_batch_edges), 'feature'),
@@ -4589,15 +4766,18 @@
         >>> net['data_0'].shape
         torch.Size([100, 5])
         """
 
         stack_node = self._virtual_nodes.get('stack_data_memory')
 
         if stack_node is not None:
-            data = data.movedim(-2, 0)
+            if isinstance(data, Tensor):
+                data = data.movedim(-2, 0)
+            else:
+                data = torch.stack(data, dim=0)
             stack_node.tensor = data
             for i, data_node in enumerate(list(self._data_nodes.values())):
                 data_node._shape = data[i].shape
         elif self._data_nodes:
             for i, data_node in enumerate(list(self._data_nodes.values())):
                 data_node.tensor = data[i]
         else:
@@ -4614,15 +4794,15 @@
           is created when :func:`stacking <stack>` :class:`ParamNodes <ParamNode>`
           (if ``auto_stack`` mode is active). If there is a ``"virtual_uniform"``
           node in the network from which all ``leaf`` nodes take their tensor,
           this is not modified.
           
         * ``virtual``: Only virtual nodes created in :class:`operations
           <Operation>` are :meth:`deleted <delete_node>`. This only includes
-          nodes using the reserved name ``"virtual_stack"``.
+          nodes using the reserved name ``"virtual_result"``.
           
         * ``resultant``: These nodes are :meth:`deleted <delete_node>` from the
           network.
         
         Also, the dictionaries of :class:`Successors <Successor>` of all ``leaf``
         and ``data`` nodes are emptied.
         
@@ -4641,17 +4821,18 @@
 
         if self._resultant_nodes or self._virtual_nodes:
             aux_dict = dict()
             aux_dict.update(self._leaf_nodes)
             aux_dict.update(self._resultant_nodes)
             aux_dict.update(self._virtual_nodes)
             for node in aux_dict.values():
-                if node._virtual and ('virtual_stack' not in node._name):
-                    # Virtual nodes named "virtual_stack" are ParamStackNodes
-                    # that result from stacking a collection of ParamNodes
+                if node._virtual and ('virtual_result' not in node._name):
+                    # Virtual nodes named "virtual_result" are nodes that are
+                    # required in some situations during contraction, like
+                    # ParamStackNodes
                     # This condition is satisfied by the rest of virtual nodes
                     continue
 
                 node._successors = dict()
 
                 node_ref = node._tensor_info['node_ref']
                 if node_ref is not None:
@@ -4682,20 +4863,20 @@
             for node in list(self._data_nodes.values()):
                 node._successors = dict()
 
             aux_dict = dict()
             aux_dict.update(self._resultant_nodes)
             aux_dict.update(self._virtual_nodes)
             for node in list(aux_dict.values()):
-                if node._virtual and ('virtual_stack' not in node._name):
+                if node._virtual and ('virtual_result' not in node._name):
                     # This condition is satisfied by the rest of virtual nodes
-                    # (e.g. "virtual_feature", "virtual_n_features")
                     continue
                 self.delete_node(node, False)
 
+    @torch.no_grad()
     def trace(self, example: Optional[Tensor] = None, *args, **kwargs) -> None:
         """
         Traces the tensor network contraction algorithm with two purposes:
 
         * Create all the intermediate ``resultant`` nodes that result from
           :class:`Operations <Operation>` so that in the next contractions only
           the tensor operations have to be computed, thus saving a lot of time.
@@ -4722,21 +4903,20 @@
             be enough to trace the contraction.
         args :
             Arguments that might be used in :meth:`contract`.
         kwargs :
             Keyword arguments that might be used in :meth:`contract`.
         """
         self.reset()
-
-        with torch.no_grad():
-            self._tracing = True
-            self(example, *args, **kwargs)
-            self._tracing = False
-            self(example, *args, **kwargs)
-            self._traced = True
+        
+        self._tracing = True
+        self(example, *args, **kwargs)
+        self._tracing = False
+        self(example, *args, **kwargs)
+        self._traced = True
 
     def contract(self) -> Node:
         """
         Contracts the whole tensor network returning a single :class:`Node`.
         This method is not implemented and subclasses of :class:`TensorNetwork`
         should override it to define the contraction algorithm of the network.
         """
@@ -4825,15 +5005,15 @@
         if isinstance(key, int):
             return self._edges[key]
         elif isinstance(key, Text):
             try:
                 return self.nodes[key]
             except Exception:
                 raise KeyError(
-                    f'Tensor network {self!s} does not have any node with '
+                    f'Tensor network "{self!s}" does not have any node with '
                     f'name {key}')
         else:
             raise TypeError('`key` should be int or str type')
 
     def __str__(self) -> Text:
         return self.name
```

### Comparing `tensorkrowch-1.0.1/tensorkrowch/initializers.py` & `tensorkrowch-1.1.0/tensorkrowch/initializers.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.0.1/tensorkrowch/models/mps.py` & `tensorkrowch-1.1.0/tensorkrowch/models/peps.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,998 +1,1197 @@
 """
 This script contains:
-    * MPS
-    * UMPS
-    * ConvMPS
-    * ConvUMPS
+    * PEPS
+    * UPEPS
+    * ConvPEPS
+    * ConvUPEPS
 """
 
-from typing import (List, Optional, Sequence,
+from typing import (List, Sequence,
                     Text, Tuple, Union)
 
 import torch
 import torch.nn as nn
 
 import tensorkrowch.operations as op
-from tensorkrowch.components import AbstractNode, Node, ParamNode
+from tensorkrowch.components import Node, ParamNode
 from tensorkrowch.components import TensorNetwork
 
 
-class MPS(TensorNetwork):
+class PEPS(TensorNetwork):
     """
-    Class for Matrix Product States, where all nodes are input nodes, that is,
-    they are all connected to ``data`` nodes that will store the input data
-    tensor(s). When contracting the MPS with new input data, the result will
-    be a just a number.
+    Class for Projected Entangled Pair States, where all nodes are input nodes,
+    that is, they are all connected to ``data`` nodes that will store the input
+    data tensor(s). When contracting the PEPS with new input data, the result
+    will be a just a number.
     
-    If the input dimensions of all the input nodes are equal, the input data
-    tensor can be passed as a single tensor. Otherwise, it would have to be
-    passed as a list of tensors with different sizes.
+    A ``PEPS`` is formed by the following nodes:
     
-    An ``MPS`` is formed by the following nodes:
-    
-    * ``left_node``, ``right_node``: `Vector` nodes with axes ``("input", "right")``
-      and ``("left", "input")``, respectively. These are the nodes at the
-      extremes of the ``MPS``. If ``boundary`` is ``"pbc""``, both are ``None``.
+    * ``left_up_corner``, ``left_down_corner``, ``right_up_corner``,
+      ``right_down_corner``: Corner nodes with 3 edges, the one corresponding
+      to the input and 2 connected to the borders.
+      
+    * ``left_border``, ``right_border``, ``up_border``, ``down_border``: Border
+      nodes with 4 edges, the one corresponding to the input, 2 connected to
+      the neighbours in the border, and 1 connected to the `interior` of the
+      grid.
       
-    * ``mats_env``: Environment of `matrix` nodes that. These nodes have axes
-      ``("left", "input", "right")``.
+    * ``grid_env``: Grid environment of nodes with 5 edges, ("input", "left",
+      "right", "up", "down"). Is is a list of lists of nodes.
 
     Parameters
     ----------
-    n_features : int
-        Number of input nodes.
-    in_dim : int, list[int] or tuple[int]
-        Input dimension(s). Equivalent to the physical dimension. If given as a
-        sequence, its length should be equal to ``n_features``.
-    bond_dim : int, list[int] or tuple[int]
-        Bond dimension(s). If given as a sequence, its length should be equal
-        to ``n_features`` (if ``boundary = "pbc"``) or ``n_features - 1`` (if
-        ``boundary = "obc"``). The i-th bond dimension is always the dimension
-        of the right edge of the i-th node.
-    boundary : {"obc", "pbc"}
-        String indicating whether periodic or open boundary conditions should
-        be used.
+    n_rows : int
+        Number of rows of the 2D grid.
+    n_cols : int
+        Number of columns of the 2D grid.
+    in_dim : int
+        Input dimension. Equivalent to the physical dimension.
+    bond_dim : list[int] or tuple[int]
+        Bond dimensions for horizontal and vertical edges (in that order). Thus
+        it should contain 2 elements.
+    boundary : list[{"obc", "pbc"}]
+        List of strings indicating whether periodic or open boundary conditions
+        should be used in the horizontal (up and down) and vertical (left and
+        right) boundaries.
     n_batches : int
         Number of batch edges of input ``data`` nodes. Usually ``n_batches = 1``
         (where the batch edge is used for the data batched) but it could also
         be ``n_batches = 2`` (one edge for data batched, other edge for image
         patches in convolutional layers).
-        
+    
     Examples
     --------
-    ``MPS`` with same input/physical dimensions:
-    
-    >>> mps = tk.models.MPS(n_features=5,
-    ...                     in_dim=2,
-    ...                     bond_dim=5)
-    >>> data = torch.ones(20, 5, 2) # batch_size x n_features x feature_size
-    >>> result = mps(data)
-    >>> result.shape
-    torch.Size([20])
-    
-    ``MPS`` with different input/physical dimensions:
-    
-    >>> mps = tk.models.MPS(n_features=5,
-    ...                     in_dim=list(range(2, 7)),
-    ...                     bond_dim=5)
-    >>> data = [torch.ones(20, i)
-    ...         for i in range(2, 7)] # n_features * [batch_size x feature_size]
-    >>> result = mps(data)
+    >>> peps = tk.models.PEPS(n_rows=2,
+    ...                       n_cols=2,
+    ...                       in_dim=3,
+    ...                       bond_dim=[5, 5])
+    >>> data = torch.ones(20, 4, 3) # batch_size x n_features x feature_size
+    >>> result = peps(data)
     >>> result.shape
     torch.Size([20])
     """
 
     def __init__(self,
-                 n_features: int,
-                 in_dim: Union[int, Sequence[int]],
-                 bond_dim: Union[int, Sequence[int]],
-                 boundary: Text = 'obc',
+                 n_rows: int,
+                 n_cols: int,
+                 in_dim: int,
+                 bond_dim: Sequence[int],
+                 boundary: Sequence[Text] = ['obc', 'obc'],
                  n_batches: int = 1) -> None:
 
-        super().__init__(name='mps')
+        super().__init__(name='peps')
 
         # boundary
-        if boundary not in ['obc', 'pbc']:
-            raise ValueError('`boundary` should be one of "obc" or "pbc"')
-        self._boundary = boundary
+        if not isinstance(boundary, Sequence):
+            raise TypeError('`boundary` should be a sequence of two elements')
+        elif len(boundary) != 2:
+            raise ValueError('`boundary` should be a sequence of two elements')
+
+        if boundary[0] == 'obc':
+            if n_rows < 2:
+                raise ValueError('If `boundary` of rows is "obc", at least '
+                                 'there has to be 2 rows')
+        elif boundary[0] == 'pbc':
+            if n_rows < 1:
+                raise ValueError('If `boundary` of rows is "pbc", at least '
+                                 'there has to be one row')
+        else:
+            raise ValueError('`boundary` elements should be one of "obc" or '
+                             '"pbc"')
 
-        # n_features
-        if boundary == 'obc':
-            if n_features < 2:
-                raise ValueError('If `boundary` is "obc", at least '
-                                 'there has to be 2 nodes')
-        elif boundary == 'pbc':
-            if n_features < 1:
-                raise ValueError('If `boundary` is "pbc", at least '
-                                 'there has to be one node')
+        if boundary[1] == 'obc':
+            if n_cols < 2:
+                raise ValueError('If `boundary` of columns is "obc", at least '
+                                 'there has to be 2 columns')
+        elif boundary[1] == 'pbc':
+            if n_cols < 1:
+                raise ValueError('If `boundary` of columns is "pbc", at least '
+                                 'there has to be one column')
         else:
-            raise ValueError('`boundary` should be one of "obc" or "pbc"')
-        self._n_features = n_features
+            raise ValueError('`boundary` elements should be one of "obc" or '
+                             '"pbc"')
+
+        self._n_rows = n_rows
+        self._n_cols = n_cols
+        self._boundary = boundary
 
         # in_dim
-        if isinstance(in_dim, (list, tuple)):
-            if len(in_dim) != n_features:
-                raise ValueError('If `in_dim` is given as a sequence of int, '
-                                 'its length should be equal to `n_features`')
-            self._in_dim = list(in_dim)
-        elif isinstance(in_dim, int):
-            self._in_dim = [in_dim] * n_features
-        else:
-            raise TypeError('`in_dim` should be int, tuple[int] or list[int] '
-                            'type')
+        if not isinstance(in_dim, int):
+            raise ValueError('`in_dim` should be int type')
+        self._in_dim = in_dim
 
         # bond_dim
         if isinstance(bond_dim, (list, tuple)):
-            if boundary == 'obc':
-                if len(bond_dim) != n_features - 1:
-                    raise ValueError('If `bond_dim` is given as a sequence of int,'
-                                     ' and `boundary` is "obc", its length '
-                                     'should be equal to `n_features` - 1')
-            elif boundary == 'pbc':
-                if len(bond_dim) != n_features:
-                    raise ValueError('If `bond_dim` is given as a sequence of int,'
-                                     ' and `boundary` is "pbc", its length '
-                                     'should be equal to `n_features`')
+            if len(bond_dim) != 2:
+                raise ValueError('`bond_dim` should be a pair of ints')
             self._bond_dim = list(bond_dim)
-        elif isinstance(bond_dim, int):
-            if boundary == 'obc':
-                self._bond_dim = [bond_dim] * (n_features - 1)
-            elif boundary == 'pbc':
-                self._bond_dim = [bond_dim] * n_features
         else:
-            raise TypeError('`in_dim` should be int, tuple[int] or list[int] '
-                            'type')
+            raise TypeError('`bond_dim` should be a pair of ints')
 
         # n_batches
         if not isinstance(n_batches, int):
-            raise TypeError('`n_batches should be int type')
+            raise TypeError('`n_batches` should be int type')
         self._n_batches = n_batches
 
         # Create Tensor Network
         self._make_nodes()
         self.initialize()
 
     @property
-    def n_features(self) -> int:
-        """Returns number of nodes."""
-        return self._n_features
+    def n_rows(self) -> int:
+        """Returns number of rows of the 2D grid."""
+        return self._n_rows
+
+    @property
+    def n_cols(self) -> int:
+        """Returns number of columns of the 2D grid."""
+        return self._n_cols
 
     @property
-    def boundary(self) -> Text:
-        """Returns boundary condition ("obc" or "pbc")."""
+    def boundary(self) -> List[Text]:
+        """
+        Returns boundary conditions in the horizontal (up and down) and
+        vertical (left and right) boundaries.
+        """
         return self._boundary
 
     @property
-    def in_dim(self) -> List[int]:
+    def in_dim(self) -> int:
         """Returns input/physical dimension."""
         return self._in_dim
 
     @property
     def bond_dim(self) -> List[int]:
-        """Returns bond dimension."""
+        """Returns bond dimensions for horizontal and vertical edges."""
         return self._bond_dim
 
     @property
     def n_batches(self) -> int:
         """Returns number of batch edges of the ``data`` nodes."""
         return self._n_batches
 
     def _make_nodes(self) -> None:
-        """Creates all the nodes of the MPS."""
+        """Creates all the nodes of the PEPS."""
         if self.leaf_nodes:
-            raise ValueError('Cannot create MPS nodes if the MPS already has '
-                             'nodes')
+            raise ValueError('Cannot create PEPS nodes if the PEPS already has'
+                             ' nodes')
 
-        self.left_node = None
-        self.right_node = None
-        self.mats_env = []
-
-        if self.boundary == 'obc':
-            self.left_node = ParamNode(shape=(self.in_dim[0], self.bond_dim[0]),
-                                       axes_names=('input', 'right'),
-                                       name='left_node',
-                                       network=self)
-
-            for i in range(self._n_features - 2):
-                node = ParamNode(shape=(self.bond_dim[i],
-                                        self.in_dim[i + 1],
-                                        self.bond_dim[i + 1]),
-                                 axes_names=('left', 'input', 'right'),
-                                 name=f'mats_env_node_({i})',
+        self.left_up_corner = None
+        self.left_down_corner = None
+        self.right_up_corner = None
+        self.right_down_corner = None
+
+        self.left_border = []
+        self.right_border = []
+        self.up_border = []
+        self.down_border = []
+
+        self.grid_env = []
+
+        in_dim = self.in_dim
+        bond_dim = self.bond_dim
+
+        if self.boundary == ['obc', 'obc']:
+            # Left up corner
+            node = ParamNode(shape=(in_dim, bond_dim[0], bond_dim[1]),
+                             axes_names=('input', 'right', 'down'),
+                             name=f'left_up_corner_node',
+                             network=self)
+            self.left_up_corner = node
+
+            # Up border
+            for j in range(self.n_cols - 2):
+                node = ParamNode(shape=(in_dim, bond_dim[0], bond_dim[0], bond_dim[1]),
+                                 axes_names=('input', 'left', 'right', 'down'),
+                                 name=f'up_border_node_({j})',
                                  network=self)
-                self.mats_env.append(node)
+                self.up_border.append(node)
 
-                if i == 0:
-                    self.left_node['right'] ^ self.mats_env[-1]['left']
+                if j == 0:
+                    self.left_up_corner['right'] ^ node['left']
                 else:
-                    self.mats_env[-2]['right'] ^ self.mats_env[-1]['left']
+                    self.up_border[-2]['right'] ^ node['left']
 
-            self.right_node = ParamNode(shape=(self.bond_dim[-1],
-                                               self.in_dim[-1]),
-                                        axes_names=('left', 'input'),
-                                        name='right_node',
-                                        network=self)
+            # Right up corner
+            node = ParamNode(shape=(in_dim, bond_dim[0], bond_dim[1]),
+                             axes_names=('input', 'left', 'down'),
+                             name=f'right_up_corner_node',
+                             network=self)
+            self.right_up_corner = node
 
-            if self._n_features > 2:
-                self.mats_env[-1]['right'] ^ self.right_node['left']
+            if self.n_cols > 2:
+                self.up_border[-1]['right'] ^ node['left']
             else:
-                self.left_node['right'] ^ self.right_node['left']
+                self.left_up_corner['right'] ^ node['left']
 
-        else:
-            for i in range(self._n_features):
-                node = ParamNode(shape=(self.bond_dim[i - 1],
-                                        self.in_dim[i],
-                                        self.bond_dim[i]),
-                                 axes_names=('left', 'input', 'right'),
-                                 name=f'mats_env_node_({i})',
+            # Left border
+            for i in range(self.n_rows - 2):
+                node = ParamNode(shape=(in_dim, bond_dim[0], bond_dim[1], bond_dim[1]),
+                                 axes_names=('input', 'right', 'up', 'down'),
+                                 name=f'left_border_node_({i})',
                                  network=self)
-                self.mats_env.append(node)
+                self.left_border.append(node)
 
                 if i == 0:
-                    periodic_edge = self.mats_env[-1]['left']
+                    self.left_up_corner['down'] ^ node['up']
                 else:
-                    self.mats_env[-2]['right'] ^ self.mats_env[-1]['left']
+                    self.left_border[-2]['down'] ^ node['up']
 
-                if i == self._n_features - 1:
-                    self.mats_env[-1]['right'] ^ periodic_edge
+            # Right border
+            for i in range(self.n_rows - 2):
+                node = ParamNode(shape=(in_dim, bond_dim[0], bond_dim[1], bond_dim[1]),
+                                 axes_names=('input', 'left', 'up', 'down'),
+                                 name=f'right_border_node_({i})',
+                                 network=self)
+                self.right_border.append(node)
 
-    def initialize(self, std: float = 1e-9) -> None:
-        """
-        Initializes all the nodes as explained `here <https://arxiv.org/abs/1605.03795>`_.
-        It can be overriden for custom initializations.
-        """
-        # Left node
-        if self.left_node is not None:
-            tensor = torch.randn(self.left_node.shape) * std
-            aux = torch.zeros(tensor.shape[1]) * std
-            aux[0] = 1.
-            tensor[0, :] = aux
-            self.left_node.tensor = tensor
-
-        # Right node
-        if self.right_node is not None:
-            tensor = torch.randn(self.right_node.shape) * std
-            aux = torch.zeros(tensor.shape[0]) * std
-            aux[0] = 1.
-            tensor[:, 0] = aux
-            self.right_node.tensor = tensor
-
-        # Mats env
-        for node in self.mats_env:
-            tensor = torch.randn(node.shape) * std
-            aux = torch.eye(tensor.shape[0], tensor.shape[2])
-            tensor[:, 0, :] = aux
-            node.tensor = tensor
+                if i == 0:
+                    self.right_up_corner['down'] ^ node['up']
+                else:
+                    self.right_border[-2]['down'] ^ node['up']
 
-    def set_data_nodes(self) -> None:
-        """
-        Creates ``data`` nodes and connects each of them to the input/physical
-        edge of each input node.
-        """
-        input_edges = []
-        if self.left_node is not None:
-            input_edges.append(self.left_node['input'])
-        input_edges += list(map(lambda node: node['input'], self.mats_env))
-        if self.right_node is not None:
-            input_edges.append(self.right_node['input'])
+            # Left down corner
+            node = ParamNode(shape=(in_dim, bond_dim[0], bond_dim[1]),
+                             axes_names=('input', 'right', 'up'),
+                             name=f'left_down_corner_node',
+                             network=self)
+            self.left_down_corner = node
 
-        super().set_data_nodes(input_edges=input_edges,
-                               num_batch_edges=self.n_batches)
+            if self.n_rows > 2:
+                self.left_border[-1]['down'] ^ node['up']
+            else:
+                self.left_up_corner['down'] ^ node['up']
 
-        if self.mats_env:
-            self.mats_env_data = list(map(lambda node: node.neighbours('input'),
-                                          self.mats_env))
-
-    def _input_contraction(self,
-                           inline_input: bool = False) -> Tuple[
-        Optional[List[Node]],
-        Optional[List[Node]]]:
-        """Contracts input data nodes with MPS nodes."""
-        if inline_input:
-            mats_result = list(map(lambda node: node @ node.neighbours('input'),
-                                   self.mats_env))
-            
-            return mats_result
+            # Down border
+            for j in range(self.n_cols - 2):
+                node = ParamNode(shape=(in_dim, bond_dim[0], bond_dim[0], bond_dim[1]),
+                                 axes_names=('input', 'left', 'right', 'up'),
+                                 name=f'down_border_node_({j})',
+                                 network=self)
+                self.down_border.append(node)
 
-        else:
-            if self.mats_env:
-                stack = op.stack(self.mats_env)
-                stack_data = op.stack(self.mats_env_data)
-
-                stack['input'] ^ stack_data['feature']
-
-                result = stack_data @ stack
-                mats_result = op.unbind(result)
-                return mats_result
+                if j == 0:
+                    self.left_down_corner['right'] ^ node['left']
+                else:
+                    self.down_border[-2]['right'] ^ node['left']
+
+            # Right down corner
+            node = ParamNode(shape=(in_dim, bond_dim[0], bond_dim[1]),
+                             axes_names=('input', 'left', 'up'),
+                             name=f'right_down_corner_node',
+                             network=self)
+            self.right_down_corner = node
+
+            if self.n_rows > 2:
+                self.right_border[-1]['down'] ^ node['up']
             else:
-                return []
+                self.right_up_corner['down'] ^ node['up']
 
-    @staticmethod
-    def _inline_contraction(nodes: List[Node]) -> Node:
-        """Contracts sequence of MPS nodes (matrices) inline."""
-        result_node = nodes[0]
-        for node in nodes[1:]:
-            result_node @= node
-        return result_node
-
-    def _contract_envs_inline(self, mats_env: List[Node]) -> Node:
-        """Contracts the left and right environments inline."""
-        if self.boundary == 'obc':
-            left_node = self.left_node @ self.left_node.neighbours('input')
-            right_node = self.right_node @ self.right_node.neighbours('input')
-            contract_lst = [left_node] + mats_env + [right_node]
-        elif len(mats_env) > 1:
-            contract_lst = mats_env
-        else:
-            return mats_env[0] @ mats_env[0]
+            if self.n_cols > 2:
+                self.down_border[-1]['right'] ^ node['left']
+            else:
+                self.left_down_corner['right'] ^ node['left']
 
-        return self._inline_contraction(contract_lst)
+            # Grid env
+            for i in range(self.n_rows - 2):
+                self.grid_env.append([])
+                for j in range(self.n_cols - 2):
+                    node = ParamNode(shape=(in_dim, bond_dim[0], bond_dim[0],
+                                            bond_dim[1], bond_dim[1]),
+                                     axes_names=('input', 'left', 'right',
+                                                 'up', 'down'),
+                                     name=f'grid_env_node_({i},{j})',
+                                     network=self)
+                    self.grid_env[-1].append(node)
 
-    def _aux_pairwise(self, nodes: List[Node]) -> Tuple[List[Node],
-    List[Node]]:
-        """Contracts a sequence of MPS nodes (matrices) pairwise."""
-        length = len(nodes)
-        aux_nodes = nodes
-        if length > 1:
-            half_length = length // 2
-            nice_length = 2 * half_length
-
-            even_nodes = aux_nodes[0:nice_length:2]
-            odd_nodes = aux_nodes[1:nice_length:2]
-            leftover = aux_nodes[nice_length:]
-
-            stack1 = op.stack(even_nodes)
-            stack2 = op.stack(odd_nodes)
-
-            stack1['right'] ^ stack2['left']
-
-            aux_nodes = stack1 @ stack2
-            aux_nodes = op.unbind(aux_nodes)
-
-            return aux_nodes, leftover
-        return nodes, []
-
-    def _pairwise_contraction(self, mats_nodes: List[Node]) -> Node:
-        """Contracts the left and right environments pairwise."""
-        length = len(mats_nodes)
-        aux_nodes = mats_nodes
-        if length > 1:
-            leftovers = []
-            while length > 1:
-                aux1, aux2 = self._aux_pairwise(aux_nodes)
-                aux_nodes = aux1
-                leftovers = aux2 + leftovers
-                length = len(aux1)
+                    if i == 0:
+                        self.up_border[j]['down'] ^ node['up']
+                    else:
+                        self.grid_env[i - 1][j]['down'] ^ node['up']
+                    if i == self.n_rows - 3:
+                        node['down'] ^ self.down_border[j]['up']
+
+                    if j == 0:
+                        self.left_border[i]['right'] ^ node['left']
+                    else:
+                        self.grid_env[i][j - 1]['right'] ^ node['left']
+                    if j == self.n_cols - 3:
+                        node['right'] ^ self.right_border[i]['left']
+
+        elif self.boundary == ['obc', 'pbc']:
+            # Up border
+            for j in range(self.n_cols):
+                node = ParamNode(shape=(in_dim, bond_dim[0], bond_dim[0], bond_dim[1]),
+                                 axes_names=('input', 'left', 'right', 'down'),
+                                 name=f'up_border_node_({j})',
+                                 network=self)
+                self.up_border.append(node)
 
-            aux_nodes = aux_nodes + leftovers
-            return self._pairwise_contraction(aux_nodes)
+                if j > 0:
+                    self.up_border[-2]['right'] ^ node['left']
+                if j == self.n_cols - 1:
+                    node['right'] ^ self.up_border[0]['left']
+
+            # Down border
+            for j in range(self.n_cols):
+                node = ParamNode(shape=(in_dim, bond_dim[0], bond_dim[0], bond_dim[1]),
+                                 axes_names=('input', 'left', 'right', 'up'),
+                                 name=f'down_border_node_({j})',
+                                 network=self)
+                self.down_border.append(node)
 
-        return self._contract_envs_inline(aux_nodes)
+                if j > 0:
+                    self.down_border[-2]['right'] ^ node['left']
+                if j == self.n_cols - 1:
+                    node['right'] ^ self.down_border[0]['left']
+                if self.n_rows == 2:
+                    self.up_border[j]['down'] ^ node['up']
+
+            # Grid env
+            for i in range(self.n_rows - 2):
+                self.grid_env.append([])
+                for j in range(self.n_cols):
+                    node = ParamNode(shape=(in_dim, bond_dim[0], bond_dim[0],
+                                            bond_dim[1], bond_dim[1]),
+                                     axes_names=('input', 'left', 'right',
+                                                 'up', 'down'),
+                                     name=f'grid_env_node_({i},{j})',
+                                     network=self)
+                    self.grid_env[-1].append(node)
 
-    def contract(self,
-                 inline_input: bool = False,
-                 inline_mats: bool = False) -> Node:
-        """
-        Contracts the whole MPS.
-        
-        Parameters
-        ----------
-        inline_input : bool
-            Boolean indicating whether input ``data`` nodes should be contracted
-            with the ``MPS`` nodes inline (one contraction at a time) or in a
-            single stacked contraction.
-        inline_mats : bool
-            Boolean indicating whether the sequence of matrices (resultant
-            after contracting the input ``data`` nodes) should be contracted
-            inline or as a sequence of pairwise stacked contrations.
+                    if i == 0:
+                        self.up_border[j]['down'] ^ node['up']
+                    else:
+                        self.grid_env[i - 1][j]['down'] ^ node['up']
+                    if i == self.n_rows - 3:
+                        node['down'] ^ self.down_border[j]['up']
+
+                    if j > 0:
+                        self.grid_env[i][j - 1]['right'] ^ node['left']
+                    if j == self.n_cols - 1:
+                        node['right'] ^ self.grid_env[i][0]['left']
+
+        elif self.boundary == ['pbc', 'obc']:
+            # Left border
+            for i in range(self.n_rows):
+                node = ParamNode(shape=(in_dim, bond_dim[0], bond_dim[1], bond_dim[1]),
+                                 axes_names=('input', 'right', 'up', 'down'),
+                                 name=f'left_border_node_({i})',
+                                 network=self)
+                self.left_border.append(node)
 
-        Returns
-        -------
-        Node
-        """
-        mats_env = self._input_contraction(inline_input)
+                if i > 0:
+                    self.left_border[-2]['down'] ^ node['up']
+                if i == self.n_rows - 1:
+                    node['down'] ^ self.left_border[0]['up']
+
+            # Right border
+            for i in range(self.n_rows):
+                node = ParamNode(shape=(in_dim, bond_dim[0], bond_dim[1], bond_dim[1]),
+                                 axes_names=('input', 'left', 'up', 'down'),
+                                 name=f'right_border_node_({i})',
+                                 network=self)
+                self.right_border.append(node)
+
+                if i > 0:
+                    self.right_border[-2]['down'] ^ node['up']
+                if i == self.n_rows - 1:
+                    node['down'] ^ self.right_border[0]['up']
+                if self.n_cols == 2:
+                    self.left_border[i]['right'] ^ node['left']
+
+            # Grid env
+            for i in range(self.n_rows):
+                self.grid_env.append([])
+                for j in range(self.n_cols - 2):
+                    node = ParamNode(shape=(in_dim, bond_dim[0], bond_dim[0],
+                                            bond_dim[1], bond_dim[1]),
+                                     axes_names=('input', 'left', 'right',
+                                                 'up', 'down'),
+                                     name=f'grid_env_node_({i},{j})',
+                                     network=self)
+                    self.grid_env[-1].append(node)
+
+                    if i > 0:
+                        self.grid_env[i - 1][j]['down'] ^ node['up']
+                    if i == self.n_rows - 1:
+                        node['down'] ^ self.grid_env[0][j]['up']
+
+                    if j == 0:
+                        self.left_border[i]['right'] ^ node['left']
+                    else:
+                        self.grid_env[i][j - 1]['right'] ^ node['left']
+                    if j == self.n_cols - 3:
+                        node['right'] ^ self.right_border[i]['left']
 
-        if inline_mats:
-            result = self._contract_envs_inline(mats_env)
         else:
-            result = self._pairwise_contraction(mats_env)
+            # Grid env
+            for i in range(self.n_rows):
+                self.grid_env.append([])
+                for j in range(self.n_cols):
+                    node = ParamNode(shape=(in_dim, bond_dim[0], bond_dim[0],
+                                            bond_dim[1], bond_dim[1]),
+                                     axes_names=('input', 'left', 'right',
+                                                 'up', 'down'),
+                                     name=f'grid_env_node_({i},{j})',
+                                     network=self)
+                    self.grid_env[-1].append(node)
 
-        return result
+                    if i > 0:
+                        self.grid_env[i - 1][j]['down'] ^ node['up']
+                    if i == self.n_rows - 1:
+                        node['down'] ^ self.grid_env[0][j]['up']
+
+                    if j > 0:
+                        self.grid_env[i][j - 1]['right'] ^ node['left']
+                    if j == self.n_cols - 1:
+                        node['right'] ^ self.grid_env[i][0]['left']
 
-    def canonicalize(self,
-                     oc: Optional[int] = None,
-                     mode: Text = 'svd',
-                     rank: Optional[int] = None,
-                     cum_percentage: Optional[float] = None,
-                     cutoff: Optional[float] = None) -> None:
-        r"""
-        Turns MPS into canonical form via local SVD/QR decompositions.
-        
-        Parameters
-        ----------
-        oc : int
-            Position of the orthogonality center. It should be between 0 and 
-            ``n_features -1``.
-        mode : {"svd", "svdr", "qr"}
-            Indicates which decomposition should be used to split a node after
-            contracting it. See more at :func:`svd_`, :func:`svdr_`, :func:`qr_`.
-            If mode is "qr", operation :func:`qr_` will be performed on nodes at
-            the left of the output node, whilst operation :func:`rq_` will be
-            used for nodes at the right.
-        rank : int, optional
-            Number of singular values to keep.
-        cum_percentage : float, optional
-            Proportion that should be satisfied between the sum of all singular
-            values kept and the total sum of all singular values.
-            
-            .. math::
-            
-                \frac{\sum_{i \in \{kept\}}{s_i}}{\sum_{i \in \{all\}}{s_i}} \ge
-                cum\_percentage
-        cutoff : float, optional
-            Quantity that lower bounds singular values in order to be kept.
+    def initialize(self, std: float = 1e-9) -> None:
+        """Initializes all the nodes."""
+        for node in self.leaf_nodes.values():
+            node.tensor = torch.randn(node.shape) * std
+
+    def set_data_nodes(self) -> None:
+        """
+        Creates data nodes and connects each of them to the physical edge of
+        an input node.
+        """
+        input_edges = []
+
+        for i in range(self.n_rows):
+            for j in range(self.n_cols):
+                if self.boundary == ['obc', 'obc']:
+                    if i == 0:
+                        if j == 0:
+                            node = self.left_up_corner
+                        elif j < self.n_cols - 1:
+                            node = self.up_border[j - 1]
+                        else:
+                            node = self.right_up_corner
+                    elif i < self.n_rows - 1:
+                        if j == 0:
+                            node = self.left_border[i - 1]
+                        elif j < self.n_cols - 1:
+                            node = self.grid_env[i - 1][j - 1]
+                        else:
+                            node = self.right_border[i - 1]
+                    else:
+                        if j == 0:
+                            node = self.left_down_corner
+                        elif j < self.n_cols - 1:
+                            node = self.down_border[j - 1]
+                        else:
+                            node = self.right_down_corner
+                elif self.boundary == ['obc', 'pbc']:
+                    if i == 0:
+                        node = self.up_border[j]
+                    elif i < self.n_rows - 1:
+                        node = self.grid_env[i - 1][j]
+                    else:
+                        node = self.down_border[j]
+                elif self.boundary == ['pbc', 'obc']:
+                    if j == 0:
+                        node = self.left_border[i]
+                    elif j < self.n_cols - 1:
+                        node = self.grid_env[i][j - 1]
+                    else:
+                        node = self.right_border[i]
+                else:
+                    node = self.grid_env[i][j]
+
+                input_edges.append(node['input'])
+
+        super().set_data_nodes(input_edges=input_edges,
+                               num_batch_edges=self.n_batches)
+
+    def _input_contraction(self):
+        """Contracts input data nodes with PEPS nodes."""
+        full_grid = []
+        for _ in range(self.n_rows):
+            full_grid.append([])
+            for _ in range(self.n_cols):
+                full_grid[-1].append(None)
+
+        # Contract with data
+        if self.boundary == ['obc', 'obc']:
+            # Corners
+            full_grid[0][0] = self.left_up_corner.neighbours('input') @ \
+                self.left_up_corner
+            full_grid[0][-1] = self.right_up_corner.neighbours('input') @ \
+                self.right_up_corner
+            full_grid[-1][0] = self.left_down_corner.neighbours('input') @ \
+                self.left_down_corner
+            full_grid[-1][-1] = self.right_down_corner.neighbours('input') @ \
+                self.right_down_corner
             
-        Examples
-        --------
-        >>> mps = tk.models.MPS(n_features=4,
-        ...                     in_dim=2,
-        ...                     bond_dim=5)
-        >>> mps.canonicalize(rank=3)
-        >>> mps.bond_dim
-        [2, 3, 2]
-        """
-        self.reset()
-
-        prev_auto_stack = self._auto_stack
-        self.auto_stack = False
-
-        if oc is None:
-            oc = self._n_features - 1
-        elif oc >= self._n_features:
-            raise ValueError(f'Orthogonality center position `oc` should be '
-                             f'between 0 and {self._n_features - 1}')
-
-        nodes = self.mats_env
-        if self.boundary == 'obc':
-            nodes = [self.left_node] + nodes + [self.right_node]
-
-        for i in range(oc):
-            if mode == 'svd':
-                result1, result2 = nodes[i]['right'].svd_(
-                    side='right',
-                    rank=rank,
-                    cum_percentage=cum_percentage,
-                    cutoff=cutoff)
-            elif mode == 'svdr':
-                result1, result2 = nodes[i]['right'].svdr_(
-                    side='right',
-                    rank=rank,
-                    cum_percentage=cum_percentage,
-                    cutoff=cutoff)
-            elif mode == 'qr':
-                result1, result2 = nodes[i]['right'].qr_()
+        if self.up_border:
+            # Up border
+            stack_up_border = op.stack(self.up_border)
+            stack_up_border_data = op.stack(
+                list(map(lambda x: x.neighbours('input'),
+                         self.up_border)))
+            stack_up_border_data['feature'] ^ stack_up_border['input']
+            result_up_border = stack_up_border_data @ stack_up_border
+            result_up_border = op.unbind(result_up_border)
+
+            # Down border
+            stack_down_border = op.stack(self.down_border)
+            stack_down_border_data = op.stack(
+                list(map(lambda x: x.neighbours('input'),
+                         self.down_border)))
+            stack_down_border_data['feature'] ^ stack_down_border['input']
+            result_down_border = stack_down_border_data @ stack_down_border
+            result_down_border = op.unbind(result_down_border)
+
+            if self.boundary[1] == 'obc':
+                full_grid[0][1:-1] = result_up_border
+                full_grid[-1][1:-1] = result_down_border
             else:
-                raise ValueError('`mode` can only be "svd", "svdr" or "qr"')
+                full_grid[0] = result_up_border
+                full_grid[-1] = result_down_border
 
-            result1 = result1.parameterize()
-            nodes[i] = result1
-            nodes[i + 1] = result2
-
-        for i in range(len(nodes) - 1, oc, -1):
-            if mode == 'svd':
-                result1, result2 = nodes[i]['left'].svd_(
-                    side='left',
-                    rank=rank,
-                    cum_percentage=cum_percentage,
-                    cutoff=cutoff)
-            elif mode == 'svdr':
-                result1, result2 = nodes[i]['left'].svdr_(
-                    side='left',
-                    rank=rank,
-                    cum_percentage=cum_percentage,
-                    cutoff=cutoff)
-            elif mode == 'qr':
-                result1, result2 = nodes[i]['left'].rq_()
+        if self.left_border:
+            # Left border
+            stack_left_border = op.stack(self.left_border)
+            stack_left_border_data = op.stack(
+                list(map(lambda x: x.neighbours('input'),
+                         self.left_border)))
+            stack_left_border_data['feature'] ^ stack_left_border['input']
+            result_left_border = stack_left_border_data @ stack_left_border
+            result_left_border = op.unbind(result_left_border)
+
+            # Right border
+            stack_right_border = op.stack(self.right_border)
+            stack_right_border_data = op.stack(
+                list(map(lambda x: x.neighbours('input'),
+                         self.right_border)))
+            stack_right_border_data['feature'] ^ stack_right_border['input']
+            result_right_border = stack_right_border_data @ stack_right_border
+            result_right_border = op.unbind(result_right_border)
+
+            if self.boundary[0] == 'obc':
+                for i in range(self.n_rows - 2):
+                    full_grid[i + 1][0] = result_left_border[i]
+                    full_grid[i + 1][-1] = result_right_border[i]
+            else:
+                for i in range(self.n_rows):
+                    full_grid[i][0] = result_left_border[i]
+                    full_grid[i][-1] = result_right_border[i]
+
+        # Grid env
+        list_grid_env = []
+        for lst in self.grid_env:
+            list_grid_env += lst
+
+        if list_grid_env:
+            stack_grid_env = op.stack(list_grid_env)
+            stack_grid_env_data = op.stack(
+                list(map(lambda x: x.neighbours('input'),
+                         list_grid_env)))
+            stack_grid_env_data['feature'] ^ stack_grid_env['input']
+            result_grid_env = stack_grid_env_data @ stack_grid_env
+            result_grid_env = op.unbind(result_grid_env)
+
+            if self.boundary == ['obc', 'obc']:
+                for i in range(self.n_rows - 2):
+                    for j in range(self.n_cols - 2):
+                        full_grid[i + 1][j + 1] = result_grid_env[
+                            i * (self.n_cols - 2) + j]
+            elif self.boundary == ['obc', 'pbc']:
+                for i in range(self.n_rows - 2):
+                    for j in range(self.n_cols):
+                        full_grid[i + 1][j] = result_grid_env[
+                            i * self.n_cols + j]
+            elif self.boundary == ['pbc', 'obc']:
+                for i in range(self.n_rows):
+                    for j in range(self.n_cols - 2):
+                        full_grid[i][j + 1] = result_grid_env[
+                            i * (self.n_cols - 2) + j]
             else:
-                raise ValueError('`mode` can only be "svd", "svdr" or "qr"')
+                for i in range(self.n_rows):
+                    for j in range(self.n_cols):
+                        full_grid[i][j] = result_grid_env[
+                            i * self.n_cols + j]
+
+        return full_grid
+
+    def _contract_2_lines(self,
+                          line1: List[Node],
+                          line2: List[Node],
+                          from_side: Text = 'up',
+                          inline: bool = False) -> List[Node]:
+        """Contracts two consecutive lines (rows or columns) of the PEPS."""
+        result_list = []
+
+        if inline:
+            for (node1, node2) in zip(line1, line2):
+                result_list.append(node1 @ node2)
 
-            result2 = result2.parameterize()
-            nodes[i] = result2
-            nodes[i - 1] = result1
-
-        nodes[oc] = nodes[oc].parameterize()
-
-        if self.boundary == 'obc':
-            self.left_node = nodes[0]
-            self.mats_env = nodes[1:-1]
-            self.right_node = nodes[-1]
         else:
-            self.mats_env = nodes
+            condition = False
+            if from_side in ['up', 'down']:
+                if self.boundary[1] == 'obc':
+                    condition = True
+            elif from_side in ['left', 'right']:
+                if self.boundary[0] == 'obc':
+                    condition = True
+
+            if condition:
+                result_list.append(line1[0] @ line2[0])
+
+                if len(line1) > 2:
+                    stack1 = op.stack(line1[1:-1])
+                    stack2 = op.stack(line2[1:-1])
+
+                    node1 = line1[1]
+                    node2 = line2[1]
+                    axes1, axes2 = [], []
+                    for i1, edge1 in enumerate(node1.edges):
+                        for edge2 in node2.edges:
+                            if edge1 == edge2:
+                                axis1 = edge1.axes[1 - node1.is_node1(i1)]
+                                axis2 = edge1.axes[node1.is_node1(i1)]
+                                axes1.append(axis1)
+                                axes2.append(axis2)
 
-        bond_dim = []
-        for node in nodes:
-            if 'right' in node.axes_names:
-                bond_dim.append(node['right'].size())
-        self._bond_dim = bond_dim
-
-        self.auto_stack = prev_auto_stack
-
-    def _project_to_bond_dim(self,
-                             nodes: List[AbstractNode],
-                             bond_dim: int,
-                             side: Text = 'right'):
-        """Projects all nodes into a space of dimension ``bond_dim``."""
-        device = nodes[0].tensor.device
-
-        if side == 'left':
-            nodes.reverse()
-        elif side != 'right':
-            raise ValueError('`side` can only be \'left\' or \'right\'')
-
-        for node in nodes:
-            if not node['input'].is_dangling():
-                self.delete_node(node.neighbours('input'))
-
-        line_mat_nodes = []
-        in_dim_lst = []
-        proj_mat_node = None
-        for j in range(len(nodes)):
-            in_dim_lst.append(nodes[j]['input'].size())
-            if bond_dim <= torch.tensor(in_dim_lst).prod().item():
-                proj_mat_node = Node(shape=(*in_dim_lst, bond_dim),
-                                     axes_names=(*(['input'] * len(in_dim_lst)),
-                                                 'bond_dim'),
-                                     name=f'proj_mat_node_{side}',
-                                     network=self)
+                    for axis1, axis2 in zip(axes1, axes2):
+                        stack1[axis1.name] ^ stack2[axis2.name]
 
-                proj_mat_node.tensor = torch.eye(
-                    torch.tensor(in_dim_lst).prod().int().item(),
-                    bond_dim).view(*in_dim_lst, -1).to(device)
-                for k in range(j + 1):
-                    nodes[k]['input'] ^ proj_mat_node[k]
-
-                aux_result = proj_mat_node
-                for k in range(j + 1):
-                    aux_result @= nodes[k]
-                line_mat_nodes.append(aux_result)  # bond_dim x left x right
-                break
+                    stack_result = stack1 @ stack2
+                    result_list += op.unbind(stack_result)
 
-        if proj_mat_node is None:
-            bond_dim = torch.tensor(in_dim_lst).prod().int().item()
-            proj_mat_node = Node(shape=(*in_dim_lst, bond_dim),
-                                 axes_names=(*(['input'] * len(in_dim_lst)),
-                                             'bond_dim'),
-                                 name=f'proj_mat_node_{side}',
-                                 network=self)
-
-            proj_mat_node.tensor = torch.eye(
-                torch.tensor(in_dim_lst).prod().int().item(),
-                bond_dim).view(*in_dim_lst, -1).to(device)
-            for k in range(j + 1):
-                nodes[k]['input'] ^ proj_mat_node[k]
-
-            aux_result = proj_mat_node
-            for k in range(j + 1):
-                aux_result @= nodes[k]
-            line_mat_nodes.append(aux_result)
-
-        k = j + 1
-        while k < len(nodes):
-            in_dim = nodes[k]['input'].size()
-            proj_vec_node = Node(shape=(in_dim,),
-                                 axes_names=('input',),
-                                 name=f'proj_vec_node_{side}_({k})',
-                                 network=self)
-
-            proj_vec_node.tensor = torch.eye(in_dim, 1).squeeze().to(device)
-            nodes[k]['input'] ^ proj_vec_node['input']
-            line_mat_nodes.append(proj_vec_node @ nodes[k])
-
-            k += 1
-
-        line_mat_nodes.reverse()
-        result = line_mat_nodes[0]
-        for node in line_mat_nodes[1:]:
-            result @= node
+                result_list.append(line1[-1] @ line2[-1])
 
-        return result  # bond_dim x left/right
+            else:
+                stack1 = op.stack(line1)
+                stack2 = op.stack(line2)
 
-    def _aux_canonicalize_univocal(self,
-                                   nodes: List[AbstractNode],
-                                   idx: int,
-                                   left_nodeL: AbstractNode):
-        """Returns canonicalize version of the tensor at site ``idx``."""
-        L = nodes[idx]  # left x input x right
-        left_nodeC = None
-
-        if idx > 0:
-            # bond_dim[-1] x input  x right  /  bond_dim[-1] x input
-            L = left_nodeL @ L
-
-        L = L.tensor
-
-        if idx < self._n_features - 1:
-            bond_dim = self._bond_dim[idx]
-
-            prod_phys_left = 1
-            for i in range(idx + 1):
-                prod_phys_left *= self.in_dim[i]
-            bond_dim = min(bond_dim, prod_phys_left)
-
-            prod_phys_right = 1
-            for i in range(idx + 1, self._n_features):
-                prod_phys_right *= self.in_dim[i]
-            bond_dim = min(bond_dim, prod_phys_right)
-
-            if bond_dim < self._bond_dim[idx]:
-                self._bond_dim[idx] = bond_dim
-
-            left_nodeC = self._project_to_bond_dim(nodes=nodes[:idx + 1],
-                                                   bond_dim=bond_dim,
-                                                   side='left')  # bond_dim x right
-            right_node = self._project_to_bond_dim(nodes=nodes[idx + 1:],
-                                                   bond_dim=bond_dim,
-                                                   side='right')  # bond_dim x left
-
-            C = left_nodeC @ right_node  # bond_dim x bond_dim
-            C = torch.linalg.inv(C.tensor)
-
-            if idx == 0:
-                L @= right_node.tensor.t()  # input x bond_dim
-                L @= C
+                node1 = line1[0]
+                node2 = line2[0]
+                axes1, axes2 = [], []
+                for i1, edge1 in enumerate(node1.edges):
+                    for edge2 in node2.edges:
+                        if edge1 == edge2:
+                            axis1 = edge1.axes[1 - node1.is_node1(i1)]
+                            axis2 = edge1.axes[node1.is_node1(i1)]
+                            axes1.append(axis1)
+                            axes2.append(axis2)
+
+                for axis1, axis2 in zip(axes1, axes2):
+                    stack1[axis1.name] ^ stack2[axis2.name]
+
+                stack_result = stack1 @ stack2
+                result_list = op.unbind(stack_result)
+
+        return result_list
+
+    def _split_line(self,
+                    line: List[Node],
+                    pbc: bool = False,
+                    from_side: Text = 'up',
+                    max_bond: int = 32) -> List[Node]:
+        """
+        After two lines have been contracted, contracts each node with its
+        neighbours and splits the result again, to reduce the bond dimension
+        (keeping it bounded by ``max_bond``).
+        """
+        nb = self.n_batches
+        for i in range(len(line) - 1):
+            contracted = line[i] @ line[i + 1]
+            split1, split2 = contracted.split(
+                node1_axes=contracted.axes[nb:(line[i].rank - 2)],
+                node2_axes=contracted.axes[(line[i].rank - 2):],
+                rank=max_bond)
+            if (from_side == 'up') or (from_side == 'down'):
+                split1.get_axis('split').name = 'right'
+                split2.get_axis('split').name = 'left'
+            else:
+                split1.get_axis('split').name = 'down'
+                split2.get_axis('split').name = 'up'
+            line[i] = split1
+            line[i + 1] = split2
+
+        if pbc and (len(line) > 2):
+            contracted = line[-1] @ line[0]
+            split1, split2 = contracted.split(
+                node1_axes=contracted.axes[nb:(line[-1].rank - 2)],
+                node2_axes=contracted.axes[(line[-1].rank - 2):],
+                rank=max_bond)
+            if (from_side == 'up') or (from_side == 'down'):
+                split1.get_axis('split').name = 'right'
+                split2.get_axis('split').name = 'left'
             else:
-                shape_L = L.shape
-                # (bond_dim[-1] * input) x bond_dim
-                L = (L.view(-1, L.shape[-1]) @ right_node.tensor.t())
-                L @= C
-                L = L.view(*shape_L[:-1], right_node.shape[0])
+                split1.get_axis('split').name = 'down'
+                split2.get_axis('split').name = 'up'
+            line[-1] = split1
+            line[0] = split2
 
-        return L, left_nodeC
+        return line
 
-    def canonicalize_univocal(self):
-        """
-        Turns MPS into the univocal canonical form defined `here
-        <https://arxiv.org/abs/2202.12319>`_.
+    def contract(self,
+                 from_side: Text = 'up',
+                 max_bond: int = 32,
+                 inline: bool = False):
         """
-        if self._boundary != 'obc':
-            raise ValueError('`canonicalize_univocal` can only be used if '
-                             'boundary is `obc`')
-
-        self.reset()
-
-        prev_auto_stack = self._auto_stack
-        self.auto_stack = False
+        Contracts the whole PEPS.
+        
+        Parameters
+        ----------
+        from_side : {"up", "down", "left", "right"}
+            Indicates from which side of the 2D grid the contraction algorithm
+            should start.
+        max_bond : int
+            The maximum allowed bond dimension. If, when contracting consecutive
+            lines (rows or columns) of the PEPS this bond dimension is exceeded,
+            the bond dimension is reduced using singular value decomposition
+            (see :func:`split`).
+        inline : bool
+            Boolean indicating whether consecutive lines should be contracted
+            inline or in parallel (using a single stacked contraction).
 
-        nodes = [self.left_node] + self.mats_env + [self.right_node]
-        for node in nodes:
-            if not node['input'].is_dangling():
-                node['input'].disconnect()
+        Returns
+        -------
+        Node
+        """
+        full_grid = self._input_contraction()
 
-        new_tensors = []
-        left_nodeC = None
-        for i in range(self._n_features):
-            tensor, left_nodeC = self._aux_canonicalize_univocal(
-                nodes=nodes,
-                idx=i,
-                left_nodeL=left_nodeC)
-            new_tensors.append(tensor)
+        pbc = False
+        if from_side == 'up':
+            if self.boundary[1] == 'pbc':
+                pbc = True
+
+        elif from_side == 'down':
+            full_grid.reverse()
+
+            if self.boundary[1] == 'pbc':
+                pbc = True
+
+        elif from_side == 'left':
+            new_grid = []
+            for j in range(len(full_grid[0])):
+                row = []
+                for i in range(len(full_grid)):
+                    row.append(full_grid[i][j])
+                new_grid.append(row)
+            full_grid = new_grid
+
+            if self.boundary[0] == 'pbc':
+                pbc = True
+
+        elif from_side == 'right':
+            new_grid = []
+            for j in range(len(full_grid[0])):
+                row = []
+                for i in range(len(full_grid)):
+                    row.append(full_grid[i][j])
+                new_grid.append(row)
+            full_grid = new_grid
+            full_grid.reverse()
+
+            if self.boundary[0] == 'pbc':
+                pbc = True
+
+        for i in range(len(full_grid) - 1):
+            line1 = full_grid[i]
+            line2 = full_grid[i + 1]
+            contracted_line = self._contract_2_lines(line1, line2,
+                                                     from_side=from_side,
+                                                     inline=inline)
+            split_line = self._split_line(contracted_line,
+                                             pbc=pbc,
+                                             from_side=from_side,
+                                             max_bond=max_bond)
 
-        for i, (node, tensor) in enumerate(zip(nodes, new_tensors)):
-            if i < self._n_features - 1:
-                if self._bond_dim[i] < node['right'].size():
-                    node['right'].change_size(self._bond_dim[i])
-            node.tensor = tensor
+            full_grid[i + 1] = split_line
 
-            if not node['input'].is_dangling():
-                self.delete_node(node.neighbours('input'))
-        self.reset()
+        result = full_grid[-1][0]
+        for node in full_grid[-1][1:]:
+            result @= node
 
-        for node, data_node in zip(nodes, self._data_nodes.values()):
-            node['input'] ^ data_node['feature']
+        for edge in result.edges:
+            if not edge.is_batch():
+                result @= result
+                break
 
-        self.auto_stack = prev_auto_stack
+        return result
 
 
-class UMPS(TensorNetwork):
+class UPEPS(TensorNetwork):
     """
-    Class for Uniform (translationally invariant) Matrix Product States where
-    all nodes are input nodes. It is the uniform version of :class:`MPS`, that
-    is, all nodes share the same tensor. Thus this class cannot have different
-    input or bond dimensions for each node, and boundary conditions are
-    always periodic (``"pbc"``).
+    Class for Uniform (translationally invariant) Projected Entangled Pair
+    States, where all nodes are input nodes. It is the uniform version of
+    :class:`PEPS`, that is, all nodes share the same tensor. Thus boundary
+    conditions are always periodic.
     
-    A ``UMPS`` is formed by the following nodes:
-      
-    * ``mats_env``: Environment of `matrix` nodes that. These nodes have axes
-      ``("left", "input", "right")``.
+    A ``UPEPS`` is formed by the following nodes:
+    
+    * ``grid_env``: Grid environment of nodes with 5 edges, ("input", "left",
+      "right", "up", "down"). Is is a list of lists of nodes.
 
     Parameters
     ----------
-    n_features : int
-        Number of input nodes.
+    n_rows : int
+        Number of rows of the 2D grid.
+    n_cols : int
+        Number of columns of the 2D grid
     in_dim : int
         Input dimension. Equivalent to the physical dimension.
-    bond_dim : int
-        Bond dimension.
+    bond_dim : list[int] or tuple[int]
+        Bond dimensions for horizontal and vertical edges (in that order). Thus
+        it should also contain 2 elements
     n_batches : int
         Number of batch edges of input ``data`` nodes. Usually ``n_batches = 1``
         (where the batch edge is used for the data batched) but it could also
-        be ``n_batches = 2`` (one edge for data batched, other edge for image
+        be ``nu_batches = 2`` (one edge for data batched, other edge for image
         patches in convolutional layers).
         
     Examples
     --------
-    >>> mps = tk.models.UMPS(n_features=4,
-    ...                      in_dim=2,
-    ...                      bond_dim=5)
-    >>> for node in mps.mats_env:
+    >>> peps = tk.models.PEPS(n_rows=2,
+    ...                       n_cols=2,
+    ...                       in_dim=3,
+    ...                       bond_dim=[5, 5])
+    >>> for node in peps.grid_env:
     ...     assert node.tensor_address() == 'virtual_uniform'
     ...
-    >>> data = torch.ones(20, 4, 2) # batch_size x n_features x feature_size
-    >>> result = mps(data)
+    >>> data = torch.ones(20, 4, 3) # batch_size x n_features x feature_size
+    >>> result = peps(data)
     >>> result.shape
     torch.Size([20])
     """
 
     def __init__(self,
-                 n_features: int,
+                 n_rows: int,
+                 n_cols: int,
                  in_dim: int,
-                 bond_dim: int,
+                 bond_dim: Sequence[int],
                  n_batches: int = 1) -> None:
 
-        super().__init__(name='mps')
+        super().__init__(name='peps')
+
+        # boundary
+        if n_rows < 1:
+            raise ValueError('There has to be one row at least')
+        if n_cols < 1:
+            raise ValueError('There has to be one column at least')
 
-        # n_features
-        if n_features < 1:
-            raise ValueError('`n_features` cannot be lower than 1')
-        self._n_features = n_features
+        self._n_rows = n_rows
+        self._n_cols = n_cols
 
         # in_dim
-        if isinstance(in_dim, int):
-            self._in_dim = in_dim
-        else:
-            raise TypeError('`in_dim` should be int type')
+        if not isinstance(in_dim, int):
+            raise ValueError('`in_dim` should be int type')
+        self._in_dim = in_dim
 
         # bond_dim
-        if isinstance(bond_dim, int):
-            self._bond_dim = bond_dim
+        if isinstance(bond_dim, (list, tuple)):
+            if len(bond_dim) != 2:
+                raise ValueError('`bond_dim` should be a pair of ints')
+            self._bond_dim = list(bond_dim)
         else:
-            raise TypeError('`bond_dim` should be int type')
+            raise TypeError('`bond_dim` should be a pair of ints')
 
         # n_batches
         if not isinstance(n_batches, int):
             raise TypeError('`n_batches should be int type')
         self._n_batches = n_batches
 
         # Create Tensor Network
         self._make_nodes()
         self.initialize()
 
     @property
-    def n_features(self) -> int:
-        """Returns number of nodes."""
-        return self._n_features
+    def n_rows(self) -> int:
+        """Returns number of rows of the 2D grid."""
+        return self._n_rows
+
+    @property
+    def n_cols(self) -> int:
+        """Returns number of columns of the 2D grid."""
+        return self._n_cols
 
     @property
     def in_dim(self) -> int:
         """Returns input/physical dimension."""
         return self._in_dim
 
     @property
-    def bond_dim(self) -> int:
-        """Returns bond dimension."""
+    def bond_dim(self) -> List[int]:
+        """Returns bond dimensions for horizontal and vertical edges."""
         return self._bond_dim
 
     @property
     def n_batches(self) -> int:
         """Returns number of batch edges of the ``data`` nodes."""
         return self._n_batches
 
     def _make_nodes(self) -> None:
-        """Creates all the nodes of the MPS."""
+        """Creates all the nodes of the PEPS."""
         if self._leaf_nodes:
-            raise ValueError('Cannot create MPS nodes if the MPS already has '
-                             'nodes')
+            raise ValueError('Cannot create PEPS nodes if the PEPS already has'
+                             ' nodes')
 
-        self.left_node = None
-        self.right_node = None
-        self.mats_env = []
-
-        for i in range(self._n_features):
-            node = ParamNode(shape=(self.bond_dim, self.in_dim, self.bond_dim),
-                             axes_names=('left', 'input', 'right'),
-                             name=f'mats_env_node_({i})',
-                             network=self)
-            self.mats_env.append(node)
+        self.grid_env = []
 
-            if i == 0:
-                periodic_edge = self.mats_env[-1]['left']
-            else:
-                self.mats_env[-2]['right'] ^ self.mats_env[-1]['left']
+        in_dim = self.in_dim
+        bond_dim = self.bond_dim
 
-            if i == self._n_features - 1:
-                self.mats_env[-1]['right'] ^ periodic_edge
+        # Grid env
+        for i in range(self.n_rows):
+            self.grid_env.append([])
+            for j in range(self.n_cols):
+                node = ParamNode(shape=(in_dim, bond_dim[0], bond_dim[0],
+                                        bond_dim[1], bond_dim[1]),
+                                 axes_names=('input', 'left', 'right',
+                                             'up', 'down'),
+                                 name=f'grid_env_node_({i},{j})',
+                                 network=self)
+                self.grid_env[-1].append(node)
+
+                if i > 0:
+                    self.grid_env[i - 1][j]['down'] ^ node['up']
+                if i == self.n_rows - 1:
+                    node['down'] ^ self.grid_env[0][j]['up']
+
+                if j > 0:
+                    self.grid_env[i][j - 1]['right'] ^ node['left']
+                if j == self.n_cols - 1:
+                    node['right'] ^ self.grid_env[i][0]['left']
 
         # Virtual node
-        uniform_memory = ParamNode(shape=(self.bond_dim, self.in_dim, self.bond_dim),
-                                   axes_names=('left', 'input', 'right'),
-                                   name='virtual_uniform',
-                                   network=self,
-                                   virtual=True)
+        uniform_memory = node = ParamNode(shape=(in_dim, bond_dim[0], bond_dim[0],
+                                                 bond_dim[1], bond_dim[1]),
+                                          axes_names=('input', 'left', 'right',
+                                                      'up', 'down'),
+                                          name='virtual_uniform',
+                                          network=self,
+                                          virtual=True)
         self.uniform_memory = uniform_memory
 
     def initialize(self, std: float = 1e-9) -> None:
-        """
-        Initializes output and uniform nodes as explained `here
-        <https://arxiv.org/abs/1605.03795>`_.
-        It can be overriden for custom initializations.
-        """
+        """Initializes all the nodes."""
         # Virtual node
         tensor = torch.randn(self.uniform_memory.shape) * std
-        random_eye = torch.randn(tensor.shape[0], tensor.shape[2]) * std
-        random_eye = random_eye + torch.eye(tensor.shape[0], tensor.shape[2])
-        tensor[:, 0, :] = random_eye
-
         self.uniform_memory.tensor = tensor
 
-        for node in self.mats_env:
-            node.set_tensor_from(self.uniform_memory)
+        for lst in self.grid_env:
+            for node in lst:
+                node.set_tensor_from(self.uniform_memory)
 
     def set_data_nodes(self) -> None:
         """
-        Creates ``data`` nodes and connects each of them to the input/physical
-        edge of each input node.
+        Creates data nodes and connects each of them to the physical edge of
+        an input node.
         """
         input_edges = []
-        if self.left_node is not None:
-            input_edges.append(self.left_node['input'])
-        input_edges += list(map(lambda node: node['input'], self.mats_env))
-        if self.right_node is not None:
-            input_edges.append(self.right_node['input'])
+
+        for i in range(self.n_rows):
+            for j in range(self.n_cols):
+                input_edges.append(self.grid_env[i][j]['input'])
 
         super().set_data_nodes(input_edges=input_edges,
-                               num_batch_edges=self._n_batches)
+                               num_batch_edges=self.n_batches)
 
-        if self.mats_env:
-            self.mats_env_data = list(map(lambda node: node.neighbours('input'),
-                                          self.mats_env))
-
-    def _input_contraction(self,
-                           inline_input: bool = False) -> Tuple[
-        Optional[List[Node]],
-        Optional[List[Node]]]:
-        """Contracts input data nodes with MPS nodes."""
-        if inline_input:
-            mats_result = []
-            for node in self.mats_env:
-                mats_result.append(node @ node.neighbours('input'))
-            return mats_result
+    def _input_contraction(self):
+        """Contracts input data nodes with PEPS nodes."""
+        full_grid = []
+        for _ in range(self.n_rows):
+            full_grid.append([])
+            for _ in range(self.n_cols):
+                full_grid[-1].append(None)
+
+        # Grid env
+        list_grid_env = []
+        for lst in self.grid_env:
+            list_grid_env += lst
+
+        if list_grid_env:
+            stack_grid_env = op.stack(list_grid_env)
+            stack_grid_env_data = op.stack(
+                list(map(lambda x: x.neighbours('input'),
+                         list_grid_env)))
+            stack_grid_env_data['feature'] ^ stack_grid_env['input']
+            result_grid_env = stack_grid_env_data @ stack_grid_env
+            result_grid_env = op.unbind(result_grid_env)
+
+            for i in range(self.n_rows):
+                for j in range(self.n_cols):
+                    full_grid[i][j] = result_grid_env[i * self.n_cols + j]
+
+        return full_grid
+
+    def _contract_2_lines(self,
+                          line1: List[Node],
+                          line2: List[Node],
+                          inline: bool = False) -> List[Node]:
+        """Contracts two consecutive lines (rows or columns) of the PEPS."""
+        result_list = []
+
+        if inline:
+            for (node1, node2) in zip(line1, line2):
+                result_list.append(node1 @ node2)
 
         else:
-            if self.mats_env:
-                stack = op.stack(self.mats_env)
-                stack_data = op.stack(self.mats_env_data)
-
-                stack['input'] ^ stack_data['feature']
-
-                result = stack_data @ stack
-                mats_result = op.unbind(result)
-                return mats_result
-            else:
-                return []
+            stack1 = op.stack(line1)
+            stack2 = op.stack(line2)
 
-    @staticmethod
-    def _inline_contraction(nodes: List[Node]) -> Node:
-        """Contracts sequence of MPS nodes (matrices) inline."""
-        result_node = nodes[0]
-        for node in nodes[1:]:
-            result_node @= node
-        return result_node
-
-    def _contract_envs_inline(self, mats_env: List[Node]) -> Node:
-        """Contracts the left and right environments inline."""
-        if len(mats_env) > 1:
-            contract_lst = mats_env
-        else:
-            return mats_env[0] @ mats_env[0]
-
-        return self._inline_contraction(contract_lst)
-
-    def _aux_pairwise(self, nodes: List[Node]) -> Tuple[List[Node],
-    List[Node]]:
-        """Contracts a sequence of MPS nodes (matrices) pairwise."""
-        length = len(nodes)
-        aux_nodes = nodes
-        if length > 1:
-            half_length = length // 2
-            nice_length = 2 * half_length
-
-            even_nodes = aux_nodes[0:nice_length:2]
-            odd_nodes = aux_nodes[1:nice_length:2]
-            leftover = aux_nodes[nice_length:]
-
-            stack1 = op.stack(even_nodes)
-            stack2 = op.stack(odd_nodes)
-
-            stack1['right'] ^ stack2['left']
-
-            aux_nodes = stack1 @ stack2
-            aux_nodes = op.unbind(aux_nodes)
-
-            return aux_nodes, leftover
-        return nodes, []
-
-    def _pairwise_contraction(self, mats_nodes: List[Node]) -> Node:
-        """Contracts the left and right environments pairwise."""
-        length = len(mats_nodes)
-        aux_nodes = mats_nodes
-        if length > 1:
-            leftovers = []
-            while length > 1:
-                aux1, aux2 = self._aux_pairwise(aux_nodes)
-                aux_nodes = aux1
-                leftovers = aux2 + leftovers
-                length = len(aux1)
-
-            aux_nodes = aux_nodes + leftovers
-            return self._pairwise_contraction(aux_nodes)
+            node1 = line1[0]
+            node2 = line2[0]
+            axes1, axes2 = [], []
+            for i1, edge1 in enumerate(node1.edges):
+                for edge2 in node2.edges:
+                    if edge1 == edge2:
+                        axis1 = edge1.axes[1 - node1.is_node1(i1)]
+                        axis2 = edge1.axes[node1.is_node1(i1)]
+                        axes1.append(axis1)
+                        axes2.append(axis2)
+
+            for axis1, axis2 in zip(axes1, axes2):
+                stack1[axis1.name] ^ stack2[axis2.name]
+
+            stack_result = stack1 @ stack2
+            result_list = op.unbind(stack_result)
+
+        return result_list
+
+    def _split_line(self,
+                    line: List[Node],
+                    from_side: Text = 'up',
+                    max_bond: int = 32) -> List[Node]:
+        """
+        After two lines have been contracted, contracts each node with its
+        neighbours and splits the result again, to reduce the bond dimension
+        (keeping it bounded by ``max_bond``).
+        """
+        nb = self.n_batches
+        for i in range(len(line) - 1):
+            contracted = line[i] @ line[i + 1]
+            split1, split2 = contracted.split(
+                node1_axes=contracted.axes[nb:(line[i].rank - 2)],
+                node2_axes=contracted.axes[(line[i].rank - 2):],
+                rank=max_bond)
+            if (from_side == 'up') or (from_side == 'down'):
+                split1.get_axis('split').name = 'right'
+                split2.get_axis('split').name = 'left'
+            else:
+                split1.get_axis('split').name = 'down'
+                split2.get_axis('split').name = 'up'
+            line[i] = split1
+            line[i + 1] = split2
+
+        if len(line) > 2:
+            contracted = line[-1] @ line[0]
+            split1, split2 = contracted.split(
+                node1_axes=contracted.axes[nb:(line[-1].rank - 2)],
+                node2_axes=contracted.axes[(line[-1].rank - 2):],
+                rank=max_bond)
+            if (from_side == 'up') or (from_side == 'down'):
+                split1.get_axis('split').name = 'right'
+                split2.get_axis('split').name = 'left'
+            else:
+                split1.get_axis('split').name = 'down'
+                split2.get_axis('split').name = 'up'
+            line[-1] = split1
+            line[0] = split2
 
-        return self._contract_envs_inline(aux_nodes)
+        return line
 
     def contract(self,
-                 inline_input: bool = False,
-                 inline_mats: bool = False) -> Node:
+                 from_side: Text = 'up',
+                 max_bond: int = 32,
+                 inline: bool = False):
         """
-        Contracts the whole MPS.
+        Contracts the whole PEPS.
         
         Parameters
         ----------
-        inline_input : bool
-            Boolean indicating whether input ``data`` nodes should be contracted
-            with the ``MPS`` nodes inline (one contraction at a time) or in a
-            single stacked contraction.
-        inline_mats : bool
-            Boolean indicating whether the sequence of matrices (resultant
-            after contracting the input ``data`` nodes) should be contracted
-            inline or as a sequence of pairwise stacked contrations.
+        from_side : {"up", "down", "left", "right"}
+            Indicates from which side of the 2D grid the contraction algorithm
+            should start.
+        max_bond : int
+            The maximum allowed bond dimension. If, when contracting consecutive
+            lines (rows or columns) of the PEPS this bond dimension is exceeded,
+            the bond dimension is reduced using singular value decomposition
+            (see :func:`split`).
+        inline : bool
+            Boolean indicating whether consecutive lines should be contracted
+            inline or in parallel (using a single stacked contraction).
 
         Returns
         -------
         Node
         """
-        mats_env = self._input_contraction(inline_input)
+        full_grid = self._input_contraction()
 
-        if inline_mats:
-            result = self._contract_envs_inline(mats_env)
-        else:
-            result = self._pairwise_contraction(mats_env)
+        if from_side == 'up':
+            pass
+
+        elif from_side == 'down':
+            full_grid.reverse()
+
+        elif from_side == 'left':
+            new_grid = []
+            for j in range(len(full_grid[0])):
+                row = []
+                for i in range(len(full_grid)):
+                    row.append(full_grid[i][j])
+                new_grid.append(row)
+            full_grid = new_grid
+
+        elif from_side == 'right':
+            new_grid = []
+            for j in range(len(full_grid[0])):
+                row = []
+                for i in range(len(full_grid)):
+                    row.append(full_grid[i][j])
+                new_grid.append(row)
+            full_grid = new_grid
+            full_grid.reverse()
+
+        for i in range(len(full_grid) - 1):
+            line1 = full_grid[i]
+            line2 = full_grid[i + 1]
+            contracted_line = self._contract_2_lines(line1, line2,
+                                                     inline=inline)
+            split_line = self._split_line(contracted_line,
+                                             from_side=from_side,
+                                             max_bond=max_bond)
+
+            full_grid[i + 1] = split_line
+
+        result = full_grid[-1][0]
+        for node in full_grid[-1][1:]:
+            result @= node
+
+        for edge in result.edges:
+            if not edge.is_batch():
+                result @= result
+                break
 
         return result
 
 
-class ConvMPS(MPS):
+class ConvPEPS(PEPS):
     """
-    Class for Matrix Product States, where all nodes are input nodes, and where
-    the input data is a batch of images. It is the convolutional version of
-    :class:`MPS`.
+    Class for Projected Entangled Pair States, where all nodes are input nodes,
+    and where the input data is a batch of images. It is the convolutional
+    version of :class:`PEPS`.
     
     Input data as well as initialization parameters are described in `torch.nn.Conv2d
     <https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html>`_.
 
     Parameters
     ----------
     in_channels : int
-        Input channels. Same as ``in_dim`` in :class:`MPS`.
-    bond_dim : int, list[int] or tuple[int]
-        Bond dimension(s). If given as a sequence, its length should be equal
-        to :math:`kernel\_size_0 \cdot kernel\_size_1` (if ``boundary = "pbc"``)
-        or :math:`kernel\_size_0 \cdot kernel\_size_1 - 1` (if
-        ``boundary = "obc"``). The i-th bond dimension is always the dimension
-        of the right edge of the i-th node.
+        Input channels. Same as ``in_dim`` in :class:`PEPS`.
+    bond_dim : list[int] or tuple[int]
+        Bond dimensions for horizontal and vertical edges (in that order). Thus
+        it should also contain 2 elements
     kernel_size : int, list[int] or tuple[int]
         Kernel size used in `torch.nn.Unfold
         <https://pytorch.org/docs/stable/generated/torch.nn.Unfold.html#torch.nn.Unfold>`_.
         If given as an ``int``, the actual kernel size will be
         ``(kernel_size, kernel_size)``.
     stride : int
         Stride used in `torch.nn.Unfold
@@ -1003,37 +1202,38 @@
         If given as an ``int``, the actual kernel size will be
         ``(kernel_size, kernel_size)``.
     dilation : int
         Dilation used in `torch.nn.Unfold
         <https://pytorch.org/docs/stable/generated/torch.nn.Unfold.html#torch.nn.Unfold>`_.
         If given as an ``int``, the actual kernel size will be
         ``(kernel_size, kernel_size)``.
-    boundary : {"obc", "pbc"}
-        String indicating whether periodic or open boundary conditions should
-        be used.
+    boundary : list[{"obc", "pbc"}]
+        List of strings indicating whether periodic or open boundary conditions
+        should be used in the horizontal (up and down) and vertical (left and
+        right) boundaries.
         
     Examples
     --------
-    >>> conv_mps = tk.models.ConvMPS(in_channels=2,
-    ...                              bond_dim=5,
-    ...                              kernel_size=2)
+    >>> conv_peps = tk.models.ConvPEPS(in_channels=2,
+    ...                                bond_dim=[5, 5],
+    ...                                kernel_size=2)
     >>> data = torch.ones(20, 2, 2, 2) # batch_size x in_channels x height x width
-    >>> result = conv_mps(data)
-    >>> print(result.shape)
+    >>> result = conv_peps(data)
+    >>> result.shape
     torch.Size([20, 1, 1])
     """
 
     def __init__(self,
                  in_channels: int,
-                 bond_dim: Union[int, Sequence[int]],
+                 bond_dim: Sequence[int],
                  kernel_size: Union[int, Sequence],
                  stride: int = 1,
                  padding: int = 0,
                  dilation: int = 1,
-                 boundary: Text = 'obc'):
+                 boundary: Sequence[Text] = ['obc', 'obc']) -> None:
 
         if isinstance(kernel_size, int):
             kernel_size = (kernel_size, kernel_size)
         elif not isinstance(kernel_size, Sequence):
             raise TypeError('`kernel_size` must be int or Sequence')
 
         if isinstance(stride, int):
@@ -1053,35 +1253,36 @@
 
         self._in_channels = in_channels
         self._kernel_size = kernel_size
         self._stride = stride
         self._padding = padding
         self._dilation = dilation
 
-        super().__init__(n_features=kernel_size[0] * kernel_size[1],
+        super().__init__(n_rows=kernel_size[0],
+                         n_cols=kernel_size[1],
                          in_dim=in_channels,
                          bond_dim=bond_dim,
                          boundary=boundary,
                          n_batches=2)
 
         self.unfold = nn.Unfold(kernel_size=kernel_size,
                                 stride=stride,
                                 padding=padding,
                                 dilation=dilation)
 
     @property
     def in_channels(self) -> int:
-        """Returns ``in_channels``. Same as ``in_dim`` in :class:`MPS`."""
+        """Returns ``in_channels``. Same as ``in_dim`` in :class:`PEPS`."""
         return self._in_channels
 
     @property
     def kernel_size(self) -> Tuple[int, int]:
         """
-        Returns ``kernel_size``. Number of nodes is given by
-        :math:`kernel\_size_0 \cdot kernel\_size_1`.
+        Returns ``kernel_size``. Number of rows and columns in the 2D grid is
+        given by :math:`kernel\_size_0` and :math:`kernel\_size_1`, respectively.
         """
         return self._kernel_size
 
     @property
     def stride(self) -> Tuple[int, int]:
         """
         Returns stride used in `torch.nn.Unfold
@@ -1101,67 +1302,44 @@
     def dilation(self) -> Tuple[int, int]:
         """
         Returns dilation used in `torch.nn.Unfold
         <https://pytorch.org/docs/stable/generated/torch.nn.Unfold.html#torch.nn.Unfold>`_.
         """
         return self._dilation
 
-    def forward(self, image, mode='flat', *args, **kwargs):
+    def forward(self, image, *args, **kwargs):
         r"""
-        Overrides ``torch.nn.Module``'s forward to compute a convolution on the
-        input image.
+        Overrides ``torch.nn.Module``'s forward to compute a convolution on the input
+        image.
         
         Parameters
         ----------
         image : torch.Tensor
             Input batch of images with shape
             
             .. math::
             
                 batch\_size \times in\_channels \times height \times width
-        mode : {"flat", "snake"}
-            Indicates the order in which MPS should take the pixels in the image.
-            When ``"flat"``, the image is flattened putting one row of the image
-            after the other. When ``"snake"``, its row is put in the opposite
-            orientation as the previous row (like a snake running through the
-            image).
         args :
-            Arguments that might be used in :meth:`~MPS.contract`.
+            Arguments that might be used in :meth:`~PEPS.contract`.
         kwargs :
-            Keyword arguments that might be used in :meth:`~MPS.contract`,
-            like ``inline_input`` or ``inline_mats``.
+            Keyword arguments that might be used in :meth:`~PEPS.contract`,
+            like ``from_size``, ``max_bond`` or inline.
         """
         # Input image shape: batch_size x in_channels x height x width
 
         patches = self.unfold(image).transpose(1, 2)
         # batch_size x nb_windows x (in_channels * nb_pixels)
 
         patches = patches.view(*patches.shape[:-1], self.in_channels, -1)
         # batch_size x nb_windows x in_channels x nb_pixels
 
         patches = patches.transpose(2, 3)
         # batch_size x nb_windows x nb_pixels x in_channels
 
-        if mode == 'snake':
-            new_patches = patches[..., :self._kernel_size[1], :]
-            for i in range(1, self._kernel_size[0]):
-                if i % 2 == 0:
-                    aux = patches[..., (i * self._kernel_size[1]):
-                                       ((i + 1) * self._kernel_size[1]), :]
-                else:
-                    aux = patches[...,
-                        (i * self._kernel_size[1]):
-                        ((i + 1) * self._kernel_size[1]), :].flip(dims=[0])
-                new_patches = torch.cat([new_patches, aux], dim=2)
-
-            patches = new_patches
-
-        elif mode != 'flat':
-            raise ValueError('`mode` can only be "flat" or "snake"')
-
         result = super().forward(patches, *args, **kwargs)
         # batch_size x nb_windows
 
         h_in = image.shape[2]
         w_in = image.shape[3]
 
         h_out = int((h_in + 2 * self.padding[0] - self.dilation[0] *
@@ -1171,30 +1349,30 @@
 
         result = result.view(*result.shape[:-1], h_out, w_out)
         # batch_size x height_out x width_out
 
         return result
 
 
-class ConvUMPS(UMPS):
+class ConvUPEPS(UPEPS):
     """
-    Class for Uniform Matrix Product States, where all nodes are input nodes,
-    and where the input data is a batch of images. It is the convolutional
-    version of :class:`UMPS`. This class cannot have different bond dimensions
-    for each site and boundary conditions are always periodic.
+    Class for Uniform Projected Entangled Pair States, where all nodes are input
+    nodes, and where the input data is a batch of images. It is the convolutional
+    version of :class:`UPEPS`.
     
     Input data as well as initialization parameters are described in `torch.nn.Conv2d
     <https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html>`_.
 
     Parameters
     ----------
     in_channels : int
-        Input channels. Same as ``in_dim`` in :class:`UMPS`.
-    bond_dim : int
-        Bond dimension.
+        Input channels. Same as ``in_dim`` in :class:`UPEPS`.
+    bond_dim : list[int] or tuple[int]
+        Bond dimensions for horizontal and vertical edges (in that order). Thus
+        it should also contain 2 elements
     kernel_size : int, list[int] or tuple[int]
         Kernel size used in `torch.nn.Unfold
         <https://pytorch.org/docs/stable/generated/torch.nn.Unfold.html#torch.nn.Unfold>`_.
         If given as an ``int``, the actual kernel size will be
         ``(kernel_size, kernel_size)``.
     stride : int
         Stride used in `torch.nn.Unfold
@@ -1205,36 +1383,36 @@
         If given as an ``int``, the actual kernel size will be
         ``(kernel_size, kernel_size)``.
     dilation : int
         Dilation used in `torch.nn.Unfold
         <https://pytorch.org/docs/stable/generated/torch.nn.Unfold.html#torch.nn.Unfold>`_.
         If given as an ``int``, the actual kernel size will be
         ``(kernel_size, kernel_size)``.
-    
+        
     Examples
     --------
-    >>> conv_mps = tk.models.ConvMPS(in_channels=2,
-    ...                              bond_dim=5,
-    ...                              kernel_size=2)
-    >>> for node in mps.mats_env:
+    >>> conv_peps = tk.models.ConvPEPS(in_channels=2,
+    ...                                bond_dim=[5, 5],
+    ...                                kernel_size=2)
+    >>> for node in conv_peps.grid_env:
     ...     assert node.tensor_address() == 'virtual_uniform'
     ...
     >>> data = torch.ones(20, 2, 2, 2) # batch_size x in_channels x height x width
-    >>> result = conv_mps(data)
-    >>> print(result.shape)
+    >>> result = conv_peps(data)
+    >>> result.shape
     torch.Size([20, 1, 1])
     """
 
     def __init__(self,
                  in_channels: int,
-                 bond_dim: int,
+                 bond_dim: Union[int, Sequence[int]],
                  kernel_size: Union[int, Sequence],
                  stride: int = 1,
                  padding: int = 0,
-                 dilation: int = 1):
+                 dilation: int = 1) -> None:
 
         if isinstance(kernel_size, int):
             kernel_size = (kernel_size, kernel_size)
         elif not isinstance(kernel_size, Sequence):
             raise TypeError('`kernel_size` must be int or Sequence')
 
         if isinstance(stride, int):
@@ -1254,34 +1432,35 @@
 
         self._in_channels = in_channels
         self._kernel_size = kernel_size
         self._stride = stride
         self._padding = padding
         self._dilation = dilation
 
-        super().__init__(n_features=kernel_size[0] * kernel_size[1],
+        super().__init__(n_rows=kernel_size[0],
+                         n_cols=kernel_size[1],
                          in_dim=in_channels,
                          bond_dim=bond_dim,
                          n_batches=2)
 
         self.unfold = nn.Unfold(kernel_size=kernel_size,
                                 stride=stride,
                                 padding=padding,
                                 dilation=dilation)
 
     @property
     def in_channels(self) -> int:
-        """Returns ``in_channels``. Same as ``in_dim`` in :class:`UMPS`."""
+        """Returns ``in_channels``. Same as ``in_dim`` in :class:`UPEPS`."""
         return self._in_channels
 
     @property
     def kernel_size(self) -> Tuple[int, int]:
         """
-        Returns ``kernel_size``. Number of nodes is given by
-        :math:`kernel\_size_0 \cdot kernel\_size_1`.
+        Returns ``kernel_size``. Number of rows and columns in the 2D grid is
+        given by :math:`kernel\_size_0` and :math:`kernel\_size_1`, respectively.
         """
         return self._kernel_size
 
     @property
     def stride(self) -> Tuple[int, int]:
         """
         Returns stride used in `torch.nn.Unfold
@@ -1301,67 +1480,44 @@
     def dilation(self) -> Tuple[int, int]:
         """
         Returns dilation used in `torch.nn.Unfold
         <https://pytorch.org/docs/stable/generated/torch.nn.Unfold.html#torch.nn.Unfold>`_.
         """
         return self._dilation
 
-    def forward(self, image, mode='flat', *args, **kwargs):
+    def forward(self, image, *args, **kwargs):
         r"""
-        Overrides ``torch.nn.Module``'s forward to compute a convolution on the
-        input image.
+        Overrides ``torch.nn.Module``'s forward to compute a convolution on the input
+        image.
         
         Parameters
         ----------
         image : torch.Tensor
             Input batch of images with shape
             
             .. math::
             
                 batch\_size \times in\_channels \times height \times width
-        mode : {"flat", "snake"}
-            Indicates the order in which MPS should take the pixels in the image.
-            When ``"flat"``, the image is flattened putting one row of the image
-            after the other. When ``"snake"``, its row is put in the opposite
-            orientation as the previous row (like a snake running through the
-            image).
         args :
-            Arguments that might be used in :meth:`~UMPS.contract`.
+            Arguments that might be used in :meth:`~PEPS.contract`.
         kwargs :
-            Keyword arguments that might be used in :meth:`~UMPS.contract`,
-            like ``inline_input`` or ``inline_mats``.
+            Keyword arguments that might be used in :meth:`~PEPS.contract`,
+            like ``from_size``, ``max_bond`` or inline.
         """
         # Input image shape: batch_size x in_channels x height x width
 
         patches = self.unfold(image).transpose(1, 2)
         # batch_size x nb_windows x (in_channels * nb_pixels)
 
         patches = patches.view(*patches.shape[:-1], self.in_channels, -1)
         # batch_size x nb_windows x in_channels x nb_pixels
 
         patches = patches.transpose(2, 3)
         # batch_size x nb_windows x nb_pixels x in_channels
 
-        if mode == 'snake':
-            new_patches = patches[..., :self._kernel_size[1], :]
-            for i in range(1, self._kernel_size[0]):
-                if i % 2 == 0:
-                    aux = patches[..., (i * self._kernel_size[1]):
-                                       ((i + 1) * self._kernel_size[1]), :]
-                else:
-                    aux = patches[...,
-                        (i * self._kernel_size[1]):
-                        ((i + 1) * self._kernel_size[1]), :].flip(dims=[0])
-                new_patches = torch.cat([new_patches, aux], dim=2)
-
-            patches = new_patches
-
-        elif mode != 'flat':
-            raise ValueError('`mode` can only be "flat" or "snake"')
-
         result = super().forward(patches, *args, **kwargs)
         # batch_size x nb_windows
 
         h_in = image.shape[2]
         w_in = image.shape[3]
 
         h_out = int((h_in + 2 * self.padding[0] - self.dilation[0] *
```

### Comparing `tensorkrowch-1.0.1/tensorkrowch/models/tree.py` & `tensorkrowch-1.1.0/tensorkrowch/models/tree.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.0.1/tensorkrowch/operations.py` & `tensorkrowch-1.1.0/tensorkrowch/operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,19 +11,24 @@
         * mul
         * add
         * sub
         
     Node-like operations:
         * split
         * split_             (in-place)
+        * svd                           (edge operation)
         * svd_               (in-place) (edge operation)
+        * svdr                          (edge operation)
         * svdr_              (in-place) (edge operation)
+        * qr                            (edge operation)
         * qr_                (in-place) (edge operation)
+        * rq                            (edge operation)
         * rq_                (in-place) (edge operation)
         * contract_edges
+        * contract                      (edge operation)
         * contract_          (in-place) (edge operation)
         * get_shared_edges
         * contract_between
         * contract_between_  (in-place)
         * stack
         * unbind
         * einsum
@@ -52,15 +57,15 @@
 
 
 ###############################################################################
 #                               OPERATION CLASS                               #
 ###############################################################################
 
 
-class Operation:
+class Operation:  # MARK: Operation
     """
     Class for node operations.
     
     A node operation is made up of two functions, the one that is executed the
     first time the operation is called and the one that is executed in every
     other call (with the same arguments). Both functions are usually similar,
     though the former computes extra things regarding the creation of the
@@ -78,15 +83,19 @@
         Function that checks if the operation has been called at least one time.
     fn_first : callable
         Function that is called the first time the operation is performed.
     fn_next : callable
         Function that is called the next times the operation is performed.
     """
 
-    def __init__(self, name: Text, check_first, fn_first, fn_next):
+    def __init__(self,
+                 name: Text,
+                 check_first: Callable,
+                 fn_first: Callable,
+                 fn_next: Callable) -> None:
         assert isinstance(check_first, Callable)
         assert isinstance(fn_first, Callable)
         assert isinstance(fn_next, Callable)
         self.fn_first = fn_first
         self.fn_next = fn_next
         self.check_first = check_first
 
@@ -103,17 +112,18 @@
 
 
 ###############################################################################
 #                           TENSOR-LIKE OPERATIONS                            #
 ###############################################################################
 
 #################################   PERMUTE    ################################
+# MARK: permute
 def _check_first_permute(node: AbstractNode,
                          axes: Sequence[Ax]) -> Optional[Successor]:
-    args = (node, axes)
+    args = (node, tuple(axes))
     successors = node._successors.get('permute')
     if not successors:
         return None
     return successors.get(args)
 
 
 def _permute_first(node: AbstractNode, axes: Sequence[Ax]) -> Node:
@@ -131,15 +141,15 @@
             network=node._network,
             tensor=node.tensor.permute(axes_nums),
             edges=permute_list(node._edges, axes_nums),
             node1_list=permute_list(node.is_node1(), axes_nums))
 
     # Create successor
     net = node._network
-    args = (node, axes)
+    args = (node, tuple(axes))
     successor = Successor(node_ref=node.node_ref(),
                           index=node._tensor_info['index'],
                           child=new_node,
                           hints=axes_nums)
 
     # Add successor to parent
     if 'permute' in node._successors:
@@ -182,18 +192,21 @@
 
 
 def permute(node: AbstractNode, axes: Sequence[Ax]) -> Node:
     """
     Permutes the nodes' tensor, as well as its axes and edges to match the new
     shape.
 
-    See `permute <https://pytorch.org/docs/stable/generated/torch.permute.html>`_.
+    See `permute <https://pytorch.org/docs/stable/generated/torch.permute.html>`_
+    in the **PyTorch** documentation.
     
     Nodes ``resultant`` from this operation are called ``"permute"``. The node
     that keeps information about the :class:`Successor` is ``node``.
+    
+    This operation is the same as :meth:`~AbstractNode.permute`.
 
     Parameters
     ----------
     node: Node or ParamNode
         Node whose tensor is to be permuted.
     axes: list[int, str or Axis]
         List of axes in the permuted order.
@@ -214,15 +227,16 @@
 
 permute_node = copy_func(permute)
 permute_node.__doc__ = \
     """
     Permutes the nodes' tensor, as well as its axes and edges to match the new
     shape.
     
-    See `permute <https://pytorch.org/docs/stable/generated/torch.permute.html>`_.
+    See `permute <https://pytorch.org/docs/stable/generated/torch.permute.html>`_
+    in the **PyTorch** documentation.
     
     Nodes ``resultant`` from this operation are called ``"permute"``. The node
     that keeps information about the :class:`Successor` is ``self``.
     
     Parameters
     ----------
     axes: list[int, str or Axis]
@@ -250,14 +264,16 @@
 
     Following the **PyTorch** convention, names of functions ended with an
     underscore indicate **in-place** operations.
 
     See `permute <https://pytorch.org/docs/stable/generated/torch.permute.html>`_.
     
     Nodes ``resultant`` from this operation use the same name as ``node``.
+    
+    This operation is the same as :meth:`~AbstractNode.permute_`.
 
     Parameters
     ----------
     node: Node or ParamNode
         Node whose tensor is to be permuted.
     axes: list[int, str or Axis]
         List of axes in the permuted order.
@@ -321,14 +337,15 @@
     torch.Size([7, 2, 5])
     """
 
 AbstractNode.permute_ = permute_node_
 
 
 ##################################   TPROD    #################################
+# MARK: tprod
 def _check_first_tprod(node1: AbstractNode,
                        node2: AbstractNode) -> Optional[Successor]:
     args = (node1, node2)
     successors = node1._successors.get('tprod')
     if not successors:
         return None
     return successors.get(args)
@@ -465,14 +482,15 @@
     torch.Size([2, 3, 4, 5])
     """
 
 AbstractNode.__mod__ = tprod_node
 
 
 ###################################   MUL    ##################################
+# MARK: mul
 def _check_first_mul(node1: AbstractNode,
                      node2: AbstractNode) -> Optional[Successor]:
     args = (node1, node2)
     successors = node1._successors.get('mul')
     if not successors:
         return None
     return successors.get(args)
@@ -598,14 +616,15 @@
     torch.Size([2, 3])
     """
 
 AbstractNode.__mul__ = mul_node
 
 
 ###################################   ADD    ##################################
+# MARK: add
 def _check_first_add(node1: AbstractNode,
                      node2: AbstractNode) -> Optional[Successor]:
     args = (node1, node2)
     successors = node1._successors.get('add')
     if not successors:
         return None
     return successors.get(args)
@@ -731,14 +750,15 @@
     torch.Size([2, 3])
     """
 
 AbstractNode.__add__ = add_node
 
 
 ###################################   SUB    ##################################
+# MARK: sub
 def _check_first_sub(node1: AbstractNode,
                      node2: AbstractNode) -> Optional[Successor]:
     args = (node1, node2)
     successors = node1._successors.get('sub')
     if not successors:
         return None
     return successors.get(args)
@@ -868,14 +888,15 @@
 
 
 ###############################################################################
 #                            NODE-LIKE OPERATIONS                             #
 ###############################################################################
 
 ##################################   SPLIT    #################################
+# MARK: split
 def _check_first_split(node: AbstractNode,
                        node1_axes: Sequence[Ax],
                        node2_axes: Sequence[Ax],
                        mode: Text = 'svd',
                        side: Optional[Text] = 'left',
                        rank: Optional[int] = None,
                        cum_percentage: Optional[float] = None,
@@ -898,17 +919,17 @@
                  node1_axes: Sequence[Ax],
                  node2_axes: Sequence[Ax],
                  mode: Text = 'svd',
                  side: Optional[Text] = 'left',
                  rank: Optional[int] = None,
                  cum_percentage: Optional[float] = None,
                  cutoff: Optional[float] = None) -> Tuple[Node, Node]:
-    if not isinstance(node1_axes, (list, tuple)):
+    if not isinstance(node1_axes, Sequence):
         raise TypeError('`node1_edges` should be list or tuple type')
-    if not isinstance(node2_axes, (list, tuple)):
+    if not isinstance(node2_axes, Sequence):
         raise TypeError('`node2_edges` should be list or tuple type')
     
     args = (node,
             tuple(node1_axes),
             tuple(node2_axes),
             mode,
             side,
@@ -962,56 +983,47 @@
         node_tensor = node.tensor \
             .reshape(*(batch_shape +
                        [node1_shape.prod().item()] +
                        [node2_shape.prod().item()]))
 
     if (mode == 'svd') or (mode == 'svdr'):
         u, s, vh = torch.linalg.svd(node_tensor, full_matrices=False)
-
-        if cum_percentage is not None:
-            if (rank is not None) or (cutoff is not None):
-                raise ValueError('Only one of `rank`, `cum_percentage` and '
-                                 '`cutoff` should be provided')
-
-            percentages = s.cumsum(-1) / s.sum(-1) \
-                .view(*s.shape[:-1], 1).expand(s.shape)
-            cum_percentage_tensor = torch.tensor(cum_percentage) \
-                .repeat(percentages.shape[:-1])
-            rank = 0
-            for i in range(percentages.shape[-1]):
-                p = percentages[..., i]
-                rank += 1
-                # Cut when ``cum_percentage`` is exceeded in all batches
-                if torch.ge(p, cum_percentage_tensor).all():
-                    break
-
-        elif cutoff is not None:
-            if rank is not None:
-                raise ValueError('Only one of `rank`, `cum_percentage` and '
-                                 '`cutoff` should be provided')
-
-            cutoff_tensor = torch.tensor(cutoff).repeat(s.shape[:-1])
-            rank = 0
-            for i in range(s.shape[-1]):
-                # Cut when ``cutoff`` is exceeded in all batches
-                if torch.le(s[..., i], cutoff_tensor).all():
-                    break
-                rank += 1
-            if rank == 0:
-                rank = 1
-
+        
+        lst_ranks = []
+        
         if rank is None:
             rank = s.shape[-1]
+            lst_ranks.append(rank)
         else:
-            if rank < s.shape[-1]:
-                u = u[..., :rank]
-                s = s[..., :rank]
-                vh = vh[..., :rank, :]
-            else:
-                rank = s.shape[-1]
+            lst_ranks.append(min(max(1, int(rank)), s.shape[-1]))
+            
+        if cum_percentage is not None:
+            s_percentages = s.cumsum(-1) / \
+                (s.sum(-1, keepdim=True).expand(s.shape) + 1e-10) # To avoid having all 0's
+            cum_percentage_tensor = cum_percentage * torch.ones_like(s)
+            cp_rank = torch.lt(
+                s_percentages,
+                cum_percentage_tensor
+                ).view(-1, s.shape[-1]).all(dim=0).sum()
+            lst_ranks.append(max(1, cp_rank.item() + 1))
+            
+        if cutoff is not None:
+            cutoff_tensor = cutoff * torch.ones_like(s)
+            co_rank = torch.ge(
+                s,
+                cutoff_tensor
+                ).view(-1, s.shape[-1]).all(dim=0).sum()
+            lst_ranks.append(max(1, co_rank.item()))
+        
+        # Select rank from specified restrictions
+        rank = min(lst_ranks)
+        
+        u = u[..., :rank]
+        s = s[..., :rank]
+        vh = vh[..., :rank, :]
 
         if mode == 'svdr':
             phase = torch.sign(torch.randn(s.shape))
             phase = torch.diag_embed(phase)
             u = u @ phase
             vh = phase @ vh
 
@@ -1170,56 +1182,47 @@
         node_tensor = node_tensor \
             .reshape(*(batch_shape +
                        [node1_shape.prod().item()] +
                        [node2_shape.prod().item()]))
 
     if (mode == 'svd') or (mode == 'svdr'):
         u, s, vh = torch.linalg.svd(node_tensor, full_matrices=False)
-
-        if cum_percentage is not None:
-            if (rank is not None) or (cutoff is not None):
-                raise ValueError('Only one of `rank`, `cum_percentage` and '
-                                 '`cutoff` should be provided')
-
-            percentages = s.cumsum(-1) / s.sum(-1) \
-                .view(*s.shape[:-1], 1).expand(s.shape)
-            cum_percentage_tensor = torch.tensor(
-                cum_percentage).repeat(percentages.shape[:-1])
-            rank = 0
-            for i in range(percentages.shape[-1]):
-                p = percentages[..., i]
-                rank += 1
-                # Cut when ``cum_percentage`` is exceeded in all batches
-                if torch.ge(p, cum_percentage_tensor).all():
-                    break
-
-        elif cutoff is not None:
-            if rank is not None:
-                raise ValueError('Only one of `rank`, `cum_percentage` and '
-                                 '`cutoff` should be provided')
-
-            cutoff_tensor = torch.tensor(cutoff).repeat(s.shape[:-1])
-            rank = 0
-            for i in range(s.shape[-1]):
-                # Cut when ``cutoff`` is exceeded in all batches
-                if torch.le(s[..., i], cutoff_tensor).all():
-                    break
-                rank += 1
-            if rank == 0:
-                rank = 1
-
+        
+        lst_ranks = []
+        
         if rank is None:
             rank = s.shape[-1]
+            lst_ranks.append(rank)
         else:
-            if rank < s.shape[-1]:
-                u = u[..., :rank]
-                s = s[..., :rank]
-                vh = vh[..., :rank, :]
-            else:
-                rank = s.shape[-1]
+            lst_ranks.append(min(max(1, rank), s.shape[-1]))
+            
+        if cum_percentage is not None:
+            s_percentages = s.cumsum(-1) / \
+                (s.sum(-1, keepdim=True).expand(s.shape) + 1e-10) # To avoid having all 0's
+            cum_percentage_tensor = cum_percentage * torch.ones_like(s)
+            cp_rank = torch.lt(
+                s_percentages,
+                cum_percentage_tensor
+                ).view(-1, s.shape[-1]).all(dim=0).sum()
+            lst_ranks.append(max(1, cp_rank.item() + 1))
+            
+        if cutoff is not None:
+            cutoff_tensor = cutoff * torch.ones_like(s)
+            co_rank = torch.ge(
+                s,
+                cutoff_tensor
+                ).view(-1, s.shape[-1]).all(dim=0).sum()
+            lst_ranks.append(max(1, co_rank.item()))
+        
+        # Select rank from specified restrictions
+        rank = min(lst_ranks)
+        
+        u = u[..., :rank]
+        s = s[..., :rank]
+        vh = vh[..., :rank, :]
 
         if mode == 'svdr':
             phase = torch.sign(torch.randn(s.shape))
             phase = torch.diag_embed(phase)
             u = u @ phase
             vh = phase @ vh
 
@@ -1279,15 +1282,15 @@
           side: Optional[Text] = 'left',
           rank: Optional[int] = None,
           cum_percentage: Optional[float] = None,
           cutoff: Optional[float] = None) -> Tuple[Node, Node]:
     r"""
     Splits one node in two via the decomposition specified in ``mode``. To
     perform this operation the set of edges has to be split in two sets,
-    corresponding to the edges of the first and second ``resultant nodes``.
+    corresponding to the edges of the first and second ``resultant`` nodes.
     Batch edges that don't appear in any of the lists will be repeated in both
     nodes, and will appear as the first edges of the ``resultant`` nodes, in
     the order they appeared in ``node``.
 
     Having specified the two sets of edges, the node's tensor is reshaped as a
     batch matrix, with batch dimensions first, a single input dimension
     (adding up all edges in the first set) and a single output dimension
@@ -1325,22 +1328,26 @@
 
       .. math::
 
         M = RQ
 
       where R is a lower triangular matrix and Q is unitary.
 
-    If ``mode`` is "svd" or "svdr", ``side`` must be provided. Besides, one
-    (and only one) of ``rank``, ``cum_percentage`` and ``cutoff`` is required.
+    If ``mode`` is "svd" or "svdr", ``side`` must be provided. Besides, at least
+    one of ``rank``, ``cum_percentage`` and ``cutoff`` is required. If more than
+    one is specified, the resulting rank will be the one that satisfies all
+    conditions.
     
     Since the node is `split` in two, a new edge appears connecting both
     nodes. The axis that corresponds to this edge has the name ``"split"``.
     
     Nodes ``resultant`` from this operation are called ``"split"``. The node
     that keeps information about the :class:`Successor` is ``node``.
+    
+    This operation is the same as :meth:`~AbstractNode.split`.
 
     Parameters
     ----------
     node : AbstractNode
         Node that is to be split.
     node1_axes : list[int, str or Axis]
         First set of edges, will appear as the edges of the first (left)
@@ -1473,14 +1480,16 @@
     Following the **PyTorch** convention, names of functions ended with an
     underscore indicate **in-place** operations.
     
     Since the node is `split` in two, a new edge appears connecting both
     nodes. The axis that corresponds to this edge has the name ``"split"``.
     
     Nodes ``resultant`` from this operation are called ``"split_ip"``.
+    
+    This operation is the same as :meth:`~AbstractNode.split_`.
 
     Parameters
     ----------
     node : AbstractNode
         Node that is to be split.
     node1_axes : list[int, str or Axis]
         First set of edges, will appear as the edges of the first (left)
@@ -1536,16 +1545,16 @@
     >>> node.network is None
     True
     
     >>> del node
     """
     node1, node2 = split(node, node1_axes, node2_axes,
                          mode, side, rank, cum_percentage, cutoff)
-    node1.reattach_edges(True)
-    node2.reattach_edges(True)
+    node1.reattach_edges(override=True)
+    node2.reattach_edges(override=True)
     node1._unrestricted_set_tensor(node1.tensor.detach())
     node2._unrestricted_set_tensor(node2.tensor.detach())
 
     # Delete node (and its edges) from the TN
     net = node._network
     net.delete_node(node)
 
@@ -1571,15 +1580,15 @@
 
     return node1, node2
 
 
 split_node_ = copy_func(split_)
 split_node_.__doc__ = \
     r"""
-    In-place version of :func:`~AbstractNode.split`.
+    In-place version of :meth:`~AbstractNode.split`.
     
     Following the **PyTorch** convention, names of functions ended with an
     underscore indicate **in-place** operations.
     
     Since the node is `split` in two, a new edge appears connecting both
     nodes. The axis that corresponds to this edge has the name ``"split"``.
     
@@ -1618,18 +1627,17 @@
     -------
     tuple[Node, Node]
     
     Examples
     --------
     >>> node = tk.randn(shape=(10, 15, 100),
     ...                 axes_names=('left', 'right', 'batch'))
-    >>> node_left, node_right = tk.split_(node,
-    ...                                   ['left'], ['right'],
-    ...                                   mode='svd',
-    ...                                   rank=5)
+    >>> node_left, node_right = node.split_(['left'], ['right'],
+    ...                                     mode='svd',
+    ...                                     rank=5)
     >>> node_left.shape
     torch.Size([100, 10, 5])
     
     >>> node_right.shape
     torch.Size([100, 5, 15])
     
     >>> node_left['split']
@@ -1643,29 +1651,224 @@
     
     >>> del node
     """
 
 AbstractNode.split_ = split_node_
 
 
+def svd(edge: Edge,
+        side: Text = 'left',
+        rank: Optional[int] = None,
+        cum_percentage: Optional[float] = None,
+        cutoff: Optional[float] = None) -> Tuple[Node, Node]:
+    r"""
+    Contracts an edge via :func:`contract` and splits it via :func:`split`
+    using ``mode = "svd"``. See :func:`split` for a more complete explanation.
+    
+    This operation is the same as :meth:`~Edge.svd`.
+
+    Parameters
+    ----------
+    edge : Edge
+        Edge whose nodes are to be contracted and split.
+    side : str, optional
+        Indicates the side to which the diagonal matrix :math:`S` should be
+        contracted. If "left", the first resultant node's tensor will be
+        :math:`US`, and the other node's tensor will be :math:`V^{\dagger}`.
+        If "right", their tensors will be :math:`U` and :math:`SV^{\dagger}`,
+        respectively.
+    rank : int, optional
+        Number of singular values to keep.
+    cum_percentage : float, optional
+        Proportion that should be satisfied between the sum of all singular
+        values kept and the total sum of all singular values.
+
+        .. math::
+
+            \frac{\sum_{i \in \{kept\}}{s_i}}{\sum_{i \in \{all\}}{s_i}} \ge
+            cum\_percentage
+    cutoff : float, optional
+        Quantity that lower bounds singular values in order to be kept.
+
+    Returns
+    -------
+    tuple[Node, Node]
+    
+    Examples
+    --------
+    >>> nodeA = tk.randn(shape=(10, 15, 100),
+    ...                  axes_names=('left', 'right', 'batch'),
+    ...                  name='nodeA')
+    >>> nodeB = tk.randn(shape=(15, 20, 100),
+    ...                  axes_names=('left', 'right', 'batch'),
+    ...                  name='nodeB')
+    ...
+    >>> new_edge = nodeA['right'] ^ nodeB['left']
+    >>> new_nodeA, new_nodeB = tk.svd(new_edge, rank=7)
+    ...
+    >>> new_nodeA.shape
+    torch.Size([10, 7, 100])
+    
+    >>> new_nodeB.shape
+    torch.Size([7, 20, 100])
+    
+    >>> print(new_nodeA.axes_names)
+    ['left', 'right', 'batch']
+    
+    >>> print(new_nodeB.axes_names)
+    ['left', 'right', 'batch']
+    
+    Original nodes still exist in the network
+    
+    >>> assert nodeA.network == new_nodeA.network
+    >>> assert nodeB.network == new_nodeB.network
+    """
+    if edge.is_dangling():
+        raise ValueError('Edge should be connected to perform SVD')
+    if edge.node1 is edge.node2:
+        raise ValueError('Edge should connect different nodes')
+
+    node1, node2 = edge.node1, edge.node2
+    axis1, axis2 = edge.axis1, edge.axis2
+
+    batch_axes = []
+    for axis in node1._axes:
+        if axis._batch and (axis._name in node2.axes_names):
+            batch_axes.append(axis)
+
+    n_batches = len(batch_axes)
+    n_axes1 = len(node1._axes) - n_batches - 1
+    n_axes2 = len(node2._axes) - n_batches - 1
+
+    contracted = edge.contract()
+    new_node1, new_node2 = split(node=contracted,
+                                 node1_axes=list(
+                                     range(n_batches,
+                                         n_batches + n_axes1)),
+                                 node2_axes=list(
+                                     range(n_batches + n_axes1,
+                                         n_batches + n_axes1 + n_axes2)),
+                                 mode='svd',
+                                 side=side,
+                                 rank=rank,
+                                 cum_percentage=cum_percentage,
+                                 cutoff=cutoff)
+
+    # new_node1
+    prev_nums = [ax.num for ax in batch_axes]
+    for i in range(new_node1.rank):
+        if (i not in prev_nums) and (i != axis1._num):
+            prev_nums.append(i)
+    prev_nums += [axis1._num]
+
+    if prev_nums != list(range(new_node1.rank)):
+        permutation = inverse_permutation(prev_nums)
+        new_node1 = new_node1.permute(permutation)
+
+    # new_node2
+    prev_nums = [node2.get_axis_num(node1.get_axis(ax)._name)
+                 for ax in batch_axes] + [axis2._num]
+    for i in range(new_node2.rank):
+        if i not in prev_nums:
+            prev_nums.append(i)
+
+    if prev_nums != list(range(new_node2.rank)):
+        permutation = inverse_permutation(prev_nums)
+        new_node2 = new_node2.permute(permutation)
+        
+    new_node1.get_axis(axis1._num).name = axis1._name
+    new_node2.get_axis(axis2._num).name = axis2._name
+
+    return new_node1, new_node2
+
+
+svd_edge = copy_func(svd)
+svd_edge.__doc__ = \
+    r"""
+    Contracts an edge via :meth:`~Edge.contract` and splits it via
+    :meth:`~AbstractNode.split` using ``mode = "svd"``. See :func:`split` for
+    a more complete explanation.
+
+    Parameters
+    ----------
+    side : str, optional
+        Indicates the side to which the diagonal matrix :math:`S` should be
+        contracted. If "left", the first resultant node's tensor will be
+        :math:`US`, and the other node's tensor will be :math:`V^{\dagger}`.
+        If "right", their tensors will be :math:`U` and :math:`SV^{\dagger}`,
+        respectively.
+    rank : int, optional
+        Number of singular values to keep.
+    cum_percentage : float, optional
+        Proportion that should be satisfied between the sum of all singular
+        values kept and the total sum of all singular values.
+
+        .. math::
+
+            \frac{\sum_{i \in \{kept\}}{s_i}}{\sum_{i \in \{all\}}{s_i}} \ge
+            cum\_percentage
+    cutoff : float, optional
+        Quantity that lower bounds singular values in order to be kept.
+
+    Returns
+    -------
+    tuple[Node, Node]
+    
+    Examples
+    --------
+    >>> nodeA = tk.randn(shape=(10, 15, 100),
+    ...                  axes_names=('left', 'right', 'batch'),
+    ...                  name='nodeA')
+    >>> nodeB = tk.randn(shape=(15, 20, 100),
+    ...                  axes_names=('left', 'right', 'batch'),
+    ...                  name='nodeB')
+    ...
+    >>> new_edge = nodeA['right'] ^ nodeB['left']
+    >>> new_nodeA, new_nodeB = new_edge.svd(rank=7)
+    ...
+    >>> new_nodeA.shape
+    torch.Size([10, 7, 100])
+    
+    >>> new_nodeB.shape
+    torch.Size([7, 20, 100])
+    
+    >>> print(new_nodeA.axes_names)
+    ['left', 'right', 'batch']
+    
+    >>> print(new_nodeB.axes_names)
+    ['left', 'right', 'batch']
+    
+    Original nodes still exist in the network
+    
+    >>> assert nodeA.network == new_nodeA.network
+    >>> assert nodeB.network == new_nodeB.network
+    """
+
+Edge.svd = svd_edge
+
+
 def svd_(edge: Edge,
          side: Text = 'left',
          rank: Optional[int] = None,
          cum_percentage: Optional[float] = None,
          cutoff: Optional[float] = None) -> Tuple[Node, Node]:
     r"""
+    In-place version of :func:`svd`.
+    
     Contracts an edge in-place via :func:`contract_` and splits it in-place via
     :func:`split_` using ``mode = "svd"``. See :func:`split` for a more complete
     explanation.
 
     Following the **PyTorch** convention, names of functions ended with an
     underscore indicate **in-place** operations.
     
     Nodes ``resultant`` from this operation use the same names as the original
     nodes connected by ``edge``.
+    
+    This operation is the same as :meth:`~Edge.svd_`.
 
     Parameters
     ----------
     edge : Edge
         Edge whose nodes are to be contracted and split.
     side : str, optional
         Indicates the side to which the diagonal matrix :math:`S` should be
@@ -1712,14 +1915,16 @@
     ['left', 'right', 'batch']
     
     >>> print(nodeB.axes_names)
     ['left', 'right', 'batch']
     """
     if edge.is_dangling():
         raise ValueError('Edge should be connected to perform SVD')
+    if edge.node1 is edge.node2:
+        raise ValueError('Edge should connect different nodes')
 
     node1, node2 = edge.node1, edge.node2
     node1_name, node2_name = node1._name, node2._name
     axis1, axis2 = edge.axis1, edge.axis2
 
     batch_axes = []
     for axis in node1._axes:
@@ -1774,16 +1979,18 @@
 
     return new_node1, new_node2
 
 
 svd_edge_ = copy_func(svd_)
 svd_edge_.__doc__ = \
     r"""
-    Contracts an edge in-place via :func:`~Edge.contract_` and splits
-    it in-place via :func:`~AbstractNode.split_` using ``mode = "svd"``. See
+    In-place version of :meth:`~Edge.svd`.
+    
+    Contracts an edge in-place via :meth:`~Edge.contract_` and splits
+    it in-place via :meth:`~AbstractNode.split_` using ``mode = "svd"``. See
     :func:`split` for a more complete explanation.
     
     Following the **PyTorch** convention, names of functions ended with an
     underscore indicate **in-place** operations.
     
     Nodes ``resultant`` from this operation use the same names as the original
     nodes connected by ``self``.
@@ -1837,29 +2044,224 @@
     >>> print(nodeB.axes_names)
     ['left', 'right', 'batch']
     """
 
 Edge.svd_ = svd_edge_
 
 
+def svdr(edge: Edge,
+         side: Text = 'left',
+         rank: Optional[int] = None,
+         cum_percentage: Optional[float] = None,
+         cutoff: Optional[float] = None) -> Tuple[Node, Node]:
+    r"""
+    Contracts an edge via :func:`contract` and splits it via :func:`split`
+    using ``mode = "svdr"``. See :func:`split` for a more complete explanation.
+    
+    This operation is the same as :meth:`~Edge.svdr`.
+
+    Parameters
+    ----------
+    edge : Edge
+        Edge whose nodes are to be contracted and split.
+    side : str, optional
+        Indicates the side to which the diagonal matrix :math:`S` should be
+        contracted. If "left", the first resultant node's tensor will be
+        :math:`US`, and the other node's tensor will be :math:`V^{\dagger}`.
+        If "right", their tensors will be :math:`U` and :math:`SV^{\dagger}`,
+        respectively.
+    rank : int, optional
+        Number of singular values to keep.
+    cum_percentage : float, optional
+        Proportion that should be satisfied between the sum of all singular
+        values kept and the total sum of all singular values.
+
+        .. math::
+
+            \frac{\sum_{i \in \{kept\}}{s_i}}{\sum_{i \in \{all\}}{s_i}} \ge
+            cum\_percentage
+    cutoff : float, optional
+        Quantity that lower bounds singular values in order to be kept.
+
+    Returns
+    -------
+    tuple[Node, Node]
+    
+    Examples
+    --------
+    >>> nodeA = tk.randn(shape=(10, 15, 100),
+    ...                  axes_names=('left', 'right', 'batch'),
+    ...                  name='nodeA')
+    >>> nodeB = tk.randn(shape=(15, 20, 100),
+    ...                  axes_names=('left', 'right', 'batch'),
+    ...                  name='nodeB')
+    ...
+    >>> new_edge = nodeA['right'] ^ nodeB['left']
+    >>> new_nodeA, new_nodeB = tk.svdr(new_edge, rank=7)
+    ...
+    >>> new_nodeA.shape
+    torch.Size([10, 7, 100])
+    
+    >>> new_nodeB.shape
+    torch.Size([7, 20, 100])
+    
+    >>> print(new_nodeA.axes_names)
+    ['left', 'right', 'batch']
+    
+    >>> print(new_nodeB.axes_names)
+    ['left', 'right', 'batch']
+    
+    Original nodes still exist in the network
+    
+    >>> assert nodeA.network == new_nodeA.network
+    >>> assert nodeB.network == new_nodeB.network
+    """
+    if edge.is_dangling():
+        raise ValueError('Edge should be connected to perform SVD')
+    if edge.node1 is edge.node2:
+        raise ValueError('Edge should connect different nodes')
+
+    node1, node2 = edge.node1, edge.node2
+    axis1, axis2 = edge.axis1, edge.axis2
+
+    batch_axes = []
+    for axis in node1._axes:
+        if axis._batch and (axis._name in node2.axes_names):
+            batch_axes.append(axis)
+
+    n_batches = len(batch_axes)
+    n_axes1 = len(node1._axes) - n_batches - 1
+    n_axes2 = len(node2._axes) - n_batches - 1
+
+    contracted = edge.contract()
+    new_node1, new_node2 = split(node=contracted,
+                                 node1_axes=list(
+                                     range(n_batches,
+                                         n_batches + n_axes1)),
+                                 node2_axes=list(
+                                     range(n_batches + n_axes1,
+                                         n_batches + n_axes1 + n_axes2)),
+                                 mode='svdr',
+                                 side=side,
+                                 rank=rank,
+                                 cum_percentage=cum_percentage,
+                                 cutoff=cutoff)
+
+    # new_node1
+    prev_nums = [ax.num for ax in batch_axes]
+    for i in range(new_node1.rank):
+        if (i not in prev_nums) and (i != axis1._num):
+            prev_nums.append(i)
+    prev_nums += [axis1._num]
+
+    if prev_nums != list(range(new_node1.rank)):
+        permutation = inverse_permutation(prev_nums)
+        new_node1 = new_node1.permute(permutation)
+
+    # new_node2
+    prev_nums = [node2.get_axis_num(node1.get_axis(ax)._name)
+                 for ax in batch_axes] + [axis2._num]
+    for i in range(new_node2.rank):
+        if i not in prev_nums:
+            prev_nums.append(i)
+
+    if prev_nums != list(range(new_node2.rank)):
+        permutation = inverse_permutation(prev_nums)
+        new_node2 = new_node2.permute(permutation)
+        
+    new_node1.get_axis(axis1._num).name = axis1._name
+    new_node2.get_axis(axis2._num).name = axis2._name
+
+    return new_node1, new_node2
+
+
+svdr_edge = copy_func(svdr)
+svdr_edge.__doc__ = \
+    r"""
+    Contracts an edge via :meth:`~Edge.contract` and splits it via
+    :meth:`~AbstractNode.split` using ``mode = "svdr"``. See :func:`split` for
+    a more complete explanation.
+
+    Parameters
+    ----------
+    side : str, optional
+        Indicates the side to which the diagonal matrix :math:`S` should be
+        contracted. If "left", the first resultant node's tensor will be
+        :math:`US`, and the other node's tensor will be :math:`V^{\dagger}`.
+        If "right", their tensors will be :math:`U` and :math:`SV^{\dagger}`,
+        respectively.
+    rank : int, optional
+        Number of singular values to keep.
+    cum_percentage : float, optional
+        Proportion that should be satisfied between the sum of all singular
+        values kept and the total sum of all singular values.
+
+        .. math::
+
+            \frac{\sum_{i \in \{kept\}}{s_i}}{\sum_{i \in \{all\}}{s_i}} \ge
+            cum\_percentage
+    cutoff : float, optional
+        Quantity that lower bounds singular values in order to be kept.
+
+    Returns
+    -------
+    tuple[Node, Node]
+    
+    Examples
+    --------
+    >>> nodeA = tk.randn(shape=(10, 15, 100),
+    ...                  axes_names=('left', 'right', 'batch'),
+    ...                  name='nodeA')
+    >>> nodeB = tk.randn(shape=(15, 20, 100),
+    ...                  axes_names=('left', 'right', 'batch'),
+    ...                  name='nodeB')
+    ...
+    >>> new_edge = nodeA['right'] ^ nodeB['left']
+    >>> new_nodeA, new_nodeB = new_edge.svdr(rank=7)
+    ...
+    >>> new_nodeA.shape
+    torch.Size([10, 7, 100])
+    
+    >>> new_nodeB.shape
+    torch.Size([7, 20, 100])
+    
+    >>> print(new_nodeA.axes_names)
+    ['left', 'right', 'batch']
+    
+    >>> print(new_nodeB.axes_names)
+    ['left', 'right', 'batch']
+    
+    Original nodes still exist in the network
+    
+    >>> assert nodeA.network == new_nodeA.network
+    >>> assert nodeB.network == new_nodeB.network
+    """
+
+Edge.svdr = svdr_edge
+
+
 def svdr_(edge: Edge,
           side: Text = 'left',
           rank: Optional[int] = None,
           cum_percentage: Optional[float] = None,
           cutoff: Optional[float] = None) -> Tuple[Node, Node]:
     r"""
+    In-place version of :func:`svdr`.
+    
     Contracts an edge in-place via :func:`contract_` and splits it in-place via
     :func:`split_` using ``mode = "svdr"``. See :func:`split` for a more complete
     explanation.
 
     Following the **PyTorch** convention, names of functions ended with an
     underscore indicate **in-place** operations.
     
     Nodes ``resultant`` from this operation use the same names as the original
     nodes connected by ``edge``.
+    
+    This operation is the same as :meth:`~Edge.svdr_`.
 
     Parameters
     ----------
     edge : Edge
         Edge whose nodes are to be contracted and split.
     side : str, optional
         Indicates the side to which the diagonal matrix :math:`S` should be
@@ -1906,14 +2308,16 @@
     ['left', 'right', 'batch']
     
     >>> print(nodeB.axes_names)
     ['left', 'right', 'batch']
     """
     if edge.is_dangling():
         raise ValueError('Edge should be connected to perform SVD')
+    if edge.node1 is edge.node2:
+        raise ValueError('Edge should connect different nodes')
 
     node1, node2 = edge.node1, edge.node2
     node1_name, node2_name = node1._name, node2._name
     axis1, axis2 = edge.axis1, edge.axis2
 
     batch_axes = []
     for axis in node1._axes:
@@ -1968,16 +2372,18 @@
 
     return new_node1, new_node2
 
 
 svdr_edge_ = copy_func(svdr_)
 svdr_edge_.__doc__ = \
     r"""
-    Contracts an edge in-place via :func:`~Edge.contract_` and splits
-    it in-place via :func:`~AbstractNode.split_` using ``mode = "svdr"``. See
+    In-place version of :meth:`~Edge.svdr`.
+    
+    Contracts an edge in-place via :meth:`~Edge.contract_` and splits
+    it in-place via :meth:`~AbstractNode.split_` using ``mode = "svdr"``. See
     :func:`split` for a more complete explanation.
     
     Following the **PyTorch** convention, names of functions ended with an
     underscore indicate **in-place** operations.
     
     Nodes ``resultant`` from this operation use the same names as the original
     nodes connected by ``self``.
@@ -2031,25 +2437,173 @@
     >>> print(nodeB.axes_names)
     ['left', 'right', 'batch']
     """
 
 Edge.svdr_ = svdr_edge_
 
 
+def qr(edge: Edge) -> Tuple[Node, Node]:
+    r"""
+    Contracts an edge via :func:`contract` and splits it via :func:`split`
+    using ``mode = "qr"``. See :func:`split` for a more complete explanation.
+    
+    This operation is the same as :meth:`~Edge.qr`.
+
+    Parameters
+    ----------
+    edge : Edge
+        Edge whose nodes are to be contracted and split.
+
+    Returns
+    -------
+    tuple[Node, Node]
+    
+    Examples
+    --------
+    >>> nodeA = tk.randn(shape=(10, 15, 100),
+    ...                  axes_names=('left', 'right', 'batch'),
+    ...                  name='nodeA')
+    >>> nodeB = tk.randn(shape=(15, 20, 100),
+    ...                  axes_names=('left', 'right', 'batch'),
+    ...                  name='nodeB')
+    ...
+    >>> new_edge = nodeA['right'] ^ nodeB['left']
+    >>> new_nodeA, new_nodeB = tk.qr(new_edge)
+    ...
+    >>> new_nodeA.shape
+    torch.Size([10, 10, 100])
+    
+    >>> new_nodeB.shape
+    torch.Size([10, 20, 100])
+    
+    >>> print(new_nodeA.axes_names)
+    ['left', 'right', 'batch']
+    
+    >>> print(new_nodeB.axes_names)
+    ['left', 'right', 'batch']
+    
+    Original nodes still exist in the network
+    
+    >>> assert nodeA.network == new_nodeA.network
+    >>> assert nodeB.network == new_nodeB.network
+    """
+    if edge.is_dangling():
+        raise ValueError('Edge should be connected to perform SVD')
+    if edge.node1 is edge.node2:
+        raise ValueError('Edge should connect different nodes')
+
+    node1, node2 = edge.node1, edge.node2
+    axis1, axis2 = edge.axis1, edge.axis2
+
+    batch_axes = []
+    for axis in node1._axes:
+        if axis._batch and (axis._name in node2.axes_names):
+            batch_axes.append(axis)
+
+    n_batches = len(batch_axes)
+    n_axes1 = len(node1._axes) - n_batches - 1
+    n_axes2 = len(node2._axes) - n_batches - 1
+
+    contracted = edge.contract()
+    new_node1, new_node2 = split(node=contracted,
+                                 node1_axes=list(
+                                     range(n_batches,
+                                         n_batches + n_axes1)),
+                                 node2_axes=list(
+                                     range(n_batches + n_axes1,
+                                         n_batches + n_axes1 + n_axes2)),
+                                 mode='qr')
+
+    # new_node1
+    prev_nums = [ax.num for ax in batch_axes]
+    for i in range(new_node1.rank):
+        if (i not in prev_nums) and (i != axis1._num):
+            prev_nums.append(i)
+    prev_nums += [axis1._num]
+
+    if prev_nums != list(range(new_node1.rank)):
+        permutation = inverse_permutation(prev_nums)
+        new_node1 = new_node1.permute(permutation)
+
+    # new_node2
+    prev_nums = [node2.get_axis_num(node1.get_axis(ax)._name)
+                 for ax in batch_axes] + [axis2._num]
+    for i in range(new_node2.rank):
+        if i not in prev_nums:
+            prev_nums.append(i)
+
+    if prev_nums != list(range(new_node2.rank)):
+        permutation = inverse_permutation(prev_nums)
+        new_node2 = new_node2.permute(permutation)
+        
+    new_node1.get_axis(axis1._num).name = axis1._name
+    new_node2.get_axis(axis2._num).name = axis2._name
+
+    return new_node1, new_node2
+
+
+qr_edge = copy_func(qr)
+qr_edge.__doc__ = \
+    r"""
+    Contracts an edge via :meth:`~Edge.contract` and splits it via
+    :meth:`~AbstractNode.split` using ``mode = "qr"``. See :func:`split` for
+    a more complete explanation.
+
+    Returns
+    -------
+    tuple[Node, Node]
+    
+    Examples
+    --------
+    >>> nodeA = tk.randn(shape=(10, 15, 100),
+    ...                  axes_names=('left', 'right', 'batch'),
+    ...                  name='nodeA')
+    >>> nodeB = tk.randn(shape=(15, 20, 100),
+    ...                  axes_names=('left', 'right', 'batch'),
+    ...                  name='nodeB')
+    ...
+    >>> new_edge = nodeA['right'] ^ nodeB['left']
+    >>> new_nodeA, new_nodeB = new_edge.qr()
+    ...
+    >>> new_nodeA.shape
+    torch.Size([10, 10, 100])
+    
+    >>> new_nodeB.shape
+    torch.Size([10, 20, 100])
+    
+    >>> print(new_nodeA.axes_names)
+    ['left', 'right', 'batch']
+    
+    >>> print(new_nodeB.axes_names)
+    ['left', 'right', 'batch']
+    
+    Original nodes still exist in the network
+    
+    >>> assert nodeA.network == new_nodeA.network
+    >>> assert nodeB.network == new_nodeB.network
+    """
+
+Edge.qr = qr_edge
+
+
 def qr_(edge) -> Tuple[Node, Node]:
     r"""
+    In-place version of :func:`qr`.
+    
     Contracts an edge in-place via :func:`contract_` and splits it in-place via
     :func:`split_` using ``mode = "qr"``. See :func:`split` for a more complete
     explanation.
 
     Following the **PyTorch** convention, names of functions ended with an
     underscore indicate **in-place** operations.
     
     Nodes ``resultant`` from this operation use the same names as the original
     nodes connected by ``edge``.
+    
+    This operation is the same as :meth:`~Edge.qr_`.
 
     Parameters
     ----------
     edge : Edge
         Edge whose nodes are to be contracted and split.
 
     Returns
@@ -2078,14 +2632,16 @@
     ['left', 'right', 'batch']
     
     >>> print(nodeB.axes_names)
     ['left', 'right', 'batch']
     """
     if edge.is_dangling():
         raise ValueError('Edge should be connected to perform SVD')
+    if edge.node1 is edge.node2:
+        raise ValueError('Edge should connect different nodes')
 
     node1, node2 = edge.node1, edge.node2
     node1_name, node2_name = node1._name, node2._name
     axis1, axis2 = edge.axis1, edge.axis2
 
     batch_axes = []
     for axis in node1._axes:
@@ -2136,16 +2692,18 @@
 
     return new_node1, new_node2
 
 
 qr_edge_ = copy_func(qr_)
 qr_edge_.__doc__ = \
     r"""
-    Contracts an edge in-place via :func:`~Edge.contract_` and splits
-    it in-place via :func:`~AbstractNode.split_` using ``mode = "qr"``. See
+    In-place version of :meth:`~Edge.qr`.
+    
+    Contracts an edge in-place via :meth:`~Edge.contract_` and splits
+    it in-place via :meth:`~AbstractNode.split_` using ``mode = "qr"``. See
     :func:`split` for a more complete explanation.
     
     Following the **PyTorch** convention, names of functions ended with an
     underscore indicate **in-place** operations.
     
     Nodes ``resultant`` from this operation use the same names as the original
     nodes connected by ``self``.
@@ -2178,25 +2736,173 @@
     >>> print(nodeB.axes_names)
     ['left', 'right', 'batch']
     """
 
 Edge.qr_ = qr_edge_
 
 
+def rq(edge: Edge) -> Tuple[Node, Node]:
+    r"""
+    Contracts an edge via :func:`contract` and splits it via :func:`split`
+    using ``mode = "rq"``. See :func:`split` for a more complete explanation.
+    
+    This operation is the same as :meth:`~Edge.rq`.
+
+    Parameters
+    ----------
+    edge : Edge
+        Edge whose nodes are to be contracted and split.
+
+    Returns
+    -------
+    tuple[Node, Node]
+    
+    Examples
+    --------
+    >>> nodeA = tk.randn(shape=(10, 15, 100),
+    ...                  axes_names=('left', 'right', 'batch'),
+    ...                  name='nodeA')
+    >>> nodeB = tk.randn(shape=(15, 20, 100),
+    ...                  axes_names=('left', 'right', 'batch'),
+    ...                  name='nodeB')
+    ...
+    >>> new_edge = nodeA['right'] ^ nodeB['left']
+    >>> new_nodeA, new_nodeB = tk.rq(new_edge)
+    ...
+    >>> new_nodeA.shape
+    torch.Size([10, 10, 100])
+    
+    >>> new_nodeB.shape
+    torch.Size([10, 20, 100])
+    
+    >>> print(new_nodeA.axes_names)
+    ['left', 'right', 'batch']
+    
+    >>> print(new_nodeB.axes_names)
+    ['left', 'right', 'batch']
+    
+    Original nodes still exist in the network
+    
+    >>> assert nodeA.network == new_nodeA.network
+    >>> assert nodeB.network == new_nodeB.network
+    """
+    if edge.is_dangling():
+        raise ValueError('Edge should be connected to perform SVD')
+    if edge.node1 is edge.node2:
+        raise ValueError('Edge should connect different nodes')
+
+    node1, node2 = edge.node1, edge.node2
+    axis1, axis2 = edge.axis1, edge.axis2
+
+    batch_axes = []
+    for axis in node1._axes:
+        if axis._batch and (axis._name in node2.axes_names):
+            batch_axes.append(axis)
+
+    n_batches = len(batch_axes)
+    n_axes1 = len(node1._axes) - n_batches - 1
+    n_axes2 = len(node2._axes) - n_batches - 1
+
+    contracted = edge.contract()
+    new_node1, new_node2 = split(node=contracted,
+                                 node1_axes=list(
+                                     range(n_batches,
+                                         n_batches + n_axes1)),
+                                 node2_axes=list(
+                                     range(n_batches + n_axes1,
+                                         n_batches + n_axes1 + n_axes2)),
+                                 mode='rq')
+
+    # new_node1
+    prev_nums = [ax.num for ax in batch_axes]
+    for i in range(new_node1.rank):
+        if (i not in prev_nums) and (i != axis1._num):
+            prev_nums.append(i)
+    prev_nums += [axis1._num]
+
+    if prev_nums != list(range(new_node1.rank)):
+        permutation = inverse_permutation(prev_nums)
+        new_node1 = new_node1.permute(permutation)
+
+    # new_node2
+    prev_nums = [node2.get_axis_num(node1.get_axis(ax)._name)
+                 for ax in batch_axes] + [axis2._num]
+    for i in range(new_node2.rank):
+        if i not in prev_nums:
+            prev_nums.append(i)
+
+    if prev_nums != list(range(new_node2.rank)):
+        permutation = inverse_permutation(prev_nums)
+        new_node2 = new_node2.permute(permutation)
+        
+    new_node1.get_axis(axis1._num).name = axis1._name
+    new_node2.get_axis(axis2._num).name = axis2._name
+
+    return new_node1, new_node2
+
+
+rq_edge = copy_func(rq)
+rq_edge.__doc__ = \
+    r"""
+    Contracts an edge via :meth:`~Edge.contract` and splits it via
+    :meth:`~AbstractNode.split` using ``mode = "rq"``. See :func:`split` for
+    a more complete explanation.
+
+    Returns
+    -------
+    tuple[Node, Node]
+    
+    Examples
+    --------
+    >>> nodeA = tk.randn(shape=(10, 15, 100),
+    ...                  axes_names=('left', 'right', 'batch'),
+    ...                  name='nodeA')
+    >>> nodeB = tk.randn(shape=(15, 20, 100),
+    ...                  axes_names=('left', 'right', 'batch'),
+    ...                  name='nodeB')
+    ...
+    >>> new_edge = nodeA['right'] ^ nodeB['left']
+    >>> new_nodeA, new_nodeB = new_edge.rq()
+    ...
+    >>> new_nodeA.shape
+    torch.Size([10, 10, 100])
+    
+    >>> new_nodeB.shape
+    torch.Size([10, 20, 100])
+    
+    >>> print(new_nodeA.axes_names)
+    ['left', 'right', 'batch']
+    
+    >>> print(new_nodeB.axes_names)
+    ['left', 'right', 'batch']
+    
+    Original nodes still exist in the network
+    
+    >>> assert nodeA.network == new_nodeA.network
+    >>> assert nodeB.network == new_nodeB.network
+    """
+
+Edge.rq = rq_edge
+
+
 def rq_(edge) -> Tuple[Node, Node]:
     r"""
+    In-place version of :func:`rq`.
+    
     Contracts an edge in-place via :func:`contract_` and splits it in-place via
     :func:`split_` using ``mode = "rq"``. See :func:`split` for a more complete
     explanation.
 
     Following the **PyTorch** convention, names of functions ended with an
     underscore indicate **in-place** operations.
     
     Nodes ``resultant`` from this operation use the same names as the original
     nodes connected by ``edge``.
+    
+    This operation is the same as :meth:`~Edge.rq_`.
 
     Parameters
     ----------
     edge : Edge
         Edge whose nodes are to be contracted and split.
 
     Returns
@@ -2225,14 +2931,16 @@
     ['left', 'right', 'batch']
     
     >>> print(nodeB.axes_names)
     ['left', 'right', 'batch']
     """
     if edge.is_dangling():
         raise ValueError('Edge should be connected to perform SVD')
+    if edge.node1 is edge.node2:
+        raise ValueError('Edge should connect different nodes')
 
     node1, node2 = edge.node1, edge.node2
     node1_name, node2_name = node1._name, node2._name
     axis1, axis2 = edge.axis1, edge.axis2
 
     batch_axes = []
     for axis in node1._axes:
@@ -2283,16 +2991,18 @@
 
     return new_node1, new_node2
 
 
 rq_edge_ = copy_func(rq_)
 rq_edge_.__doc__ = \
     r"""
-    Contracts an edge in-place via :func:`~Edge.contract_` and splits
-    it in-place via :func:`~AbstractNode.split_` using ``mode = "qr"``. See
+    In-place version of :meth:`~Edge.rq`.
+    
+    Contracts an edge in-place via :meth:`~Edge.contract_` and splits
+    it in-place via :meth:`~AbstractNode.split_` using ``mode = "qr"``. See
     :func:`split` for a more complete explanation.
     
     Following the **PyTorch** convention, names of functions ended with an
     underscore indicate **in-place** operations.
     
     Nodes ``resultant`` from this operation use the same names as the original
     nodes connected by ``self``.
@@ -2326,14 +3036,15 @@
     ['left', 'right', 'batch']
     """
 
 Edge.rq_ = rq_edge_
 
 
 ################################   CONTRACT    ################################
+# MARK: contract_edges
 def _check_first_contract_edges(edges: Optional[List[Edge]],
                                 node1: AbstractNode,
                                 node2: AbstractNode) -> Optional[Successor]:
     args = (None if edges is None else tuple(edges), node1, node2)
     successors = node1._successors.get('contract_edges')
     if successors is None:
         return None
@@ -2678,23 +3389,95 @@
     >>> result2 = tk.contract_edges([result['two_0']], result, result)
     >>> result2.shape
     torch.Size([])
     """
     return contract_edges_op(edges, node1, node2)
 
 
+def contract(edge: Edge) -> Node:
+    """
+    Contracts the nodes that are connected through the edge.
+    
+    Nodes ``resultant`` from this operation are called ``"contract_edges"``.
+    The node that keeps information about the :class:`Successor` is
+    ``edge.node1``.
+    
+    This operation is the same as :meth:`~Edge.contract`.
+
+    Parameters
+    ----------
+    edge : Edge
+        Edge that is to be contracted. Batch contraction is automatically
+        performed when both nodes have batch edges with the same names.
+
+    Returns
+    -------
+    Node
+    
+    Examples
+    --------
+    >>> nodeA = tk.randn(shape=(10, 15, 20),
+    ...                  axes_names=('one', 'two', 'three'),
+    ...                  name='nodeA')
+    >>> nodeB = tk.randn(shape=(10, 15, 20),
+    ...                  axes_names=('one', 'two', 'three'),
+    ...                  name='nodeB')
+    ...
+    >>> _ = nodeA['one'] ^ nodeB['one']
+    >>> _ = nodeA['two'] ^ nodeB['two']
+    >>> _ = nodeA['three'] ^ nodeB['three']
+    >>> result = tk.contract(nodeA['one'])
+    >>> result.shape
+    torch.Size([15, 20, 15, 20])
+    """
+    return contract_edges_op([edge], edge.node1, edge.node2)
+
+contract_edge = copy_func(contract)
+contract_edge.__doc__ = \
+    """
+    Contracts the nodes that are connected through the edge.
+    
+    Nodes ``resultant`` from this operation are called ``"contract_edges"``.
+    The node that keeps information about the :class:`Successor` is
+    ``self.node1``.
+
+    Returns
+    -------
+    Node
+    
+    Examples
+    --------
+    >>> nodeA = tk.randn(shape=(10, 15, 20),
+    ...                  axes_names=('one', 'two', 'three'),
+    ...                  name='nodeA')
+    >>> nodeB = tk.randn(shape=(10, 15, 20),
+    ...                  axes_names=('one', 'two', 'three'),
+    ...                  name='nodeB')
+    ...
+    >>> _ = nodeA['one'] ^ nodeB['one']
+    >>> _ = nodeA['two'] ^ nodeB['two']
+    >>> _ = nodeA['three'] ^ nodeB['three']
+    >>> result = nodeA['one'].contract()
+    >>> result.shape
+    torch.Size([15, 20, 15, 20])
+    """
+
+Edge.contract = contract_edge
+
+
 def contract_(edge: Edge) -> Node:
     """
-    Contracts in-place the nodes that are connected through the edge. See
-    :func:`contract` for a more complete explanation.
+    In-place version of :func:`contract`.
 
     Following the **PyTorch** convention, names of functions ended with an
     underscore indicate **in-place** operations.
     
     Nodes ``resultant`` from this operation are called ``"contract_edges_ip"``.
+    
+    This operation is the same as :meth:`~Edge.contract_`.
 
     Parameters
     ----------
     edge : Edge
         Edges that is to be contracted. Batch contraction is automatically
         performed when both nodes have batch edges with the same names.
 
@@ -2725,43 +3508,88 @@
     
     >>> nodeB.network is None
     True
     
     >>> del nodeA
     >>> del nodeB
     """
-    result = contract_edges([edge], edge.node1, edge.node2)
-    result.reattach_edges(True)
+    nodes = [edge.node1, edge.node2]
+    result = contract_edges_op([edge], nodes[0], nodes[1])
+    result.reattach_edges(override=True)
     result._unrestricted_set_tensor(result.tensor.detach())
+    
+    nodes = set(nodes)
 
     # Delete nodes (and their edges) from the TN
     net = result.network
-    net.delete_node(edge.node1)
-    net.delete_node(edge.node2)
+    for node in nodes:
+        net.delete_node(node)
 
     # Add edges of result to the TN
     for res_edge in result._edges:
         net._add_edge(res_edge)
 
     # Transform resultant to leaf nodes
     result._leaf = True
     del net._resultant_nodes[result._name]
     net._leaf_nodes[result._name] = result
-
-    edge.node1._successors = dict()
-    edge.node2._successors = dict()
+    
+    for node in nodes:
+        node._successors = dict()
     net._seq_ops = []
 
     # Remove resultant name
     result.name = 'contract_edges_ip'
 
     return result
 
 
-Edge.contract_ = contract_
+contract_edge_ = copy_func(contract_)
+contract_edge_.__doc__ = \
+    """
+    In-place version of :meth:`~Edge.contract`.
+
+    Following the **PyTorch** convention, names of functions ended with an
+    underscore indicate **in-place** operations.
+    
+    Nodes ``resultant`` from this operation are called ``"contract_edges_ip"``.
+
+    Returns
+    -------
+    Node
+    
+    Examples
+    --------
+    >>> nodeA = tk.randn(shape=(10, 15, 20),
+    ...                  axes_names=('one', 'two', 'three'),
+    ...                  name='nodeA')
+    >>> nodeB = tk.randn(shape=(10, 15, 20),
+    ...                  axes_names=('one', 'two', 'three'),
+    ...                  name='nodeB')
+    ...
+    >>> _ = nodeA['one'] ^ nodeB['one']
+    >>> _ = nodeA['two'] ^ nodeB['two']
+    >>> _ = nodeA['three'] ^ nodeB['three']
+    >>> result = nodeA['one'].contract_()
+    >>> result.shape
+    torch.Size([15, 20, 15, 20])
+    
+    ``nodeA`` and ``nodeB`` have been removed from the network.
+    
+    >>> nodeA.network is None
+    True
+    
+    >>> nodeB.network is None
+    True
+    
+    >>> del nodeA
+    >>> del nodeB
+    """
+
+Edge.contract_ = contract_edge_
 
 
 def get_shared_edges(node1: AbstractNode,
                      node2: AbstractNode) -> List[Edge]:
     """Returns list of edges shared between two nodes."""
     edges = set()
     for i1, edge1 in enumerate(node1._edges):
@@ -2774,18 +3602,20 @@
 
 
 def contract_between(node1: AbstractNode,
                      node2: AbstractNode) -> Node:
     """
     Contracts all edges shared between two nodes. Batch contraction is
     automatically performed when both nodes have batch edges with the same
-    names.
+    names. It can also be performed using the operator ``@``.
     
     Nodes ``resultant`` from this operation are called ``"contract_edges"``.
     The node that keeps information about the :class:`Successor` is ``node1``.
+    
+    This operation is the same as :meth:`~AbstractNode.contract_between`.
 
     Parameters
     ----------
     node1 : AbstractNode
         First node of the contraction. Its non-contracted edges will appear
         first in the list of inherited edges of the resultant node.
     node2 : AbstractNode
@@ -2806,15 +3636,15 @@
     ...                  name='nodeB')
     ...
     >>> _ = nodeA['right'] ^ nodeB['left']
     >>> result = tk.contract_between(nodeA, nodeB)
     >>> result.shape
     torch.Size([100, 10, 7])
     """
-    return contract_edges(None, node1, node2)
+    return contract_edges_op(None, node1, node2)
 
 
 contract_between_node = copy_func(contract_between)
 contract_between_node.__doc__ = \
     """
     Contracts all edges shared between two nodes. Batch contraction is
     automatically performed when both nodes have batch edges with the same
@@ -2857,14 +3687,16 @@
     """
     In-place version of :func:`contract_between`.
 
     Following the **PyTorch** convention, names of functions ended with an
     underscore indicate **in-place** operations.
     
     Nodes ``resultant`` from this operation are called ``"contract_edges_ip"``.
+    
+    This operation is the same as :meth:`~AbstractNode.contract_between_`.
 
     Parameters
     ----------
     node1 : AbstractNode
         First node of the contraction. Its non-contracted edges will appear
         first in the list of inherited edges of the resultant node.
     node2 : AbstractNode
@@ -2897,33 +3729,35 @@
     >>> nodeB.network is None
     True
     
     >>> del nodeA
     >>> del nodeB
     """
     result = contract_between(node1, node2)
-    result.reattach_edges(True)
+    result.reattach_edges(override=True)
     result._unrestricted_set_tensor(result.tensor.detach())
+    
+    nodes = set([node1, node2])
 
     # Delete nodes (and their edges) from the TN
     net = result.network
-    net.delete_node(node1)
-    net.delete_node(node2)
+    for node in nodes:
+        net.delete_node(node)
 
     # Add edges of result to the TN
     for res_edge in result._edges:
         net._add_edge(res_edge)
 
     # Transform resultant to leaf nodes
     result._leaf = True
     del net._resultant_nodes[result._name]
     net._leaf_nodes[result._name] = result
-
-    node1._successors = dict()
-    node2._successors = dict()
+    
+    for node in nodes:
+        node._successors = dict()
     net._seq_ops = []
 
     # Remove resultant name
     result.name = 'contract_edges_ip'
 
     return result
 
@@ -2974,14 +3808,15 @@
     >>> del nodeB
     """
 
 AbstractNode.contract_between_ = contract_between_node_
 
 
 #####################################   STACK   ###############################
+# MARK: stack
 def _check_first_stack(nodes: Sequence[AbstractNode]) -> Optional[Successor]:
     if not nodes:
         raise ValueError('`nodes` should be a non-empty sequence of nodes')
     
     args = (tuple(nodes),)
     successors = nodes[0]._successors.get('stack')
     if not successors:
@@ -2996,15 +3831,15 @@
     all_same_ref = True       # Check if all the nodes' memories are stored in
                               # the same reference node's memory
     node_ref_is_stack = True  # Check if the shared reference node is a stack
     stack_node_ref = None     # In the case above, the reference node
     stack_indices = []        # In the case above, stack indices of each node in
                               # the reference node's memory
 
-    if not (isinstance(nodes, (list, tuple)) and isinstance(nodes[0], AbstractNode)):
+    if not (isinstance(nodes, Sequence) and isinstance(nodes[0], AbstractNode)):
         raise TypeError('`nodes` should be a list or tuple of AbstractNodes')
 
     net = nodes[0]._network
     for node in nodes:
         if not node._leaf:
             all_leaf = False
 
@@ -3024,23 +3859,27 @@
                         all_same_ref = False
                         continue
 
                 if not isinstance(node_ref, (StackNode, ParamStackNode)):
                     all_same_ref = False
                     node_ref_is_stack = False
                     continue
-
-                stack_indices.append(node._tensor_info['index'][0])
+                
+                aux_index = node._tensor_info['index']
+                if isinstance(aux_index, int):
+                    stack_indices.append(aux_index)
+                else:
+                    stack_indices.append(aux_index[0])
 
             else:
                 all_same_ref = False
 
     if all_param and node_ref_is_stack and net._auto_stack:
         stack_node = ParamStackNode(nodes=nodes,
-                                    name='virtual_stack',
+                                    name='virtual_result_stack',
                                     virtual=True)
     else:
         stack_node = StackNode._create_resultant(nodes=nodes,
                                                  name='stack')
         
     # Stack nodes' tensors
     nodes_tensors = [node.tensor for node in nodes]
@@ -3190,17 +4029,17 @@
     
     See :class:`ParamStackNode` and :class:`TensorNetwork` to learn how the
     :meth:`~TensorNetwork.auto_stack` mode affects the computation of
     :func:`stack`.
     
     Nodes ``resultant`` from this operation are called ``"stack"``. If this
     operation returns a ``virtual`` :class:`ParamStackNode`, it will be called
-    ``"virtual_stack"``. See :class:AbstractNode` to learn about this **reserved
-    name**.  The node that keeps information about the :class:`Successor` is
-    ``nodes[0]``, the first stacked node.
+    ``"virtual_result_stack"``. See :class:AbstractNode` to learn about this
+    **reserved name**.  The node that keeps information about the
+    :class:`Successor` is ``nodes[0]``, the first stacked node.
 
     Parameters
     ----------
     nodes : list[AbstractNode] or tuple[AbstractNode]
         Sequence of nodes that are to be stacked. They must be of the same type,
         have the same rank and axes names, be in the same tensor network, and
         have edges with the same types.
@@ -3216,14 +4055,15 @@
     >>> stack_node.shape
     torch.Size([10, 2, 4, 2])
     """
     return stack_op(nodes)
 
 
 ##################################   UNBIND   #################################
+# MARK: unbind
 def _check_first_unbind(node: AbstractStackNode) -> Optional[Successor]:
     args = (node,)
     successors = node._successors.get('unbind')
     if not successors:
         return None
     return successors.get(args)
 
@@ -3245,15 +4085,21 @@
             node1_lists.append(edge._node1_list)
             if edge.is_batch():
                 # Save position of batch edge, whose dimension might change
                 batch_ids.append(i)
         else:
             edges_lists.append([edge] * len(tensors))
             node1_lists.append([True] * len(tensors))
-    lst = list(zip(tensors, list(zip(*edges_lists)), list(zip(*node1_lists))))
+    
+    if node._edges[1:]:
+        lst = list(zip(tensors,
+                       list(zip(*edges_lists)),
+                       list(zip(*node1_lists))))
+    else:
+        lst = [(t, [], []) for t in tensors]
 
     net = node._network
     for i, (tensor, edges, node1_list) in enumerate(lst):
         new_node = Node._create_resultant(axes_names=node.axes_names[1:],
                                           name='unbind',
                                           network=net,
                                           tensor=tensor,
@@ -3304,15 +4150,14 @@
                 for j, (max_dim, dim) in enumerate(zip(node._shape[1:],
                                                        new_node._shape)):
                     if new_node._axes[j]._batch:
                         # Admit any size in batch edges
                         index.append(slice(0, None))
                     else:
                         index.append(slice(max_dim - dim, max_dim))
-                new_node._tensor_info['index'] = index
 
             else:
                 node_index = node._tensor_info['index']
                 aux_slice = node_index[0]
                 if isinstance(aux_slice, list):
                     index = [aux_slice[i]]
                 else:
@@ -3329,23 +4174,25 @@
                             index.append(slice(0, None))
                         else:
                             index.append(slice(aux_slice.stop - dim,
                                                aux_slice.stop))
 
                 else:
                     # If node has the same shape as the original stack
-                    for j, (max_dim, dim) in enumerate(zip(node.shape[1:],
+                    for j, (max_dim, dim) in enumerate(zip(node._shape[1:],
                                                            new_node._shape)):
                         if new_node._axes[j]._batch:
                             # Admit any size in batch edges
                             index.append(slice(0, None))
                         else:
                             index.append(slice(max_dim - dim, max_dim))
 
-                new_node._tensor_info['index'] = index
+            if len(index) == 1:
+                index = index[0]
+            new_node._tensor_info['index'] = index
 
     # Create successor
     args = (node,)
     successor = Successor(node_ref=node.node_ref(),
                           index=node._tensor_info['index'],
                           child=new_nodes,
                           hints={'batch_ids': batch_ids,
@@ -3466,15 +4313,72 @@
 
     >>> result[0].shape
     torch.Size([2, 2])
     """
     return unbind_op(node)
 
 
+unbind_node = copy_func(unbind)
+unbind_node.__doc__ = \
+    """
+    Unbinds a :class:`StackNode` or :class:`ParamStackNode`, where the first
+    dimension is assumed to be the stack dimension.
+
+    If :meth:`~TensorNetwork.auto_unbind` is set to ``False``, each resultant
+    node will store its own tensor. Otherwise, they will have only a reference
+    to the corresponding slice of the ``(Param)StackNode``.
+    
+    See :class:`TensorNetwork` to learn how the ``auto_unbind`` mode affects
+    the computation of :func:`unbind`.
+    
+    Nodes ``resultant`` from this operation are called ``"unbind"``. The node
+    that keeps information about the :class:`Successor` is ``self``.
+
+    Returns
+    -------
+    list[Node]
+    
+    Examples
+    --------
+    >>> net = tk.TensorNetwork()
+    >>> nodes = [tk.randn(shape=(2, 4, 2),
+    ...                   axes_names=('left', 'input', 'right'),
+    ...                   network=net)
+    ...          for _ in range(10)]
+    >>> data = [tk.randn(shape=(4,),
+    ...                  axes_names=('feature',),
+    ...                  network=net)
+    ...         for _ in range(10)]
+    ...
+    >>> for i in range(10):
+    ...     _ = nodes[i]['input'] ^ data[i]['feature']
+    ...
+    >>> stack_nodes = tk.stack(nodes)
+    >>> stack_data = tk.stack(data)
+    ...
+    >>> # It is necessary to re-connect stacks
+    >>> _ = stack_nodes['input'] ^ stack_data['feature']
+    >>> result = stack_nodes @ stack_data
+    >>> result = result.unbind()
+    >>> print(result[0].name)
+    unbind_0
+
+    >>> result[0].axes
+    [Axis( left (0) ), Axis( right (1) )]
+
+    >>> result[0].shape
+    torch.Size([2, 2])
+    """
+
+StackNode.unbind = unbind_node
+ParamStackNode.unbind = unbind_node
+
+
 ##################################   EINSUM   #################################
+# MARK: einsum
 def _check_first_einsum(string: Text,
                         *nodes: AbstractNode) -> Optional[Successor]:
     if not nodes:
         raise ValueError('No nodes were provided')
     
     args = (string, *nodes)
     successors = nodes[0]._successors.get('einsum')
```

### Comparing `tensorkrowch-1.0.1/tensorkrowch/utils.py` & `tensorkrowch-1.1.0/tensorkrowch/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,17 +9,19 @@
     * permute_list
     * is_permutation
     * inverse_permutation
     * fact
     * binomial_coeffs
     * stack_unequal_tensors
     * list2slice
+    * split_sequence_into_regions
+    * random_unitary
 """
 
-from typing import List, Sequence, Text, Union
+from typing import Optional, List, Sequence, Text, Union
 
 import torch
 import torch.nn as nn
 
 
 def print_list(lst: List) -> Text:
     return '[' + '\n '.join(f'{item}' for item in lst) + ']'
@@ -248,7 +250,73 @@
                     use_slice = False
                     break
 
     if use_slice:
         aux_slice[1] += 1
         return slice(*aux_slice)
     return lst
+
+def split_sequence_into_regions(lst: Sequence[int]) -> List[List[int]]:
+    """
+    Splits a sequence of integers into regions where each region contains
+    consecutive integers.
+
+    Parameters
+    ----------
+    lst : list[int] or tuple[int]
+        List of integers in ascending order.
+
+    Returns
+    -------
+    list[list[int]]
+
+    Raises
+    ------
+    TypeError
+        If the input is not a sequence of integers.
+    ValueError
+        If the input sequence is not ordered.
+
+    Example
+    -------
+    >>> sequence = [1, 2, 3, 5, 6, 7, 10, 11, 13]
+    >>> split_sequence_into_regions(sequence)
+    [[1, 2, 3], [5, 6, 7], [10, 11], [13]]
+    """
+    if not isinstance(lst, Sequence) or not all(isinstance(x, int) for x in lst):   #TODO: use this in my code
+        raise TypeError('Input must be a sequence of integers')
+    
+    if len(lst) != len(set(lst)):
+        raise ValueError('Input sequence cannot contain repeated elements')
+
+    if any(lst[i + 1] < lst[i] for i in range(len(lst) - 1)):
+        raise ValueError('Input sequence must be in ascending order')
+
+    if not lst:
+        return []
+
+    regions = []
+    current_region = [lst[0]]
+
+    for i in range(1, len(lst)):
+        if lst[i] == lst[i - 1] + 1:
+            current_region.append(lst[i])
+        else:
+            regions.append(current_region)
+            current_region = [lst[i]]
+
+    regions.append(current_region)
+    return regions
+
+def random_unitary(n, device: Optional[torch.device] = None):
+    """
+    Returns random unitary matrix from the Haar measure of size n x n.
+    
+    Unitary matrix is created as described in this `paper
+    <https://arxiv.org/abs/math-ph/0609050v2>`_.
+    """
+    mat = torch.randn(n, n, device=device)
+    q, r = torch.linalg.qr(mat)
+    d = torch.diagonal(r)
+    ph = d / d.abs()
+    q = q @ torch.diag(ph)
+    return q
```

### Comparing `tensorkrowch-1.0.1/tensorkrowch.egg-info/PKG-INFO` & `tensorkrowch-1.1.0/tensorkrowch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorkrowch
-Version: 1.0.1
+Version: 1.1.0
 Summary: Tensor Networks with PyTorch
 Author-email: José Ramón Pareja Monturiol <joserapa98@gmail.com>
 Maintainer-email: José Ramón Pareja Monturiol <joserapa98@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 José Ramón Pareja Monturiol
         
@@ -24,15 +24,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: GitHub, https://github.com/joserapa98/tensorkrowch
 Project-URL: Documentation, https://joserapa98.github.io/tensorkrowch
-Keywords: tensor,network,tensor network,tensor networks,mps,peps,quantum
+Keywords: tensor,network,tensor network,tensor networks,mps,mpo,peps,quantum
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: torch>=1.9
 Requires-Dist: opt_einsum>=3.0
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
@@ -47,16 +47,14 @@
 Requires-Dist: sphinxcontrib-serializinghtml==1.1.5; extra == "docs"
 
 ![logo](https://github.com/joserapa98/tensorkrowch/blob/master/docs/figures/svg/tensorkrowch_logo_dark.svg#gh-dark-mode-only)
 ![logo](https://github.com/joserapa98/tensorkrowch/blob/master/docs/figures/svg/tensorkrowch_logo_light.svg#gh-light-mode-only)
 
 [![DOI](https://zenodo.org/badge/453954432.svg)](https://zenodo.org/badge/latestdoi/453954432)
 
-[![DOI](https://zenodo.org/badge/453954432.svg)](https://zenodo.org/badge/latestdoi/453954432)
-
 # Tensor Networks with PyTorch
 
 **TensorKrowch** is a Python library built on top of **PyTorch** that simplifies
 the training of Tensor Networks as machine learning models and their integration
 into deep learning pipelines.
 
 The primary goal of **TensorKrowch** is to offer an efficient and user-friendly
@@ -168,15 +166,15 @@
 In **TensorKrowch** ``TensorNetworks`` work like **PyTorch** layers. Thus
 creating hybrid neural-tensor network models is straightforward:
 
 ```python
 import torch.nn as nn
 
 my_model = nn.Sequential(
-    tk.models.MPSLayer(n_features=100,
+    tk.models.MPSLayer(n_features=101,
                        in_dim=3,
                        out_dim=10,
                        bond_dim=5),
     nn.ReLU(),
     nn.Linear(10, 10))
 
 data = torch.randn(500, 100, 3)  # batch x n_features x in_dim
```

### Comparing `tensorkrowch-1.0.1/tensorkrowch.egg-info/SOURCES.txt` & `tensorkrowch-1.1.0/tensorkrowch.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -10,12 +10,15 @@
 tensorkrowch/operations.py
 tensorkrowch/utils.py
 tensorkrowch.egg-info/PKG-INFO
 tensorkrowch.egg-info/SOURCES.txt
 tensorkrowch.egg-info/dependency_links.txt
 tensorkrowch.egg-info/requires.txt
 tensorkrowch.egg-info/top_level.txt
+tensorkrowch/decompositions/__init__.py
+tensorkrowch/decompositions/svd_decompositions.py
 tensorkrowch/models/__init__.py
+tensorkrowch/models/mpo.py
 tensorkrowch/models/mps.py
-tensorkrowch/models/mps_layer.py
+tensorkrowch/models/mps_data.py
 tensorkrowch/models/peps.py
 tensorkrowch/models/tree.py
```


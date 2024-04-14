# Comparing `tmp/grapes-0.7.1.tar.gz` & `tmp/grapes-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grapes-0.7.1.tar", last modified: Sun Mar 19 14:27:24 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `grapes-0.7.1.tar` & `grapes-0.8.0.tar`

### file list

```diff
@@ -1,35 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-03-19 14:27:24.930904 grapes-0.7.1/
--rw-rw-rw-   0        0        0      179 2021-08-07 13:40:46.000000 grapes-0.7.1/.gitattributes
--rw-rw-rw-   0        0        0      106 2021-08-07 13:40:46.000000 grapes-0.7.1/.gitignore
--rw-rw-rw-   0        0        0    10347 2021-08-07 13:40:46.000000 grapes-0.7.1/LICENSE.txt
--rw-rw-rw-   0        0        0      566 2021-08-07 13:40:46.000000 grapes-0.7.1/NOTICE.txt
--rw-rw-rw-   0        0        0     2471 2023-03-19 14:27:24.929900 grapes-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     2085 2023-03-19 13:29:16.000000 grapes-0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-19 14:27:24.892899 grapes-0.7.1/grapes/
--rw-rw-rw-   0        0        0       42 2023-03-19 14:09:37.000000 grapes-0.7.1/grapes/__init__.py
--rw-rw-rw-   0        0        0    37901 2023-03-19 13:46:30.000000 grapes-0.7.1/grapes/core.py
--rw-rw-rw-   0        0        0     3786 2023-03-19 13:20:25.000000 grapes-0.7.1/grapes/function_composer.py
--rw-rw-rw-   0        0        0     8772 2023-03-19 13:29:16.000000 grapes-0.7.1/grapes/util.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:27:24.911898 grapes-0.7.1/grapes/visualize/
--rw-rw-rw-   0        0        0       26 2023-03-19 14:18:07.000000 grapes-0.7.1/grapes/visualize/__init__.py
--rw-rw-rw-   0        0        0     4999 2023-03-19 13:46:22.000000 grapes-0.7.1/grapes/visualize/visualize.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:27:24.908899 grapes-0.7.1/grapes.egg-info/
--rw-rw-rw-   0        0        0     2471 2023-03-19 14:27:24.000000 grapes-0.7.1/grapes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      573 2023-03-19 14:27:24.000000 grapes-0.7.1/grapes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-19 14:27:24.000000 grapes-0.7.1/grapes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-05-02 20:46:21.000000 grapes-0.7.1/grapes.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       96 2023-03-19 14:27:24.000000 grapes-0.7.1/grapes.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-19 14:27:24.000000 grapes-0.7.1/grapes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-19 14:27:24.930904 grapes-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1346 2023-03-19 14:25:01.000000 grapes-0.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:27:24.917898 grapes-0.7.1/tests/
-drwxrwxrwx   0        0        0        0 2023-03-19 14:27:24.921898 grapes-0.7.1/tests/data/
--rw-rw-rw-   0        0        0       48 2023-03-19 13:29:16.000000 grapes-0.7.1/tests/data/example.json
--rw-rw-rw-   0        0        0       49 2023-03-19 13:29:16.000000 grapes-0.7.1/tests/data/example.toml
-drwxrwxrwx   0        0        0        0 2023-03-19 14:27:24.927899 grapes-0.7.1/tests/expected/
--rw-rw-rw-   0        0        0    25023 2023-03-19 14:20:31.000000 grapes-0.7.1/tests/expected/expected.pkl
--rw-rw-rw-   0        0        0     2320 2023-01-21 16:49:30.000000 grapes-0.7.1/tests/expected/simple.gv
--rw-rw-rw-   0        0        0    15536 2022-12-26 17:28:57.000000 grapes-0.7.1/tests/expected/simple.gv.pdf
--rw-rw-rw-   0        0        0    18639 2023-03-19 13:29:16.000000 grapes-0.7.1/tests/test_basic.py
--rw-rw-rw-   0        0        0     4053 2023-03-19 14:19:49.000000 grapes-0.7.1/tests/test_graphviz.py
--rw-rw-rw-   0        0        0     7013 2023-03-19 13:29:16.000000 grapes-0.7.1/tests/test_util.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 grapes-0.8.0/grapes/__init__.py
+-rw-r--r--   0        0        0    42807 2020-02-02 00:00:00.000000 grapes-0.8.0/grapes/core.py
+-rw-r--r--   0        0        0     4366 2020-02-02 00:00:00.000000 grapes-0.8.0/grapes/function_composer.py
+-rw-r--r--   0        0        0    10734 2020-02-02 00:00:00.000000 grapes-0.8.0/grapes/util.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 grapes-0.8.0/grapes/visualize/__init__.py
+-rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 grapes-0.8.0/grapes/visualize/visualize.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 grapes-0.8.0/.gitignore
+-rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 grapes-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 grapes-0.8.0/NOTICE.txt
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 grapes-0.8.0/README.md
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 grapes-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 grapes-0.8.0/PKG-INFO
```

### Comparing `grapes-0.7.1/LICENSE.txt` & `grapes-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grapes-0.7.1/NOTICE.txt` & `grapes-0.8.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `grapes-0.7.1/PKG-INFO` & `grapes-0.8.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: grapes
-Version: 0.7.1
-Summary: Helper for dataflow based programming
-Home-page: https://github.com/giuliofoletto/grapes
-Author: Giulio Foletto
-Author-email: giulio.foletto@outlook.com
-License: Apache
-Description-Content-Type: text/markdown
-Provides-Extra: visualize
-Provides-Extra: testing
-License-File: LICENSE.txt
-License-File: NOTICE.txt
-
 # grapes 
 
 A simple library for dataflow programming in python.
 It is inspired by [`pythonflow`](https://github.com/spotify/pythonflow) but with substantial modifications.
 
 ## Dependencies
 The core `grapes` module depends on [`networkx`](https://github.com/networkx/networkx), which can be found on PyPI and is included in the Anaconda distribution.
@@ -49,8 +35,8 @@
 
 * Better explanation of what `grapes` is.
 * Usage examples.
 * Better comments and documentation.
 
 ## Authorship and License
 The bulk of `grapes` development was done by Giulio Foletto in his spare time.
-See `LICENSE.txt` and `NOTICE.txt` for details on how `grapes` is distributed.
+See `LICENSE.txt` and `NOTICE.txt` for details on how `grapes` is distributed.
```

### Comparing `grapes-0.7.1/grapes/core.py` & `grapes-0.8.0/grapes/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 """
 Core of the grapes package. Includes the classes for nodes and graphs.
 
 Author: Giulio Foletto <giulio.foletto@outlook.com>.
 License: See project-level license file.
 """
 
-from typing import ValuesView
-import networkx as nx
-from . import function_composer
+import copy
 import inspect
 
+import networkx as nx
+
+from . import function_composer
 
-starting_node_properties = {"type": "standard", "has_value": False, "value": None, "is_frozen": False, "is_recipe": False, "topological_generation_index": -1, "has_reachability": False, "reachability": None}
+starting_node_properties = {
+    "type": "standard",
+    "has_value": False,
+    "value": None,
+    "is_frozen": False,
+    "is_recipe": False,
+    "topological_generation_index": -1,
+    "has_reachability": False,
+    "reachability": None,
+}
 
 
-class Graph():
+class Graph:
     """
     Class that represents a graph of nodes.
     """
 
     def __init__(self, nx_digraph=None):
         # Internally, we handle a nx_digraph
         if nx_digraph == None:
@@ -40,15 +50,17 @@
         """
         self.set_value(node, value)
 
     def __eq__(self, other):
         """
         Equality check based on all members.
         """
-        return (isinstance(other, self.__class__) and nx.is_isomorphic(self._nxdg, other._nxdg, dict.__eq__, dict.__eq__))
+        return isinstance(other, self.__class__) and nx.is_isomorphic(
+            self._nxdg, other._nxdg, dict.__eq__, dict.__eq__
+        )
 
     def add_step(self, name, recipe=None, *args, **kwargs):
         """
         Interface to add a node to the graph, with all its dependencies.
         """
         # Check that if a node has dependencies, it also has a recipe
         if recipe is None and (len(args) > 0 or len(kwargs.keys()) > 0):
@@ -99,19 +111,23 @@
         Interface to quickly add a step by passing a name and a function.
 
         The recipe node takes the name of the passed function.
         Dependency nodes are built from the args and kwonlyargs of the passed function.
         """
         # Check that the passed recipe is a valid function
         if not inspect.isfunction(recipe):
-            raise TypeError("The passed recipe should be a function, but it is a " + type(recipe))
+            raise TypeError(
+                "The passed recipe should be a function, but it is a " + type(recipe)
+            )
         argspec = inspect.getfullargspec(recipe)
         # varargs and varkw are not supported because add_step_quick needs parameter names to build nodes
         if argspec.varargs is not None or argspec.varkw is not None:
-            raise ValueError("Functions with varargs or varkwargs are not supported by add_step_quick because there would be no way to name dependency nodes")
+            raise ValueError(
+                "Functions with varargs or varkwargs are not supported by add_step_quick because there would be no way to name dependency nodes"
+            )
 
         # Get function name and parameters
         recipe_name = recipe.__name__
         # Lambdas are all automatically named "<lambda>" so we change this
         if recipe_name == "<lambda>":
             recipe_name = "recipe_for_" + name
         args = argspec.args
@@ -123,15 +139,17 @@
         # Directly set the value of recipe_name to recipe
         self.set_value(recipe_name, recipe)
 
     def add_simple_conditional(self, name, condition, value_true, value_false):
         """
         Interface to add a conditional to the graph.
         """
-        self.add_multiple_conditional(name, conditions=[condition], possibilities=[value_true, value_false])
+        self.add_multiple_conditional(
+            name, conditions=[condition], possibilities=[value_true, value_false]
+        )
 
     def add_multiple_conditional(self, name, conditions, possibilities):
         """
         Interface to add a multiple conditional to the graph.
         """
         # Add all nodes and connect all edges
         # Avoid adding existing node so as not to overwrite attributes
@@ -254,15 +272,19 @@
         return self.get_node_attribute(node, "topological_generation_index")
 
     def set_topological_generation_index(self, node, index):
         self.set_node_attribute(node, "topological_generation_index", index)
 
     def get_value(self, node):
         attributes = self.nodes[node]
-        if "value" in attributes and attributes["value"] is not None and self.nodes[node]["has_value"]:
+        if (
+            "value" in attributes
+            and attributes["value"] is not None
+            and self.nodes[node]["has_value"]
+        ):
             return attributes["value"]
         else:
             raise ValueError("Node " + node + " has no value")
 
     def set_value(self, node, value):
         # Note: This changes reachability
         self.nodes[node]["value"] = value
@@ -270,15 +292,19 @@
 
     def unset_value(self, node):
         # Note: This changes reachability
         self.nodes[node]["has_value"] = False
 
     def get_reachability(self, node):
         attributes = self.nodes[node]
-        if "reachability" in attributes and attributes["reachability"] is not None and self.nodes[node]["has_reachability"]:
+        if (
+            "reachability" in attributes
+            and attributes["reachability"] is not None
+            and self.nodes[node]["has_reachability"]
+        ):
             return attributes["reachability"]
         else:
             raise ValueError("Node " + node + " has no reachability")
 
     def set_reachability(self, node, reachability):
         if reachability not in ("unreachable", "uncertain", "reachable"):
             raise ValueError(reachability + " is not a valid reachability value.")
@@ -366,17 +392,23 @@
 
         Parameters
         ----------
         exclude_recipes: bool
             Whether to exclude recipes from the returned dictionary or keep them.
         """
         if exclude_recipes:
-            return {key: self.get_value(key) for key in self.nodes if (self.has_value(key) and not self.is_recipe(key))}
+            return {
+                key: self.get_value(key)
+                for key in self.nodes
+                if (self.has_value(key) and not self.is_recipe(key))
+            }
         else:
-            return {key: self.get_value(key) for key in self.nodes if self.has_value(key)}
+            return {
+                key: self.get_value(key) for key in self.nodes if self.has_value(key)
+            }
 
     def get_list_of_values(self, list_of_keys):
         """
         Get values as list.
 
         Parameters
         ----------
@@ -430,15 +462,19 @@
         Generic interface to evaluate a GenericNode.
         """
         if self.get_type(target) == "standard":
             return self.evaluate_standard(target, continue_on_fail)
         elif self.get_type(target) == "conditional":
             return self.evaluate_conditional(target, continue_on_fail)
         else:
-            raise ValueError("Evaluation of nodes of type " + self.get_type(target) + " is not supported")
+            raise ValueError(
+                "Evaluation of nodes of type "
+                + self.get_type(target)
+                + " is not supported"
+            )
 
     def evaluate_standard(self, node, continue_on_fail=False):
         """
         Evaluate of a node.
         """
         # Check if it already has a value
         if self.has_value(node):
@@ -448,22 +484,27 @@
         for dependency_name in self._nxdg.predecessors(node):
             self.evaluate_target(dependency_name, continue_on_fail)
 
         # Actual computation happens here
         try:
             recipe = self.get_recipe(node)
             func = self.get_value(recipe)
-            res = func(*self.get_list_of_values(self.get_args(node)), **self.get_kwargs_values(self.get_kwargs(node)))
+            res = func(
+                *self.get_list_of_values(self.get_args(node)),
+                **self.get_kwargs_values(self.get_kwargs(node))
+            )
         except Exception as e:
             if continue_on_fail:
                 # Do nothing, we want to keep going
                 return
             else:
                 if len(e.args) > 0:
-                    e.args = ("While evaluating " + node + ": " + str(e.args[0]),) + e.args[1:]
+                    e.args = (
+                        "While evaluating " + node + ": " + str(e.args[0]),
+                    ) + e.args[1:]
                 raise
         # Save results
         self.set_value(node, res)
 
     def evaluate_conditional(self, conditional, continue_on_fail=False):
         """
         Evaluate a conditional.
@@ -541,15 +582,19 @@
         Generic interface to find the reachability of a GenericNode.
         """
         if self.get_type(target) == "standard":
             return self.find_reachability_standard(target)
         elif self.get_type(target) == "conditional":
             return self.find_reachability_conditional(target)
         else:
-            raise ValueError("Finding the reachability of nodes of type " + self.get_type(target) + " is not supported")
+            raise ValueError(
+                "Finding the reachability of nodes of type "
+                + self.get_type(target)
+                + " is not supported"
+            )
 
     def find_reachability_standard(self, node):
         """
         Find the reachability of a standard node.
         """
         # Check if it already has a reachability
         if self.has_reachability(node):
@@ -593,26 +638,47 @@
             # If all conditions and possibilities are reachable -> reachable
             # If all conditions and possibilities are unreachable -> unreachable
             # If some conditions are reachable or uncertain but the corresponding possibilities are all unreachable -> unreachable
             # In all other cases -> uncertain
             self.find_reachability_targets(*self.get_conditions(conditional))
             self.find_reachability_targets(*self.get_possibilities(conditional))
 
-            if self.get_worst_reachability(*(self.get_conditions(conditional)+self.get_possibilities(conditional))) == "reachable":
+            if (
+                self.get_worst_reachability(
+                    *(
+                        self.get_conditions(conditional)
+                        + self.get_possibilities(conditional)
+                    )
+                )
+                == "reachable"
+            ):
                 # All conditions and possibilities are reachable -> reachable
                 self.set_reachability(conditional, "reachable")
-            elif self.get_best_reachability(*(self.get_conditions(conditional)+self.get_possibilities(conditional))) == "unreachable":
+            elif (
+                self.get_best_reachability(
+                    *(
+                        self.get_conditions(conditional)
+                        + self.get_possibilities(conditional)
+                    )
+                )
+                == "unreachable"
+            ):
                 # All conditions and possibilities are unreachable -> unreachable
                 self.set_reachability(conditional, "unreachable")
             else:
                 not_unreachable_condition_possibilities = []
                 for index, condition in enumerate(self.get_conditions(conditional)):
                     if self.get_reachability(condition) != "unreachable":
-                        not_unreachable_condition_possibilities.append(self.get_possibilities(conditional)[index])
-                if self.get_best_reachability(*not_unreachable_condition_possibilities) == "unreachable":
+                        not_unreachable_condition_possibilities.append(
+                            self.get_possibilities(conditional)[index]
+                        )
+                if (
+                    self.get_best_reachability(*not_unreachable_condition_possibilities)
+                    == "unreachable"
+                ):
                     # All corresponding possibilities are unreachable -> unreachable
                     self.set_reachability(conditional, "unreachable")
                 else:
                     self.set_reachability(conditional, "uncertain")
 
     def get_worst_reachability(self, *nodes):
         list_of_reachabilities = []
@@ -644,24 +710,37 @@
         # If types differ, return False
         if self.get_type(node) != other.get_type(other_node):
             return False
         # If nodes are equal, return True
         if self.nodes[node] == other._nxdg.nodes[other_node]:
             return True
         # If they both have values but they differ, return False. If only one has a value, proceed
-        if self.has_value(node) and other.has_value(other_node) and self.get_value(node) != other.get_value(other_node):
+        if (
+            self.has_value(node)
+            and other.has_value(other_node)
+            and self.get_value(node) != other.get_value(other_node)
+        ):
             # Plot twist! Both are functions and have the same code: proceed
-            if inspect.isfunction(self.get_value(node)) and inspect.isfunction(other.get_value(other_node)) and self.get_value(node).__code__.co_code == other.get_value(other_node).__code__.co_code:
+            if (
+                inspect.isfunction(self.get_value(node))
+                and inspect.isfunction(other.get_value(other_node))
+                and self.get_value(node).__code__.co_code
+                == other.get_value(other_node).__code__.co_code
+            ):
                 pass
             else:
                 return False
         # If they both have dependencies but they differ, return False. If only one has dependencies, proceed
         predecessors = list(self._nxdg.predecessors(node))
         other_predecessors = list(other._nxdg.predecessors(other_node))
-        if len(predecessors) != 0 and len(other_predecessors) != 0 and predecessors != other_predecessors:
+        if (
+            len(predecessors) != 0
+            and len(other_predecessors) != 0
+            and predecessors != other_predecessors
+        ):
             return False
         # Return True if at least one has no dependencies (or they are the same), at least one has no value (or they are the same)
         return True
 
     def is_compatible(self, other):
         """
         Check if self and other can be composed. Currently DAG status is not verified.
@@ -683,45 +762,83 @@
         res = nx.compose(self._nxdg, other._nxdg)
         self._nxdg = res
         # Refresh alias for easy access
         self.nodes = self._nxdg.nodes
 
     def simplify_dependency(self, node_name, dependency_name):
         # Make everything a keyword argument. This is the fate of a simplified node
-        self.get_kwargs(node_name).update({argument: argument for argument in self.get_args(node_name)})
+        self.get_kwargs(node_name).update(
+            {argument: argument for argument in self.get_args(node_name)}
+        )
         # Build lists of dependencies
         func_dependencies = list(self.get_kwargs(node_name).values())
         subfuncs = []
         subfuncs_dependencies = []
         for argument in self.get_kwargs(node_name):
             if argument == dependency_name:
                 if self.get_type(dependency_name) != "standard":
-                    raise TypeError("Simplification only supports standard nodes, while the type of " + dependency_name + " is " + self.get_type(dependency_name))
+                    raise TypeError(
+                        "Simplification only supports standard nodes, while the type of "
+                        + dependency_name
+                        + " is "
+                        + self.get_type(dependency_name)
+                    )
                 if self.get_type(self.get_recipe(dependency_name)) != "standard":
-                    raise TypeError("Simplification only supports standard nodes, while the type of " + self.get_recipe(dependency_name) + " is " + self.get_type(self.get_recipe(dependency_name)))
-                subfuncs.append(self[self.get_recipe(dependency_name)])  # Get python function
-                subfuncs_dependencies.append(list(self.get_args(dependency_name)) + list(self.get_kwargs(dependency_name).values()))
+                    raise TypeError(
+                        "Simplification only supports standard nodes, while the type of "
+                        + self.get_recipe(dependency_name)
+                        + " is "
+                        + self.get_type(self.get_recipe(dependency_name))
+                    )
+                subfuncs.append(
+                    self[self.get_recipe(dependency_name)]
+                )  # Get python function
+                subfuncs_dependencies.append(
+                    list(self.get_args(dependency_name))
+                    + list(self.get_kwargs(dependency_name).values())
+                )
             else:
                 subfuncs.append(function_composer.identity_token)
                 subfuncs_dependencies.append([argument])
         # Compose the functions
-        self[self.get_recipe(node_name)] = function_composer.function_compose_simple(self[self.get_recipe(node_name)], subfuncs, func_dependencies, subfuncs_dependencies)
+        self[self.get_recipe(node_name)] = function_composer.function_compose_simple(
+            self[self.get_recipe(node_name)],
+            subfuncs,
+            func_dependencies,
+            subfuncs_dependencies,
+        )
         # Change edges
         self._nxdg.remove_edge(dependency_name, node_name)
-        for argument in self.get_args(dependency_name) + tuple(self.get_kwargs(dependency_name).values()):
+        for argument in self.get_args(dependency_name) + tuple(
+            self.get_kwargs(dependency_name).values()
+        ):
             self._nxdg.add_edge(argument, node_name, accessor=argument)
         # Update node
         self.set_args(node_name, ())
         new_kwargs = self.get_kwargs(node_name)
-        new_kwargs.update({argument: argument for argument in self.get_args(dependency_name) + tuple(self.get_kwargs(dependency_name).values())})
-        new_kwargs = {key: value for key, value in new_kwargs.items() if value != dependency_name}
+        new_kwargs.update(
+            {
+                argument: argument
+                for argument in self.get_args(dependency_name)
+                + tuple(self.get_kwargs(dependency_name).values())
+            }
+        )
+        new_kwargs = {
+            key: value for key, value in new_kwargs.items() if value != dependency_name
+        }
         self.set_kwargs(node_name, new_kwargs)
 
-    def simplify_all_dependencies(self, node_name, exclude=[]):
-        dependencies = self.get_args(node_name) + tuple(self.get_kwargs(node_name).values())
+    def simplify_all_dependencies(self, node_name, exclude=set()):
+        if not isinstance(exclude, set):
+            exclude = set(exclude)
+        # If a dependency is a source, it cannot be simplified
+        exclude |= self.get_all_sources()
+        dependencies = self.get_args(node_name) + tuple(
+            self.get_kwargs(node_name).values()
+        )
         for dependency in dependencies:
             if dependency not in exclude:
                 self.simplify_dependency(node_name, dependency)
 
     def freeze(self, *args):
         if len(args) == 0:  # Interpret as "Freeze everything"
             nodes_to_freeze = self.nodes
@@ -739,21 +856,28 @@
             nodes_to_unfreeze = args & self.nodes  # Intersection
 
         for key in nodes_to_unfreeze:
             self.set_is_frozen(key, False)
 
     def make_recipe_dependencies_also_recipes(self):
         """
-        Make dependencies (parents) of recipes also recipes
+        Make dependencies (predecessors) of recipes also recipes, if they have only recipe successors
         """
-        # Work in reverse topological order, to get children before parents
+        # Work in reverse topological order, to get successors before predecessors
         for node in reversed(self.get_topological_order()):
             if self.is_recipe(node):
                 for parent in self._nxdg.predecessors(node):
-                    self.set_is_recipe(parent, True)
+                    if not self.is_recipe(parent):
+                        all_children_are_recipes = True
+                        for child in self._nxdg.successors(parent):
+                            if not self.is_recipe(child):
+                                all_children_are_recipes = False
+                                break
+                        if all_children_are_recipes:
+                            self.set_is_recipe(parent, True)
 
     def finalize_definition(self):
         """
         Perform operations that should typically be done after the definition of a graph is completed
 
         Currently, this freezes all values, because it is assumed that values given during definition are to be frozen.
         It also marks dependencies of recipes as recipes themselves.
@@ -796,15 +920,17 @@
         for node in self.nodes:
             if exclude_recipes and self.is_recipe(node):
                 continue
             if self._nxdg.out_degree(node) == 0:
                 sinks.add(node)
         return sinks
 
-    def convert_conditional_to_trivial_step(self, conditional, execute_towards_conditions=False):
+    def convert_conditional_to_trivial_step(
+        self, conditional, execute_towards_conditions=False
+    ):
         """
         Convert a conditional to a trivial step that returns the dependency corresponding to the true condition.
 
         Parameters
         ----------
         conditional: hashable (typically string)
             The name of the conditional node to be converted
@@ -814,33 +940,40 @@
         if execute_towards_conditions:
             self.execute_towards_all_conditions_of_conditional(conditional)
 
         for index, condition in enumerate(self.get_conditions(conditional)):
             if self.has_value(condition) and self.get_value(condition):
                 break
         else:  # Happens if loop is never broken, i.e. when no conditions are true
-            if len(self.get_conditions(conditional)) == len(self.get_possibilities(conditional)) - 1:
+            if (
+                len(self.get_conditions(conditional))
+                == len(self.get_possibilities(conditional)) - 1
+            ):
                 # We assume that the last possibility is considered a default
                 index = -1
             else:
-                raise ValueError("Cannot convert conditional " + conditional + " if no condition is true")
+                raise ValueError(
+                    "Cannot convert conditional "
+                    + conditional
+                    + " if no condition is true"
+                )
         # Get the correct possibility
         selected_possibility = self.get_possibilities(conditional)[index]
 
         # Remove all previous edges (the correct one will be readded later)
         for condition in self.get_conditions(conditional):
             self._nxdg.remove_edge(condition, conditional)
         for possibility in self.get_possibilities(conditional):
             self._nxdg.remove_edge(possibility, conditional)
         # Rewrite node attributes
         nx.set_node_attributes(self._nxdg, {conditional: starting_node_properties})
         # Add a trivial recipe
         recipe = "trivial_recipe_for_" + conditional
         self.set_recipe(conditional, recipe)
-        self.set_args(conditional, [selected_possibility])
+        self.set_args(conditional, (selected_possibility,))
         self.set_kwargs(conditional, dict())
 
         # Add and connect the recipe
         # Avoid adding existing recipe so as not to overwrite attributes
         if recipe not in self.nodes:
             self._nxdg.add_node(recipe, **starting_node_properties)
         self.set_is_recipe(recipe, True)
@@ -857,19 +990,80 @@
         """
         conditionals = set()
         for node in self.nodes:
             if self.get_type(node) == "conditional":
                 conditionals.add(node)
         return conditionals
 
-    def convert_all_conditionals_to_trivial_steps(self, execute_towards_conditions=False):
+    def convert_all_conditionals_to_trivial_steps(
+        self, execute_towards_conditions=False
+    ):
         """
         Convert all conditionals in the graph to trivial steps that return the dependency corresponding to the true condition.
 
         Parameters
         ----------
         execute_towards_conditions: bool
             Whether to execute the graph towards the conditions until one is found true (default: False)
         """
         conditionals = self.get_all_conditionals()
         for conditional in conditionals:
-            self.convert_conditional_to_trivial_step(conditional, execute_towards_conditions)
+            self.convert_conditional_to_trivial_step(
+                conditional, execute_towards_conditions
+            )
+
+    def get_subgraph(self, nodes):
+        h = copy.deepcopy(self)
+        h._nxdg.remove_nodes_from([n for n in self._nxdg if n not in nodes])
+        return h
+
+    def get_all_ancestors_target(self, target):
+        """
+        Get all the ancestors of a node.
+        """
+        return nx.ancestors(self._nxdg, target)
+
+    def get_path_to_target(self, target):
+        """
+        Generic interface to get the path from the last valued nodes to a target.
+        """
+        if self.get_type(target) == "standard":
+            return self.get_path_to_standard(target)
+        elif self.get_type(target) == "conditional":
+            return self.get_path_to_conditional(target)
+        else:
+            raise ValueError(
+                "Getting the ancestors of nodes of type "
+                + self.get_type(target)
+                + " is not supported"
+            )
+
+    def get_path_to_standard(self, node):
+        """
+        Get the path from the last valued nodes to a standard node.
+        """
+        result = set((node,))
+        if self.has_value(node):
+            return result
+        dependencies = self._nxdg.predecessors(node)
+        for dependency in dependencies:
+            result = result | self.get_path_to_target(dependency)
+        return result
+
+    def get_path_to_conditional(self, conditional):
+        """
+        Get the path from the last valued nodes to a conditional node.
+        """
+        result = set((conditional,))
+        if self.has_value(conditional):
+            return result
+        # If not, evaluate the conditions until one is found true
+        for index, condition in enumerate(self.get_conditions(conditional)):
+            if self.has_value(condition) and self.get_value(condition):
+                # A condition is true
+                possibility = self.get_possibilities(conditional)[index]
+                result = result | self.get_path_to_standard(condition)
+                result = result | self.get_path_to_standard(possibility)
+                return result
+        # If no conditions are true, we need to compute them, so all ancestors are in the path
+        result = self.get_path_to_standard(conditional)
+        return result
```

### Comparing `grapes-0.7.1/grapes/function_composer.py` & `grapes-0.8.0/grapes/function_composer.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,15 +11,22 @@
 def identity_token():
     """
     A trivial token that has the only purpose of being identifiable
     """
     pass
 
 
-def function_compose(func, subfuncs, func_dependencies, subfuncs_dependencies, func_signature, subfuncs_signatures):
+def function_compose(
+    func,
+    subfuncs,
+    func_dependencies,
+    subfuncs_dependencies,
+    func_signature,
+    subfuncs_signatures,
+):
     """
     Compose functions.
 
     Parameters
     ----------
     func: callable
         External function
@@ -30,18 +37,41 @@
     subfuncs_dependencies: list of lists of hashables
         Names of the arguments that are passed to the subfuncs when calling the new function (usually they should correspond to node names in a graph)
     func_signature: list of hashables
         Names of the arguments of the old func
     subfuncs_dependencies: list of lists of hashables
         Names of the arguments of the old subfuncs
     """
-    return lambda **kwargs: func(**{func_signature[i]: (subfuncs[i](**{signature_name: kwargs[dependency_name] for signature_name, dependency_name in zip(subfuncs_signatures[i], subfuncs_dependencies[i])}) if subfuncs[i] is not identity_token else kwargs[func_dependencies[i]]) for i in range(len(subfuncs))})
-
-
-def function_compose_simple(func, subfuncs, func_dependencies, subfuncs_dependencies, func_signature=None, subfuncs_signatures=None):
+    return lambda **kwargs: func(
+        **{
+            func_signature[i]: (
+                subfuncs[i](
+                    **{
+                        signature_name: kwargs[dependency_name]
+                        for signature_name, dependency_name in zip(
+                            subfuncs_signatures[i], subfuncs_dependencies[i]
+                        )
+                    }
+                )
+                if subfuncs[i] is not identity_token
+                else kwargs[func_dependencies[i]]
+            )
+            for i in range(len(subfuncs))
+        }
+    )
+
+
+def function_compose_simple(
+    func,
+    subfuncs,
+    func_dependencies,
+    subfuncs_dependencies,
+    func_signature=None,
+    subfuncs_signatures=None,
+):
     """
     Compose functions, without the need to pass signatures, as they are found automatically.
 
     Parameters
     ----------
     func: callable
         External function
@@ -54,23 +84,40 @@
     func_signature: list of hashables
         Names of the arguments of the old func
     subfuncs_dependencies: list of lists of hashables
         Names of the arguments of the old subfuncs
     """
     if func_signature is None:
         if inspect.getfullargspec(func).varargs is not None:
-            raise ValueError("Functions with varargs are not supported by Function Composer")
-        elif inspect.getfullargspec(func).varargs is None and inspect.getfullargspec(func).varkw is None:  # Well defined spec
+            raise ValueError(
+                "Functions with varargs are not supported by Function Composer"
+            )
+        elif (
+            inspect.getfullargspec(func).varargs is None
+            and inspect.getfullargspec(func).varkw is None
+        ):  # Well defined spec
             func_signature = list(inspect.signature(func).parameters.keys())
         else:
             func_signature = func_dependencies
     if subfuncs_signatures is None:
         subfuncs_signatures = []
         for index, subfunc in enumerate(subfuncs):
             if inspect.getfullargspec(func).varargs is not None:
-                raise ValueError("Functions with varargs are not supported by Function Composer")
-            elif inspect.getfullargspec(subfunc).varargs is None and inspect.getfullargspec(subfunc).varkw is None:  # Well defined spec
+                raise ValueError(
+                    "Functions with varargs are not supported by Function Composer"
+                )
+            elif (
+                inspect.getfullargspec(subfunc).varargs is None
+                and inspect.getfullargspec(subfunc).varkw is None
+            ):  # Well defined spec
                 this_signature = list(inspect.signature(subfunc).parameters.keys())
             else:
                 this_signature = subfuncs_dependencies[index]
             subfuncs_signatures.append(this_signature)
-    return function_compose(func, subfuncs, func_dependencies, subfuncs_dependencies, func_signature, subfuncs_signatures)
+    return function_compose(
+        func,
+        subfuncs,
+        func_dependencies,
+        subfuncs_dependencies,
+        func_signature,
+        subfuncs_signatures,
+    )
```

### Comparing `grapes-0.7.1/grapes/util.py` & `grapes-0.8.0/grapes/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """
 Some utilities. Also, a more functional API to the execution of graphs.
 
 Author: Giulio Foletto <giulio.foletto@outlook.com>.
 License: See project-level license file.
 """
 
-import json
 import copy
+import json
+import sys
 import warnings
+
 # Since tomllib is only standard in 3.11, we import tomli in prior versions
-import sys
 if sys.version_info.major >= 3 and sys.version_info.minor >= 11:
     import tomllib
 else:
     import tomli as tomllib
 
 
-def execute_graph_from_context(graph, context, *targets, inplace=False, check_feasibility=True):
+def execute_graph_from_context(
+    graph, context, *targets, inplace=False, check_feasibility=True
+):
     """Execute a graph up to a target given a context.
 
     Parameters
     ----------
     graph : grapes Graph
         Graph of the computation.
     context : dict
@@ -38,19 +41,27 @@
         Graph with context updated after computation.
     """
     # No target is interpreted as compute everything
     if len(targets) == 0:
         targets = graph.get_all_sinks(exclude_recipes=True)
 
     if check_feasibility:
-        feasibility, missing_dependencies = check_feasibility_of_execution(graph, context, *targets, inplace=inplace)
+        feasibility, missing_dependencies = check_feasibility_of_execution(
+            graph, context, *targets, inplace=inplace
+        )
         if feasibility == "unreachable":
-            raise ValueError("The requested computation is unfeasible because of the following missing dependencies: " + ", ".join(missing_dependencies))
+            raise ValueError(
+                "The requested computation is unfeasible because of the following missing dependencies: "
+                + ", ".join(missing_dependencies)
+            )
         elif feasibility == "uncertain":
-            warnings.warn("The feasibility of the requested computation is uncertain because of the following missing dependencies: " + ", ".join(missing_dependencies))
+            warnings.warn(
+                "The feasibility of the requested computation is uncertain because of the following missing dependencies: "
+                + ", ".join(missing_dependencies)
+            )
 
     if not inplace:
         graph = copy.deepcopy(graph)
         context = copy.deepcopy(context)
 
     graph.set_internal_context(context)
     graph.execute_to_targets(*targets)
@@ -75,20 +86,22 @@
     context = graph.get_internal_context(exclude_recipes=True)
     non_serializable_items = {}
     for key, value in context.items():
         try:
             json.dumps(value)
         except:
             non_serializable_items.update({key: str(value)})
-    if len(non_serializable_items) > 0:  # We must copy the context, to preserve it, and dump a modified version of it
+    if (
+        len(non_serializable_items) > 0
+    ):  # We must copy the context, to preserve it, and dump a modified version of it
         res = copy.deepcopy(context)
         res.update(non_serializable_items)
     else:
         res = context
-    return json.dumps(res, sort_keys=True, indent=4, separators=(',', ': '))
+    return json.dumps(res, sort_keys=True, indent=4, separators=(",", ": "))
 
 
 def context_from_json_file(file_name):
     """
     Load a json file into a dictionary.
 
     Parameters
@@ -96,15 +109,15 @@
     file_name: str
         Path to the json file.
 
     Returns
     dict
         Content of the file as dictionary.
     """
-    with open(file_name, encoding='utf-8') as json_file:
+    with open(file_name, encoding="utf-8") as json_file:
         data = json.load(json_file)
     return data
 
 
 def context_from_toml_file(file_name):
     """
     Load a toml file into a dictionary.
@@ -141,18 +154,26 @@
     for func in reading_functions:
         try:
             data = func(file_name)
             return data
         except (json.decoder.JSONDecodeError, tomllib.TOMLDecodeError):
             pass
     # If we arrive here, there has been an issue in all reading functions
-    raise ValueError("File " + file_name + " is not valid in any of the supported formats (" + ",".join(supported_formats) + ")")
+    raise ValueError(
+        "File "
+        + file_name
+        + " is not valid in any of the supported formats ("
+        + ",".join(supported_formats)
+        + ")"
+    )
 
 
-def wrap_graph_with_function(graph, input_keys, *targets, constants={}, input_as_kwargs=True):
+def wrap_graph_with_function(
+    graph, input_keys, *targets, constants={}, input_as_kwargs=True
+):
     # Copy graph so as not to pollute the original
     operational_graph = copy.deepcopy(graph)
     # Pass all constants to the graph
     operational_graph.update_internal_context(constants)
     # Freeze so that the constants are fixed
     operational_graph.freeze()
     # Unfreeze the input.
@@ -164,33 +185,43 @@
     if len(targets) == 0:
         targets = operational_graph.get_all_sinks(exclude_recipes=True)
     # Move as much as possible towards targets
     operational_graph.progress_towards_targets(*targets)
     # Check feasibility
     placeholder_value = 0
     context = {key: placeholder_value for key in input_keys}
-    feasibility, missing_dependencies = check_feasibility_of_execution(operational_graph, context, *targets)
+    feasibility, missing_dependencies = check_feasibility_of_execution(
+        operational_graph, context, *targets
+    )
     if feasibility == "unreachable":
-        raise ValueError("The requested computation is unfeasible because of the following missing dependencies: " + ", ".join(missing_dependencies))
+        raise ValueError(
+            "The requested computation is unfeasible because of the following missing dependencies: "
+            + ", ".join(missing_dependencies)
+        )
     elif feasibility == "uncertain":
-        warnings.warn("The feasibility of the requested computation is uncertain because of the following missing dependencies: " + ", ".join(missing_dependencies))
+        warnings.warn(
+            "The feasibility of the requested computation is uncertain because of the following missing dependencies: "
+            + ", ".join(missing_dependencies)
+        )
 
     if input_as_kwargs:
+
         def specific_function(**kwargs):
             # Use for loop rather than dict comprehension because it is a more basic operation
             for key in input_keys:
                 operational_graph[key] = kwargs[key]
             operational_graph.execute_to_targets(*targets)
             list_of_values = operational_graph.get_list_of_values(targets)
             # Clear values so that the function can be called again
             operational_graph.clear_values()
             if len(list_of_values) == 1:
                 return list_of_values[0]
             else:
                 return list_of_values
+
     else:
         input_keys = list(input_keys)
 
         def specific_function(*args):
             # Use for loop rather than dict comprehension because it is a more basic operation
             for i in range(len(input_keys)):
                 operational_graph[input_keys[i]] = args[i]
@@ -198,26 +229,56 @@
             list_of_values = operational_graph.get_list_of_values(targets)
             # Clear values so that the function can be called again
             operational_graph.clear_values()
             if len(list_of_values) == 1:
                 return list_of_values[0]
             else:
                 return list_of_values
+
     return specific_function
 
 
-def lambdify_graph(graph, input_keys, target):
-    graph = copy.deepcopy(graph)
-    graph.unfreeze()
+def lambdify_graph(graph, input_keys, target, constants={}):
+    # Copy graph so as not to pollute the original
+    operational_graph = copy.deepcopy(graph)
+    # Pass all constants to the graph
+    operational_graph.update_internal_context(constants)
+    # Freeze so that the constants are fixed
+    operational_graph.freeze()
+    # Unfreeze the input.
+    # Note that this has precedence over constants (i.e., if a key is both input and constant, it is treated as input)
     if len(input_keys) > 0:
-        graph.clear_values(*input_keys)
-    graph.progress_towards_targets(target)
-    while not set(graph.get_args(target) + tuple(graph.get_kwargs(target).values())).issubset(set(input_keys)):
-        graph.simplify_all_dependencies(target, exclude=input_keys)
-    return graph[graph.get_recipe(target)]
+        operational_graph.unfreeze(*input_keys)
+        operational_graph.clear_values(*input_keys)
+    # Convert all conditional, progressing to the conditions
+    operational_graph.convert_all_conditionals_to_trivial_steps(
+        execute_towards_conditions=True
+    )
+    # Progress as much as possible
+    operational_graph.progress_towards_targets(target)
+    # The starting point of the computation will include the constants
+    initial_keys = set(input_keys) | set(constants.keys())
+    # Simplify until the graph is a single function
+    while not set(
+        operational_graph.get_args(target)
+        + tuple(operational_graph.get_kwargs(target).values())
+    ).issubset(initial_keys):
+        operational_graph.simplify_all_dependencies(target, exclude=initial_keys)
+    # Get the function representing the graph
+    function = operational_graph[operational_graph.get_recipe(target)]
+    # If needed, get a function only of the input keys
+    if len(constants) > 0:
+
+        def function_only_input_keys(**kwargs):
+            kwargs.update(constants)
+            return function(**kwargs)
+
+        return function_only_input_keys
+    else:
+        return function
 
 
 def check_feasibility_of_execution(graph, context, *targets, inplace=False):
     # No target is interpreted as compute everything
     if len(targets) == 0:
         targets = graph.get_all_sinks(exclude_recipes=True)
 
@@ -228,10 +289,24 @@
     graph.clear_reachabilities()
     graph.set_internal_context(context)
     graph.find_reachability_targets(*targets)
     feasibility = graph.get_worst_reachability(*targets)
     missing_dependencies = set()
     if feasibility in {"unreachable", "uncertain"}:
         for node in graph.nodes:
-            if graph.get_topological_generation_index(node) == 0 and graph.has_reachability(node) and graph.get_reachability(node) != "reachable":
+            if (
+                graph.get_topological_generation_index(node) == 0
+                and graph.has_reachability(node)
+                and graph.get_reachability(node) != "reachable"
+            ):
                 missing_dependencies.add(node)
     return feasibility, missing_dependencies
+
+
+def get_execution_subgraph(graph, context, *targets):
+    graph = copy.deepcopy(graph)
+    context = copy.deepcopy(context)
+    graph.update_internal_context(context)
+    path = set()
+    for target in targets:
+        path = path | graph.get_path_to_target(target)
+    return graph.get_subgraph(path)
```

### Comparing `grapes-0.7.1/grapes/visualize/visualize.py` & `grapes-0.8.0/grapes/visualize/visualize.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 """
 Tools that allow the visualization of a graph using graphviz. Requires pygraphviz.
 
 Author: Giulio Foletto <giulio.foletto@outlook.com>.
 License: See project-level license file.
 """
 
+import matplotlib
 import networkx
-from matplotlib.cm import get_cmap
+
 from .. import *
 
 
-def get_graphviz_digraph(graph, hide_recipes=False, pretty_names=False, include_values=False, color_by_generation=False, colormap="viridis", **attrs):
+def get_graphviz_digraph(
+    graph,
+    hide_recipes=False,
+    pretty_names=False,
+    include_values=False,
+    color_mode="none",
+    colormap="viridis",
+    **attrs,
+):
     # Get a graphviz AGraph
     g = nx.drawing.nx_agraph.to_agraph(graph._nxdg)
     # Add attributes to the AGraph
     g.graph_attr.update(**attrs)
     # Save some values that will be useful later
-    max_topological_generation_index = len(graph.get_topological_generations())-1
-    cmap = get_cmap(colormap)
+    max_topological_generation_index = len(graph.get_topological_generations()) - 1
+    sources = graph.get_all_sources()
+    sinks = graph.get_all_sinks()
+    cmap = matplotlib.colormaps[colormap]
 
     for node_name in g.nodes():
         new_attrs = {}
         node = graph._nxdg.nodes[node_name]
 
         # Remove recipes if needed, or eliminate attribute of function
         if node["is_recipe"] and hide_recipes:
@@ -35,57 +46,78 @@
 
         # Add values to the label if required
         if include_values and node.attr["has_value"]:
             if isinstance(node.attr["value"], float):
                 value_in_label = "{:.2e}".format(node.attr["value"])
             else:
                 value_in_label = str(node.attr["value"])
-            label += "\n" + value_in_label.partition('\n')[0]
+            label += "\n" + value_in_label.partition("\n")[0]
             if value_in_label.find("\n") != -1:
                 label += "\n..."
         new_attrs.update(label=label)
 
         # Manipulate shapes
         if node["is_recipe"]:
             shape = "ellipse"
         elif node["type"] == "conditional":
             shape = "diamond"
         else:
             shape = "box"
         new_attrs.update(shape=shape)
 
         # Manipulate colors
-        if color_by_generation:
-            topological_generation_index = graph.get_node_attribute(node_name, "topological_generation_index")
+        must_be_colored = False
+        if color_mode.lower() == "by_generation":
+            topological_generation_index = graph.get_node_attribute(
+                node_name, "topological_generation_index"
+            )
             # The __call__ method of the colormap returns a tuple of rgba values in [0, 1]
             # We call it passing the ratio between the topological_generation_index of this node and the max of the graph
-            color_rgba = cmap(topological_generation_index/max_topological_generation_index)
+            color_rgba = cmap(
+                topological_generation_index / max_topological_generation_index
+            )
+            must_be_colored = True
+        elif color_mode.lower() == "sources_and_sinks":
+            if node_name in sources:
+                color_rgba = cmap(0.0)
+                must_be_colored = True
+            elif node_name in sinks:
+                color_rgba = cmap(1.0)
+                must_be_colored = True
+        if must_be_colored:
             # Note that graphviz wants colors in hex form
-            new_attrs.update(style="filled", fillcolor=hex_string_from_rgba(*color_rgba), fontcolor=hex_string_from_rgba(*best_text_from_background_color(*color_rgba)))
-
+            new_attrs.update(
+                style="filled",
+                fillcolor=hex_string_from_rgba(*color_rgba),
+                fontcolor=hex_string_from_rgba(
+                    *best_text_from_background_color(*color_rgba)
+                ),
+            )
         # Pass these attributes to the actual AGraph
         g.get_node(node_name).attr.update(new_attrs)
 
         # Handle edge shapes
-        special_dependencies = []
         if node["type"] == "standard" and "recipe" in node:
-            if not hide_recipes:
+            # This condition might be false for example because of hide_recipes
+            if node["recipe"] in g.nodes():
                 g.get_edge(node["recipe"], node_name).attr.update(arrowhead="dot")
-            special_dependencies.append(node["recipe"])
         elif node["type"] == "conditional":
             for condition in node["conditions"]:
-                g.get_edge(condition, node_name).attr.update(arrowhead="diamond")
-            special_dependencies.extend(node["conditions"])
+                if condition in g.nodes():
+                    g.get_edge(condition, node_name).attr.update(arrowhead="diamond")
 
     # Return the AGraph (no layout is computed yet)
     return g
 
 
 def prettify_label(name):
-    return "".join(c.upper() if ((i > 0 and name[i-1] == "_") or i == 0) else c for i, c in enumerate(name)).replace("_", " ")
+    return "".join(
+        c.upper() if ((i > 0 and name[i - 1] == "_") or i == 0) else c
+        for i, c in enumerate(name)
+    ).replace("_", " ")
 
 
 def hex_string_from_rgba(r, g, b, a):
     """
     Get a formatted hex string from RGBA values.
 
     Parameters
@@ -101,19 +133,19 @@
 
     Returns
     -------
     str
         Formatted hex string starting with # and then 8 hex characters (4 bytes).
     """
     # Convert float values in [0, 1] to hex strings of two characters, e.g. 1->ff
-    r_hex = f'{int(r*255):02x}'
-    g_hex = f'{int(g*255):02x}'
-    b_hex = f'{int(b*255):02x}'
-    a_hex = f'{int(a*255):02x}'
-    return u"#" + r_hex + g_hex + b_hex + a_hex
+    r_hex = f"{int(r*255):02x}"
+    g_hex = f"{int(g*255):02x}"
+    b_hex = f"{int(b*255):02x}"
+    a_hex = f"{int(a*255):02x}"
+    return "#" + r_hex + g_hex + b_hex + a_hex
 
 
 def best_text_from_background_color(r, g, b, a=1):
     """
     Get the best text color from background.
 
     Parameters
@@ -128,9 +160,9 @@
         Alpha color channel in [0, 1] (default: 1). This value is ignored.
 
     Returns
     -------
     tuple
         Tuple of RGBA values representing pure white (1, 1, 1, 1) or pure black (0, 0, 0, 1) depending on luminance of input color.
     """
-    luminance = 0.212*r + 0.701*g + 0.087*b
+    luminance = 0.212 * r + 0.701 * g + 0.087 * b
     return (1, 1, 1, 1) if luminance < 0.5 else (0, 0, 0, 1)
```


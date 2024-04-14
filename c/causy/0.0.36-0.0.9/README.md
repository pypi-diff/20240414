# Comparing `tmp/causy-0.0.36.tar.gz` & `tmp/causy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causy-0.0.36.tar", max compression
+gzip compressed data, was "causy-0.0.9.tar", max compression
```

## Comparing `causy-0.0.36.tar` & `causy-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,13 @@
--rw-r--r--   0        0        0     1062 2024-04-14 20:46:36.353726 causy-0.0.36/LICENSE
--rw-r--r--   0        0        0     5645 2024-04-14 20:46:36.353726 causy-0.0.36/README.md
--rw-r--r--   0        0        0      374 2024-04-14 20:46:36.353726 causy-0.0.36/causy/__init__.py
--rw-r--r--   0        0        0       31 2024-04-14 20:46:36.353726 causy-0.0.36/causy/algorithms/__init__.py
--rw-r--r--   0        0        0       96 2024-04-14 20:46:36.353726 causy-0.0.36/causy/algorithms/fci.py
--rw-r--r--   0        0        0     3180 2024-04-14 20:46:36.353726 causy-0.0.36/causy/algorithms/pc.py
--rw-r--r--   0        0        0     2245 2024-04-14 20:46:36.353726 causy-0.0.36/causy/causal_effect_estimation/multivariate_regression.py
--rw-r--r--   0        0        0     3913 2024-04-14 20:46:36.353726 causy-0.0.36/causy/cli.py
--rw-r--r--   0        0        0        0 2024-04-14 20:46:36.353726 causy-0.0.36/causy/common_pipeline_steps/__init__.py
--rw-r--r--   0        0        0     1397 2024-04-14 20:46:36.353726 causy-0.0.36/causy/common_pipeline_steps/calculation.py
--rw-r--r--   0        0        0      806 2024-04-14 20:46:36.353726 causy-0.0.36/causy/common_pipeline_steps/exit_conditions.py
--rw-r--r--   0        0        0     1815 2024-04-14 20:46:36.353726 causy-0.0.36/causy/common_pipeline_steps/logic.py
--rw-r--r--   0        0        0      732 2024-04-14 20:46:36.353726 causy-0.0.36/causy/common_pipeline_steps/placeholder.py
--rw-r--r--   0        0        0     6554 2024-04-14 20:46:36.353726 causy-0.0.36/causy/generators.py
--rw-r--r--   0        0        0    15922 2024-04-14 20:46:36.353726 causy-0.0.36/causy/graph.py
--rw-r--r--   0        0        0    12267 2024-04-14 20:46:36.353726 causy-0.0.36/causy/graph_model.py
--rw-r--r--   0        0        0     1160 2024-04-14 20:46:36.353726 causy-0.0.36/causy/graph_utils.py
--rw-r--r--   0        0        0        0 2024-04-14 20:46:36.353726 causy-0.0.36/causy/independence_tests/__init__.py
--rw-r--r--   0        0        0     7127 2024-04-14 20:46:36.353726 causy-0.0.36/causy/independence_tests/common.py
--rw-r--r--   0        0        0     6686 2024-04-14 20:46:36.353726 causy-0.0.36/causy/interfaces.py
--rw-r--r--   0        0        0      698 2024-04-14 20:46:36.353726 causy-0.0.36/causy/math_utils.py
--rw-r--r--   0        0        0        0 2024-04-14 20:46:36.353726 causy-0.0.36/causy/orientation_rules/__init__.py
--rw-r--r--   0        0        0     3743 2024-04-14 20:46:36.353726 causy-0.0.36/causy/orientation_rules/fci.py
--rw-r--r--   0        0        0    12954 2024-04-14 20:46:36.353726 causy-0.0.36/causy/orientation_rules/pc.py
--rw-r--r--   0        0        0    15360 2024-04-14 20:46:36.353726 causy-0.0.36/causy/sample_generator.py
--rw-r--r--   0        0        0     2141 2024-04-14 20:46:36.353726 causy-0.0.36/causy/serialization.py
--rw-r--r--   0        0        0     7229 2024-04-02 20:42:18.000000 causy-0.0.36/causy/static/assets/index-ce329d65.css
--rw-r--r--   0        0        0   480050 2024-04-02 20:42:18.000000 causy-0.0.36/causy/static/assets/index-d3464cb3.js
--rw-r--r--   0        0        0     3442 2024-04-02 20:42:18.000000 causy-0.0.36/causy/static/assets/style-8961fb08.css
--rw-r--r--   0        0        0     2695 2024-04-02 20:42:18.000000 causy-0.0.36/causy/static/assets/vueflow-3647b393.css
--rw-r--r--   0        0        0     4286 2024-04-02 20:42:18.000000 causy-0.0.36/causy/static/favicon.ico
--rw-r--r--   0        0        0      423 2024-04-02 20:42:18.000000 causy-0.0.36/causy/static/index.html
--rw-r--r--   0        0        0     2568 2024-04-14 20:46:36.353726 causy-0.0.36/causy/ui.py
--rw-r--r--   0        0        0      844 2024-04-14 20:46:36.357726 causy-0.0.36/pyproject.toml
--rw-r--r--   0        0        0     6291 1970-01-01 00:00:00.000000 causy-0.0.36/PKG-INFO
+-rw-r--r--   0        0        0     1202 2023-10-22 12:24:06.291515 causy-0.0.9/README.md
+-rw-r--r--   0        0        0        1 2023-10-22 12:24:06.292007 causy-0.0.9/causy/__init__.py
+-rw-r--r--   0        0        0     2789 2023-10-22 12:24:06.292377 causy-0.0.9/causy/algorithms.py
+-rw-r--r--   0        0        0     4285 2023-10-22 12:24:06.292726 causy-0.0.9/causy/cli.py
+-rw-r--r--   0        0        0      798 2023-10-22 12:24:06.293066 causy-0.0.9/causy/exit_conditions.py
+-rw-r--r--   0        0        0     6072 2023-10-22 12:24:06.293405 causy-0.0.9/causy/generators.py
+-rw-r--r--   0        0        0    19508 2023-10-22 12:24:06.293831 causy-0.0.9/causy/graph.py
+-rw-r--r--   0        0        0    10748 2023-10-22 12:24:06.294233 causy-0.0.9/causy/independence_tests.py
+-rw-r--r--   0        0        0     6778 2023-10-22 12:24:06.294595 causy-0.0.9/causy/interfaces.py
+-rw-r--r--   0        0        0    11462 2023-10-22 12:24:06.295032 causy-0.0.9/causy/orientation_tests.py
+-rw-r--r--   0        0        0     4926 2023-10-22 12:24:06.295413 causy-0.0.9/causy/utils.py
+-rw-r--r--   0        0        0      725 2023-10-22 12:24:06.296713 causy-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1776 1970-01-01 00:00:00.000000 causy-0.0.9/PKG-INFO
```

### Comparing `causy-0.0.36/causy/algorithms/pc.py` & `causy-0.0.9/causy/algorithms.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,55 @@
-from causy.causal_effect_estimation.multivariate_regression import (
-    ComputeDirectEffectsMultivariateRegression,
-)
-from causy.common_pipeline_steps.exit_conditions import ExitOnNoActions
+from causy.exit_conditions import ExitOnNoActions
 from causy.generators import PairsWithNeighboursGenerator, RandomSampleGenerator
-from causy.graph_model import graph_model_factory
-from causy.common_pipeline_steps.logic import Loop
-from causy.independence_tests.common import (
+from causy.graph import graph_model_factory, Loop
+from causy.independence_tests import (
+    CalculateCorrelations,
     CorrelationCoefficientTest,
     PartialCorrelationTest,
     ExtendedPartialCorrelationTestMatrix,
 )
-from causy.common_pipeline_steps.calculation import (
-    CalculatePearsonCorrelations,
-)
 from causy.interfaces import AS_MANY_AS_FIELDS, ComparisonSettings
-from causy.orientation_rules.pc import (
+from causy.orientation_tests import (
     ColliderTest,
     NonColliderTest,
     FurtherOrientTripleTest,
     OrientQuadrupleTest,
     FurtherOrientQuadrupleTest,
 )
 
 PC = graph_model_factory(
     pipeline_steps=[
-        CalculatePearsonCorrelations(),
-        CorrelationCoefficientTest(threshold=0.05),
-        PartialCorrelationTest(threshold=0.05),
-        ExtendedPartialCorrelationTestMatrix(threshold=0.05),
+        CalculateCorrelations(),
+        CorrelationCoefficientTest(threshold=0.01),
+        PartialCorrelationTest(threshold=0.01),
+        ExtendedPartialCorrelationTestMatrix(threshold=0.01),
         ColliderTest(),
         Loop(
             pipeline_steps=[
                 NonColliderTest(),
                 FurtherOrientTripleTest(),
                 OrientQuadrupleTest(),
                 FurtherOrientQuadrupleTest(),
             ],
             exit_condition=ExitOnNoActions(),
         ),
-        ComputeDirectEffectsMultivariateRegression(),
     ]
 )
 
 
 ParallelPC = graph_model_factory(
     pipeline_steps=[
-        CalculatePearsonCorrelations(),
-        CorrelationCoefficientTest(threshold=0.005),
+        CalculateCorrelations(),
+        CorrelationCoefficientTest(threshold=0.01),
         PartialCorrelationTest(
-            threshold=0.005, parallel=True, chunk_size_parallel_processing=50000
+            threshold=0.01, parallel=True, chunk_size_parallel_processing=50000
         ),
         ExtendedPartialCorrelationTestMatrix(
             # run first a sampled version of the test so we can minimize the number of tests in the full version
-            threshold=0.005,
+            threshold=0.01,
             chunk_size_parallel_processing=5000,
             parallel=True,
             generator=RandomSampleGenerator(
                 generator=PairsWithNeighboursGenerator(
                     chunked=False,
                     shuffle_combinations=True,
                     comparison_settings=ComparisonSettings(
@@ -64,15 +57,15 @@
                     ),
                 ),
                 chunked=False,
                 every_nth=200,
             ),
         ),
         ExtendedPartialCorrelationTestMatrix(
-            threshold=0.005,
+            threshold=0.01,
             chunk_size_parallel_processing=20000,
             parallel=True,
             generator=PairsWithNeighboursGenerator(
                 chunked=False,
                 shuffle_combinations=True,
                 comparison_settings=ComparisonSettings(min=4, max=AS_MANY_AS_FIELDS),
             ),
@@ -83,10 +76,9 @@
                 NonColliderTest(),
                 FurtherOrientTripleTest(),
                 OrientQuadrupleTest(),
                 FurtherOrientQuadrupleTest(),
             ],
             exit_condition=ExitOnNoActions(),
         ),
-        ComputeDirectEffectsMultivariateRegression(),
     ]
 )
```

### Comparing `causy-0.0.36/causy/cli.py` & `causy-0.0.9/causy/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 import json
 from datetime import datetime
 from json import JSONEncoder
 import logging
 
 import typer
 
-from causy.graph_model import graph_model_factory
-from causy.serialization import serialize_model
-from causy.graph_utils import (
+from causy.graph import graph_model_factory
+from causy.utils import (
     load_pipeline_steps_by_definition,
     retrieve_edges,
 )
-from causy.ui import server
 
 app = typer.Typer()
 
 
 def load_json(pipeline_file: str):
     with open(pipeline_file, "r") as file:
         pipeline = json.loads(file.read())
@@ -33,43 +31,39 @@
 
 def create_pipeline(pipeline_config: dict):
     return load_pipeline_steps_by_definition(pipeline_config["steps"])
 
 
 class MyJSONEncoder(JSONEncoder):
     def default(self, obj):
-        return obj.serialize()
+        return obj.to_dict()
 
 
 @app.command()
 def eject(algorithm: str, output_file: str):
     typer.echo(f"💾 Loading algorithm {algorithm}")
     model = load_algorithm(algorithm)()
-    result = serialize_model(model, algorithm_name=algorithm)
+    output = []
+    for step in model.pipeline_steps:
+        output.append(step.serialize())
+
+    result = {"name": algorithm, "steps": output}
+
     typer.echo(f"💾 Saving algorithm {algorithm} to {output_file}")
     with open(output_file, "w") as file:
         file.write(json.dumps(result, indent=4))
 
 
 @app.command()
-def ui(result_file: str):
-    result = load_json(result_file)
-
-    server_config, server_runner = server(result)
-    typer.launch(f"http://{server_config.host}:{server_config.port}")
-    typer.echo(f"🚀 Starting server at http://{server_config.host}:{server_config.port}")
-    server_runner.run()
-
-
-@app.command()
 def execute(
     data_file: str,
     pipeline: str = None,
     algorithm: str = None,
     output_file: str = None,
+    render_save_file: str = None,
     log_level: str = "ERROR",
 ):
     logging.basicConfig(level=log_level)
     if pipeline:
         typer.echo(f"💾 Loading pipeline from {pipeline}")
         pipeline_config = load_json(pipeline)
         pipeline = create_pipeline(pipeline_config)
@@ -100,16 +94,16 @@
     edges = []
     for edge in retrieve_edges(model.graph):
         print(
             f"{model.graph.nodes[edge[0]].name} -> {model.graph.nodes[edge[1]].name}: {model.graph.edges[edge[0]][edge[1]]}"
         )
         edges.append(
             {
-                "from": model.graph.nodes[edge[0]].serialize(),
-                "to": model.graph.nodes[edge[1]].serialize(),
+                "from": model.graph.nodes[edge[0]].to_dict(),
+                "to": model.graph.nodes[edge[1]].to_dict(),
                 "value": model.graph.edges[edge[0]][edge[1]],
             }
         )
 
     if output_file:
         typer.echo(f"💾 Saving graph actions to {output_file}")
         with open(output_file, "w") as file:
@@ -119,10 +113,29 @@
                 "algorithm": algorithm_reference,
                 "steps": model.graph.action_history,
                 "nodes": model.graph.nodes,
                 "edges": edges,
             }
             file.write(json.dumps(export, cls=MyJSONEncoder, indent=4))
 
+    if render_save_file:
+        # I'm just a hacky rendering function, pls replace me with causy ui 🙄
+        typer.echo(f"💾 Saving graph to {render_save_file}")
+        import networkx as nx
+        import matplotlib.pyplot as plt
+
+        n_graph = nx.DiGraph()
+        for u in model.graph.edges:
+            for v in model.graph.edges[u]:
+                n_graph.add_edge(model.graph.nodes[u].name, model.graph.nodes[v].name)
+        fig = plt.figure(figsize=(10, 10))
+        nx.draw(n_graph, with_labels=True, ax=fig.add_subplot(111))
+        fig.savefig(render_save_file)
+
+
+@app.command()
+def visualize(output: str):
+    raise NotImplementedError()
+
 
 if __name__ == "__main__":
     app()
```

### Comparing `causy-0.0.36/causy/common_pipeline_steps/exit_conditions.py` & `causy-0.0.9/causy/exit_conditions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from causy.interfaces import ExitConditionInterface
 
 
 class ExitOnNoActions(ExitConditionInterface):
-    def check(self, graph, graph_model_instance_, actions_taken, iteration) -> bool:
+    def check(self, graph, graph_model_instance_, actions_taken, iteration):
         """
         Check if there are no actions taken in the last iteration and if so, break the loop
         If it is the first iteration, do not break the loop (we need to execute the first step)
         :param graph: the graph
         :param graph_model_instance_: the graph model instance
         :param actions_taken: the actions taken in the last iteration
         :param iteration: iteration number
```

### Comparing `causy-0.0.36/causy/generators.py` & `causy-0.0.9/causy/generators.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from causy.interfaces import (
     ComparisonSettings,
     GeneratorInterface,
     BaseGraphInterface,
     GraphModelInterface,
     AS_MANY_AS_FIELDS,
 )
-from causy.graph_utils import load_pipeline_artefact_by_definition
+from causy.utils import load_pipeline_artefact_by_definition
 
 logger = logging.getLogger(__name__)
 
 
 class AllCombinationsGenerator(GeneratorInterface):
     """
     Generates all combinations of nodes in the graph
@@ -44,42 +44,14 @@
 
         # create all combinations
         for r in range(start, stop):
             for i in itertools.combinations(graph.nodes, r):
                 yield i
 
 
-class PairsWithEdgesInBetweenGenerator(GeneratorInterface):
-    def __init__(
-        self, comparison_settings: ComparisonSettings = None, chunked: bool = None
-    ):
-        self.chunked = chunked
-        super().__init__(comparison_settings, chunked)
-
-    CHUNK_SIZE = 100
-
-    def generate(
-        self, graph: BaseGraphInterface, graph_model_instance_: GraphModelInterface
-    ):
-        local_edges = copy.deepcopy(graph.edges)
-
-        edges = []
-
-        for f_node in local_edges:
-            for t_node in graph.edges[f_node]:
-                edges.append((f_node, t_node))
-
-        if self.chunked:
-            for i in range(0, len(edges), self.CHUNK_SIZE):
-                yield edges[i : i + self.CHUNK_SIZE]
-
-        for edge in edges:
-            yield edge
-
-
 class PairsWithNeighboursGenerator(GeneratorInterface):
     """
     Generates all combinations of pairs of nodes with their neighbours
     """
 
     shuffle_combinations = True
     chunked = True
@@ -90,16 +62,18 @@
         chunked: bool = None,
         shuffle_combinations: bool = None,
     ):
         super().__init__(comparison_settings, chunked)
         if shuffle_combinations is not None:
             self.shuffle_combinations = shuffle_combinations
 
-        if chunked is not None:
-            self.chunked = chunked
+    def serialize(self):
+        result = super().serialize()
+        result["params"]["shuffle_combinations"] = self.shuffle_combinations
+        return result
 
     def generate(
         self, graph: BaseGraphInterface, graph_model_instance_: GraphModelInterface
     ):
         start = self.comparison_settings.min
         # if min is longer then our dataset, we can't create any combinations
         if start > len(graph.nodes):
@@ -182,14 +156,20 @@
             if isinstance(generator, GeneratorInterface):
                 self.generator = generator
             else:
                 self.generator = load_pipeline_artefact_by_definition(generator)
         else:
             raise ValueError("RandomSampleGenerator: generator must be set")
 
+    def serialize(self):
+        result = super().serialize()
+        result["params"]["every_nth"] = self.every_nth
+        result["params"]["generator"] = self.generator.serialize()
+        return result
+
     def generate(self, graph: BaseGraphInterface, graph_model_instance_: dict):
         """
         Executes another generator and returns a random sample of the results
         :param graph:
         :param graph_model_instance_:
         :return: yields a random sample of the results
         """
```

### Comparing `causy-0.0.36/causy/independence_tests/common.py` & `causy-0.0.9/causy/independence_tests.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,101 @@
 import itertools
 from typing import Tuple, List, Optional
 import logging
 
 import torch
 
 from causy.generators import AllCombinationsGenerator, PairsWithNeighboursGenerator
-from causy.math_utils import get_t_and_critical_t
+from causy.utils import get_t_and_critical_t, get_correlation, pearson_correlation
 from causy.interfaces import (
-    PipelineStepInterface,
+    IndependenceTestInterface,
     BaseGraphInterface,
     NodeInterface,
     TestResult,
     TestResultAction,
     AS_MANY_AS_FIELDS,
     ComparisonSettings,
 )
 
 logger = logging.getLogger(__name__)
 
 
-class CorrelationCoefficientTest(PipelineStepInterface):
-    generator = AllCombinationsGenerator(
+class CalculateCorrelations(IndependenceTestInterface):
+    GENERATOR = AllCombinationsGenerator(
         comparison_settings=ComparisonSettings(min=2, max=2)
     )
-    chunk_size_parallel_processing = 1
-    parallel = False
+    CHUNK_SIZE_PARALLEL_PROCESSING = 1
+    PARALLEL = False
+
+    def test(self, nodes: Tuple[str], graph: BaseGraphInterface) -> TestResult:
+        """
+        Calculate the correlation between each pair of nodes and store it to the respective edge.
+        :param nodes: list of nodes
+        :return: A TestResult with the action to take
+        """
+        x = graph.nodes[nodes[0]]
+        y = graph.nodes[nodes[1]]
+        edge_value = graph.edge_value(graph.nodes[nodes[0]], graph.nodes[nodes[1]])
+        edge_value["correlation"] = pearson_correlation(
+            x.values,
+            y.values,
+        ).item()
+        return TestResult(
+            x=x,
+            y=y,
+            action=TestResultAction.UPDATE_EDGE,
+            data=edge_value,
+        )
+
+
+class CorrelationCoefficientTest(IndependenceTestInterface):
+    GENERATOR = AllCombinationsGenerator(
+        comparison_settings=ComparisonSettings(min=2, max=2)
+    )
+    CHUNK_SIZE_PARALLEL_PROCESSING = 1
+    PARALLEL = False
 
     def test(self, nodes: List[str], graph: BaseGraphInterface) -> Optional[TestResult]:
         """
-        Test if u and v are independent and delete edge in graph if they are.
+        Test if x and y are independent and delete edge in graph if they are.
         :param nodes: list of nodes
         :return: A TestResult with the action to take
         """
         x = graph.nodes[nodes[0]]
         y = graph.nodes[nodes[1]]
 
-        # make t test for independency of u and v
+        # make t test for independency of x and y
         sample_size = len(x.values)
         nb_of_control_vars = 0
         corr = graph.edge_value(x, y)["correlation"]
         t, critical_t = get_t_and_critical_t(
             sample_size, nb_of_control_vars, corr, self.threshold
         )
         if abs(t) < critical_t:
             logger.debug(f"Nodes {x.name} and {y.name} are uncorrelated")
             return TestResult(
-                u=x,
-                v=y,
+                x=x,
+                y=y,
                 action=TestResultAction.REMOVE_EDGE_UNDIRECTED,
                 data={},
             )
 
 
-class PartialCorrelationTest(PipelineStepInterface):
-    generator = AllCombinationsGenerator(
+class PartialCorrelationTest(IndependenceTestInterface):
+    GENERATOR = AllCombinationsGenerator(
         comparison_settings=ComparisonSettings(min=3, max=3)
     )
-    chunk_size_parallel_processing = 1
-    parallel = False
+    CHUNK_SIZE_PARALLEL_PROCESSING = 1
+    PARALLEL = False
 
     def test(
         self, nodes: Tuple[str], graph: BaseGraphInterface
     ) -> Optional[List[TestResult]]:
         """
-        Test if nodes u,v are independent given node z based on a partial correlation test.
+        Test if nodes x,y are independent given node z based on a partial correlation test.
         We use this test for all combinations of 3 nodes because it is faster than the extended test (which supports combinations of n nodes). We can
         use it to remove edges between nodes which are not independent given another node and so reduce the number of combinations for the extended test.
         :param nodes: the nodes to test
         :return: A TestResult with the action to take
 
         TODO: we are testing (C and E given B) and (E and C given B), we just need one of these, remove redundant tests.
         """
@@ -85,60 +113,114 @@
             if not graph.edge_exists(x, y) or (y, x) in already_deleted_edges:
                 continue
 
             try:
                 cor_xy = graph.edge_value(x, y)["correlation"]
                 cor_xz = graph.edge_value(x, z)["correlation"]
                 cor_yz = graph.edge_value(y, z)["correlation"]
-            except (KeyError, TypeError):
+            except KeyError:
                 return
 
             numerator = cor_xy - cor_xz * cor_yz
             denominator = ((1 - cor_xz**2) * (1 - cor_yz**2)) ** 0.5
 
             # Avoid division by zero
             if denominator == 0:
                 return
 
             par_corr = numerator / denominator
 
-            # make t test for independency of u and v given z
+            # make t test for independency of x and y given z
             sample_size = len(x.values)
             nb_of_control_vars = len(nodes) - 2
             t, critical_t = get_t_and_critical_t(
                 sample_size, nb_of_control_vars, par_corr, self.threshold
             )
 
             if abs(t) < critical_t:
                 logger.debug(
                     f"Nodes {x.name} and {y.name} are uncorrelated given {z.name}"
                 )
 
                 results.append(
                     TestResult(
-                        u=x,
-                        v=y,
+                        x=x,
+                        y=y,
                         action=TestResultAction.REMOVE_EDGE_UNDIRECTED,
                         data={"separatedBy": [z]},
                     )
                 )
                 already_deleted_edges.add((x, y))
         return results
 
 
-class ExtendedPartialCorrelationTestMatrix(PipelineStepInterface):
-    generator = PairsWithNeighboursGenerator(
+class ExtendedPartialCorrelationTestLinearRegression(IndependenceTestInterface):
+    GENERATOR = AllCombinationsGenerator(
+        comparison_settings=ComparisonSettings(min=4, max=AS_MANY_AS_FIELDS)
+    )
+    CHUNK_SIZE_PARALLEL_PROCESSING = 1000
+    PARALLEL = True
+
+    def test(
+        self, nodes: List[str], graph: BaseGraphInterface
+    ) -> Optional[List[TestResult]]:
+        """
+        Test if nodes x,y are independent given Z (set of nodes) based on partial correlation using linear regression and a correlation test on the residuals.
+        We use this test for all combinations of more than 3 nodes because it is slower.
+        :param nodes: the nodes to test
+        :return: A TestResult with the action to take
+
+        TODO: Does not run in reasonable time yet.
+        """
+        n = len(nodes)
+        sample_size = len(graph.nodes[nodes[0]].values)
+        nodes_set = set([graph.nodes[n] for n in nodes])
+
+        nb_of_control_vars = n - 2
+        results = []
+        for i in range(n):
+            for j in range(i + 1, n):
+                x = graph.nodes[nodes[i]]
+                y = graph.nodes[nodes[j]]
+                exclude_indices = [i, j]
+                other_nodes = [
+                    graph.nodes[n].values
+                    for idx, n in enumerate(nodes)
+                    if idx not in exclude_indices
+                ]
+                par_corr = get_correlation(x, y, other_nodes)
+                logger.debug(f"par_corr {par_corr}")
+                # make t test for independence of a and y given other nodes
+                t, critical_t = get_t_and_critical_t(
+                    sample_size, nb_of_control_vars, par_corr, self.threshold
+                )
+
+                if abs(t) < critical_t:
+                    results.append(
+                        TestResult(
+                            x=x,
+                            y=y,
+                            action=TestResultAction.REMOVE_EDGE_UNDIRECTED,
+                            data={"separatedBy": list(nodes_set - {x, y})},
+                        )
+                    )
+
+        return results
+
+
+class ExtendedPartialCorrelationTestMatrix(IndependenceTestInterface):
+    GENERATOR = PairsWithNeighboursGenerator(
         comparison_settings=ComparisonSettings(min=4, max=AS_MANY_AS_FIELDS)
     )
-    chunk_size_parallel_processing = 1000
-    parallel = False
+    CHUNK_SIZE_PARALLEL_PROCESSING = 1000
+    PARALLEL = False
 
     def test(self, nodes: List[str], graph: BaseGraphInterface) -> Optional[TestResult]:
         """
-        Test if nodes u,v are independent given Z (set of nodes) based on partial correlation using the inverted covariance matrix (precision matrix).
+        Test if nodes x,y are independent given Z (set of nodes) based on partial correlation using the inverted covariance matrix (precision matrix).
         https://en.wikipedia.org/wiki/Partial_correlation#Using_matrix_inversion
         We use this test for all combinations of more than 3 nodes because it is slower.
         :param nodes: the nodes to test
         :return: A TestResult with the action to take
         """
 
         if not graph.edge_exists(graph.nodes[nodes[0]], graph.nodes[nodes[1]]):
@@ -149,18 +231,17 @@
 
         if not set(nodes[2:]).issubset(set([on for on in list(other_neighbours)])):
             return
 
         inverse_cov_matrix = torch.inverse(
             torch.cov(torch.stack([graph.nodes[node].values for node in nodes]))
         )
-
         n = inverse_cov_matrix.size(0)
         diagonal = torch.diag(inverse_cov_matrix)
-        diagonal_matrix = torch.zeros((n, n), dtype=torch.float32)
+        diagonal_matrix = torch.zeros((n, n), dtype=torch.float64)
         for i in range(n):
             diagonal_matrix[i, i] = diagonal[i]
 
         helper = torch.mm(torch.sqrt(diagonal_matrix), inverse_cov_matrix)
         precision_matrix = torch.mm(helper, torch.sqrt(diagonal_matrix))
 
         sample_size = len(graph.nodes[nodes[0]].values)
@@ -178,16 +259,34 @@
 
         if abs(t) < critical_t:
             logger.debug(
                 f"Nodes {graph.nodes[nodes[0]].name} and {graph.nodes[nodes[1]].name} are uncorrelated given nodes {','.join([graph.nodes[on].name for on in other_neighbours])}"
             )
             nodes_set = set([graph.nodes[n] for n in nodes])
             return TestResult(
-                u=graph.nodes[nodes[0]],
-                v=graph.nodes[nodes[1]],
+                x=graph.nodes[nodes[0]],
+                y=graph.nodes[nodes[1]],
                 action=TestResultAction.REMOVE_EDGE_UNDIRECTED,
                 data={
                     "separatedBy": list(
                         nodes_set - {graph.nodes[nodes[0]], graph.nodes[nodes[1]]}
                     )
                 },
             )
+
+
+class PlaceholderTest(IndependenceTestInterface):
+    NUM_OF_COMPARISON_ELEMENTS = 2
+    CHUNK_SIZE_PARALLEL_PROCESSING = 10
+    PARALLEL = False
+
+    def test(
+        self, nodes: Tuple[str], graph: BaseGraphInterface
+    ) -> List[TestResult] | TestResult:
+        """
+        Placeholder test for testing purposes
+        :param nodes:
+        :param graph:
+        :return:
+        """
+        logger.debug(f"PlaceholderTest {nodes}")
+        return TestResult(x=None, y=None, action=TestResultAction.DO_NOTHING, data={})
```

### Comparing `causy-0.0.36/causy/interfaces.py` & `causy-0.0.9/causy/interfaces.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,130 +1,100 @@
 import enum
 import multiprocessing
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import List, Dict, Optional
 import logging
 
-import torch
-
-from causy.serialization import SerializeMixin
-from causy.graph_utils import load_pipeline_artefact_by_definition
+from causy.utils import serialize_module_name, load_pipeline_artefact_by_definition
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_THRESHOLD = 0.01
 
 AS_MANY_AS_FIELDS = 0
 
 
 @dataclass
-class ComparisonSettings(SerializeMixin):
+class ComparisonSettings:
     min: int = 2
     max: int = AS_MANY_AS_FIELDS
 
+    def serialize(self):
+        return {
+            "name": serialize_module_name(self),
+            "params": {
+                "min": self.min,
+                "max": self.max,
+            },
+        }
 
-class NodeInterface(SerializeMixin):
-    """
-    Node interface for the graph. A node is defined by a name and a value.
-    """
 
+class NodeInterface:
     name: str
     id: str
-    values: torch.Tensor
+    values: List[float]
 
-    def serialize(self):
+    def to_dict(self):
         return {"id": self.id, "name": self.name}
 
 
-class EdgeTypeInterface:
-    pass
-
-
-class EdgeInterface(SerializeMixin):
-    """
-    Edge interface for the graph
-    A graph edge is defined by two nodes and an edge type. It can also have metadata.
-    """
-
-    u: NodeInterface
-    v: NodeInterface
-    edge_type: EdgeTypeInterface
-    metadata: Dict[str, any] = None
-
-    def serialize(self):
-        return {
-            "edge_type": self.edge_type,
-            "metadata": self.metadata,
-        }
-
-
 class TestResultAction(enum.StrEnum):
-    """
-    Actions that can be taken on the graph. These actions are used to keep track of the history of the graph.
-    """
-
     REMOVE_EDGE_UNDIRECTED = "REMOVE_EDGE_UNDIRECTED"
     UPDATE_EDGE = "UPDATE_EDGE"
-    UPDATE_EDGE_TYPE = "UPDATE_EDGE_TYPE"
     UPDATE_EDGE_DIRECTED = "UPDATE_EDGE_DIRECTED"
-    UPDATE_EDGE_TYPE_DIRECTED = "UPDATE_EDGE_TYPE_DIRECTED"
     DO_NOTHING = "DO_NOTHING"
     REMOVE_EDGE_DIRECTED = "REMOVE_EDGE_DIRECTED"
 
 
 @dataclass
-class TestResult(SerializeMixin):
-    u: NodeInterface
-    v: NodeInterface
+class TestResult:
+    x: NodeInterface
+    y: NodeInterface
     action: TestResultAction
     data: Optional[Dict] = None
 
-    def serialize(self):
+    def to_dict(self):
         return {
-            "from": self.u.serialize(),
-            "to": self.v.serialize(),
+            "x": self.x.to_dict(),
+            "y": self.y.to_dict(),
             "action": self.action.name,
         }
 
 
 class BaseGraphInterface(ABC):
     nodes: Dict[str, NodeInterface]
     edges: Dict[str, Dict[str, Dict]]
 
     @abstractmethod
     def retrieve_edge_history(self, u, v, action: TestResultAction) -> List[TestResult]:
         pass
 
     @abstractmethod
-    def add_edge_history(self, u, v, action: TestResult):
+    def add_edge_history(self, u, v, action: TestResultAction):
         pass
 
     @abstractmethod
-    def add_edge(self, u, v, metadata):
+    def add_edge(self, u, v, w):
         pass
 
     @abstractmethod
     def remove_edge(self, u, v):
         pass
 
     @abstractmethod
     def remove_directed_edge(self, u, v):
         pass
 
     @abstractmethod
-    def update_edge(self, u, v, metadata=None, edge_type=None):
+    def update_edge(self, u, v, w):
         pass
 
     @abstractmethod
-    def update_directed_edge(self, u, v, metadata=None, edge_type=None):
-        pass
-
-    @abstractmethod
-    def add_node(self, name, values) -> NodeInterface:
+    def add_node(self, name, values):
         pass
 
     @abstractmethod
     def edge_value(self, u, v):
         pass
 
     @abstractmethod
@@ -152,100 +122,128 @@
         pass
 
     @abstractmethod
     def execute_pipeline_step(self, step):
         pass
 
 
-class GeneratorInterface(ABC, SerializeMixin):
+class GeneratorInterface(ABC):
     comparison_settings: ComparisonSettings
     chunked: bool = False
 
     @abstractmethod
     def generate(self, graph: BaseGraphInterface, graph_model_instance_: dict):
         pass
 
+    def serialize(self) -> dict:
+        return {
+            "name": serialize_module_name(self),
+            "params": {
+                "comparison_settings": self.comparison_settings.serialize()
+                if self.comparison_settings
+                else None,
+                "chunked": self.chunked,
+            },
+        }
+
     def __init__(self, comparison_settings: ComparisonSettings, chunked: bool = None):
         if isinstance(comparison_settings, dict):
             comparison_settings = load_pipeline_artefact_by_definition(
                 comparison_settings
             )
 
         if chunked is not None:
             self.chunked = chunked
 
         self.comparison_settings = comparison_settings
 
 
-class PipelineStepInterface(ABC, SerializeMixin):
-    num_of_comparison_elements: int = 0
-    generator: Optional[GeneratorInterface] = None
+class IndependenceTestInterface(ABC):
+    NUM_OF_COMPARISON_ELEMENTS: int = 0
+    GENERATOR: Optional[GeneratorInterface] = None
 
-    chunk_size_parallel_processing: int = 1
+    CHUNK_SIZE_PARALLEL_PROCESSING: int = 1
 
-    parallel: bool = True
+    PARALLEL: bool = True
 
     def __init__(
         self,
         threshold: float = DEFAULT_THRESHOLD,
         generator: Optional[GeneratorInterface] = None,
         num_of_comparison_elements: int = None,
         chunk_size_parallel_processing: int = None,
         parallel: bool = None,
     ):
         if generator:
             if isinstance(generator, dict):
-                self.generator = load_pipeline_artefact_by_definition(generator)
+                self.GENERATOR = load_pipeline_artefact_by_definition(generator)
             else:
-                self.generator = generator
+                self.GENERATOR = generator
 
         if num_of_comparison_elements:
             if isinstance(num_of_comparison_elements, dict):
-                self.num_of_comparison_elements = load_pipeline_artefact_by_definition(
+                self.NUM_OF_COMPARISON_ELEMENTS = load_pipeline_artefact_by_definition(
                     num_of_comparison_elements
                 )
             else:
-                self.num_of_comparison_elements = num_of_comparison_elements
+                self.NUM_OF_COMPARISON_ELEMENTS = num_of_comparison_elements
 
         if chunk_size_parallel_processing:
-            self.chunk_size_parallel_processing = chunk_size_parallel_processing
+            self.CHUNK_SIZE_PARALLEL_PROCESSING = chunk_size_parallel_processing
 
         if parallel:
-            self.parallel = parallel
+            self.PARALLEL = parallel
 
         self.threshold = threshold
 
     @abstractmethod
     def test(self, nodes: List[str], graph: BaseGraphInterface) -> Optional[TestResult]:
         """
-        Test if u and v are independent
-        :param u: u values
-        :param v: v values
+        Test if x and y are independent
+        :param x: x values
+        :param y: y values
         :return: True if independent, False otherwise
         """
         pass
 
     def __call__(
         self, nodes: List[str], graph: BaseGraphInterface
     ) -> Optional[TestResult]:
         return self.test(nodes, graph)
 
+    def serialize(self) -> dict:
+        return {
+            "name": serialize_module_name(self),
+            "params": {
+                "threshold": self.threshold,
+                "generator": self.GENERATOR.serialize(),
+                "num_of_comparison_elements": self.NUM_OF_COMPARISON_ELEMENTS,
+                "chunk_size_parallel_processing": self.CHUNK_SIZE_PARALLEL_PROCESSING,
+                "parallel": self.PARALLEL,
+            },
+        }
+
 
-class LogicStepInterface(ABC, SerializeMixin):
+class LogicStepInterface(ABC):
     @abstractmethod
     def execute(self, graph: BaseGraphInterface, graph_model_instance_: dict):
         pass
 
+    def serialize(self) -> dict:
+        return {
+            "name": serialize_module_name(self),
+        }
 
-class ExitConditionInterface(ABC, SerializeMixin):
+
+class ExitConditionInterface(ABC):
     @abstractmethod
     def check(
         self,
         graph: BaseGraphInterface,
-        graph_model_instance_: GraphModelInterface,
+        graph_model_instance_: dict,
         actions_taken: List[TestResult],
         iteration: int,
     ) -> bool:
         """
         :param graph:
         :param graph_model_instance_:
         :param actions_taken:
@@ -253,12 +251,17 @@
         :return: True if you want to break an iteration, False otherwise
         """
         pass
 
     def __call__(
         self,
         graph: BaseGraphInterface,
-        graph_model_instance_: GraphModelInterface,
+        graph_model_instance_: dict,
         actions_taken: List[TestResult],
         iteration: int,
     ) -> bool:
         return self.check(graph, graph_model_instance_, actions_taken, iteration)
+
+    def serialize(self):
+        return {
+            "name": serialize_module_name(self),
+        }
```

### Comparing `causy-0.0.36/causy/orientation_rules/pc.py` & `causy-0.0.9/causy/orientation_tests.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,117 +1,113 @@
-from typing import Tuple, List, Optional
+from typing import Tuple, List
 import itertools
 
 from causy.generators import AllCombinationsGenerator
 from causy.interfaces import (
     BaseGraphInterface,
     TestResult,
     TestResultAction,
-    PipelineStepInterface,
+    IndependenceTestInterface,
     ComparisonSettings,
 )
 
-# theory for all orientation rules with pictures:
-# https://hpi.de/fileadmin/user_upload/fachgebiete/plattner/teaching/CausalInference/2019/Introduction_to_Constraint-Based_Causal_Structure_Learning.pdf
+# theory for all orientation rules with pictures: https://hpi.de/fileadmin/user_upload/fachgebiete/plattner/teaching/CausalInference/2019/Introduction_to_Constraint-Based_Causal_Structure_Learning.pdf
 
-# TODO: refactor ColliderTest -> ColliderRule and move to folder orientation_rules (after checking for duplicates)
 
-
-class ColliderTest(PipelineStepInterface):
-    generator = AllCombinationsGenerator(
+class ColliderTest(IndependenceTestInterface):
+    GENERATOR = AllCombinationsGenerator(
         comparison_settings=ComparisonSettings(min=2, max=2)
     )
-    chunk_size_parallel_processing = 1
-    parallel = False
+    CHUNK_SIZE_PARALLEL_PROCESSING = 1
+    PARALLEL = False
 
     def test(
         self, nodes: Tuple[str], graph: BaseGraphInterface
-    ) -> Optional[List[TestResult] | TestResult]:
+    ) -> List[TestResult] | TestResult:
         """
-        We call triples u, v, z of nodes v structures if u and v that are NOT adjacent but share an adjacent node z.
-        V structures looks like this in the undirected skeleton: (u - z - v).
+        We call triples x, y, z of nodes v structures if x and y that are NOT adjacent but share an adjacent node z.
+        V structures looks like this in the undirected skeleton: (x - z - y).
         We now check if z is in the separating set.
-        If z is not in the separating set, we know that u and v are uncorrelated given z.
-        So, the edges must be oriented from u to z and from v to z (u -> z <- v).
+        If z is not in the separating set, we know that x and y are uncorrelated given z.
+        So, the edges must be oriented from x to z and from y to z (x -> z <- y).
         :param nodes: list of nodes
         :param graph: the current graph
         :returns: list of actions that will be executed on graph
         """
         # https://github.com/pgmpy/pgmpy/blob/1fe10598df5430295a8fc5cdca85cf2d9e1c4330/pgmpy/estimators/PC.py#L416
 
         x = graph.nodes[nodes[0]]
         y = graph.nodes[nodes[1]]
 
-        # if u and v are adjacent, do nothing
+        # if x and y are adjacent, do nothing
         if graph.undirected_edge_exists(x, y):
-            return TestResult(u=x, v=y, action=TestResultAction.DO_NOTHING, data={})
+            return TestResult(x=x, y=y, action=TestResultAction.DO_NOTHING, data={})
 
-        # if u and v are NOT adjacent, store all shared adjacent nodes
+        # if x and y are NOT adjacent, store all shared adjacent nodes
         potential_zs = set(graph.edges[x.id].keys()).intersection(
             set(graph.edges[y.id].keys())
         )
 
-        actions = graph.retrieve_edge_history(
-            x, y, TestResultAction.REMOVE_EDGE_UNDIRECTED
-        )
-
-        # if u and v are not independent given z, safe action: make z a collider
+        # if x and y are not independent given z, safe action: make z a collider
         results = []
         for z in potential_zs:
             z = graph.nodes[z]
+            actions = graph.retrieve_edge_history(
+                x, y, TestResultAction.REMOVE_EDGE_UNDIRECTED
+            )
 
             separators = []
             for action in actions:
                 if "separatedBy" in action.data:
                     separators += [a.id for a in action.data["separatedBy"]]
 
             if z.id not in separators:
                 results += [
                     TestResult(
-                        u=z,
-                        v=x,
+                        x=z,
+                        y=x,
                         action=TestResultAction.REMOVE_EDGE_DIRECTED,
                         data={},
                     ),
                     TestResult(
-                        u=z,
-                        v=y,
+                        x=z,
+                        y=y,
                         action=TestResultAction.REMOVE_EDGE_DIRECTED,
                         data={},
                     ),
                 ]
         return results
 
 
-class NonColliderTest(PipelineStepInterface):
-    generator = AllCombinationsGenerator(
+class NonColliderTest(IndependenceTestInterface):
+    GENERATOR = AllCombinationsGenerator(
         comparison_settings=ComparisonSettings(min=2, max=2)
     )
-    chunk_size_parallel_processing = 1
-    parallel = False
+    CHUNK_SIZE_PARALLEL_PROCESSING = 1
+    PARALLEL = False
 
     def test(
         self, nodes: Tuple[str], graph: BaseGraphInterface
-    ) -> Optional[List[TestResult] | TestResult]:
+    ) -> List[TestResult] | TestResult:
         """
         Further orientation rule: all v structures that are colliders are already oriented.
         We now orient all v structures that have a single alternative to being a collider.
         :param nodes: list of nodes
         :param graph: the current graph
         :returns: list of actions that will be executed on graph
         """
 
         x = graph.nodes[nodes[0]]
         y = graph.nodes[nodes[1]]
 
-        # if u and v are adjacent, do nothing
+        # if x and y are adjacent, do nothing
         if graph.edge_exists(x, y):
             return
 
-        # if u and v are NOT adjacent, store all shared adjacent nodes
+        # if x and y are NOT adjacent, store all shared adjacent nodes
         potential_zs = set(graph.edges[x.id].keys()).intersection(
             set(graph.edges[y.id].keys())
         )
         # if one edge has an arrowhead at z, orient the other one pointing away from z.
         # It cannot be a collider because we have already oriented all unshielded triples that contain colliders.
         for z in potential_zs:
             z = graph.nodes[z]
@@ -122,245 +118,208 @@
                 for node in graph.nodes:
                     if graph.only_directed_edge_exists(graph.nodes[node], y):
                         breakflag = True
                         break
                 if breakflag is True:
                     continue
                 return TestResult(
-                    u=y,
-                    v=z,
+                    x=y,
+                    y=z,
                     action=TestResultAction.REMOVE_EDGE_DIRECTED,
                     data={},
                 )
 
             if graph.only_directed_edge_exists(y, z) and graph.undirected_edge_exists(
                 z, x
             ):
                 for node in graph.nodes:
                     if graph.only_directed_edge_exists(graph.nodes[node], x):
                         continue
                 return TestResult(
-                    u=x,
-                    v=z,
+                    x=x,
+                    y=z,
                     action=TestResultAction.REMOVE_EDGE_DIRECTED,
                     data={},
                 )
+        return
 
 
-class FurtherOrientTripleTest(PipelineStepInterface):
-    generator = AllCombinationsGenerator(
+class FurtherOrientTripleTest(IndependenceTestInterface):
+    GENERATOR = AllCombinationsGenerator(
         comparison_settings=ComparisonSettings(min=2, max=2)
     )
-    chunk_size_parallel_processing = 1
-    parallel = False
+    CHUNK_SIZE_PARALLEL_PROCESSING = 1
+    PARALLEL = False
 
     def test(
         self, nodes: Tuple[str], graph: BaseGraphInterface
-    ) -> Optional[List[TestResult] | TestResult]:
+    ) -> List[TestResult] | TestResult:
         """
         Further orientation rule.
         :param nodes: list of nodes
         :param graph: the current graph
         :returns: list of actions that will be executed on graph
         """
 
         x = graph.nodes[nodes[0]]
         y = graph.nodes[nodes[1]]
 
+        potential_zs = set(graph.edges[x.id].keys()).intersection(
+            set(graph.edges[y.id].keys())
+        )
+
         results = []
-        for z in graph.nodes:
+        for z in potential_zs:
             z = graph.nodes[z]
-            # check if it is a potential z
-            if not (graph.edge_exists(y, z) and graph.edge_exists(x, z)):
-                continue
-
             if (
                 graph.undirected_edge_exists(x, y)
                 and graph.only_directed_edge_exists(x, z)
                 and graph.only_directed_edge_exists(z, y)
             ):
                 results.append(
                     TestResult(
-                        u=y,
-                        v=x,
+                        x=y,
+                        y=x,
                         action=TestResultAction.REMOVE_EDGE_DIRECTED,
                         data={},
                     )
                 )
             if (
                 graph.undirected_edge_exists(x, y)
                 and graph.only_directed_edge_exists(y, z)
                 and graph.only_directed_edge_exists(z, x)
             ):
                 results.append(
                     TestResult(
-                        u=x,
-                        v=y,
+                        x=x,
+                        y=y,
                         action=TestResultAction.REMOVE_EDGE_DIRECTED,
                         data={},
                     )
                 )
         return results
 
 
-class OrientQuadrupleTest(PipelineStepInterface):
-    generator = AllCombinationsGenerator(
+class OrientQuadrupleTest(IndependenceTestInterface):
+    GENERATOR = AllCombinationsGenerator(
         comparison_settings=ComparisonSettings(min=2, max=2)
     )
-    chunk_size_parallel_processing = 1
-    parallel = False
+    CHUNK_SIZE_PARALLEL_PROCESSING = 1
+    PARALLEL = False
 
     def test(
         self, nodes: Tuple[str], graph: BaseGraphInterface
-    ) -> Optional[List[TestResult] | TestResult]:
+    ) -> List[TestResult] | TestResult:
         """
         Further orientation rule.
         :param nodes: list of nodes
         :param graph: the current graph
         :returns: list of actions that will be executed on graph
         """
 
-        y = graph.nodes[nodes[0]]
-        w = graph.nodes[nodes[1]]
-
-        potential_zs = set()
+        x = graph.nodes[nodes[0]]
+        y = graph.nodes[nodes[1]]
 
-        # TODO: just iterate over edges
-        for z in graph.nodes:
-            z = graph.nodes[z]
-            if graph.edge_exists(y, z) and graph.edge_exists(z, w):
-                potential_zs.add(z)
+        potential_zs = set(graph.edges[x.id].keys()).intersection(
+            set(graph.edges[y.id].keys())
+        )
 
         results = []
         for zs in itertools.combinations(potential_zs, 2):
-            x, z = zs
+            z = graph.nodes[zs[0]]
+            w = graph.nodes[zs[1]]
             if (
-                not graph.edge_exists(y, w)
+                not graph.undirected_edge_exists(x, y)
+                and graph.only_directed_edge_exists(x, z)
                 and graph.only_directed_edge_exists(y, z)
-                and graph.only_directed_edge_exists(w, z)
-                and graph.undirected_edge_exists(x, y)
                 and graph.undirected_edge_exists(x, w)
-                and graph.undirected_edge_exists(x, z)
+                and graph.undirected_edge_exists(y, w)
+                and graph.undirected_edge_exists(z, w)
             ):
                 results.append(
                     TestResult(
-                        u=z,
-                        v=x,
+                        x=z,
+                        y=w,
                         action=TestResultAction.REMOVE_EDGE_DIRECTED,
                         data={},
                     )
                 )
             if (
-                not graph.edge_exists(y, w)
-                and graph.only_directed_edge_exists(y, x)
-                and graph.only_directed_edge_exists(w, x)
-                and graph.undirected_edge_exists(y, z)
-                and graph.undirected_edge_exists(w, z)
+                not graph.undirected_edge_exists(x, y)
+                and graph.only_directed_edge_exists(x, w)
+                and graph.only_directed_edge_exists(y, w)
                 and graph.undirected_edge_exists(x, z)
+                and graph.undirected_edge_exists(y, z)
+                and graph.undirected_edge_exists(z, w)
             ):
                 results.append(
                     TestResult(
-                        u=x,
-                        v=z,
+                        x=w,
+                        y=z,
                         action=TestResultAction.REMOVE_EDGE_DIRECTED,
                         data={},
                     )
                 )
         return results
 
 
-class FurtherOrientQuadrupleTest(PipelineStepInterface):
-    generator = AllCombinationsGenerator(
+class FurtherOrientQuadrupleTest(IndependenceTestInterface):
+    GENERATOR = AllCombinationsGenerator(
         comparison_settings=ComparisonSettings(min=2, max=2)
     )
-    chunk_size_parallel_processing = 1
-    parallel = False
+    CHUNK_SIZE_PARALLEL_PROCESSING = 1
+    PARALLEL = False
 
     def test(
         self, nodes: Tuple[str], graph: BaseGraphInterface
-    ) -> Optional[List[TestResult] | TestResult]:
+    ) -> List[TestResult] | TestResult:
         """
         Further orientation rule.
         :param nodes: list of nodes
         :param graph: the current graph
         :returns: list of actions that will be executed on graph
         """
 
         x = graph.nodes[nodes[0]]
-        w = graph.nodes[nodes[1]]
-
-        potential_zs = set()
+        y = graph.nodes[nodes[1]]
 
-        # TODO: just iterate over edges
-        for z in graph.nodes:
-            z = graph.nodes[z]
-            if graph.edge_exists(x, z) and graph.edge_exists(z, w):
-                potential_zs.add(z)
+        potential_zs = set(graph.edges[x.id].keys()).intersection(
+            set(graph.edges[y.id].keys())
+        )
 
         results = []
         for zs in itertools.combinations(potential_zs, 2):
-            y, z = zs
+            z = graph.nodes[zs[0]]
+            w = graph.nodes[zs[1]]
             if (
-                not graph.edge_exists(y, z)
-                and graph.undirected_edge_exists(x, z)
-                and graph.undirected_edge_exists(x, w)
-                and graph.undirected_edge_exists(x, y)
-                and graph.only_directed_edge_exists(y, w)
-                and graph.only_directed_edge_exists(w, z)
-            ):
-                results.append(
-                    TestResult(
-                        u=z,
-                        v=x,
-                        action=TestResultAction.REMOVE_EDGE_DIRECTED,
-                        data={},
-                    )
-                )
-            elif (
-                not graph.edge_exists(z, y)
-                and graph.undirected_edge_exists(x, y)
-                and graph.undirected_edge_exists(x, w)
-                and graph.undirected_edge_exists(x, z)
-                and graph.only_directed_edge_exists(z, w)
-                and graph.only_directed_edge_exists(w, y)
-            ):
-                results.append(
-                    TestResult(
-                        u=y,
-                        v=x,
-                        action=TestResultAction.REMOVE_EDGE_DIRECTED,
-                        data={},
-                    )
-                )
-            elif (
-                not graph.edge_exists(y, z)
-                and graph.undirected_edge_exists(w, z)
-                and graph.undirected_edge_exists(x, w)
-                and graph.undirected_edge_exists(w, y)
-                and graph.only_directed_edge_exists(y, x)
+                not graph.undirected_edge_exists(x, y)
                 and graph.only_directed_edge_exists(x, z)
+                and graph.only_directed_edge_exists(z, y)
+                and graph.undirected_edge_exists(z, w)
+                and graph.undirected_edge_exists(x, z)
+                and graph.undirected_edge_exists(y, z)
             ):
                 results.append(
                     TestResult(
-                        u=z,
-                        v=w,
+                        x=y,
+                        y=z,
                         action=TestResultAction.REMOVE_EDGE_DIRECTED,
                         data={},
                     )
                 )
-            elif (
-                not graph.edge_exists(z, y)
-                and graph.undirected_edge_exists(w, y)
-                and graph.undirected_edge_exists(x, w)
-                and graph.undirected_edge_exists(w, z)
+            if (
+                not graph.undirected_edge_exists(y, x)
+                and graph.only_directed_edge_exists(y, z)
                 and graph.only_directed_edge_exists(z, x)
-                and graph.only_directed_edge_exists(x, y)
+                and graph.undirected_edge_exists(z, w)
+                and graph.undirected_edge_exists(x, z)
+                and graph.undirected_edge_exists(y, z)
             ):
                 results.append(
                     TestResult(
-                        u=y,
-                        v=w,
+                        x=x,
+                        y=z,
                         action=TestResultAction.REMOVE_EDGE_DIRECTED,
                         data={},
                     )
                 )
         return results
```


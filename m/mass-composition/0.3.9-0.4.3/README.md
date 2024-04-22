# Comparing `tmp/mass_composition-0.3.9.tar.gz` & `tmp/mass_composition-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mass_composition-0.3.9.tar", max compression
+gzip compressed data, was "mass_composition-0.4.3.tar", max compression
```

## Comparing `mass_composition-0.3.9.tar` & `mass_composition-0.4.3.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0     1069 2024-01-05 11:19:12.028882 mass_composition-0.3.9/LICENSE
--rw-r--r--   0        0        0     3449 2024-01-05 11:19:12.028882 mass_composition-0.3.9/README.md
--rw-r--r--   0        0        0      318 2024-01-05 11:19:12.436881 mass_composition-0.3.9/elphick/mass_composition/__init__.py
--rw-r--r--   0        0        0     9833 2024-01-05 11:19:12.436881 mass_composition-0.3.9/elphick/mass_composition/balance.py
--rw-r--r--   0        0        0       35 2024-01-05 11:19:12.436881 mass_composition-0.3.9/elphick/mass_composition/config/__init__.py
--rw-r--r--   0        0        0      765 2024-01-05 11:19:12.436881 mass_composition-0.3.9/elphick/mass_composition/config/config_read.py
--rw-r--r--   0        0        0      364 2024-01-05 11:19:12.436881 mass_composition-0.3.9/elphick/mass_composition/config/flowsheet_example.yaml
--rw-r--r--   0        0        0      838 2024-01-05 11:19:12.436881 mass_composition-0.3.9/elphick/mass_composition/config/mc_config.yml
--rw-r--r--   0        0        0       59 2024-01-05 11:19:12.436881 mass_composition-0.3.9/elphick/mass_composition/datasets/__init__.py
--rw-r--r--   0        0        0     1892 2024-01-05 11:19:12.436881 mass_composition-0.3.9/elphick/mass_composition/datasets/datasets.py
--rw-r--r--   0        0        0     1622 2024-01-05 11:19:12.436881 mass_composition-0.3.9/elphick/mass_composition/datasets/downloader.py
--rw-r--r--   0        0        0     3046 2024-01-05 11:19:12.436881 mass_composition-0.3.9/elphick/mass_composition/datasets/register.csv
--rw-r--r--   0        0        0     6569 2024-01-05 11:19:12.436881 mass_composition-0.3.9/elphick/mass_composition/datasets/sample_data.py
--rw-r--r--   0        0        0     1829 2024-01-05 11:19:12.436881 mass_composition-0.3.9/elphick/mass_composition/layout.py
--rw-r--r--   0        0        0    52055 2024-01-05 11:19:12.436881 mass_composition-0.3.9/elphick/mass_composition/mass_composition.py
--rw-r--r--   0        0        0     4350 2024-01-05 11:19:12.436881 mass_composition-0.3.9/elphick/mass_composition/mc_node.py
--rw-r--r--   0        0        0      638 2024-01-05 11:19:12.436881 mass_composition-0.3.9/elphick/mass_composition/mc_status.py
--rw-r--r--   0        0        0    19410 2024-01-05 11:19:12.436881 mass_composition-0.3.9/elphick/mass_composition/mc_xarray.py
--rw-r--r--   0        0        0    39393 2024-01-05 11:19:12.436881 mass_composition-0.3.9/elphick/mass_composition/network.py
--rw-r--r--   0        0        0     5752 2024-01-05 11:19:12.436881 mass_composition-0.3.9/elphick/mass_composition/plot.py
--rw-r--r--   0        0        0       42 2024-01-05 11:19:12.436881 mass_composition-0.3.9/elphick/mass_composition/utils/__init__.py
--rw-r--r--   0        0        0      214 2024-01-05 11:19:12.440881 mass_composition-0.3.9/elphick/mass_composition/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3909 2024-01-05 11:19:12.440881 mass_composition-0.3.9/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc
--rw-r--r--   0        0        0     2197 2024-01-05 11:19:12.440881 mass_composition-0.3.9/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc
--rw-r--r--   0        0        0     1494 2024-01-05 11:19:12.440881 mass_composition-0.3.9/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc
--rw-r--r--   0        0        0     1874 2024-01-05 11:19:12.440881 mass_composition-0.3.9/elphick/mass_composition/utils/amenability.py
--rw-r--r--   0        0        0     2914 2024-01-05 11:19:12.440881 mass_composition-0.3.9/elphick/mass_composition/utils/components.py
--rw-r--r--   0        0        0       80 2024-01-05 11:19:12.440881 mass_composition-0.3.9/elphick/mass_composition/utils/geometry.py
--rw-r--r--   0        0        0     1193 2024-01-05 11:19:12.440881 mass_composition-0.3.9/elphick/mass_composition/utils/hash_utils.py
--rw-r--r--   0        0        0     9591 2024-01-05 11:19:12.440881 mass_composition-0.3.9/elphick/mass_composition/utils/interp.py
--rw-r--r--   0        0        0     3556 2024-01-05 11:19:12.440881 mass_composition-0.3.9/elphick/mass_composition/utils/loader.py
--rw-r--r--   0        0        0     2611 2024-01-05 11:19:12.440881 mass_composition-0.3.9/elphick/mass_composition/utils/moisture.py
--rw-r--r--   0        0        0     1033 2024-01-05 11:19:12.440881 mass_composition-0.3.9/elphick/mass_composition/utils/partition.py
--rw-r--r--   0        0        0     7955 2024-01-05 11:19:12.440881 mass_composition-0.3.9/elphick/mass_composition/utils/pd_utils.py
--rw-r--r--   0        0        0       61 2024-01-05 11:19:12.440881 mass_composition-0.3.9/elphick/mass_composition/utils/sampling.py
--rw-r--r--   0        0        0      929 2024-01-05 11:19:12.440881 mass_composition-0.3.9/elphick/mass_composition/utils/size.py
--rw-r--r--   0        0        0     2630 2024-01-05 11:19:12.440881 mass_composition-0.3.9/elphick/mass_composition/utils/size_distribution.py
--rw-r--r--   0        0        0     1717 2024-01-05 11:19:12.440881 mass_composition-0.3.9/elphick/mass_composition/utils/viz.py
--rw-r--r--   0        0        0     8510 2024-01-05 11:19:12.440881 mass_composition-0.3.9/elphick/mass_composition/variables.py
--rw-r--r--   0        0        0     1762 2024-01-05 11:19:12.440881 mass_composition-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     4960 1970-01-01 00:00:00.000000 mass_composition-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-22 01:50:02.508773 mass_composition-0.4.3/LICENSE
+-rw-r--r--   0        0        0     3449 2024-04-22 01:50:02.508773 mass_composition-0.4.3/README.md
+-rw-r--r--   0        0        0      318 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/__init__.py
+-rw-r--r--   0        0        0     9833 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/balance.py
+-rw-r--r--   0        0        0       35 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/config/__init__.py
+-rw-r--r--   0        0        0      765 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/config/config_read.py
+-rw-r--r--   0        0        0      364 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/config/flowsheet_example.yaml
+-rw-r--r--   0        0        0      838 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/config/mc_config.yml
+-rw-r--r--   0        0        0     9284 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/dag.py
+-rw-r--r--   0        0        0       59 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/datasets/__init__.py
+-rw-r--r--   0        0        0     1892 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/datasets/datasets.py
+-rw-r--r--   0        0        0     1622 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/datasets/downloader.py
+-rw-r--r--   0        0        0     3046 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/datasets/register.csv
+-rw-r--r--   0        0        0     6569 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/datasets/sample_data.py
+-rw-r--r--   0        0        0     2080 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/layout.py
+-rw-r--r--   0        0        0    52166 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/mass_composition.py
+-rw-r--r--   0        0        0     4350 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/mc_node.py
+-rw-r--r--   0        0        0      638 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/mc_status.py
+-rw-r--r--   0        0        0    19410 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/mc_xarray.py
+-rw-r--r--   0        0        0    41220 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/network.py
+-rw-r--r--   0        0        0     5752 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/plot.py
+-rw-r--r--   0        0        0       42 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/utils/__init__.py
+-rw-r--r--   0        0        0      214 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3909 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc
+-rw-r--r--   0        0        0     2197 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc
+-rw-r--r--   0        0        0     1494 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc
+-rw-r--r--   0        0        0     1874 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/utils/amenability.py
+-rw-r--r--   0        0        0     2914 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/utils/components.py
+-rw-r--r--   0        0        0       80 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/utils/geometry.py
+-rw-r--r--   0        0        0     1193 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/utils/hash_utils.py
+-rw-r--r--   0        0        0     9591 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/utils/interp.py
+-rw-r--r--   0        0        0     3556 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/utils/loader.py
+-rw-r--r--   0        0        0     2611 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/utils/moisture.py
+-rw-r--r--   0        0        0     1033 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/utils/partition.py
+-rw-r--r--   0        0        0     7955 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/utils/pd_utils.py
+-rw-r--r--   0        0        0       61 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/utils/sampling.py
+-rw-r--r--   0        0        0     2164 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/utils/size.py
+-rw-r--r--   0        0        0     2630 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/utils/size_distribution.py
+-rw-r--r--   0        0        0     1717 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/utils/viz.py
+-rw-r--r--   0        0        0     8510 2024-04-22 01:50:02.912775 mass_composition-0.4.3/elphick/mass_composition/variables.py
+-rw-r--r--   0        0        0     1878 2024-04-22 01:50:02.916775 mass_composition-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     4989 1970-01-01 00:00:00.000000 mass_composition-0.4.3/PKG-INFO
```

### Comparing `mass_composition-0.3.9/LICENSE` & `mass_composition-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/README.md` & `mass_composition-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/balance.py` & `mass_composition-0.4.3/elphick/mass_composition/balance.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/config/config_read.py` & `mass_composition-0.4.3/elphick/mass_composition/config/config_read.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/config/mc_config.yml` & `mass_composition-0.4.3/elphick/mass_composition/config/mc_config.yml`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/datasets/datasets.py` & `mass_composition-0.4.3/elphick/mass_composition/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/datasets/downloader.py` & `mass_composition-0.4.3/elphick/mass_composition/datasets/downloader.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/datasets/register.csv` & `mass_composition-0.4.3/elphick/mass_composition/datasets/register.csv`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/datasets/sample_data.py` & `mass_composition-0.4.3/elphick/mass_composition/datasets/sample_data.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/layout.py` & `mass_composition-0.4.3/elphick/mass_composition/layout.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,25 +34,32 @@
     Intended for use with DiGraphs with a single degree 1 node with an out-edge
 
     This algorithm currently only works in two dimensions and does not
     try to minimize edge crossings.
 
     """
 
-    g.nodes[0]['_dist'] = 0
+    src_nodes = [n for n, d in g.in_degree() if d == 0]
+    g.nodes[src_nodes[0]]['_dist'] = 0
     for x_dist in range(1, len(g.nodes) + 1):
-        # get the x position from the tree "depth" / distance from the source node.
-        nodes_at_x_dist: dict = nx.descendants_at_distance(g, 0, x_dist)
+        nodes_at_x_dist: dict = nx.descendants_at_distance(g, src_nodes[0], x_dist)
         if not nodes_at_x_dist:
             break
         else:
-            # add the distance to the graph node to enable calling the multipartite layout
             for node in nodes_at_x_dist:
                 g.nodes[node]['_dist'] = x_dist
 
+    # Ensure all nodes have a _dist attribute
+    for node in g.nodes:
+        if '_dist' not in g.nodes[node]:
+            try:
+                g.nodes[node]['_dist'] = nx.shortest_path_length(g, source=src_nodes[0], target=node)
+            except nx.NetworkXNoPath:
+                g.nodes[node]['_dist'] = 0.0  # or any other default distance
+
     if orientation == 'vertical':
         orientation = 'horizontal'
     elif orientation == 'horizontal':
         orientation = 'vertical'
         scale = -scale
     else:
         raise ValueError("orientation argument not in 'vertical'|'horizontal'")
```

### Comparing `mass_composition-0.3.9/elphick/mass_composition/mass_composition.py` & `mass_composition-0.4.3/elphick/mass_composition/mass_composition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import logging
 from copy import deepcopy
 from pathlib import Path
-from typing import Dict, List, Optional, Union, Tuple, Iterable, Callable, Set, Literal
+from typing import Dict, List, Optional, Union, Tuple, Iterable, Callable, Set, Literal, Any
 
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 import xarray as xr
 
-
 from elphick.mass_composition.config import read_yaml
 from elphick.mass_composition.mc_status import Status
 from elphick.mass_composition.plot import parallel_plot, comparison_plot
 from elphick.mass_composition.utils import solve_mass_moisture
 from elphick.mass_composition.utils.amenability import amenability_index
 from elphick.mass_composition.utils.interp import mass_preserving_interp
 from elphick.mass_composition.utils.pd_utils import weight_average, calculate_recovery, calculate_partition
@@ -74,15 +73,15 @@
 
         if data is not None:
             self.set_data(data, constraints=constraints)
 
     def set_data(self, data: Union[pd.DataFrame, xr.Dataset],
                  constraints: Optional[Dict[str, List]] = None):
         if isinstance(data, xr.Dataset):
-            # we assume it is a complianct mc-xarray
+            # we assume it is a compliant mc-xarray
             self._data = data
             self.variables = Variables(config=self.config['vars'],
                                        supplied=[str(v) for v in data.variables if v not in data.dims],
                                        specified_map=self._specified_columns)
         elif isinstance(data, pd.DataFrame):
             if sum(data.index.duplicated()) > 0:
                 raise KeyError('The data has duplicate indexes.')
@@ -105,14 +104,18 @@
 
             self._data = xr_ds
 
         # explicitly define the constraints
         self.constraints: Dict = self.get_constraint_bounds(constraints=constraints)
         self.status = Status(self._check_constraints())
 
+    def rename(self, new_name: str) -> 'MassComposition':
+        self.name = new_name
+        return self
+
     def get_constraint_bounds(self, constraints: Optional[Dict[str, List]]) -> Dict[str, List]:
         d_constraints: Dict = {}
 
         # populate from the defaults
         for v in self.variables.mass_moisture.get_var_names():
             if 'mass' in v:
                 d_constraints[v] = self.config['constraints']['mass']
```

### Comparing `mass_composition-0.3.9/elphick/mass_composition/mc_node.py` & `mass_composition-0.4.3/elphick/mass_composition/mc_node.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/mc_status.py` & `mass_composition-0.4.3/elphick/mass_composition/mc_status.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/mc_xarray.py` & `mass_composition-0.4.3/elphick/mass_composition/mc_xarray.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/network.py` & `mass_composition-0.4.3/elphick/mass_composition/network.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import webbrowser
 from copy import deepcopy
 from pathlib import Path
-from typing import Dict, List, Optional, Tuple, Union, Iterable
+from typing import Dict, List, Optional, Tuple, Union
 
 import matplotlib
 import networkx as nx
 import numpy as np
 import pandas as pd
 import plotly.graph_objects as go
 from matplotlib import pyplot as plt
@@ -14,22 +14,21 @@
 import matplotlib.cm as cm
 import seaborn as sns
 from networkx import cytoscape_data
 
 from plotly.subplots import make_subplots
 
 from elphick.mass_composition import MassComposition
-from elphick.mass_composition.config import read_yaml
 from elphick.mass_composition.config.config_read import read_flowsheet_yaml
+from elphick.mass_composition.dag import DAG
 from elphick.mass_composition.layout import digraph_linear_layout
 from elphick.mass_composition.mc_node import MCNode, NodeType
 from elphick.mass_composition.plot import parallel_plot, comparison_plot
 from elphick.mass_composition.utils.geometry import midpoint
 from elphick.mass_composition.utils.loader import streams_from_dataframe
-from elphick.mass_composition.utils.pd_utils import column_prefix_counts, column_prefixes
 from elphick.mass_composition.utils.sampling import random_int
 
 
 class MCNetwork:
     def __init__(self, name: str = 'Flowsheet'):
         self.name: str = name
         self.graph: nx.DiGraph = nx.DiGraph()
@@ -122,14 +121,47 @@
             d_node_objects[node] = MCNode(node_id=int(node), node_name=config['nodes'][node]['name'],
                                           node_subset=config['nodes'][node]['subset'])
         nx.set_node_attributes(graph, d_node_objects, 'mc')
 
         obj.graph = graph
         return obj
 
+    @classmethod
+    def from_dag(cls, dag: DAG) -> 'MCNetwork':
+        """Construct a flowsheet from a dag object
+
+        Args:
+            dag: The dag object that has been run previously.
+
+        Returns:
+
+        """
+
+        # Create a new instance of MCNetwork
+        mcn = cls(name=dag.name)
+
+        # Copy the nodes from the dag to the MCNetwork
+        for nid, (node, data) in enumerate(dag.graph.nodes(data=True)):
+            mcn.graph.add_node(data['name'], mc=MCNode(node_id=nid, node_name=data['name']))
+
+        # Copy the edges from the dag to the MCNetwork
+        for edge in dag.graph.edges:
+            # Retrieve the MassComposition object from the edge
+            mc = dag.graph.edges[edge]['mc']
+            # Use the name of the MassComposition object as the name of the edge
+            mcn.graph.add_edge(*edge, name=mc.name, **dag.graph.edges[edge])
+
+        # Populate the inputs and outputs properties of the MCNode objects
+        for node in mcn.graph.nodes:
+            mc_node = mcn.graph.nodes[node]['mc']
+            mc_node.inputs = [mcn.graph.edges[edge]['mc'] for edge in mcn.graph.in_edges(node)]
+            mc_node.outputs = [mcn.graph.edges[edge]['mc'] for edge in mcn.graph.out_edges(node)]
+
+        return mcn
+
     @property
     def balanced(self) -> bool:
         bal_vals: List = [self.graph.nodes[n]['mc'].balanced for n in self.graph.nodes]
         bal_vals = [bv for bv in bal_vals if bv is not None]
         return all(bal_vals)
 
     @property
@@ -181,26 +213,30 @@
     def get_input_streams(self) -> List[MassComposition]:
         """Get the input (feed) streams (edge objects)
 
         Returns:
             List of MassComposition objects
         """
 
-        degrees = [d for n, d in self.graph.degree()]
+        # Create a dictionary that maps node names to their degrees
+        degrees = {n: d for n, d in self.graph.degree()}
+
         res: List[MassComposition] = [d['mc'] for u, v, d in self.graph.edges(data=True) if degrees[u] == 1]
         return res
 
     def get_output_streams(self) -> List[MassComposition]:
         """Get the output (product) streams (edge objects)
 
         Returns:
             List of MassComposition objects
         """
 
-        degrees = [d for n, d in self.graph.degree()]
+        # Create a dictionary that maps node names to their degrees
+        degrees = {n: d for n, d in self.graph.degree()}
+
         res: List[MassComposition] = [d['mc'] for u, v, d in self.graph.edges(data=True) if degrees[v] == 1]
         return res
 
     def get_column_formats(self, columns: List[str], strip_percent: bool = False) -> Dict[str, str]:
         """
 
         Args:
@@ -319,15 +355,15 @@
                     node_colors.append('red')
             else:
                 node_colors.append('gray')
 
         nx.draw(self.graph, pos=pos, ax=ax, with_labels=True, font_weight='bold',
                 node_color=node_colors, edge_color=edge_colors)
 
-        nx.draw_networkx_edge_labels(self, pos=pos, ax=ax, edge_labels=edge_labels, font_color='black')
+        nx.draw_networkx_edge_labels(self.graph, pos=pos, ax=ax, edge_labels=edge_labels, font_color='black')
         ax.set_title(self._plot_title(html=False), fontsize=10)
 
         return hf
 
     def plot_balance(self, facet_col_wrap: int = 3,
                      color: Optional[str] = 'node') -> go.Figure:
         """Plot input versus output across all nodes in the network
@@ -411,17 +447,22 @@
             edge_colormap: The optional colormap.  Used with color_var.
             vmin: The value that maps to the minimum color
             vmax: The value that maps to the maximum color
 
         Returns:
 
         """
-        if self.get_input_streams()[0].data.to_dataframe().empty:
-            raise KeyError("Cannot generate Sankey for an empty dataset")
-        d_sankey: Dict = self._generate_sankey_args(color_var, edge_colormap, width_var, vmin, vmax)
+        # Create a mapping of node names to indices, and the integer nodes
+        node_indices = {node: index for index, node in enumerate(self.graph.nodes)}
+        int_graph = nx.relabel_nodes(self.graph, node_indices)
+
+        # Generate the sankey diagram arguments using the new graph with integer nodes
+        d_sankey = self._generate_sankey_args(int_graph, color_var, edge_colormap, width_var, vmin, vmax)
+
+        # Create the sankey diagram
         node, link = self._get_sankey_node_link_dicts(d_sankey)
         fig = go.Figure(data=[go.Sankey(node=node, link=link)])
         title = self._plot_title()
         fig.update_layout(title_text=title, font_size=10)
         return fig
 
     def table_plot(self,
@@ -488,19 +529,24 @@
                        align='left', format=fmt,
                        fill_color=[
                            [table_odd_color if i % 2 == 0 else table_even_color for i in range(len(df))] * len(
                                df.columns)]),
             **d_table)
 
         if plot_type == 'sankey':
-            d_sankey: Dict = self._generate_sankey_args(sankey_color_var,
-                                                        sankey_edge_colormap,
-                                                        sankey_width_var,
-                                                        sankey_vmin,
-                                                        sankey_vmax)
+            # Create a mapping of node names to indices, and the integer nodes
+            node_indices = {node: index for index, node in enumerate(self.graph.nodes)}
+            int_graph = nx.relabel_nodes(self.graph, node_indices)
+
+            # Generate the sankey diagram arguments using the new graph with integer nodes
+            d_sankey = self._generate_sankey_args(int_graph, sankey_color_var,
+                                                  sankey_edge_colormap,
+                                                  sankey_width_var,
+                                                  sankey_vmin,
+                                                  sankey_vmax)
             node, link = self._get_sankey_node_link_dicts(d_sankey)
             fig.add_trace(go.Sankey(node=node, link=link), **d_plot)
 
         elif plot_type == 'network':
             # pos = nx.spring_layout(self, seed=1234)
             pos = digraph_linear_layout(self.graph, orientation=network_orientation)
 
@@ -716,15 +762,15 @@
                 plot_kwargs['row'] = 1
 
         if plot_type == 'network':  # different arguments for different plots
             plot_kwargs = {f'{k}s': v for k, v in plot_kwargs.items()}
 
         return subplot_kwargs, table_kwargs, plot_kwargs
 
-    def _generate_sankey_args(self, color_var, edge_colormap, width_var, v_min, v_max):
+    def _generate_sankey_args(self, int_graph, color_var, edge_colormap, width_var, v_min, v_max):
         rpt: pd.DataFrame = self.report()
         if color_var is not None:
             cmap = sns.color_palette(edge_colormap, as_cmap=True)
             rpt: pd.DataFrame = self.report()
             if not v_min:
                 v_min = np.floor(rpt[color_var].min())
             if not v_max:
@@ -737,29 +783,29 @@
         value: List = []
         edge_custom_data = []
         edge_color: List = []
         edge_labels: List = []
         node_colors: List = []
         node_labels: List = []
 
-        for n in self.graph.nodes:
-            if self.graph.nodes[n]['mc'].node_name != 'Node':
-                node_labels.append(self.graph.nodes[n]['mc'].node_name)
+        for n in int_graph.nodes:
+            if int_graph.nodes[n]['mc'].node_name != 'Node':
+                node_labels.append(int_graph.nodes[n]['mc'].node_name)
             else:
                 node_labels.append(str(n))  # the integer string
 
-            if self.graph.nodes[n]['mc'].node_type == NodeType.BALANCE:
-                if self.graph.nodes[n]['mc'].balanced:
+            if int_graph.nodes[n]['mc'].node_type == NodeType.BALANCE:
+                if int_graph.nodes[n]['mc'].balanced:
                     node_colors.append('green')
                 else:
                     node_colors.append('red')
             else:
                 node_colors.append('blue')
 
-        for u, v, data in self.graph.edges(data=True):
+        for u, v, data in int_graph.edges(data=True):
             edge_labels.append(data['mc'].name)
             source.append(u)
             target.append(v)
             value.append(float(data['mc'].aggregate()[width_var].iloc[0]))
             edge_custom_data.append(d_custom_data[data['mc'].name])
 
             if color_var is not None:
```

### Comparing `mass_composition-0.3.9/elphick/mass_composition/plot.py` & `mass_composition-0.4.3/elphick/mass_composition/plot.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc` & `mass_composition-0.4.3/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc` & `mass_composition-0.4.3/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc` & `mass_composition-0.4.3/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/utils/amenability.py` & `mass_composition-0.4.3/elphick/mass_composition/utils/amenability.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/utils/components.py` & `mass_composition-0.4.3/elphick/mass_composition/utils/components.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/utils/hash_utils.py` & `mass_composition-0.4.3/elphick/mass_composition/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/utils/interp.py` & `mass_composition-0.4.3/elphick/mass_composition/utils/interp.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/utils/loader.py` & `mass_composition-0.4.3/elphick/mass_composition/utils/loader.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/utils/moisture.py` & `mass_composition-0.4.3/elphick/mass_composition/utils/moisture.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/utils/partition.py` & `mass_composition-0.4.3/elphick/mass_composition/utils/partition.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/utils/pd_utils.py` & `mass_composition-0.4.3/elphick/mass_composition/utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/utils/size_distribution.py` & `mass_composition-0.4.3/elphick/mass_composition/utils/size_distribution.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/utils/viz.py` & `mass_composition-0.4.3/elphick/mass_composition/utils/viz.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/elphick/mass_composition/variables.py` & `mass_composition-0.4.3/elphick/mass_composition/variables.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.3.9/pyproject.toml` & `mass_composition-0.4.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mass-composition"
-version = "0.3.9"
+version = "0.4.3"
 description = "For managing multi-dimensional mass-composition datasets, supporting weighted mathematical operations and visualisation."
 authors = ["Greg <greg@elphick.com.au>"]
 packages = [{ include = "elphick/mass_composition" }]
 repository = "https://github.com/elphick/mass-composition"
 documentation = "https://elphick.github.io/mass-composition"
 readme = "README.md"
 
@@ -14,35 +14,37 @@
 #priority = "primary"
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "primary"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
-xarray = "^2022.6.0"
+python = ">=3.9,<3.12"
+xarray = ">=2022.6.0"
 periodictable = "^1.6.1"
 pyyaml = "^6.0"
 scipy = "^1.9.0"
 matplotlib = "^3.3"  # "^3.6.2"
 plotly = "^5.3"  # "^5.13.0"
 seaborn = ">0.11"  # "^0.12.2"
 pooch = "^1.7.0"
 jsonpickle = ">=3.0.1"
 
 kaleido = { version = "0.2.1", optional = true }
-pyvista = { version = "^0.37.0", optional = true }
-statsmodels = { version = "^0.14.0", optional = true }
-pyvista-xarray = { version = "^0.1.2", optional = true }
+pyvista = { version = ">=0.37.0", optional = true }
+statsmodels = { version = ">=0.14.0", optional = true }
+pyvista-xarray = { version = ">=0.1.2", optional = true }
 networkx = { version = ">2.0,<4.0", optional = true }
-omfvista = { version = "^0.2.5", optional = true }
+omfvista = { version = ">=0.2.5", optional = true }
+joblib = {version = "^1.4.0", optional = true}
+tqdm = {version = "^4.66.2", optional = true}
 
 [tool.poetry.extras]
 viz = ["kaleido", "pyvista", "statsmodels", "pyvista-xarray"]
-network = ["networkx"]
+network = ["networkx", "joblib", "tqdm"]
 omf = ["omfvista"]
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.0.5"
 notebook = "^6.5.2"
 pytest = "^7.2.0"
 Sphinx = "^5.0.2"
```

### Comparing `mass_composition-0.3.9/PKG-INFO` & `mass_composition-0.4.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: mass-composition
-Version: 0.3.9
+Version: 0.4.3
 Summary: For managing multi-dimensional mass-composition datasets, supporting weighted mathematical operations and visualisation.
 Home-page: https://github.com/elphick/mass-composition
 Author: Greg
 Author-email: greg@elphick.com.au
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: network
 Provides-Extra: omf
 Provides-Extra: viz
+Requires-Dist: joblib (>=1.4.0,<2.0.0) ; extra == "network"
 Requires-Dist: jsonpickle (>=3.0.1)
 Requires-Dist: kaleido (==0.2.1) ; extra == "viz"
 Requires-Dist: matplotlib (>=3.3,<4.0)
 Requires-Dist: networkx (>2.0,<4.0) ; extra == "network"
-Requires-Dist: omfvista (>=0.2.5,<0.3.0) ; extra == "omf"
+Requires-Dist: omfvista (>=0.2.5) ; extra == "omf"
 Requires-Dist: periodictable (>=1.6.1,<2.0.0)
 Requires-Dist: plotly (>=5.3,<6.0)
 Requires-Dist: pooch (>=1.7.0,<2.0.0)
-Requires-Dist: pyvista (>=0.37.0,<0.38.0) ; extra == "viz"
-Requires-Dist: pyvista-xarray (>=0.1.2,<0.2.0) ; extra == "viz"
+Requires-Dist: pyvista (>=0.37.0) ; extra == "viz"
+Requires-Dist: pyvista-xarray (>=0.1.2) ; extra == "viz"
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: scipy (>=1.9.0,<2.0.0)
 Requires-Dist: seaborn (>0.11)
-Requires-Dist: statsmodels (>=0.14.0,<0.15.0) ; extra == "viz"
-Requires-Dist: xarray (>=2022.6.0,<2023.0.0)
+Requires-Dist: statsmodels (>=0.14.0) ; extra == "viz"
+Requires-Dist: tqdm (>=4.66.2,<5.0.0) ; extra == "network"
+Requires-Dist: xarray (>=2022.6.0)
 Project-URL: Documentation, https://elphick.github.io/mass-composition
 Project-URL: Repository, https://github.com/elphick/mass-composition
 Description-Content-Type: text/markdown
 
 # MassComposition
 
 [![Run Tests](https://github.com/Elphick/mass-composition/actions/workflows/build_and_test.yml/badge.svg?branch=main)](https://github.com/Elphick/mass-composition/actions/workflows/build_and_test.yml)
```


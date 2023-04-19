# Comparing `tmp/tessif_oemof_4_4-0.1.6.tar.gz` & `tmp/tessif_oemof_4_4-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tessif_oemof_4_4-0.1.6.tar", max compression
+gzip compressed data, was "tessif_oemof_4_4-0.1.8.tar", max compression
```

## Comparing `tessif_oemof_4_4-0.1.6.tar` & `tessif_oemof_4_4-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-02-14 15:51:35.880359 tessif_oemof_4_4-0.1.6/LICENSE
--rw-r--r--   0        0        0     5715 2023-02-14 15:51:35.880359 tessif_oemof_4_4-0.1.6/README.rst
--rw-r--r--   0        0        0     1650 2023-02-14 15:51:35.880359 tessif_oemof_4_4-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      196 2023-02-14 15:51:35.880359 tessif_oemof_4_4-0.1.6/src/tessif_oemof_4_4/__init__.py
--rw-r--r--   0        0        0     2972 2023-02-14 15:51:35.880359 tessif_oemof_4_4-0.1.6/src/tessif_oemof_4_4/optimize.py
--rw-r--r--   0        0        0    52433 2023-02-14 15:51:35.880359 tessif_oemof_4_4-0.1.6/src/tessif_oemof_4_4/post_process.py
--rw-r--r--   0        0        0    50468 2023-02-14 15:51:35.880359 tessif_oemof_4_4-0.1.6/src/tessif_oemof_4_4/transform.py
--rw-r--r--   0        0        0     6652 1970-01-01 00:00:00.000000 tessif_oemof_4_4-0.1.6/setup.py
--rw-r--r--   0        0        0     6572 1970-01-01 00:00:00.000000 tessif_oemof_4_4-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-02-28 19:33:04.954621 tessif_oemof_4_4-0.1.8/LICENSE
+-rw-r--r--   0        0        0     5715 2023-02-28 19:33:04.954621 tessif_oemof_4_4-0.1.8/README.rst
+-rw-r--r--   0        0        0     1678 2023-02-28 19:33:04.958621 tessif_oemof_4_4-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      196 2023-02-28 19:33:04.958621 tessif_oemof_4_4-0.1.8/src/tessif_oemof_4_4/__init__.py
+-rw-r--r--   0        0        0     2972 2023-02-28 19:33:04.958621 tessif_oemof_4_4-0.1.8/src/tessif_oemof_4_4/optimize.py
+-rw-r--r--   0        0        0    53254 2023-02-28 19:33:04.958621 tessif_oemof_4_4-0.1.8/src/tessif_oemof_4_4/post_process.py
+-rw-r--r--   0        0        0    50283 2023-02-28 19:33:04.958621 tessif_oemof_4_4-0.1.8/src/tessif_oemof_4_4/transform.py
+-rw-r--r--   0        0        0     6652 1970-01-01 00:00:00.000000 tessif_oemof_4_4-0.1.8/setup.py
+-rw-r--r--   0        0        0     6572 1970-01-01 00:00:00.000000 tessif_oemof_4_4-0.1.8/PKG-INFO
```

### Comparing `tessif_oemof_4_4-0.1.6/LICENSE` & `tessif_oemof_4_4-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tessif_oemof_4_4-0.1.6/README.rst` & `tessif_oemof_4_4-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `tessif_oemof_4_4-0.1.6/pyproject.toml` & `tessif_oemof_4_4-0.1.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "tessif-oemof-4-4"
-version = "0.1.6"
+version = "0.1.8"
 description = "Tessif-Plugin for providing oemof version 4.4. support."
 authors = ["Mathias Ammon <tz3ma.coding@use.startmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/tZ3ma/tessif_oemof_4_4"
 homepage = "https://github.com/tZ3ma/tessif_oemof_4_4"
 keywords = ["Tessif", "Tessif-Oemof", "tessif-oemof", "ESSMOS", "optimization", "energy supply system modelling"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 oemof-solph = "0.4.4"
-tessif = ">=0.0.24"
+tessif = ">=0.0.27"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 coverage = {extras = ["toml"], version = "^6.3.2"}
 pytest-cov = "^3.0.0"
 pytest-mock = "^3.7.0"
 black = "^22.3.0"
@@ -30,14 +30,15 @@
 Sphinx = "^4.5.0"
 pep8-naming = "^0.12.1"
 pyupgrade = "^2.32.1"
 sphinx-paramlinks = "^0.5.2"
 pylint = "^2.14.0"
 nox = "^2022.1.7"
 nox-poetry = "^1.0.2"
+tessif-examples = ">=0.3.1"
 
 [tool.poetry.group.plugin.dependencies]
 oemof-solph = "0.4.4"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
```

### Comparing `tessif_oemof_4_4-0.1.6/src/tessif_oemof_4_4/optimize.py` & `tessif_oemof_4_4-0.1.8/src/tessif_oemof_4_4/optimize.py`

 * *Files identical despite different names*

### Comparing `tessif_oemof_4_4-0.1.6/src/tessif_oemof_4_4/post_process.py` & `tessif_oemof_4_4-0.1.8/src/tessif_oemof_4_4/post_process.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 """Wrapping the tessif-oemof post-processing."""
-from collections import defaultdict, abc
+from collections import abc, defaultdict
 
 import numpy as np
-from oemof import solph
 import pandas as pd
-
-from tessif.frused import (
-    namedtuples as nts,
-)
-
-from tessif.frused.defaults import energy_system_nodes as esn_defs
-
 import tessif.post_process as base
+from oemof import solph
+from tessif.frused import namedtuples as nts
+from tessif.frused.defaults import energy_system_nodes as esn_defs
 
 
 class OmfResultier(base.Resultier):
-    """ Transform nodes and edges into their name representation. Child of
+    """Transform nodes and edges into their name representation. Child of
     :class:`~tessif.transform.es2mapping.base.Resultier` and mother of all
     oemof Resultiers.
 
     Parameters
     ----------
     optimized_es: :class:`~oemof.core.energy_system.EnergySystem`
         An optimized oemof energy system containing its
         :ref:`results <omf_results>`.
     """
 
     component_type_mapping = {
-        solph.components.GenericStorage: 'storage',
-        solph.components.ExtractionTurbineCHP: 'transformer',
-        solph.components.GenericCHP: 'transformer',
-        solph.components.OffsetTransformer: 'transformer',
-        solph.custom.Link: 'connector',
-
-        solph.network.Bus: 'bus',
-        solph.network.Sink: 'sink',
-        solph.network.Source: 'source',
-        solph.network.Transformer: 'transformer',
+        solph.components.GenericStorage: "storage",
+        solph.components.ExtractionTurbineCHP: "transformer",
+        solph.components.GenericCHP: "transformer",
+        solph.components.OffsetTransformer: "transformer",
+        solph.custom.Link: "connector",
+        solph.network.Bus: "bus",
+        solph.network.Sink: "sink",
+        solph.network.Source: "source",
+        solph.network.Transformer: "transformer",
     }
 
     def __init__(self, optimized_es, **kwargs):
 
         super().__init__(optimized_es=optimized_es, **kwargs)
 
     def _map_nodes(self, optimized_es):
@@ -50,28 +44,41 @@
     def _map_node_uids(self, optimized_es):
         """Return a list of node uids."""
         _uid_nodes = dict()
         for node in optimized_es.nodes:
             prelim_uid = node.label
             if prelim_uid.component is None:
                 uid_dict = prelim_uid._asdict()
-                uid_dict['component'] = OmfResultier.component_type_mapping[
-                    type(node)]
+                uid_dict["component"] = OmfResultier.component_type_mapping[type(node)]
                 uid = nts.Uid(**uid_dict)
             else:
                 uid = prelim_uid
 
             _uid_nodes[str(node.label)] = uid
 
         return _uid_nodes
 
     def _map_edges(self, optimized_es):
         r"""Return list of (inflow, node) label string representation."""
-        return [nts.Edge(str(inflow), str(node)) for node in optimized_es.nodes
-                for inflow in node.inputs.keys()]
+        return [
+            nts.Edge(str(inflow), str(node))
+            for node in optimized_es.nodes
+            for inflow in node.inputs.keys()
+        ]
+
+    def dct_repr(self):
+        """Extend the base dict reprsentation."""
+        excluded = [
+            "_inflow_characterized_components",
+            "_outflow_characterized_components",
+        ]
+        dct = {
+            key: value for key, value in self.__dict__.items() if key not in excluded
+        }
+        return dct
 
 
 class IntegratedGlobalResultier(OmfResultier, base.IntegratedGlobalResultier):
     """Extracting the integrated global results out of the energy system and
     conveniently aggregating them (rounded to unit place) inside a dictionairy
     keyed by result name.
 
@@ -149,130 +156,167 @@
         capital_costs = 0.0
 
         for edge in self.edges:
             net_energy_flow = flow_results.edge_net_energy_flow[edge]
             specific_emissions = flow_results.edge_specific_emissions[edge]
             specific_flow_costs = flow_results.edge_specific_flow_costs[edge]
 
-            total_emissions += (
-                net_energy_flow *
-                specific_emissions
-            )
+            total_emissions += net_energy_flow * specific_emissions
 
-            flow_costs += (
-                net_energy_flow *
-                specific_flow_costs
-            )
+            flow_costs += net_energy_flow * specific_flow_costs
 
         for node in self.nodes:
             initial_capacity = cap_results.node_original_capacity[node]
             final_capacity = cap_results.node_installed_capacity[node]
             expansion_cost = cap_results.node_expansion_costs[node]
 
-            if not any(
-                    [cap is None
-                     for cap in (final_capacity, initial_capacity)]
-            ):
+            if not any([cap is None for cap in (final_capacity, initial_capacity)]):
                 node_expansion_costs = (
-                    (final_capacity - initial_capacity) *
-                    expansion_cost
-                )
+                    final_capacity - initial_capacity
+                ) * expansion_cost
             else:
                 node_expansion_costs = 0
 
             if isinstance(initial_capacity, pd.Series):
                 node_expansion_costs = sum(node_expansion_costs)
 
             capital_costs += node_expansion_costs
 
         return {
-            'emissions (sim)': round(total_emissions, 0),
-            'costs (sim)': round(optimized_es.results['global']['costs'], 0,),
-            'opex (ppcd)': round(flow_costs, 0),
-            'capex (ppcd)': round(capital_costs, 0),
+            "emissions (sim)": round(total_emissions, 0),
+            "costs (sim)": round(
+                optimized_es.results["global"]["costs"],
+                0,
+            ),
+            "opex (ppcd)": round(flow_costs, 0),
+            "capex (ppcd)": round(capital_costs, 0),
         }
 
-        return optimized_es.results['global']
+        return optimized_es.results["global"]
+
+
+class ScaleResultier(OmfResultier, base.ScaleResultier):
+    """Extract number of constraints.
+
+    Parameters
+    ----------
+    optimized_es:
+        :ref:`Model <SupportedModels>` specific, optimized energy system
+        containing its results.
+
+    See Also
+    --------
+    For functionality documentation see the respective :class:`base class
+    <tessif.post_process.ScaleResultier>`.
+    """
+
+    def __init__(self, optimized_es, **kwargs):
+        super().__init__(optimized_es=optimized_es, **kwargs)
+
+    def _map_number_of_constraints(self, optimized_es):
+        """Interface to extract the number of constraints out of the
+        optimized oemof system model.
+        """
+        return optimized_es.results.problem.number_of_constraints
 
 
 class LoadResultier(OmfResultier, base.LoadResultier):
     """
     Transforming flow results into dictionairies keyed by node.
 
     Parameters
     ----------
     optimized_es: :class:`~oemof.core.energy_system.EnergySystem`
         An optimized oemof energy system containing its
         :ref:`results <omf_results>`.
 
-    See also
+    See Also
     --------
     For functionality documentation see the respective :class:`base class
     <tessif.transform.es2mapping.base.LoadResultier>`.
     """
 
     def __init__(self, optimized_es, **kwargs):
         super().__init__(optimized_es=optimized_es, **kwargs)
 
     def _map_loads(self, optimized_es):
-        """ Map loads to node labels"""
+        """Map loads to node labels."""
         # Use defaultdict of empty DataFrame as loads container:
         _loads = defaultdict(lambda: pd.DataFrame())
 
         for node in optimized_es.nodes:
             time_series_results = solph.views.node(
-                optimized_es.results['main'], node).get(
-                    'sequences', pd.DataFrame())
+                optimized_es.results["main"], node
+            ).get("sequences", pd.DataFrame())
 
             # only keep columns with 'flow' results
             time_series_results = time_series_results[
-                np.array([col for col in time_series_results.columns
-                          if 'flow' == col[1]], dtype=object)]
+                np.array(
+                    [col for col in time_series_results.columns if "flow" == col[1]],
+                    dtype=object,
+                )
+            ]
 
             # rename time_series_results to to edge labels
             time_series_results.rename(
-                columns={col: (str(col[0][0].label), str(col[0][1].label))
-                         for col in time_series_results.columns}, inplace=True)
+                columns={
+                    col: (str(col[0][0].label), str(col[0][1].label))
+                    for col in time_series_results.columns
+                },
+                inplace=True,
+            )
 
             temp_df = time_series_results.copy()
             # rename time_series_results inflow columns to inflow node name
             time_series_results.rename(
                 columns={
-                    col: n for col in time_series_results.columns
-                    for n in col if not any(
-                        str(x.label) == col[1]
-                        for x in node.outputs.keys()) and
-                    n != str(node.label)}, inplace=True)
-
-            inflows = time_series_results.drop(columns=[
-                col for col in time_series_results.columns if isinstance(
-                    col, tuple)])
+                    col: n
+                    for col in time_series_results.columns
+                    for n in col
+                    if not any(str(x.label) == col[1] for x in node.outputs.keys())
+                    and n != str(node.label)
+                },
+                inplace=True,
+            )
+
+            inflows = time_series_results.drop(
+                columns=[
+                    col for col in time_series_results.columns if isinstance(col, tuple)
+                ]
+            )
 
             # make inflow values negative
             inflows = inflows.multiply(-1)
             # enforce -0. on inflows
             inflows = inflows.replace({0: -float(0), float(0): -float(0)})
 
-            outflows = time_series_results.drop(columns=[
-                col for col in time_series_results.columns if not isinstance(
-                    col, tuple)])
+            outflows = time_series_results.drop(
+                columns=[
+                    col
+                    for col in time_series_results.columns
+                    if not isinstance(col, tuple)
+                ]
+            )
 
             # enforce +0. on outflows
             outflows = outflows.replace({-float(0): float(0)})
 
             # rename time_series_results out columns to outflow node name
             outflows.rename(
                 columns={
-                    col: n for col in temp_df.columns
-                    for n in col if not any(
-                        str(x.label) == col[0] for x in node.inputs.keys()) and
-                    n != str(node.label)}, inplace=True)
+                    col: n
+                    for col in temp_df.columns
+                    for n in col
+                    if not any(str(x.label) == col[0] for x in node.inputs.keys())
+                    and n != str(node.label)
+                },
+                inplace=True,
+            )
 
-            time_series_results = pd.concat(
-                [inflows, outflows], axis='columns')
+            time_series_results = pd.concat([inflows, outflows], axis="columns")
             time_series_results.columns.name = str(node.label)
             _loads[str(node.label)] = time_series_results
 
         return dict(_loads)
 
 
 class CapacityResultier(base.CapacityResultier, LoadResultier):
@@ -288,28 +332,25 @@
     --------
     For functionality documentation see the respective :class:`base class
     <tessif.transform.es2mapping.base.CapacityResultier>`.
     """
 
     def __init__(self, optimized_es, **kwargs):
 
-        self._inflow_characterized_components = (
-            solph.Sink,
-        )
+        self._inflow_characterized_components = (solph.Sink,)
 
         self._outflow_characterized_components = (
             solph.Transformer,
             solph.Source,
             solph.components.OffsetTransformer,
             solph.components.ExtractionTurbineCHP,
-            solph.components.GenericCHP
+            solph.components.GenericCHP,
         )
 
-        super().__init__(optimized_es=optimized_es,
-                         **kwargs)
+        super().__init__(optimized_es=optimized_es, **kwargs)
 
     @property
     def node_characteristic_value(self):
         r"""Map node label to characteristic value.
 
         Components of variable size have a characteristic value of ``None``.
 
@@ -378,47 +419,46 @@
             node_inst_cap_dict = dict()
             # map inflow characterized nodes:
             if isinstance(node, self._inflow_characterized_components):
                 for inflow in node.inputs.keys():
                     if (inflow, node) in optimized_es.flows():
                         # parse investment objects
                         inv_obj = getattr(
-                            optimized_es.flows()[(inflow, node)],
-                            'investment'
+                            optimized_es.flows()[(inflow, node)], "investment"
                         )
                         # is inflow -> node characterized by investment?
                         if inv_obj:
 
                             # yes, so get the results sub dict holding it ...
                             scalar_results = solph.views.node(
-                                optimized_es.results['main'],
-                                node
-                            ).get('scalars', dict())
+                                optimized_es.results["main"], node
+                            ).get("scalars", dict())
 
                             # ... extract the value
                             # ... and add start value
-                            inst_cap = scalar_results.get(
-                                ((inflow, node), 'invest'), 0) \
+                            inst_cap = (
+                                scalar_results.get(((inflow, node), "invest"), 0)
                                 + inv_obj.existing
+                            )
 
                         else:
                             # Extract nominal_value if present
                             inst_cap = getattr(
                                 optimized_es.flows()[(inflow, node)],
-                                'nominal_value',
-                                esn_defs[
-                                    'variable_capacity']
+                                "nominal_value",
+                                esn_defs["variable_capacity"],
                             )
 
                             # or the inst cap is inferred by using the
                             # max inflow
-                            if inst_cap == esn_defs['variable_capacity']:
+                            if inst_cap == esn_defs["variable_capacity"]:
                                 inst_cap = max(
-                                    self.node_inflows[
-                                        str(node.label)][str(inflow.label)]
+                                    self.node_inflows[str(node.label)][
+                                        str(inflow.label)
+                                    ]
                                 )
                         node_inst_cap_dict[str(inflow.label)] = inst_cap
 
                 if len(node.inputs.keys()) > 1:
                     # distinguish between multiple inflows characterized nodes
                     inst_cap = pd.Series(node_inst_cap_dict)
                 else:
@@ -428,52 +468,50 @@
                 _installed_capacities[str(node.label)] = inst_cap
 
             elif isinstance(node, self._outflow_characterized_components):
                 for outflow in node.outputs.keys():
                     if (node, outflow) in optimized_es.flows():
                         # parse investment objects
                         inv_obj = getattr(
-                            optimized_es.flows()[(node, outflow)],
-                            'investment'
+                            optimized_es.flows()[(node, outflow)], "investment"
                         )
 
                         if inv_obj:
                             # is node -> outflow characterized by investment?
 
                             # yes, so get the results sub dict holding it ...
                             scalar_results = solph.views.node(
-                                optimized_es.results['main'],
-                                node
-                            ).get('scalars', dict())
+                                optimized_es.results["main"], node
+                            ).get("scalars", dict())
 
                             # ... extract the value
                             # ... and add start value
-                            inst_cap = scalar_results.get(
-                                ((node, outflow), 'invest'), 0) \
+                            inst_cap = (
+                                scalar_results.get(((node, outflow), "invest"), 0)
                                 + inv_obj.existing
+                            )
 
                         else:
                             # No, so nominal value is the installed capacity ..
                             inst_cap = getattr(
                                 optimized_es.flows()[(node, outflow)],
-                                'nominal_value',
-                                esn_defs['variable_capacity']
+                                "nominal_value",
+                                esn_defs["variable_capacity"],
                             )
 
                             # or the inst cap is inferred by using the
                             # max outflow
-                            if inst_cap == esn_defs['variable_capacity']:
-                                outflow_series = self.node_outflows[
-                                    str(node.label)][str(outflow.label)]
+                            if inst_cap == esn_defs["variable_capacity"]:
+                                outflow_series = self.node_outflows[str(node.label)][
+                                    str(outflow.label)
+                                ]
                                 # inst_cap = max(outflow_series)
                                 # account for unused storages
                                 if not outflow_series.empty:
-                                    inst_cap = max(
-                                        outflow_series
-                                    )
+                                    inst_cap = max(outflow_series)
                                 else:
                                     inst_cap = 0
 
                         node_inst_cap_dict[str(outflow.label)] = inst_cap
 
                 if len(node.outputs.keys()) > 1:
                     # distinguish between multiple outflows characterized
@@ -482,33 +520,34 @@
                 else:
                     # and singular ones
                     inst_cap = tuple(node_inst_cap_dict.values())[0]
 
                 _installed_capacities[str(node.label)] = inst_cap
 
             elif isinstance(node, (solph.Bus, solph.custom.Link)):
-                _installed_capacities[
-                    str(node.label)] = esn_defs['variable_capacity']
+                _installed_capacities[str(node.label)] = esn_defs["variable_capacity"]
 
             elif isinstance(node, solph.components.GenericStorage):
 
                 if node.investment:
 
                     additional_capacity = solph.views.node(
-                        optimized_es.results['main'], node).get('scalars')[
-                        ((node, None), 'invest')]
+                        optimized_es.results["main"], node
+                    ).get("scalars")[((node, None), "invest")]
 
                     existing_capacity = node.investment.existing
 
                     _installed_capacities[str(node.label)] = (
-                        additional_capacity + existing_capacity)
+                        additional_capacity + existing_capacity
+                    )
 
                 else:
-                    _installed_capacities[str(node.label)] = (
-                        node.nominal_storage_capacity)
+                    _installed_capacities[
+                        str(node.label)
+                    ] = node.nominal_storage_capacity
 
         return dict(_installed_capacities)
 
     def _map_original_capacities(self, optimized_es):
         """Map pre-optimized installed capacities to node labels.
         tessif.frused.esn_defs['variable_capacity'] for
         nodes of variable size"""
@@ -521,33 +560,31 @@
             node_inst_cap_dict = dict()
             # map inflow characterized nodes:
             if isinstance(node, self._inflow_characterized_components):
                 for inflow in node.inputs.keys():
                     if (inflow, node) in optimized_es.flows():
                         # parse investment objects
                         inv_obj = getattr(
-                            optimized_es.flows()[(inflow, node)],
-                            'investment'
+                            optimized_es.flows()[(inflow, node)], "investment"
                         )
                         # is inflow -> node characterized by investment?
                         if inv_obj:
                             inst_cap = inv_obj.existing
 
                         else:
                             # Extract nominal_value if present
                             inst_cap = getattr(
                                 optimized_es.flows()[(inflow, node)],
-                                'nominal_value',
-                                esn_defs[
-                                    'variable_capacity']
+                                "nominal_value",
+                                esn_defs["variable_capacity"],
                             )
 
                             # or the inst cap is set to 0 if no value was set
                             # an thus a fallback on the default occurred
-                            if inst_cap == esn_defs['variable_capacity']:
+                            if inst_cap == esn_defs["variable_capacity"]:
                                 inst_cap = 0
 
                         node_inst_cap_dict[str(inflow.label)] = inst_cap
 
                 if len(node.inputs.keys()) > 1:
                     # distinguish between multiple inflows characterized nodes
                     inst_cap = pd.Series(node_inst_cap_dict)
@@ -558,49 +595,47 @@
                 _installed_capacities[str(node.label)] = inst_cap
 
             elif isinstance(node, self._outflow_characterized_components):
                 for outflow in node.outputs.keys():
                     if (node, outflow) in optimized_es.flows():
                         # parse investment objects
                         inv_obj = getattr(
-                            optimized_es.flows()[(node, outflow)],
-                            'investment'
+                            optimized_es.flows()[(node, outflow)], "investment"
                         )
 
                         if inv_obj:
                             # is node -> outflow characterized by investment?
                             inst_cap = inv_obj.existing
 
                         else:
                             # No, so nominal value is the installed capacity ..
                             inst_cap = getattr(
                                 optimized_es.flows()[(node, outflow)],
-                                'nominal_value',
-                                esn_defs['variable_capacity']
+                                "nominal_value",
+                                esn_defs["variable_capacity"],
                             )
 
                             # or the inst cap is set to 0 if no value was set
                             # an thus a fallback on the default occurred
-                            if inst_cap == esn_defs['variable_capacity']:
+                            if inst_cap == esn_defs["variable_capacity"]:
                                 inst_cap = 0
 
                         node_inst_cap_dict[str(outflow.label)] = inst_cap
 
                 if len(node.outputs.keys()) > 1:
                     # distinguish between multiple outflows characterized nodes
                     inst_cap = pd.Series(node_inst_cap_dict)
                 else:
                     # and singular ones
                     inst_cap = tuple(node_inst_cap_dict.values())[0]
 
                 _installed_capacities[str(node.label)] = inst_cap
 
             elif isinstance(node, (solph.Bus, solph.custom.Link)):
-                _installed_capacities[
-                    str(node.label)] = esn_defs['variable_capacity']
+                _installed_capacities[str(node.label)] = esn_defs["variable_capacity"]
 
             elif isinstance(node, solph.components.GenericStorage):
 
                 if node.investment:
                     inst_cap = node.investment.existing
 
                 else:
@@ -619,23 +654,22 @@
             node_expansion_costs_dict = dict()
             # map inflow characterized nodes:
             if isinstance(node, self._inflow_characterized_components):
                 for inflow in node.inputs.keys():
                     if (inflow, node) in optimized_es.flows():
                         # parse investment objects
                         inv_obj = getattr(
-                            optimized_es.flows()[(inflow, node)],
-                            'investment'
+                            optimized_es.flows()[(inflow, node)], "investment"
                         )
                         # is inflow -> node characterized by investment?
                         if inv_obj:
                             cost = inv_obj.ep_costs
 
                         else:
-                            cost = esn_defs['expansion_costs']
+                            cost = esn_defs["expansion_costs"]
 
                         node_expansion_costs_dict[str(inflow.label)] = cost
 
                 if len(node.inputs.keys()) > 1:
                     # distinguish between multiple inflows characterized nodes
                     inst_cap = pd.Series(node_expansion_costs_dict)
                 else:
@@ -645,23 +679,22 @@
                 expansion_costs[str(node.label)] = inst_cap
 
             elif isinstance(node, self._outflow_characterized_components):
                 for outflow in node.outputs.keys():
                     if (node, outflow) in optimized_es.flows():
                         # parse investment objects
                         inv_obj = getattr(
-                            optimized_es.flows()[(node, outflow)],
-                            'investment'
+                            optimized_es.flows()[(node, outflow)], "investment"
                         )
 
                         if inv_obj:
                             # is node -> outflow characterized by investment?
                             cost = inv_obj.ep_costs
                         else:
-                            cost = esn_defs['expansion_costs']
+                            cost = esn_defs["expansion_costs"]
 
                         node_expansion_costs_dict[str(outflow.label)] = cost
 
                 if len(node.outputs.keys()) > 1:
                     # distinguish between multiple outflows characterized nodes
                     costs = pd.Series(node_expansion_costs_dict)
                 else:
@@ -672,96 +705,97 @@
 
             elif isinstance(node, solph.components.GenericStorage):
 
                 if node.investment:
                     costs = node.investment.ep_costs
 
                 else:
-                    costs = esn_defs['expansion_costs']
+                    costs = esn_defs["expansion_costs"]
 
                 expansion_costs[str(node.label)] = costs
 
             else:
-                expansion_costs[str(node.label)] = esn_defs['expansion_costs']
+                expansion_costs[str(node.label)] = esn_defs["expansion_costs"]
 
         return expansion_costs
 
     def _map_characteristic_values(self, optimized_es):
         """Map node label to characteristic value."""
 
         # Use default dict as capacity factors container:
         _characteristic_values = defaultdict(float)
 
         # Map the respective capacity factors:
         for node in optimized_es.nodes:
 
-            characteristic_mean = pd.Series()
+            characteristic_mean = pd.Series(dtype="float64")
 
             inst_cap = self._installed_capacities[str(node.label)]
 
             # is the installed capacity a singular value?
             if not isinstance(inst_cap, abc.Iterable):
 
                 # yes, it is
-                if inst_cap != esn_defs[
-                        'variable_capacity']:
+                if inst_cap != esn_defs["variable_capacity"]:
 
-                    if isinstance(node,
-                                  solph.components.GenericCHP):
+                    if isinstance(node, solph.components.GenericCHP):
                         char_tar = list(node.electrical_output)[0]
-                        characteristic_mean = self._outflows[
-                            str(node.label)][str(char_tar)].mean(axis='index')
+                        characteristic_mean = self._outflows[str(node.label)][
+                            str(char_tar)
+                        ].mean(axis="index")
 
                     elif isinstance(node, solph.components.GenericStorage):
-                        characteristic_mean = StorageResultier(
-                            optimized_es).node_soc[str(node.label)].mean(
-                                axis='index')
+                        characteristic_mean = (
+                            StorageResultier(optimized_es)
+                            .node_soc[str(node.label)]
+                            .mean(axis="index")
+                        )
 
                     # map all other nodes
                     else:
                         characteristic_mean = self.node_summed_loads[
-                            str(node.label)].mean(axis='index')
+                            str(node.label)
+                        ].mean(axis="index")
 
                     # deal with node of variable size, left unused:
                     if inst_cap == 0:
                         _characteristic_values[str(node.label)] = 0
                     else:
-                        _characteristic_values[
-                            str(node.label)] = characteristic_mean / inst_cap
+                        _characteristic_values[str(node.label)] = (
+                            characteristic_mean / inst_cap
+                        )
                     # print(characteristic_mean, inst_cap)
 
                 else:
-                    _characteristic_values[
-                        str(node.label)] = esn_defs[
-                            'characteristic_value']
+                    _characteristic_values[str(node.label)] = esn_defs[
+                        "characteristic_value"
+                    ]
 
             # not its not, so keep the series format
             else:
 
-                characteristic_mean = self._outflows[
-                    str(node.label)].mean()
+                characteristic_mean = self._outflows[str(node.label)].mean()
 
                 # create the series beforehand
-                char_values = pd.Series()
+                char_values = pd.Series(dtype="float64")
                 for idx, cap in inst_cap.fillna(0).items():
 
                     if cap != 0:
                         char_values[idx] = characteristic_mean[idx] / cap
                     else:
                         char_values[idx] = 0
 
                 # to replace nans by 0:
-                _characteristic_values[
-                    str(node.label)] = char_values.fillna(0)
+                _characteristic_values[str(node.label)] = char_values.fillna(0)
 
         return dict(_characteristic_values)
 
 
 class StorageResultier(OmfResultier, base.StorageResultier):
-    r""" Transforming storage results into dictionairies keyed by node.
+    r"""Transforming storage results into dictionairies keyed by node.
 
     Parameters
     ----------
     optimized_es: :class:`~oemof.core.energy_system.EnergySystem`
         An optimized oemof energy system containing its
         :ref:`results <omf_results>`.
 
@@ -771,32 +805,31 @@
     <tessif.transform.es2mapping.base.StorageResultier>`.
     """
 
     def __init__(self, optimized_es, **kwargs):
         super().__init__(optimized_es=optimized_es, **kwargs)
 
     def _map_states_of_charge(self, optimized_es):
-        """ Map storage labels to their states of charge"""
+        """Map storage labels to their states of charge"""
 
-        _socs = defaultdict(lambda: pd.Series())
+        _socs = defaultdict(lambda: pd.Series(dtype="float64"))
         for node in optimized_es.nodes:
-            if isinstance(node,
-                          solph.components.GenericStorage):
-                soc = solph.views.node(
-                    optimized_es.results['main'], node).get(
-                        'sequences')[((node, None), 'storage_content')]
+            if isinstance(node, solph.components.GenericStorage):
+                soc = solph.views.node(optimized_es.results["main"], node).get(
+                    "sequences"
+                )[((node, None), "storage_content")]
                 soc.name = str(node.label)
 
                 _socs[str(node.label)] = soc
 
         return dict(_socs)
 
 
 class NodeCategorizer(OmfResultier, base.NodeCategorizer):
-    r""" Categorizing the nodes of an optimized oemof energy system.
+    r"""Categorizing the nodes of an optimized oemof energy system.
 
     Categorization utilizes :attr:`~tessif.frused.namedtuples.Uid`.
 
     Nodes are categorized by:
 
         - Energy :paramref:`component
           <tessif.frused.namedtuples.Uid.component>`
@@ -836,67 +869,68 @@
         """Nodes ordered by component "Bus" "Sink" etc.."""
 
         # Use default dict as sector strings container
         _component_nodes = defaultdict(list)
 
         # Map the respective sectors:
         for node in optimized_es.nodes:
-            if hasattr(node.label, 'component'):
+            if hasattr(node.label, "component"):
                 _component_nodes[node.label.component.lower().capitalize()].append(
-                    str(node.label))
+                    str(node.label)
+                )
             # Node has no component attributed in node.label
             else:
-                _component_nodes['Unspecified'].append(str(node.label))
+                _component_nodes["Unspecified"].append(str(node.label))
 
         return dict(_component_nodes)
 
     def _map_node_sectors(self, optimized_es):
         """Nodes ordered by sector. i.e "Power" "Heat" "Mobility" "Coupled"."""
 
         # Use default dict as sector strings container
         _sectored_nodes = defaultdict(list)
 
         # Map the respective sectors:
         for node in optimized_es.nodes:
-            if hasattr(node.label, 'sector'):
+            if hasattr(node.label, "sector"):
                 _sectored_nodes[node.label.sector].append(str(node.label))
             # Node has no sector attributed in node.label
             else:
-                _sectored_nodes['Unspecified'].append(str(node.label))
+                _sectored_nodes["Unspecified"].append(str(node.label))
 
         return dict(_sectored_nodes)
 
     def _map_node_regions(self, optimized_es):
         """Nodes ordered by region. i.e "World" "South" "Antinational"."""
 
         # Use default dict as sector strings container
         _regionalized_nodes = defaultdict(list)
 
         # Map the respective sectors:
         for node in optimized_es.nodes:
-            if hasattr(node.label, 'region'):
+            if hasattr(node.label, "region"):
                 _regionalized_nodes[node.label.region].append(str(node.label))
             # Node has no region attributed in node.label
             else:
-                _regionalized_nodes['Unspecified'].append(str(node.label))
+                _regionalized_nodes["Unspecified"].append(str(node.label))
 
         return dict(_regionalized_nodes)
 
     def _map_node_coordinates(self, optimized_es):
         """Longitude and Latitude of each node present in energy system."""
 
         # Use default dict as coordinate namedtuple container
         _coordinates = defaultdict(nts.Coordinates)
 
         # 3.) Map the respective coordinates:
         for node in optimized_es.nodes:
-            if (hasattr(node.label, 'latitude') and
-                    hasattr(node.label, 'latitude')):
+            if hasattr(node.label, "latitude") and hasattr(node.label, "latitude"):
                 _coordinates[str(node.label)] = nts.Coordinates(
-                    node.label.latitude, node.label.longitude)
+                    node.label.latitude, node.label.longitude
+                )
 
             # Node has no coordinates attributed in node.label
             else:
                 _coordinates[str(node.label)] = nts.Coordinates(None, None)
 
         return dict(_coordinates)
 
@@ -905,39 +939,38 @@
 
         # Use default dict as carrier strings container
         _carrier_grouped_nodes = defaultdict(list)
         _node_energy_carriers = defaultdict(str)
 
         # Map the respective carriers:
         for node in optimized_es.nodes:
-            if hasattr(node.label, 'carrier'):
-                _carrier_grouped_nodes[node.label.carrier].append(
-                    str(node.label))
+            if hasattr(node.label, "carrier"):
+                _carrier_grouped_nodes[node.label.carrier].append(str(node.label))
                 _node_energy_carriers[str(node.label)] = node.label.carrier
 
             # Node has no region attributed in node.label
             else:
-                _carrier_grouped_nodes['Unspecified'].append(str(node.label))
-                _node_energy_carriers[str(node.label)] = 'Unspecified'
+                _carrier_grouped_nodes["Unspecified"].append(str(node.label))
+                _node_energy_carriers[str(node.label)] = "Unspecified"
 
         return (dict(_carrier_grouped_nodes), dict(_node_energy_carriers))
 
     def _map_node_types(self, optimized_es):
         """Nodes grouped by "type" (arbitrary classification)"""
 
         # Use default dict as sector strings container
         _typed_nodes = defaultdict(list)
 
         # Map the respective sectors:
         for node in optimized_es.nodes:
-            if hasattr(node.label, 'node_type'):
+            if hasattr(node.label, "node_type"):
                 _typed_nodes[node.label.node_type].append(str(node.label))
             # Node has no sector attributed in node.label
             else:
-                _typed_nodes['Unspecified'].append(str(node.label))
+                _typed_nodes["Unspecified"].append(str(node.label))
 
         return dict(_typed_nodes)
 
 
 class FlowResultier(base.FlowResultier, LoadResultier):
     """
     Transforming flow results into dictionairies keyed by edges.
@@ -952,44 +985,43 @@
     --------
     For functionality documentation see the respective :class:`base class
     <tessif.transform.es2mapping.base.FlowResultier>`.
     """
 
     def __init__(self, optimized_es, **kwargs):
 
-        super().__init__(optimized_es=optimized_es,
-                         **kwargs)
+        super().__init__(optimized_es=optimized_es, **kwargs)
 
     def _map_specific_flow_costs(self, optimized_es):
         r"""Energy specific flow costs mapped to edges."""
         # Use default dict as net energy flows container:
         _specific_flow_costs = defaultdict(float)
 
         # Map the respective flow costs:
         for node in optimized_es.nodes:
             for inflow in node.inputs.keys():
                 _specific_flow_costs[
-                    nts.Edge(str(inflow.label), str(node.label))] = getattr(
-                        optimized_es.flows()[
-                            (inflow, node)], 'variable_costs', 0)[0]
+                    nts.Edge(str(inflow.label), str(node.label))
+                ] = getattr(optimized_es.flows()[(inflow, node)], "variable_costs", 0)[
+                    0
+                ]
 
         return dict(_specific_flow_costs)
 
     def _map_specific_emissions(self, optimized_es):
         r"""Energy specific emissions mapped to edges."""
         # Use default dict as net energy flows container:
         _specific_emissions = defaultdict(float)
 
         # Map the respective capacity factors:
         for node in optimized_es.nodes:
             for inflow in node.inputs.keys():
                 _specific_emissions[
-                    nts.Edge(str(inflow.label), str(node.label))] = getattr(
-                        optimized_es.flows()[
-                            (inflow, node)], 'emissions', 0)
+                    nts.Edge(str(inflow.label), str(node.label))
+                ] = getattr(optimized_es.flows()[(inflow, node)], "emissions", 0)
 
         return dict(_specific_emissions)
 
 
 class AllResultier(CapacityResultier, FlowResultier, StorageResultier):
     r"""
     Transforming energy system results into a dictionary keyed by attribute.
@@ -1068,21 +1100,19 @@
 
     See also
     --------
     For functionality documentation see the respective :class:`base class
     <tessif.transform.es2mapping.base.NodeFormatier>`.
     """
 
-    def __init__(self, optimized_es, cgrp='name', drawutil='nx', **kwargs):
+    def __init__(self, optimized_es, cgrp="name", drawutil="nx", **kwargs):
 
         super().__init__(
-            optimized_es=optimized_es,
-            cgrp=cgrp,
-            drawutil=drawutil,
-            **kwargs)
+            optimized_es=optimized_es, cgrp=cgrp, drawutil=drawutil, **kwargs
+        )
 
 
 class MplLegendFormatier(base.MplLegendFormatier, CapacityResultier):
     r"""
     Generating visually enhanced matplotlib legends for nodes and edges.
 
     Parameters
@@ -1113,33 +1143,32 @@
 
     See also
     --------
     For functionality documentation see the respective :class:`base class
     <tessif.transform.es2mapping.base.MplLegendFormatier>`.
     """
 
-    def __init__(self, optimized_es, cgrp='all',
-                 markers='formatier', **kwargs):
+    def __init__(self, optimized_es, cgrp="all", markers="formatier", **kwargs):
 
         # needed transformers
 
         # mpl legend formatier is the only class needing an extra formatier
         # instead of just inheriting it. This allows bundling as done in the
         # AllFormatier with its specific color group (cgrp) and still be able
         # to map the legends for all colors
 
         # a different plausible approach would be to only map the bundled
         # color, and implement some if clauses to only map the legend
         # requested. This also implies chaining the behaviour of
         # MplLegendFormatier.node_legend
-        self._nformats = NodeFormatier(
-            optimized_es, drawutil='nx', cgrp='all')
+        self._nformats = NodeFormatier(optimized_es, drawutil="nx", cgrp="all")
 
-        super().__init__(optimized_es=optimized_es, cgrp='all',
-                         markers=markers, **kwargs)
+        super().__init__(
+            optimized_es=optimized_es, cgrp="all", markers=markers, **kwargs
+        )
 
 
 class EdgeFormatier(base.EdgeFormatier, FlowResultier):
     r"""Transforming energy system results into edge visuals.
 
     Parameters
     ----------
@@ -1180,25 +1209,22 @@
 
     See also
     --------
     For functionality documentation see the respective :class:`base class
     <tessif.transform.es2mapping.base.EdgeFormatier>`.
     """
 
-    def __init__(self, optimized_es, drawutil='nx', cls=None, **kwargs):
+    def __init__(self, optimized_es, drawutil="nx", cls=None, **kwargs):
 
         super().__init__(
-            optimized_es=optimized_es,
-            drawutil=drawutil,
-            cls=cls,
-            **kwargs)
+            optimized_es=optimized_es, drawutil=drawutil, cls=cls, **kwargs
+        )
 
 
-class AllFormatier(
-        LabelFormatier, NodeFormatier, MplLegendFormatier, EdgeFormatier):
+class AllFormatier(LabelFormatier, NodeFormatier, MplLegendFormatier, EdgeFormatier):
     r"""
     Transforming ES results into visual expression dicts keyed by attribute.
     Incorporates all the functionalities from its
     parents.
 
     Parameters
     ----------
@@ -1269,31 +1295,37 @@
     It is meant to be a "one fits all" solution for small energy systems.
     Perfectly fit for showing "proof of concepts" or debugging energy system
     components.
 
     **Potentially Unfit For Large System Models**.
     """
 
-    def __init__(self, optimized_es, cgrp='all',
-                 markers='formatier',
-                 drawutil='nx',
-                 cls=None,
-                 **kwargs):
+    def __init__(
+        self,
+        optimized_es,
+        cgrp="all",
+        markers="formatier",
+        drawutil="nx",
+        cls=None,
+        **kwargs
+    ):
 
         super().__init__(
             optimized_es=optimized_es,
-            cgrp=cgrp, markers=markers, drawutil=drawutil, **kwargs)
+            cgrp=cgrp,
+            markers=markers,
+            drawutil=drawutil,
+            **kwargs
+        )
 
         # initializing edge formatier seperately, because of differing
         # init signature causing a wierd unrespecting of drawutl
         super(EdgeFormatier, self).__init__(
-            optimized_es=optimized_es,
-            drawutil=drawutil,
-            cls=cls,
-            **kwargs)
+            optimized_es=optimized_es, drawutil=drawutil, cls=cls, **kwargs
+        )
 
 
 class ICRHybridier(OmfResultier, base.ICRHybridier):
     """
     Aggregate numerical and visual information for visualizing
     the :ref:`Integrated_Component_Results` (ICR).
 
@@ -1306,22 +1338,23 @@
     See also
     --------
     For non :ref:`model <SupportedModels>` specific attributes see
     the respective :class:`base class
     <tessif.transform.es2mapping.base.ICRHybridier>`.
     """
 
-    def __init__(self, optimized_es, colored_by='name', **kwargs):
+    def __init__(self, optimized_es, colored_by="name", **kwargs):
         base.ICRHybridier.__init__(
             self,
             optimized_es=optimized_es,
             node_formatier=NodeFormatier(optimized_es, cgrp=colored_by),
             edge_formatier=EdgeFormatier(optimized_es),
             mpl_legend_formatier=MplLegendFormatier(optimized_es),
-            **kwargs)
+            **kwargs
+        )
 
     @property
     def node_characteristic_value(self):
         r"""Map node label to characteristic value.
 
         Components of variable size have a characteristic value of ``None``.
```

### Comparing `tessif_oemof_4_4-0.1.6/src/tessif_oemof_4_4/transform.py` & `tessif_oemof_4_4-0.1.8/src/tessif_oemof_4_4/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import logging
 import numbers
 from warnings import warn
 
 import numpy as np
 import oemof.solph as solph
 import tessif.frused.namedtuples as nts
-from tessif.frused import spellings
 from tessif import components
+from tessif.frused import spellings
 
 logger = logging.getLogger(__name__)
 
 
 def _to_oemof_conversions(tessif_conversions):
     """
     Translate tessif's conversions dictionairy into oemof's.
@@ -105,16 +105,15 @@
             )
     else:
         if component.timeseries:
             if component.timeseries[target] is not None:
                 # preset nominal value in case a timeseries is used
                 # to parse specific values and existing when dealing with
                 # expandable values
-                flow_params["nominal_value"] = max(
-                    component.timeseries[target].max)
+                flow_params["nominal_value"] = max(component.timeseries[target].max)
                 nominal_value = flow_params["nominal_value"]
             else:
                 flow_params["nominal_value"] = nominal_value
         else:
             flow_params["nominal_value"] = nominal_value
 
         flow_params["min"] = 0.0
@@ -141,41 +140,37 @@
     # component specific linear flow params:
     if hasattr(component, "accumulated_amounts"):
         if target in component.accumulated_amounts:
             # parse minimum = 0 to None, to match oemof:
             if component.accumulated_amounts[target].min == 0:
                 summed_min = None
             else:
-                summed_min = component.accumulated_amounts[target].min / \
-                    nominal_value
+                summed_min = component.accumulated_amounts[target].min / nominal_value
 
             if component.accumulated_amounts[target].max == float("inf"):
                 summed_max = None
             else:
-                summed_max = component.accumulated_amounts[target].max / \
-                    nominal_value
+                summed_max = component.accumulated_amounts[target].max / nominal_value
 
             flow_params.update(
                 {
                     "summed_min": summed_min,
                     "summed_max": summed_max,
                 }
             )
 
     # expansion problem parameters:
     if component.expandable[target]:
         flow_params.pop("positive_gradient")
         flow_params.pop("negative_gradient")
         max_expansion = (
-            component.expansion_limits[target].max -
-            flow_params["nominal_value"]
+            component.expansion_limits[target].max - flow_params["nominal_value"]
         )
         min_expansion = (
-            component.expansion_limits[target].min -
-            flow_params["nominal_value"]
+            component.expansion_limits[target].min - flow_params["nominal_value"]
         )
 
         if max_expansion < 0:
             msg = (
                 "Requested maximum expansion limit of "
                 + f"'{component.expansion_limits[target].max}' of flow "
                 f"'{target}' of component '{component.uid.name}' is below "
@@ -482,16 +477,15 @@
 
         # temp dict for translating tessif's conversions to oemof's
         oemof_conversions = {}
         oemof_cffc = {}
         if chp.conversions:
             oemof_conversions = _to_oemof_conversions(chp.conversions)
         if chp.conversion_factor_full_condensation:
-            oemof_cffc = _to_oemof_conversions(
-                chp.conversion_factor_full_condensation)
+            oemof_cffc = _to_oemof_conversions(chp.conversion_factor_full_condensation)
         for bus in tessif_busses:
             for input_ in chp.inputs:
                 bus_id = ".".join([chp.uid.name, input_])
                 if bus_id in bus.outputs:
 
                     # parse conversion factor if applicable:
                     if input_ in oemof_conversions:
@@ -633,16 +627,15 @@
                         # the FIRST tuple entry
                         if str(bus.uid) == str(bus_tuple[0]):
 
                             # the resulting tuple key is constructed by taking
                             # the first input uid as first entry and the output
                             # uid (the one left in the conversion factors bus
                             # tuple) as second entry
-                            t = (bus_dict[bus.uid.name],
-                                 bus_dict[bus_tuple[1]])
+                            t = (bus_dict[bus.uid.name], bus_dict[bus_tuple[1]])
                             conversion_factors[t] = conv_factor
 
                     # parse input flow (oemof flows are keyed to objects!)
                     inputs[bus_dict[bus.uid.name]] = solph.Flow()
                     # **_parse_oemof_flow_parameters(link, input_))
 
             # to the same for outputs as for the inputs (see comments there)...
@@ -982,19 +975,17 @@
         else:
             initial_storage_level = 0
             loss_rate = 0
 
         # Initialize default "capacity" Investment (expansion problem)
         if storage.expandable["capacity"]:
 
-            max_expansion = storage.expansion_limits["capacity"].max - \
-                storage.capacity
+            max_expansion = storage.expansion_limits["capacity"].max - storage.capacity
 
-            min_expansion = storage.expansion_limits["capacity"].min - \
-                storage.capacity
+            min_expansion = storage.expansion_limits["capacity"].min - storage.capacity
 
             if max_expansion < 0:
                 msg = (
                     "Requested maximum expansion limit of "
                     + f"'{storage.expansion_limits['capacity'].max}' of storage "
                     f"'{storage.uid.name}' is below current installed "
                     f"capacity of '{storage.capacity}' Falling back on "
@@ -1386,14 +1377,14 @@
         storages=tessif_es.storages,
         tessif_busses=tessif_es.busses,
         oemof_busses=oemof_busses,
     ):
         energy_system_components.append(storage)
 
     energy_system = solph.EnergySystem(timeindex=tessif_es.timeframe)
-    energy_system.add(*energy_system_components, **kwargs)
+    energy_system.add(*energy_system_components)
 
     # add global constraints (no parsing here, since oemof allocates global
     # constraints to the underlying solver model exclusively)
     energy_system.global_constraints = tessif_es.global_constraints
 
     return energy_system
```

### Comparing `tessif_oemof_4_4-0.1.6/setup.py` & `tessif_oemof_4_4-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 packages = \
 ['tessif_oemof_4_4']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['oemof-solph==0.4.4', 'tessif>=0.0.24']
+['oemof-solph==0.4.4', 'tessif>=0.0.27']
 
 setup_kwargs = {
     'name': 'tessif-oemof-4-4',
-    'version': '0.1.6',
+    'version': '0.1.8',
     'description': 'Tessif-Plugin for providing oemof version 4.4. support.',
     'long_description': 'tessif-oemof-4-4\n====================================================================================================\n\n|PyPI| |Python Version| |License| |Status|\n\n|Stable Release| |Develop Release|\n\n|Read the Docs| |Tests| |Safety| |Pylinting| |Flake8 Linting| |Pre-Commit|\n\n|Codecov| |Codacy| |Codeclimate| |Scrutinizer|\n\n|pre-commit| |Black| |Pylint| |Flake8|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/tessif-oemof-4-4.svg\n   :target: https://pypi.org/project/tessif-oemof-4-4/\n   :alt: PyPI\n\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/tessif-oemof-4-4\n   :target: https://pypi.org/project/tessif-oemof-4-4\n   :alt: Python Version\n\n.. |License| image:: https://img.shields.io/pypi/l/tessif-oemof-4-4\n   :target: https://opensource.org/licenses/MIT\n   :alt: License\n\n.. |Status| image:: https://badgen.net/badge/status/alpha/d8624d\n   :target: https://pypi.org/project/tessif-oemof-4-4/\n   :alt: Status\n\n.. |Stable Release| image:: https://github.com/tZ3ma/tessif-oemof-4-4/workflows/Stable-PyPI-Release/badge.svg\n   :target: https://github.com/tZ3ma/tessif-oemof-4-4/actions?workflow=Stable-PyPI-Release\n   :alt: Stable PyPI Release Workflow Status\n\n.. |Develop Release| image:: https://github.com/tZ3ma/tessif-oemof-4-4/workflows/Develop-TestPyPI-Release/badge.svg\n   :target: https://github.com/tZ3ma/tessif-oemof-4-4/actions?workflow=Develop-TestPyPI-Release\n   :alt: Develop TestPyPI Release Workflow Status\n\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/tessif-oemof-4-4/latest.svg?label=Read%20the%20Docs\n   :target: https://tessif-oemof-4-4.readthedocs.io/\n   :alt: Read the documentation at https://tessif-oemof-4-4.readthedocs.io/\n\n.. |Tests| image:: https://github.com/tZ3ma/tessif-oemof-4-4/workflows/Tests-and-Coverage/badge.svg\n   :target: https://github.com/tZ3ma/tessif-oemof-4-4/actions?workflow=Tests-and-Coverage\n   :alt: Tests Workflow Status\n\n.. |Safety| image:: https://github.com/tZ3ma/tessif-oemof-4-4/workflows/Safety/badge.svg\n   :target: https://github.com/tZ3ma/tessif-oemof-4-4/actions?workflow=Safety\n   :alt: Safety Workflow Status\n\n.. |Pylinting| image:: https://github.com/tZ3ma/tessif-oemof-4-4/workflows/Pylinting/badge.svg\n   :target: https://github.com/tZ3ma/tessif-oemof-4-4/actions?workflow=Pylinting\n   :alt: Pylint Workflow Status\n\n.. |Flake8 Linting| image:: https://github.com/tZ3ma/tessif-oemof-4-4/workflows/Flake8-Linting/badge.svg\n   :target: https://github.com/tZ3ma/tessif-oemof-4-4/actions?workflow=Flake8-Linting\n   :alt: Flake8-Linting Workflow Status\n\n.. |Pre-Commit| image:: https://github.com/tZ3ma/tessif-oemof-4-4/workflows/Pre-Commit/badge.svg\n   :target: https://github.com/tZ3ma/tessif-oemof-4-4/actions?workflow=Pre-Commit\n   :alt: Pre-Commit Workflow Status\n\n.. |Codecov| image:: https://codecov.io/gh/tZ3ma/tessif-oemof-4-4/branch/main/graph/badge.svg\n   :target: https://codecov.io/gh/tZ3ma/tessif-oemof-4-4\n   :alt: Codecov\n\n.. |Codacy| image:: https://app.codacy.com/project/badge/Grade/b278433bb9224147a2e6231d783b62e4\n   :target: https://app.codacy.com/gh/tZ3ma/tessif-oemof-4-4/dashboard\n   :alt: Codacy Code Quality Status\n\n.. |Codeclimate| image:: https://api.codeclimate.com/v1/badges/ff119252f0bb7f40aecb/maintainability\n   :target: https://codeclimate.com/github/tZ3ma/tessif-oemof-4-4/maintainability\n   :alt: Maintainability\n\n.. |Scrutinizer| image:: https://scrutinizer-ci.com/g/tZ3ma/tessif-oemof-4-4/badges/quality-score.png?b=main\n   :target: https://scrutinizer-ci.com/g/tZ3ma/tessif-oemof-4-4/\n   :alt: Scrutinizer Code Quality\n\n.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white\n   :target: https://github.com/pre-commit/pre-commit\n   :alt: pre-commit\n\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Black\n\n.. |Pylint| image:: https://img.shields.io/badge/linting-pylint-yellowgreen\n   :target: https://github.com/PyCQA/pylint\n   :alt: Package uses pylint\n\n.. |Flake8| image:: https://img.shields.io/badge/linting-flake8-yellogreen\n   :target: https://github.com/pycqa/flake8\n   :alt: Package uses flake8\n\n\nTessif-Plugin for including the software-tool oemof version 4.4.\n\nInstallation\n------------\n\nPlease see the `Installation Guide`_ (`Github Repo Link`_) for details.\n\n\nUsage\n-----\n\nPlease see the `Worklow Reference <Workflow-Guide_>`_ (`Github Repo Link`_) for details.\n\n\nContributing\n------------\n\nContributions are very welcome.\nTo learn more, see the `Contributor Guide`_ (`Github Repo Link`_).\n\n\nLicense\n-------\n\nDistributed under the terms of the `MIT license`_ (`Github Repo Link`_),\n*tessif-oemof-4-4* is free and open source software.\n\n\nIssues\n------\n\nIf you encounter any problems,\nplease `file an issue`_ along with a detailed description.\n\nCredits\n-------\n\nThis project was created using the `Mathias Ammon <tZ3ma>`_ tweaked version of the\nHypermodern-Python_ project foundation proposed by `Claudio Jolowicz <cj>`_.\n\n.. _Hypermodern-Python: https://cjolowicz.github.io/posts/hypermodern-python-01-setup/\n.. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n.. _cj: https://github.com/cjolowicz\n\n.. _MIT license: https://opensource.org/licenses/MIT\n.. _PyPI: https://pypi.org/\n\n.. _file an issue: https://github.com/tZ3ma/tessif-oemof-4-4/issues\n.. _pip: https://pip.pypa.io/\n\n.. _tZ3ma: https://github.com/tZ3ma\n.. working on github-only\n.. _Contributor Guide: CONTRIBUTING.rst\n.. _Installation Guide: docs/source/getting_started/installation.rst\n.. _Workflow-Guide: docs/source/developer_guide/workflows.rst\n\n.. _Github Repo Link: https://github.com/tZ3ma/tessif-oemof-4-4\n',
     'author': 'Mathias Ammon',
     'author_email': 'tz3ma.coding@use.startmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tZ3ma/tessif_oemof_4_4',
```

### Comparing `tessif_oemof_4_4-0.1.6/PKG-INFO` & `tessif_oemof_4_4-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: tessif-oemof-4-4
-Version: 0.1.6
+Version: 0.1.8
 Summary: Tessif-Plugin for providing oemof version 4.4. support.
 Home-page: https://github.com/tZ3ma/tessif_oemof_4_4
 License: MIT
 Keywords: Tessif,Tessif-Oemof,tessif-oemof,ESSMOS,optimization,energy supply system modelling
 Author: Mathias Ammon
 Author-email: tz3ma.coding@use.startmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: oemof-solph (==0.4.4)
-Requires-Dist: tessif (>=0.0.24)
+Requires-Dist: tessif (>=0.0.27)
 Project-URL: Repository, https://github.com/tZ3ma/tessif_oemof_4_4
 Description-Content-Type: text/x-rst
 
 tessif-oemof-4-4
 ====================================================================================================
 
 |PyPI| |Python Version| |License| |Status|
```


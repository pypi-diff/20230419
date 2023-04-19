# Comparing `tmp/optgraphstate-0.1.1-py3-none-any.whl.zip` & `tmp/optgraphstate-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 23399 bytes, number of entries: 9
--rw-r--r--  2.0 unx    67049 b- defN 23-Apr-18 10:31 optgraphstate/__init__.py
+Zip file size: 23789 bytes, number of entries: 9
+-rw-r--r--  2.0 unx    68529 b- defN 23-Apr-19 10:55 optgraphstate/__init__.py
 -rw-r--r--  2.0 unx    14819 b- defN 23-Apr-18 10:28 optgraphstate/graph_tools.py
 -rw-r--r--  2.0 unx      686 b- defN 23-Apr-06 04:55 optgraphstate/utils.py
--rw-r--r--  2.0 unx     8936 b- defN 23-Apr-17 12:41 optgraphstate/visualization.py
--rw-r--r--  2.0 unx     1070 b- defN 23-Apr-18 10:35 optgraphstate-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1881 b- defN 23-Apr-18 10:35 optgraphstate-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 10:35 optgraphstate-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-18 10:35 optgraphstate-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      750 b- defN 23-Apr-18 10:35 optgraphstate-0.1.1.dist-info/RECORD
-9 files, 95297 bytes uncompressed, 22105 bytes compressed:  76.8%
+-rw-r--r--  2.0 unx     9075 b- defN 23-Apr-19 10:05 optgraphstate/visualization.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-Apr-19 11:31 optgraphstate-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1900 b- defN 23-Apr-19 11:31 optgraphstate-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 11:31 optgraphstate-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-19 11:31 optgraphstate-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      750 b- defN 23-Apr-19 11:31 optgraphstate-0.1.2.dist-info/RECORD
+9 files, 96935 bytes uncompressed, 22495 bytes compressed:  76.8%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: optgraphstate/utils.py
 Comment: 
 
 Filename: optgraphstate/visualization.py
 Comment: 
 
-Filename: optgraphstate-0.1.1.dist-info/LICENSE
+Filename: optgraphstate-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: optgraphstate-0.1.1.dist-info/METADATA
+Filename: optgraphstate-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: optgraphstate-0.1.1.dist-info/WHEEL
+Filename: optgraphstate-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: optgraphstate-0.1.1.dist-info/top_level.txt
+Filename: optgraphstate-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: optgraphstate-0.1.1.dist-info/RECORD
+Filename: optgraphstate-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## optgraphstate/__init__.py

```diff
@@ -1,19 +1,19 @@
 """
-**Version 0.1.1**
+**Version 0.1.2**
 
 **OptGraphState** is a python package that implements the graph-theoretical
 strategy to optimize the fusion-based generation of any graph state.
 The package has the following features:
 
 - Finding a resource-efficient method of generating a given graph state through
 type-II fusions from multiple basic resource states, which are three-qubit
 linear graph states.
 - Computing the corresponding resource overhead, which is quantified by the
-average number of required basic resource states.
+average number of required basic resource states or fusion attempts.
 - Visualizing the original graph (of the graph state you want to generate),
 unraveled graphs, and fusion networks. An unraveled graph is a simplified graph
 where the corresponding graph state is equivalent to the desired graph state up
 to fusions and single-qubit Clifford operations. A fusion network is a graph
 that instructs the fusions between basic resource states required to generate
 the desired graph state.
 - Various predefined sample graphs for input.
@@ -731,29 +731,33 @@
         self.fusion_network = network
 
         if plot:
             print("Final:")
             self.plot_fusion_network()
             plt.show()
 
-    def _contract_edge(self, fusion_network, ename_to_merge):
+    def _contract_edge(self,
+                       fusion_network,
+                       ename_to_merge):
         ename_to_merge = str(ename_to_merge)
 
         e_to_merge = fusion_network.es.find(name=ename_to_merge)
-        v_merged, v_removed = e_to_merge.source_vertex, e_to_merge.target_vertex
+        v_merged, v_removed \
+            = e_to_merge.source_vertex, e_to_merge.target_vertex
         enames_updated_weight = []
 
         if v_merged.degree() < v_removed.degree():
             v_merged, v_removed = v_removed, v_merged
 
         vname_merged = v_merged['name']
         vname_removed = v_removed['name']
 
         v_merged['weight'] = e_to_merge['weight']
-        v_merged['step'] = max(v_merged['step'], v_removed['step']) + 1
+        v_merged['weight_f'] = e_to_merge['weight_f']
+        v_merged['order'] = max(v_merged['order'], v_removed['order']) + 1
 
         assert vname_merged != vname_removed
 
         eids_to_delete = list(set(fusion_network.incident(v_removed)))
         v_removed['on'] = False
 
         for eid_connected in eids_to_delete:
@@ -764,128 +768,139 @@
                 vs_ngh = e_connected.source_vertex, e_connected.target_vertex
                 new_edge = [v_merged if v_ngh['name'] == vname_removed
                             else v_ngh for v_ngh in vs_ngh]
                 if new_edge[0] == new_edge[1]:  # If a loop is formed
                     v_vrt = fusion_network.add_vertex(
                         name=f'vrt_{fusion_network.vcount()}',
                         weight=0,
-                        step=0
+                        weight_f=0,
+                        order=0
                     )
                     new_edge = [v_merged, v_vrt]
 
                 fusion_network.add_edge(*new_edge,
                                         name=ename_connected,
-                                        weight=None, )
+                                        weight=None,
+                                        weight_f=None)
 
         fusion_network.delete_edges(eids_to_delete)
 
         p_succ = fusion_network['p_succ']
         for eid_connected in list(set(fusion_network.incident(v_merged))):
             e_connected = fusion_network.es[eid_connected]
             v_ngh1, v_ngh2 = e_connected.source_vertex, e_connected.target_vertex
 
             assert v_ngh1 != v_ngh2
-            new_weight = (v_ngh1['weight'] + v_ngh2['weight']) / p_succ
-            e_connected['weight'] = new_weight
+            e_connected['weight'] \
+                = (v_ngh1['weight'] + v_ngh2['weight']) / p_succ
+            e_connected['weight_f'] \
+                = (v_ngh1['weight_f'] + v_ngh2['weight_f'] + 1) / p_succ
 
-        self.fusion_network.es.find(name=ename_to_merge)['step'] = v_merged[
-            'step']
+        self.fusion_network.es.find(name=ename_to_merge)['order'] \
+            = v_merged['order']
 
         return enames_updated_weight
 
     def calculate_overhead(self,
                            p_succ=0.5,
                            strategy='weight_and_matching',
-                           fusion_order=None,
-                           get_fusion_order=False, ):
+                           optimize_num_fusions=False,
+                           fusion_order=None):
         """
         Calculate the resource overhead from the fusion network.
 
         `GraphState.build_fusion_network()` must be executed beforehand.
 
         The resulting data is saved in `GraphState.data`.
 
         Parameters
         ----------
         p_succ : float (default: 0.5)
             Success probability of a fusion.
 
         strategy: str, one of ['weight', 'matching', 'weight_and_matching', 'random'] (default: 'weight_and_matching')
-            Strategy for determining the edge to contract in each step.
+            Strategy for determining the edge to contract.
 
             - `'weight'`: Contract a random one among the edges with the
             smallest weight.
             - `'matching'`: Contract an edge in a maximum matching.
             - `'weight_and_matching'`: Contract an edge in a maximum matching
             of the subgraph of the intermediate fusion network induced by
             the edges with the smallest weight.
             - `'random'`: Contract a random edge.
 
+        optimize_num_fusions : bool
+            If `True`, the average number of required fusion attempts are used
+            to quantify resource overheads instead of the average number of
+            required basic resource states.
+
         fusion_order : None or list of {int or str} (default: None)
             Fusion order given explicitly as vertex names.
 
             If it is not `None`, parameter `strategy` is ignored.
 
-        get_fusion_order : bool (default: False)
-            Whether to include the determined fusion order in the returned
-            data.
-
         Returns
         -------
         data : dict
             Outcomes of the calculation, which is a shallow copy of
             `GraphState.data`.<br>
             The calculated overhead and number of steps can be obtained from
-            `data['overhead']` and `data['step']`, respectively.
+            `data['overhead']` and `data['num_steps']`, respectively.
         """
 
         if self.fusion_network is None:
             raise ValueError("No fusion network created")
 
         # Trivial cases
         node_num = self.fusion_network.vcount()
         if node_num == 0:
             self.data['overhead'] = 0
-            self.data['step'] = 0
+            self.data['num_fusions'] = 0
+            self.data['num_steps'] = 0
             return self.data
         elif node_num == 1:
             self.data['overhead'] = 1
-            self.data['step'] = 0
+            self.data['num_fusions'] = 0
+            self.data['num_steps'] = 0
             return self.data
 
         if fusion_order is None:
             fusion_order = []
             is_fusion_order_given = False
         else:
             is_fusion_order_given = True
 
-        self.fusion_network.es['step'] = None
+        self.fusion_network.es['order'] = None
 
         # Initialize intermediate fusion network
         network = self.fusion_network.copy()
         network['p_succ'] = p_succ
         network.vs['weight'] = 1
-        network.vs['step'] = 0
+        network.vs['weight_f'] = 0
+        network.vs['order'] = 0
         network.vs['on'] = True
         network.es['weight'] = 2 / p_succ
-        del network.es['step']
+        network.es['weight_f'] = 1 / p_succ
+        del network.es['order']
 
         turn = 0
 
+        weight_key = 'weight_f' if optimize_num_fusions else 'weight'
+
         # Iterate until no edges remain in the fusion network
         while True:
             if not network.ecount():
                 break
 
             if is_fusion_order_given:
                 enames_curr_step = [str(fusion_order[turn])]
                 is_parellel = True
 
             elif strategy == 'weight':
-                min_weight = min(network.es['weight'])
+                min_weight = min(network.es[weight_key])
                 eids_min_weight = network.es.select(weight=min_weight)
                 enames_curr_step = eids_min_weight['name']
                 is_parellel = len(enames_curr_step) == 1
 
             # elif strategy == 'betweenness':
             #     eb = np.array(network.edge_betweenness())
             #     min_eb = np.min(eb)
@@ -904,16 +919,19 @@
             #     min_eb = np.min(ebs_min_ovh)
             #     enames_curr_step = [es_min_ovh[i]['name'] for i in
             #     np.nonzero(ebs_min_ovh == min_eb)[0]]
             #     is_parellel = len(enames_curr_step) == 1
 
             elif 'matching' in strategy:
                 if strategy == 'weight_and_matching':
-                    min_weight = min(network.es['weight'])
-                    es_min_weight = network.es.select(weight=min_weight)
+                    min_weight = min(network.es[weight_key])
+                    if optimize_num_fusions:
+                        es_min_weight = network.es.select(weight_f=min_weight)
+                    else:
+                        es_min_weight = network.es.select(weight=min_weight)
                     subnetwork = network.subgraph_edges(es_min_weight)
                 else:
                     subnetwork = network
 
                 subnetwork_nx = subnetwork.to_networkx()
                 if isinstance(subnetwork_nx, nx.MultiGraph):
                     subnetwork_nx = nx.Graph(subnetwork_nx)
@@ -928,17 +946,17 @@
                 is_parellel = True
 
             else:
                 raise ValueError
 
             recalculated_enames = []
 
-            if get_fusion_order and not is_fusion_order_given:
-                fusion_order_curr_step = set()
-                fusion_order.append(fusion_order_curr_step)
+            # if get_fusion_order and not is_fusion_order_given:
+            #     fusion_order_curr_step = set()
+            #     fusion_order.append(fusion_order_curr_step)
 
             while True:
                 if not is_parellel:
                     for rec_ename in recalculated_enames:
                         try:
                             enames_curr_step.remove(rec_ename)
                         except ValueError:
@@ -951,37 +969,44 @@
 
                 if is_parellel:
                     ename_to_merge = enames_curr_step.pop()
                 else:
                     ename_to_merge = np.random.choice(enames_curr_step)
                     enames_curr_step.remove(ename_to_merge)
 
-                if get_fusion_order:
-                    e_to_merge = self.fusion_network.es.find(name=ename_to_merge)
-                    v1, v2 = e_to_merge.source_vertex, e_to_merge.target_vertex
-                    fusion_order_curr_step.add((v1['name'], v2['name'],
-                                                ename_to_merge))
-
-                enames_updated_weight = self._contract_edge(network,
-                                                            ename_to_merge)
+                # if get_fusion_order:
+                #     e_to_merge = self.fusion_network.es.find(name=ename_to_merge)
+                #     v1, v2 = e_to_merge.source_vertex, e_to_merge.target_vertex
+                #     fusion_order_curr_step.add((v1['name'], v2['name'],
+                #                                 ename_to_merge))
+
+                enames_updated_weight \
+                    = self._contract_edge(network,
+                                          ename_to_merge)
 
                 recalculated_enames.extend(enames_updated_weight)
 
         v_final = network.vs.select(on=True)
         overhead = sum(v_final['weight'])
-        step = max(v_final['step'])
+        num_fusions = sum(v_final['weight_f'])
+        num_steps = max(v_final['order'])
 
         results = {
             'overhead': overhead,
-            'step': step,
+            'num_fusions': num_fusions,
+            'num_steps': num_steps,
             'fusion_order_strategy': strategy,
-            'p_succ': p_succ}
+            'p_succ': p_succ,
+        }
 
-        if get_fusion_order:
-            results['fusion_order'] = fusion_order
+        if optimize_num_fusions:
+            results['optimize_num_fusions'] = True
+
+        # if get_fusion_order:
+        #     results['fusion_order'] = fusion_order
 
         self.data.update(results)
 
         return self.data.copy()
 
     def simulate(self,
                  n_iter,
@@ -990,14 +1015,15 @@
                  n_procs=None,
                  get_all_data=False,
                  get_all_graphs=False,
                  get_all_fusion_networks=False,
                  unravel=True,
                  unravel_bcs_first='random',
                  fusion_order_strategy='weight_and_matching',
+                 optimize_num_fusions=False,
                  seed='keep',
                  verbose=True,
                  pbar=False,
                  **kwargs):
         """
         Execute the strategy for a fixed number of iterations and obtain the
         best one only (by default).
@@ -1053,14 +1079,19 @@
             smallest weight.
             - `'matching'`: Contract an edge in a maximum matching.
             - `'weight_and_matching'`: Contract an edge in a maximum matching
             of the subgraph of the intermediate fusion network induced by
             the edges with the smallest weight.
             - `'random'`: Contract a random edge.
 
+        optimize_num_fusions : bool
+            If `True`, use the averagte number of fusion attempts to quantify
+            resource overheads instead of the average number of basic resource
+            states.
+
         seed : 'keep' or None or int (default: 'keep')
             Random seed.
 
             - `'keep'`: The seed is not initialized.
             - `None`: The current time is used as the random seed.
             - `int`: The given number is used as the random seed.
 
@@ -1087,14 +1118,16 @@
             Result of the iterations.
 
             By default, only the information of the best sample is returned.
         """
 
         t0 = time.time()
 
+        overhead_key = 'num_fusions' if optimize_num_fusions else 'overhead'
+
         if seed != 'keep':
             np.random.seed(seed)
 
         if mp:
             if n_procs is None:
                 n_procs = os.cpu_count()
             mp = mp and n_iter >= n_procs
@@ -1106,15 +1139,16 @@
 
             if n_iter == 1 and seed is not None and seed != 'keep':
                 seeds_samples = [seed]
             else:
                 seeds_samples = np.random.randint(0, _max_seed(), size=n_iter)
 
             overheads = [] if get_all_data else None
-            steps = [] if get_all_data else None
+            nums_fusions = [] if get_all_data else None
+            nums_steps = [] if get_all_data else None
             seeds = [] if get_all_data else None
             unravalled_graphs = [] if get_all_graphs else None
             fusion_networks = [] if get_all_fusion_networks else None
 
             best_sample = None
             lowest_overhead = None
             for i_sample in range(n_iter):
@@ -1134,57 +1168,62 @@
                     self.build_fusion_network(use_unraveled_graph=unravel)
                 except:
                     print('Error occurs during building fusion network')
                     print('seed =', seed_sample)
                     raise ValueError
 
                 try:
-                    data_now = self.calculate_overhead(p_succ=p_succ,
-                                                       strategy=fusion_order_strategy,
-                                                       **kwargs)
+                    data_now = self.calculate_overhead(
+                        p_succ=p_succ,
+                        strategy=fusion_order_strategy,
+                        optimize_num_fusions=optimize_num_fusions,
+                        **kwargs)
                 except:
                     print('Error occurs during calculating overhead')
                     print('seed =', seed_sample)
                     raise ValueError
 
-                overhead_now = data_now['overhead']
-                step_now = data_now['step']
+                overhead_now = data_now[overhead_key]
+                num_steps_now = data_now['num_steps']
                 self.data['seed'] = seed_sample
 
                 if lowest_overhead is None or overhead_now < lowest_overhead:
                     best_sample = i_sample
                     lowest_overhead = overhead_now
                     best_ogs = self.copy()
 
                 if get_all_data:
-                    overheads.append(overhead_now)
-                    steps.append(step_now)
+                    overheads.append(data_now['overhead'])
+                    nums_fusions.append(data_now['num_fusions'])
+                    nums_steps.append(num_steps_now)
                     seeds.append(seed_sample)
 
                 if get_all_graphs:
                     unravalled_graphs.append(self.unraveled_graph)
 
                 if get_all_fusion_networks:
                     fusion_networks.append(self.fusion_network)
 
             res = {
                 'best_overhead': best_ogs.data['overhead'],
-                'best_step': best_ogs.data['step'],
+                'best_num_fusions': best_ogs.data['num_fusions'],
+                'best_num_steps': best_ogs.data['num_steps'],
                 'best_seed': best_ogs.data['seed'],
                 'n_iter': n_iter}
 
             if unravel:
                 res['unravel_bcs_first'] = best_ogs.data['unravel_bcs_first']
 
             if get_all_data or get_all_graphs or get_all_fusion_networks:
                 res['best_sample'] = best_sample
 
                 if get_all_data:
                     res['overheads'] = overheads
-                    res['steps'] = steps
+                    res['nums_fusions'] = nums_fusions
+                    res['nums_steps'] = nums_steps
                     res['seeds'] = seeds
 
                 if get_all_graphs:
                     res['unraveled_graphs'] = unravalled_graphs
 
                 if get_all_fusion_networks:
                     res['fusion_networks'] = fusion_networks
@@ -1195,56 +1234,59 @@
 
             if verbose:
                 print(f"Multiprocessing ON: n_procs = {n_procs}")
                 print(f"Calculating for n_iter = {n_iter}... ", end='')
 
             additional_keys = []
             if get_all_data:
-                additional_keys.extend(['overheads', 'steps', 'seeds'])
+                additional_keys.extend(['overheads', 'nums_fusions',
+                                        'nums_steps', 'seeds'])
             if get_all_graphs:
                 additional_keys.append('unraveled_graphs')
             if get_all_fusion_networks:
                 additional_keys.append('fusion_networks')
 
             left = n_iter % n_procs
             ns_samples = [n_iter // n_procs] * n_procs
             for i in range(left):
                 ns_samples[i] += 1
 
             seeds = np.random.randint(0, _max_seed(), size=n_procs)
 
-            res_procs = parmap.starmap(_simulate_single,
-                                       list(zip(ns_samples, seeds)),
-                                       self.graph,
-                                       p_succ=p_succ,
-                                       get_all_data=get_all_data,
-                                       get_all_graphs=get_all_graphs,
-                                       get_all_fusion_networks=get_all_fusion_networks,
-                                       unravel=unravel,
-                                       unravel_bcs_first=unravel_bcs_first,
-                                       fusion_order_strategy=fusion_order_strategy,
-                                       pm_pbar=pbar,
-                                       **kwargs)
-            best_overheads = [res_each['best_overhead'] for res_each in
-                              res_procs]
-            best_proc = np.argmin(best_overheads)
+            res_procs = parmap.starmap(
+                _simulate_single,
+                list(zip(ns_samples, seeds)),
+                self.graph,
+                p_succ=p_succ,
+                get_all_data=get_all_data,
+                get_all_graphs=get_all_graphs,
+                get_all_fusion_networks=get_all_fusion_networks,
+                unravel=unravel,
+                unravel_bcs_first=unravel_bcs_first,
+                fusion_order_strategy=fusion_order_strategy,
+                optimize_num_fusions=optimize_num_fusions,
+                pm_pbar=pbar,
+                **kwargs)
+            best_proc = np.argmin(
+                [res_each[f'best_{overhead_key}'] for res_each in res_procs]
+            )
             res = res_procs[best_proc]
             res['n_iter'] = n_iter
             best_ogs = res['best_ogs']
             del res['best_ogs']
 
             if additional_keys:
                 res['best_sample'] += sum(ns_samples[:best_proc])
 
             for key in additional_keys:
                 vals = [res_each[key] for res_each in res_procs]
                 res[key] = list(itertools.chain(*vals))
 
         if verbose:
-            print(f"Done. Best: {res['best_overhead']:.2f} "
+            print(f"Done. Best: {res[f'best_{overhead_key}']:.2f} "
                   f"({time.time() - t0:.2f} s)")
 
         self.unraveled_graph = best_ogs.unraveled_graph
         self.fusion_network = best_ogs.fusion_network
         self.data = best_ogs.data
 
         return res
@@ -1257,14 +1299,15 @@
                           n_procs=None,
                           get_all_data=False,
                           get_all_graphs=False,
                           get_all_fusion_networks=False,
                           unravel=True,
                           unravel_bcs_first='random',
                           fusion_order_strategy='weight_and_matching',
+                          optimize_num_fusions=False,
                           seed='keep',
                           verbose=True,
                           pbar=False,
                           **kwargs):
         """
         Run the adaptive iteration method for the strategy and obtain the
         best one only (by default).
@@ -1301,104 +1344,94 @@
             n_procs = os.cpu_count()
 
         if seed != 'keep':
             np.random.seed(seed)
 
         additional_keys = []
         if get_all_data:
-            additional_keys.extend(['overheads', 'steps'])
+            additional_keys.extend(['overheads', 'nums_fusions', 'nums_steps'])
         if get_all_graphs:
             additional_keys.append('unraveled_graphs')
         if get_all_fusion_networks:
             additional_keys.append('fusion_networks')
 
         if verbose:
             if mp:
                 print(f"Multiprocessing (n_procs = {n_procs})")
             else:
                 print("No multiprocessing")
 
+        best_overhead_key \
+            = 'best_num_fusions' if optimize_num_fusions else 'best_overhead'
+
         n_iter_history = []
         n_iter_now = init_n_iter
         res = None
+
         while True:
             if verbose:
                 print(f"Calculating for n_iter = {n_iter_now}... ", end='')
             t0 = time.time()
 
             n_iter_history.append(n_iter_now)
-            res_now = self.simulate(n_iter=n_iter_now,
-                                    p_succ=p_succ,
-                                    mp=mp,
-                                    n_procs=n_procs,
-                                    get_all_data=get_all_data,
-                                    get_all_graphs=get_all_graphs,
-                                    get_all_fusion_networks=get_all_fusion_networks,
-                                    unravel=unravel,
-                                    unravel_bcs_first=unravel_bcs_first,
-                                    fusion_order_strategy=fusion_order_strategy,
-                                    verbose=False,
-                                    pbar=pbar,
-                                    **kwargs)
+            res_now = self.simulate(
+                n_iter=n_iter_now,
+                p_succ=p_succ,
+                mp=mp,
+                n_procs=n_procs,
+                get_all_data=get_all_data,
+                get_all_graphs=get_all_graphs,
+                get_all_fusion_networks=get_all_fusion_networks,
+                unravel=unravel,
+                unravel_bcs_first=unravel_bcs_first,
+                fusion_order_strategy=fusion_order_strategy,
+                optimize_num_fusions=optimize_num_fusions,
+                verbose=False,
+                pbar=pbar,
+                **kwargs
+            )
 
             if res is None:
                 res = res_now
                 best_ogs = self.copy()
                 n_iter_now *= mul
 
             else:
                 for key in additional_keys:
                     res[key].extend(res_now[key])
 
-                if res_now['best_overhead'] < res['best_overhead']:
+                if res_now[best_overhead_key] < res[best_overhead_key]:
                     for key in additional_keys:
                         res_now[key] = res[key]
                     res = res_now
                     best_ogs = self.copy()
 
                     n_iter_now *= mul
 
                 else:
                     if verbose:
-                        print(f"Done. Best: {res['best_overhead']:.2f} ("
+                        print(f"Done. Best: {res[best_overhead_key]:.2f} ("
                               f"{time.time() - t0:.2f} s)")
                     break
 
             if verbose:
-                print(f"Done. Best: {res['best_overhead']:.2f} "
+                print(f"Done. Best: {res[best_overhead_key]:.2f} "
                       f"({time.time() - t0:.2f} s)")
 
         res['n_iter'] = sum(n_iter_history)
 
         if additional_keys:
             res['best_sample'] += res['best_sample']
 
         self.unraveled_graph = best_ogs.unraveled_graph
         self.fusion_network = best_ogs.fusion_network
         self.data = best_ogs.data
 
         return res
 
-    def _get_graph(self, graph):
-        if isinstance(graph, ig.Graph):
-            return graph
-
-        if graph == 'graph':
-            return self.graph
-        elif graph in ['unraveled', 'unraveled_graph']:
-            if self.unraveled_graph is None:
-                raise ValueError('No unraveled graph created.')
-            return self.unraveled_graph
-        elif graph in ['network', 'fusion_network']:
-            if self.fusion_network is None:
-                raise ValueError('No fusion network created')
-            return self.fusion_network
-        else:
-            raise ValueError('Wrong input.')
-
     def get_instructions(self):
         """
         Get the instruction to generate the desired graph state from multiple
         three-qubit linear graph states.
 
         One of `GraphState.calculate_overhead()`, `GraphState.simulate()`, and
         `GraphState.simulate_adaptive()` must be executed beforehand.
@@ -1435,19 +1468,19 @@
             `'R'` or `'L'` that indicates whether the qubit is a root or leaf
             qubit, and `cl` is the Clifford gate applied to the qubit.
         """
         network = self.fusion_network
 
         # Fusions
         fusions = {}
-        steps = network.es['step']
-        max_step = max(steps)
-        for step in range(1, max_step + 1):
-            inst_same_step = []
-            links = network.es.select(step=step)
+        orders = network.es['order']
+        num_steps = max(orders)
+        for order in range(1, num_steps + 1):
+            inst_same_order = []
+            links = network.es.select(order=order)
             for link in links:
                 nname1 = link.source_vertex['name']
                 nname2 = link.target_vertex['name']
                 kind = link['kind']
                 if kind == 'RR':
                     qubit1 = qubit2 = 'R'
                 elif kind == 'LL':
@@ -1462,18 +1495,18 @@
                 except KeyError:
                     cl1 = None
                 try:
                     cl2 = cliffords[nname2]
                 except KeyError:
                     cl2 = None
 
-                inst_same_step.append(((nname1, qubit1, cl1),
-                                       (nname2, qubit2, cl2)))
+                inst_same_order.append(((nname1, qubit1, cl1),
+                                        (nname2, qubit2, cl2)))
 
-            fusions[step] = inst_same_step
+            fusions[order] = inst_same_order
 
         # Final remaining qubits & Clifford gates on them
         qubit_correspondence = {}
         remaining_leaves = {}
         for vname in self.graph.vs['name']:
             v_unrv: ig.Vertex = self.unraveled_graph.vs.find(name=vname)
             cl = v_unrv['clifford']
@@ -1612,16 +1645,16 @@
 
         figsize : 2-tuple of float (default: (5, 5))
             Size of the figure in inches.
 
         save : None or str (default: None)
             Path to save the figure.
 
-        show_vertex_name : bool (default: True)
-            Whether to show vertex names.
+        show_vertex_names : bool (default: True)
+            If `True`, vertex names are shown.
 
         vertex_color_normal : str (default: 'white')
             Color of vertices without Clifford gates.
 
         vertex_color_clifford : str (default: 'orange')
             Color of vertices with Clifford gates.
 
@@ -1661,28 +1694,26 @@
 
         return fig, ax
 
     def plot_fusion_network(self, **kwargs):
         """
         Plot the fusion network.
 
-        Links have different styles depending on their types:
+        Links have different styles and colors depending on their types:
 
-        - 'LL': Solid line
-        - 'RR': Dotted line
-        - 'RL': Arrow from leaf to root.
+        - 'LL': Black solid line.
+        - 'RR': Red dashed line.
+        - 'RL': Blue arrow from leaf to root.
 
-        The number placed on each link indicates the step of the fusion. It is
+        The number placed on each link indicates the order of the fusion. It is
         presented only when the resource overhead has been computed beforehand.
 
-        A red link indicates that particular Clifford gates should be
-        applied to the qubits involved in the fusion before it is performed.
-
-        These Clifford gates can be obtained by using
-        `GraphState.get_link_clifford()`.
+        Links with `'C'` written on them indicate fusions accompanied by
+        non-trivial Clifford gates. These Clifford gates can be obtained by
+        using `GraphState.get_link_clifford()`.
 
         Parameters
         ----------
         ax : None or matplotlib Axes object (default: None)
             If given, the figure is plotted on the given `Axes` object.
 
         layout : str (default: 'auto')
@@ -1691,33 +1722,47 @@
 
         figsize : 2-tuple of float (default: (5, 5))
             Size of the figure in inches.
 
         save : None or str (default: None)
             Path to save the figure.
 
-        show_node_name : bool (default: True)
-            Whether to show node names.
+        show_node_names : bool (default: True)
+            If `True`, node names are shown.
 
         node_color : str (default: 'white')
             Color of nodes.
 
-        show_link_name : bool (default: False)
-            Whether to show link names.
+        show_link_names : bool (default: False)
+            If `True`, link names are shown.
+
+        show_fusion_orders : bool (default: True)
+            If `True`, fusion orders are shown on links.
 
-        show_fusion_order : bool (default: True)
-            Whether to show fusion orders on links.<br>
-            If both `show_link_name` and `show_fusion_order` are `True`,
+            If both `show_link_names` and `show_fusion_orders` are `True`,
             it is shown as `'{link name}-{fusion order}'`
 
-        link_color : str (default: 'black')
-            Color of links.
+        show_link_cliffords : bool (default: True)
+            If `True`, links that correspond to fusions accompanied by
+            non-trivial Clifford gates are marked as `'C'`.
+
+            If `show_link_names` or `show_fusion_orders` are `True`, `'C'` is
+            appended to the end of the label.
+
+        link_color_ll : str (default: 'black')
+            Color of leaf-to-leaf links.
+
+        link_color_rl : str (default: 'blue')
+            Color of root-to-leaf links.
+
+        link_color_rr : str (default: 'red')
+            Color of root-to-root links.
 
-        link_color_clifford : str (default: 'orange')
-            Color of links with Clifford gates.
+        arrow_size : float (default: 0.02)
+            Size of arrows for root-to-leaf links.
 
         Any other keyword arguments in igraph.plot can be directly used.<br>
         See https://python.igraph.org/en/stable/tutorial.html#layouts-and-plotting <br>
         If they are given, they override the above parameters.<br>
 
         Returns
         -------
```

## optgraphstate/visualization.py

```diff
@@ -20,15 +20,15 @@
 
 
 def plot_graph(graph,
                ax=None,
                layout='auto',
                figsize=(5, 5),
                save=None,
-               show_vertex_name=True,
+               show_vertex_names=True,
                vertex_color_normal='white',
                vertex_color_clifford='orange',
                vertices_to_highlight=None,
                vertex_color_highlight='purple',
                edge_color_normal='black',
                edge_color_fusion='red',
                edge_style_fusion='--',
@@ -83,15 +83,15 @@
                 done.add(vname_fusion)
 
         visual_style = {
             'vertex_color': vertex_colors,
             'edge_color': [edge_color_normal] * org_ecount + [
                 edge_color_fusion] * round(len(vs_with_ext_fusion) / 2), }
 
-        if show_vertex_name:
+        if show_vertex_names:
             visual_style['vertex_label'] = graph.vs['name']
 
         visual_style.update(kwargs)
         _plot_base(graph, ax=ax, layout=layout, **visual_style)
 
         children = ax.get_children()
         ecount = graph.ecount()
@@ -99,19 +99,21 @@
         assert len(lines) == ecount
         for eid in range(org_ecount, ecount):
             lines[eid].set(linestyle=edge_style_fusion)
 
     else:
         graph = graph
         visual_style = {
-            'vertex_label': graph.vs['name'],
             'vertex_color': vertex_colors,
             'edge_color': edge_color_normal
         }
 
+        if show_vertex_names:
+            visual_style['vertex_label'] = graph.vs['name']
+
         visual_style.update(kwargs)
         _plot_base(graph, ax=ax, layout=layout, **visual_style)
 
     plt.tight_layout()
 
     if save is not None:
         plt.savefig(save, transparent=True)
@@ -120,24 +122,23 @@
 
 
 def plot_fusion_network(network,
                         ax=None,
                         layout='auto',
                         figsize=(5, 5),
                         save=None,
-                        # show_vertex_overhead=False,
-                        # show_edge_overhead=False,
-                        show_node_name=True,
+                        show_node_names=True,
                         node_color='white',
-                        # node_color_clifford='orange',
-                        show_link_name=False,
-                        show_fusion_order=True,
-                        # uniform_link_style=False,
-                        link_color='black',
-                        link_color_clifford='red',
+                        show_link_names=False,
+                        show_fusion_orders=True,
+                        show_link_cliffords=True,
+                        link_color_ll='black',
+                        link_color_rl='blue',
+                        link_color_rr='red',
+                        arrow_size=0.02,
                         **kwargs):
     """
     Plot a fusion network.
 
     See the description of `optgraphstate.GraphState.plot_fusion_network()`
     for details.
 
@@ -160,15 +161,15 @@
     if not isinstance(network, ig.Graph):
         raise TypeError("Parameter 'network' is not ig.Graph.")
 
     # show_vertex_overhead = show_vertex_overhead and 'overhead' in
     # network.vs.attributes()
     # show_edge_overhead = show_edge_overhead and 'overhead' in
     # network.es.attributes()
-    show_fusion_order = show_fusion_order and 'step' in network.es.attributes()
+    show_fusion_orders = show_fusion_orders and 'order' in network.es.attributes()
     rl_exists = 'RL' in network.es['kind']
 
     if rl_exists:
         network_directed = network.copy()
         network_directed.to_directed()
 
         es_to_delete = []
@@ -182,18 +183,20 @@
             else:
                 e_to_delete = (vname2, vname1)
             es_to_delete.append(e_to_delete)
 
         network_directed.delete_edges(es_to_delete)
         network = network_directed
 
-    # edge_color_dict = {
-    #     'RR': link_color_rr,
-    #     'RL': link_color_rl,
-    #     'LL': link_color_ll}
+    link_color_dict = {
+        'RR': link_color_rr,
+        'RL': link_color_rl,
+        'LL': link_color_ll
+    }
+
     # cliffords = [
     #     v['clifford_root'] is not None or v['clifford_leaves'] is not None for
     #     v in network.vs]
     # if show_vertex_overhead:
     #     vertex_label = []
     #     for v in network.vs:
     #         name = v['name']
@@ -206,74 +209,81 @@
     visual_style = {
         # 'vertex_color': [node_color_clifford if clifford else node_color
         #                  for clifford in cliffords],
         'vertex_color': node_color,
         # 'vertex_shape': ['square' if clifford else 'circle' for clifford in
         # cliffords],
         'edge_align_label': False,
-        'edge_color': [link_color_clifford if link['cliffords'] else link_color
-                       for link in network.es],
+        'edge_color': [link_color_dict[kind] for kind in network.es['kind']],
     }
 
-    if show_node_name:
+    if show_node_names:
         visual_style['vertex_label'] \
             = network.vs['name'] if network.vcount() else []
 
     if rl_exists:
         visual_style['vertex_size'] = 0.4
-        visual_style['edge_arrow_size'] = [0.02 if e['kind'] == 'RL' else 0 for
-                                           e in network.es]
+        visual_style['edge_arrow_size'] = [
+            arrow_size if e['kind'] == 'RL' else 0 for
+            e in network.es]
         # visual_style['edge_color'] = [edge_color_dict[e['kind']] for e in
         #                               network.es]
 
-    if network.ecount() and (show_fusion_order or show_link_name):
+    if network.ecount() and (show_fusion_orders or show_link_names):
         visual_style['edge_background'] = 'white'
 
-        if sum([show_fusion_order, show_link_name]) == 1:
-            if show_fusion_order:
-                key = 'step'
+        if sum([show_fusion_orders, show_link_names]) == 1:
+            if show_fusion_orders:
+                key = 'order'
             # elif show_edge_overhead:
             #     key = 'overhead'
             else:
                 key = 'name'
             edge_label = network.es[key]
 
         else:
             edge_label = []
             for e in network.es:
                 # label = []
                 # if show_edge_labels:
                 #     label.append(f"{e['name']}")
                 # if show_fusion_order:
-                #     label.append(f"{e['step']}")
+                #     label.append(f"{e['order']}")
                 # if show_edge_overhead:
                 #     overhead = e['overhead']
                 #     if abs(overhead % 1) < 1e-6:
                 #         overhead = round(overhead)
                 #     label.append(f"W{overhead}")
                 # label = '_'.join(label)
-                label = f"{e['name']}-{e['step']}"
+                label = f"{e['name']}-{e['order']}"
                 edge_label.append(label)
 
+        if show_link_cliffords:
+            for link in network.es.select(cliffords_ne={}):
+                eid = link.index
+                edge_label[eid] = str(edge_label[eid]) + 'C'
+
         visual_style['edge_label'] = edge_label
 
     visual_style.update(kwargs)
 
     _plot_base(network, ax=ax, layout=layout, **visual_style)
 
     if network.ecount():
         children = ax.get_children()
         lines = [child for child in children if isinstance(child, PathPatch)]
 
         edge_style = {
-            'RR': ':',
+            'RR': '--',
             'RL': '-',
-            'LL': '-'}
+            'LL': '-'
+        }
         for eid, line in enumerate(lines):
-            line.set(linestyle=edge_style[network.es[eid]['kind']])
+            link = network.es[eid]
+            line.set(linestyle=edge_style[link['kind']])
 
     plt.tight_layout()
 
     if save is not None:
         plt.savefig(save, transparent=True)
 
     return fig, ax
```

## Comparing `optgraphstate-0.1.1.dist-info/LICENSE` & `optgraphstate-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `optgraphstate-0.1.1.dist-info/METADATA` & `optgraphstate-0.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: optgraphstate
-Version: 0.1.1
+Version: 0.1.2
 Summary: Graph-theoretical optimization of fusion-based graph state generation
 Home-page: https://github.com/seokhyung-lee/OptGraphState
 Author: Seok-Hyung Lee
 Author-email: sh.lee1524@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OptGraphState
 
-**Version 0.1.1**
+**Version 0.1.2**
 
 *Graph-theoretical optimization of fusion-based graph state generation.*
 
 **OptGraphState** is a python package that implements the graph-theoretical strategy to optimize the fusion-based
 generation of any graph state. The package has the following features:
 
 - Finding a resource-efficient method of generating a given graph state through type-II fusions from multiple basic
   resource states, which are three-qubit linear graph states.
 - Computing the corresponding resource overhead, which is quantified by the average number of required basic resource
-  states.
+  states or fusion attempts.
 - Visualizing the original graph (of the graph state you want to generate), unraveled graphs, and fusion networks. An
   unraveled graph is a simplified graph where the corresponding graph state is equivalent to the desired graph state up
   to fusions and single-qubit Clifford operations. A fusion network is a graph that instructs the fusions between basic
   resource states required to generate the desired graph state.
 - Various predefined sample graphs for input.
 
 ## Installation
```

## Comparing `optgraphstate-0.1.1.dist-info/RECORD` & `optgraphstate-0.1.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-optgraphstate/__init__.py,sha256=HK-MWS9owZPXYepHgTfxuq7E8-dvqo0huocygbV8jsc,67049
+optgraphstate/__init__.py,sha256=el-mtgl_TeJ3JiBpGU69jWpGEbDPvIt3lWEqLPRjCr4,68529
 optgraphstate/graph_tools.py,sha256=foGOoB5jUwToLVSP5iuhn00fk-uokV_cZVdrWWR3uy8,14819
 optgraphstate/utils.py,sha256=11ak92ZwuPQl6DVVEI45mS_gjS-QKZONObwuRvRpmpE,686
-optgraphstate/visualization.py,sha256=GILVTwwmpr6VFO5CW3mu7vkPPbcBK-pPohHCzaEsywY,8936
-optgraphstate-0.1.1.dist-info/LICENSE,sha256=rB8sqYvzli01OnnAHmeXktkq7ye_YYJjOWP25yuN8VY,1070
-optgraphstate-0.1.1.dist-info/METADATA,sha256=CSsTR64ATx3T20PGdLyxz2kq4kt8uVyAscFCZtNhyV4,1881
-optgraphstate-0.1.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-optgraphstate-0.1.1.dist-info/top_level.txt,sha256=Rj9Sk6j_-PrVy4Gk6bDHLQEpm37egogxHKxd9xLk0A0,14
-optgraphstate-0.1.1.dist-info/RECORD,,
+optgraphstate/visualization.py,sha256=uqadIHvlo201dImbcp93di5QVJN4na9IyyTV3gCqtXs,9075
+optgraphstate-0.1.2.dist-info/LICENSE,sha256=rB8sqYvzli01OnnAHmeXktkq7ye_YYJjOWP25yuN8VY,1070
+optgraphstate-0.1.2.dist-info/METADATA,sha256=H87KTajmcKjbt4Hum7wxXCzYLKbxpDYGPPKblYBsMHs,1900
+optgraphstate-0.1.2.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+optgraphstate-0.1.2.dist-info/top_level.txt,sha256=Rj9Sk6j_-PrVy4Gk6bDHLQEpm37egogxHKxd9xLk0A0,14
+optgraphstate-0.1.2.dist-info/RECORD,,
```

